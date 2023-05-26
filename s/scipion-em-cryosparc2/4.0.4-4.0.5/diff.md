# Comparing `tmp/scipion-em-cryosparc2-4.0.4.tar.gz` & `tmp/scipion-em-cryosparc2-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryosparc2-4.0.4.tar", last modified: Wed Mar 29 14:01:50 2023, max compression
+gzip compressed data, was "scipion-em-cryosparc2-4.0.5.tar", last modified: Fri May 26 15:55:45 2023, max compression
```

## Comparing `scipion-em-cryosparc2-4.0.4.tar` & `scipion-em-cryosparc2-4.0.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:01:50.430294 scipion-em-cryosparc2-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-03-29 14:01:50.430294 scipion-em-cryosparc2-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:01:50.426294 scipion-em-cryosparc2-4.0.4/cryosparc2/
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)    32630 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:01:50.426294 scipion-em-cryosparc2-4.0.4/cryosparc2/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/convert/cs2Start.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/cryosparc2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:01:50.430294 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryorefine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
--rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_ab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23794 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    20831 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_sharppening.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:01:50.430294 scipion-em-cryosparc2-4.0.4/cryosparc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/tests/test_protocols_cryosparc2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33958 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:01:50.430294 scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_2Dclassify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_partsubtract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/cryosparc2/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:01:50.430294 scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-03-29 14:01:50.000000 scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-29 14:01:50.000000 scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:01:50.000000 scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-29 14:01:50.000000 scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-29 14:01:50.000000 scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 14:01:50.000000 scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 14:01:50.430294 scipion-em-cryosparc2-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-03-29 14:00:09.000000 scipion-em-cryosparc2-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.395722 scipion-em-cryosparc2-4.0.5/cryosparc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32630 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.395722 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/cs2Start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/cryosparc2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.395722 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryorefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_ab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23794 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20831 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_sharppening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_protocols_cryosparc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34295 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_2Dclassify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_partsubtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/setup.py
```

### Comparing `scipion-em-cryosparc2-4.0.4/LICENSE` & `scipion-em-cryosparc2-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/PKG-INFO` & `scipion-em-cryosparc2-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.4
+Version: 4.0.5
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
```

### Comparing `scipion-em-cryosparc2-4.0.4/README.rst` & `scipion-em-cryosparc2-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/__init__.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import os
 import pwem as em
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
-__version__ = '4.0.4'
+__version__ = '4.0.5'
 _references = ['Punjani2017', 'Brubaker2017', 'daniel_asarnow_2019_3576630']
 _logo = 'cryosparc2_logo.png'
 
 
 class Plugin(em.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-cryosparc2"
     _homeVar = CRYOSPARC_HOME
@@ -77,15 +77,15 @@
     def addPyemPackage(cls, env):
         PYEM_INSTALLED = f"pyem_{PYEM_VERSION}_installed"
         ENV_NAME = getPyemEnvName(PYEM_VERSION)
 
         installCmd = ["pip uninstall -y pyem && ",
                       cls.getCondaActivationCmd(),
                       f'conda create -y -n {ENV_NAME} python=3.8 -c conda-forge -c anaconda && ',
-                      f'conda activate {ENV_NAME} && pip install git+https://github.com/asarnow/pyem.git@47cf8f70488500be5988b4db1b6ef7002916e0e0']
+                      f'conda activate {ENV_NAME} && pip install git+https://github.com/asarnow/pyem.git@47cf8f70488500be5988b4db1b6ef7002916e0e0 && pip install numpy==1.23.5']
 
         # install pyem
         #installCmd.append('pip install git+https://github.com/asarnow/pyem.git@47cf8f70488500be5988b4db1b6ef7002916e0e0')
 
         # Flag installation finished
         installCmd.append(f'&& touch {PYEM_INSTALLED}')
```

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/bibtex.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/constants.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/convert/__init__.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/convert/convert.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from collections import OrderedDict
 
 import emtable
 import numpy as np
 import os
 import argparse
 import sys
+import logging
+logger = logging.getLogger(__name__)
 
 from emtable.metadata import _guessType
 from pwem.emlib.image import ImageHandler
 import pwem.emlib.metadata as md
 from pwem.objects import (String, Integer, Transform, Particle,
                           Coordinate, Acquisition, CTFModel)
 from pyworkflow.object import ObjectWrap, Float
@@ -261,15 +264,15 @@
 
     if is2D:
         angle = angles[0] + angles[2]
         alignmentRow.set(RELIONCOLUMNS.rlnAnglePsi.value, -angle)
 
         flip = bool(np.linalg.det(matrix[0:2, 0:2]) < 0)
         if flip:
-            print("FLIP in 2D not implemented")
+            logger.debug("FLIP in 2D not implemented")
     elif is3D:
         raise Exception("3D alignment conversion for Relion not implemented. "
                         "It seems the particles were generated with an "
                         "incorrect alignment type. You may either re-launch "
                         "the protocol that generates the particles "
                         "with angles or set 'Consider previous alignment?' "
                         "to No")
@@ -441,15 +444,15 @@
         M = inv(M)
     else:
         M[:3, 3] = shifts[:3]
 
     return M
 
 
-def convertBinaryFiles(imgSet, outputDir, extension='mrcs'):
+def convertBinaryFiles(imgSet, outputDir, extension='mrcs', **kwargs):
     """ Convert binary images files to a format read by Cryosparc.
     Params:
         imgSet: input image set to be converted.
         outputDir: where to put the converted file(s)
     Return:
         A dictionary with old-file as key and new-file as value
         If empty, not conversion was done.
@@ -483,43 +486,43 @@
     def createBinaryLink(fn):
         """ Just create a link named .mrcs to cryoSPARC understand
         that it is a binary stack file and not a volume.
         """
         newFn = getUniqueFileName(fn, extension)
         if not os.path.exists(newFn):
             pwutils.createAbsLink(os.path.abspath(fn), newFn)
-            print("   %s -> %s" % (newFn, fn))
+            logger.debug("   %s -> %s" % (newFn, fn))
         return newFn
 
     def convertStack(fn):
         """ Convert from a format that is not read by Cryosparc
         to an spider stack.
         """
         newFn = getUniqueFileName(fn, 'mrc')
         ih.convertStack(fn, newFn)
-        print("   %s -> %s" % (fn, newFn))
+        logger.debug("   %s -> %s" % (fn, newFn))
         return newFn
 
     def replaceRoot(fn):
         """ Link create to the root folder, so just replace that
         in the name, no need to do anything else.
         """
         return fn.replace(rootDir, outputRoot)
 
     if ext == extension:
-        print("convertBinaryFiles: creating soft links.")
-        print("   Root: %s -> %s" % (outputRoot, rootDir))
+        logger.debug("convertBinaryFiles: creating soft links.")
+        logger.debug("   Root: %s -> %s" % (outputRoot, rootDir))
         mapFunc = replaceRoot
         pwutils.createAbsLink(os.path.abspath(rootDir), outputRoot)
     elif ext == 'mrc' and extension == 'mrcs':
-        print("convertBinaryFiles: creating soft links (mrcs -> mrc).")
+        logger.debug("convertBinaryFiles: creating soft links (mrcs -> mrc).")
         mapFunc = createBinaryLink
     elif ext.endswith('hdf') or ext.endswith(
             'stk'):  # assume eman .hdf format or .stk format
-        print("convertBinaryFiles: converting stacks. (%s -> %s)"
+        logger.debug("convertBinaryFiles: converting stacks. (%s -> %s)"
               % (ext, extension))
         mapFunc = convertStack
     else:
         mapFunc = None
 
     if mapFunc is not None:
         pwutils.makePath(outputRoot)
@@ -534,16 +537,27 @@
     args = {'outputDir': extraPath,
             'fillMagnification': True,
             'fillRandomSubset': True}
 
     if imgSet.hasAlignmentProj() and imgSet.getAttributeValue(
             "_rlnRandomSubset") is None:
         args['postprocessImageRow'] = addRandomSubset
-
-    cryosPARCwriteSetOfParticles(imgSet, fileName, **args)
+    try:
+        logger.info('Trying to generate the star file with Relion convert...')
+        from relion import convert
+        alignType = ALIGN_PROJ if imgSet.hasAlignmentProj() else ALIGN_NONE
+        args['alignType'] = alignType
+        args['incompatibleExtensions'] = ['hdf', 'stk']
+        convert.writeSetOfParticles(imgSet, fileName, **args)
+        logger.info('The star file was generate successfully ...')
+    except Exception:
+        logger.info('The star file generation with Relion convert failed ...')
+        logger.info('Trying to generate the star file with cryoSPARC convert ...')
+        cryosPARCwriteSetOfParticles(imgSet, fileName, **args)
+        logger.info('The star file was generate successfully ...')
 
 
 def cryosPARCwriteSetOfParticles(imgSet, starFile, outputDir, **kwargs):
     if outputDir is not None:
         filesDict = convertBinaryFiles(imgSet, outputDir)
         kwargs['filesDict'] = filesDict
     partMd = md.MetaData()
```

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/convert/cs2Start.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/cs2Start.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/convert/dataimport.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/cryosparc2_logo.png` & `scipion-em-cryosparc2-4.0.5/cryosparc2/cryosparc2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/__init__.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_base.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryorefine.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryorefine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc2d.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,46 +33,46 @@
 from pwem import ALIGN_2D
 from pyworkflow.object import String
 from pyworkflow.protocol.params import (PointerParam, FloatParam, IntParam,
                                         BooleanParam, Positive)
 import pyworkflow.utils as pwutils
 
 from .protocol_base import ProtCryosparcBase
-from ..convert import (rowToAlignment, convertCs2Star,  cryosparcToLocation)
+from ..convert import (rowToAlignment, convertCs2Star, cryosparcToLocation)
 from ..utils import (addComputeSectionParams, cryosparcValidate, gpusValidate,
                      enqueueJob, waitForCryosparc, clearIntermediateResults,
-                     copyFiles, getOutputPreffix)
+                     copyFiles, getOutputPreffix, isCryosparcStandalone)
 from ..constants import *
 
 
 class ProtCryo2D(ProtCryosparcBase, pwprot.ProtClassify2D):
     """ Wrapper to CryoSparc 2D clustering program.
         Classify particles into multiple 2D classes to facilitate stack cleaning
         and removal of junk particles. Also useful as a sanity check to
         investigate particle quality.
     """
     _label = '2D classification'
     IS_2D = True
     _className = "class_2D"
-    
+
     def __init__(self, **args):
         pwprot.ProtClassify2D.__init__(self, **args)
         if self.numberOfMpi.get() < 2:
             self.numberOfMpi.set(2)
-    
+
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
-                  'input_particles': self._getTmpPath('input_particles.star'),
-                  'out_particles': self._getExtraPath() + '/output_particle.star',
-                  'out_class': self._getExtraPath() + '/output_class.star',
-                  'out_class_m2': self._getExtraPath() + '/output_class_m2.star'
-                  }
+            'input_particles': self._getTmpPath('input_particles.star'),
+            'out_particles': self._getExtraPath() + '/output_particle.star',
+            'out_class': self._getExtraPath() + '/output_class.star',
+            'out_class_m2': self._getExtraPath() + '/output_class_m2.star'
+        }
         self._updateFilenamesDict(myDict)
-    
+
     # --------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputParticles', PointerParam,
                       pointerClass='SetOfParticles',
                       label="Input particles", important=True,
                       help='Select the input images from the project.')
@@ -116,17 +116,17 @@
                            'each 2D class has no density outside the circular '
                            'window. By default, the window is a circle that only '
                            'masks out the corners of the 2D classes.')
 
         form.addParam('class2D_window_inner_A', FloatParam, default=None,
                       label='Circular mask diameter (A)',
                       help='The inner diameter (in Angstroms) of the window '
-                            'that is applied to 2D classes during '
-                            'classification. If None, the window only masks out '
-                            'the corners of each 2D class.',
+                           'that is applied to 2D classes during '
+                           'classification. If None, the window only masks out '
+                           'the corners of each 2D class.',
                       allowsNull=True,
                       condition='useCircular2D==True')
 
         form.addParam('class2D_window_outer_A', FloatParam, default=None,
                       label='Circular mask diameter outer (A)',
                       help='The outer diameter (in Angstroms) of the window. '
                            'If None, outer diameter is 20 percent larger than '
@@ -278,26 +278,27 @@
                                                                mrcFileName])
 
         csPartFile = os.path.join(self._getExtraPath(), csParticlesName)
         outputStarFn = self._getFileName('out_particles')
         argsList = [csPartFile, outputStarFn]
         convertCs2Star(argsList)
 
-        csClassAverageFile = os.path.join(self._getExtraPath(), csClassAveragesName)
+        csClassAverageFile = os.path.join(self._getExtraPath(),
+                                          csClassAveragesName)
         outputClassFn = self._getFileName('out_class')
         argsList = [csClassAverageFile, outputClassFn]
 
         convertCs2Star(argsList)
 
         self._createModelFile()
         self._loadClassesInfo(self._getFileName('out_class_m2'))
         # Use the pointer with extended (indirect)
         classes2DSet = self._createSetOfClasses2D(self.inputParticles)
         self._fillClassesFromLevel(classes2DSet)
-  
+
         self._defineOutputs(outputClasses=classes2DSet)
         self._defineSourceRelation(self.inputParticles.get(), classes2DSet)
 
     # --------------------------- INFO functions -------------------------------
     def _validate(self):
         validateMsgs = cryosparcValidate()
         if not validateMsgs:
@@ -320,27 +321,28 @@
 
     def _methods(self):
         methods = "We classified input particles %s (%d items) " % (
             self.getObjectTag('inputParticles'),
             self._getInputParticles().getSize())
         methods += "into %d classes using CryoSparc " % self.numberOfClasses.get()
         return [methods]
-    
+
     # --------------------------- UTILS functions ------------------------------
     def _loadClassesInfo(self, filename):
         """ Read some information about the produced 2D classes
         from the metadata file.
         """
         self._classesInfo = {}  # store classes info, indexed by class id
 
         mdFileName = '%s@%s' % ('particles', filename)
         table = emtable.Table(fileName=filename)
 
         for classNumber, row in enumerate(table.iterRows(mdFileName)):
-            index, fn = cryosparcToLocation(row.get(RELIONCOLUMNS.rlnImageName.value))
+            index, fn = cryosparcToLocation(
+                row.get(RELIONCOLUMNS.rlnImageName.value))
 
             # Store info indexed by id, we need to store the row.clone() since
             # the same reference is used for iteration
             scaledFile = self._getScaledAveragesFile(fn)
             self._classesInfo[classNumber + 1] = (index, scaledFile, row)
         self._numClass = index
 
@@ -348,20 +350,21 @@
         """ Create the SetOfClasses2D from a given iteration. """
 
         # the particle with orientation parameters (all_parameters)
         xmpMd = 'particles@' + self._getFileName("out_particles")
 
         clsSet.classifyItems(updateItemCallback=self._updateParticle,
                              updateClassCallback=self._updateClass,
-                             itemDataIterator=emtable.Table.iterRows(xmpMd))  # relion style
+                             itemDataIterator=emtable.Table.iterRows(
+                                 xmpMd))  # relion style
 
     def _updateParticle(self, item, row):
         item.setClassId(row.get(RELIONCOLUMNS.rlnClassNumber.value))
         item.setTransform(rowToAlignment(row, ALIGN_2D))
-        
+
     def _updateClass(self, class2D):
         classId = class2D.getObjId()
         if classId in self._classesInfo:
             index, fn, row = self._classesInfo[classId]
             class2D.setAlignment2D()
             class2Drep = class2D.getRepresentative()
             class2Drep.setLocation(index, fn)
@@ -371,15 +374,16 @@
         with open(self._getFileName('out_class'), 'r') as input_file, \
                 open(self._getFileName('out_class_m2'), 'w') as output_file:
             for line in input_file:
                 if "@" in line:
                     row = "%s@%s/%s"
                     classNumber = line.split('@')[0]
                     image = line.split('/')[1]
-                    output_file.write(row % (classNumber, self._getExtraPath(), image))
+                    output_file.write(
+                        row % (classNumber, self._getExtraPath(), image))
                 else:
                     output_file.write(line)
 
     def _getNumberOfIterSuffix(self):
         _numberOfIter = (self.numberOnlineEMIterator.get() +
                          self.numberFinalIterator.get() - 1)
         _numberOfIterSuffix = "_00%s" % str(self.numberOnlineEMIterator.get())
@@ -392,37 +396,44 @@
     def _defineParamsName(self):
         """ Define a list with all protocol parameters names"""
         self.lane = str(self.getAttributeValue('compute_lane'))
 
     def assignParamValue(self):
         params = {"class2D_K": str(self.numberOfClasses.get()),
                   "class2D_max_res": str(self.maximunResolution.get()),
-                  "class2D_sigma_init_factor": str(self.initialClassification.get()),
+                  "class2D_sigma_init_factor": str(
+                      self.initialClassification.get()),
                   "class2D_window": str(self.useCircular2D.get()),
                   "class2D_recenter": str(self.reCenter2D.get()),
                   "class2D_recenter_thresh": str(self.reCenterMask.get()),
                   "class2D_recenter_binary": str(self.reCenterMaskBinary.get()),
                   "class2D_force_max": str(self.forceMaxover.get()),
                   "class2D_ctf_phase_flip_only": str(self.ctfFlipPhases.get()),
                   "class2D_num_full_iter": str(self.numberFinalIterator.get()),
-                  "class2D_num_full_iter_batch": str(self.numberOnlineEMIterator.get()),
-                  "class2D_num_full_iter_batchsize_per_class": str(self.batchSizeClass.get()),
+                  "class2D_num_full_iter_batch": str(
+                      self.numberOnlineEMIterator.get()),
+                  "class2D_num_full_iter_batchsize_per_class": str(
+                      self.batchSizeClass.get()),
                   "class2D_init_scale": str(self.initialScale2D.get()),
                   "class2D_zp_factor": str(self.zeropadFactor.get()),
                   "class2D_use_frc_reg": str(self.useFRCRegularized.get()),
                   "class2D_use_frc_reg_full": str(self.useFullFRC.get()),
-                  "class2D_sigma_init_iter": str(self.iterationToStartAnneling.get()),
-                  "class2D_sigma_num_anneal_iters": str(self.iterationToStartAnneal.get()),
+                  "class2D_sigma_init_iter": str(
+                      self.iterationToStartAnneling.get()),
+                  "class2D_sigma_num_anneal_iters": str(
+                      self.iterationToStartAnneal.get()),
                   "class2D_sigma_use_white": str(self.useWhiteNoiseModel.get()),
                   "intermediate_plots": str('False'),
                   "compute_use_ssd": str(self.compute_use_ssd.get())}
         if self.class2D_window_inner_A.get() is not None:
-                params["class2D_window_inner_A"] = str(self.class2D_window_inner_A.get())
+            params["class2D_window_inner_A"] = str(
+                self.class2D_window_inner_A.get())
         if self.class2D_window_outer_A.get() is not None:
-                params["class2D_window_outer_A"] = str(self.class2D_window_outer_A.get())
+            params["class2D_window_outer_A"] = str(
+                self.class2D_window_outer_A.get())
         return params
 
     def doRunClass2D(self):
         """
         do_run_class_2D:  do_job(job_type, puid='P1', wuid='W1',
                                  uuid='devuser', params={},
                                  input_group_connects={})
@@ -435,22 +446,25 @@
         # the cryosparc version)
         try:
             gpusToUse = self.getGpuList()
             numberGPU = len(gpusToUse)
         except Exception:
             gpusToUse = False
             numberGPU = 1
-
         params = self.assignParamValue()
+        if not isCryosparcStandalone():  # Cluster case
+            gpusToUse = False
+            numberGPU = self.compute_num_gpus.get()
+
         params["compute_num_gpus"] = str(numberGPU)
         runClass2DJob = enqueueJob(self._className, self.projectName.get(),
-                                     self.workSpaceName.get(),
-                                     str(params).replace('\'', '"'),
-                                     str(input_group_connect).replace('\'', '"'),
-                                     self.lane, gpusToUse)
+                                   self.workSpaceName.get(),
+                                   str(params).replace('\'', '"'),
+                                   str(input_group_connect).replace('\'', '"'),
+                                   self.lane, gpusToUse)
 
         self.runClass2D = String(runClass2DJob.get())
         self.currenJob.set(runClass2DJob.get())
         self._store(self)
 
         waitForCryosparc(self.projectName.get(), self.runClass2D.get(),
                          "An error occurred in the 2D classification process. "
```

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_classification.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_classification.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3d_variability.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_ab.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_ab.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_part_subtract.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_part_subtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_sharppening.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_sharppening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/protocols.conf` & `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/tests/__init__.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/tests/test_protocols_cryosparc2.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_protocols_cryosparc2.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/tests/test_utils.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import getpass
 import unittest
 from unittest.mock import patch
 
-from cryosparc2 import V2_14_2, V_UNKNOWN
+from cryosparc2 import V_UNKNOWN
 from cryosparc2.utils import (cryosparcValidate, cryosparcExists,
                               isCryosparcRunning, calculateNewSamplingRate,
                               getProjectName, getCryosparcVersion)
 
 import cryosparc2.utils as csutils
 
 class TestUtils(unittest.TestCase):
```

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/utils.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from pkg_resources import parse_version
 
 import pyworkflow.utils as pwutils
 from pwem.constants import SCIPION_SYM_NAME
 from pwem.constants import (SYM_CYCLIC, SYM_TETRAHEDRAL,
                             SYM_OCTAHEDRAL, SYM_I222, SYM_I222r)
 from pwem.convert import Ccp4Header
+from pyworkflow.protocol import IntParam
 
 from . import Plugin
 from .constants import *
 
 VERSION = 'version'
 
 STATUS_FAILED = "failed"
@@ -785,14 +786,20 @@
     defaultLane = getCryosparcDefaultLane()
     if defaultLane is None:
         defaultLane = 'default'
     form.addParam('compute_lane', StringParam, default=defaultLane,
                   label='Lane name:', readOnly=True,
                   help='The scheduler lane name to add the protocol execution')
 
+    from .protocols import ProtCryo2D
+    if not isCryosparcStandalone() and isinstance(form._protocol, ProtCryo2D):
+        form.addParam('compute_num_gpus', IntParam, default=1,
+                      label='Number of GPUs to compute:',
+                      help='Number of GPUs to compute:')
+
 
 def addSymmetryParam(form, help=""):
     """
     Add the symmetry param with the conventions
     :param form:
     :return:
     """
```

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/__init__.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_2Dclassify.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_2Dclassify.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_initialmodel.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_partsubtract.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_partsubtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/viewers/viewer_refinement.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_refinement.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 import pwem.viewers.showj as showj
 from pwem import Domain
 from pwem.objects import FSC, SetOfFSCs
 from pyworkflow.gui.dialog import showInfo
 from pyworkflow.protocol.constants import *
 from pyworkflow.protocol.params import (LabelParam, FloatParam, EnumParam)
 from pyworkflow.viewer import DESKTOP_TKINTER, WEB_DJANGO
-from pwem.viewers import (ChimeraView, ChimeraClientView,
-                          ObjectView, EmProtocolViewer, FscViewer)
+from pwem.viewers import (ChimeraView, ObjectView, EmProtocolViewer, FscViewer)
 
 from ..protocols import (ProtCryoSparcLocalRefine, ProtCryoSparcHelicalRefine3D,
                          ProtCryoSparc3DHomogeneousRefine,
                          ProtCryoSparcNewNonUniformRefine3D,
                          ProtCryoSparcHomogeneousReconstruct)
 from ..constants import *
 from ..utils import *
@@ -201,15 +200,15 @@
                         localVol = os.path.relpath(vol,
                                                    self.protocol._getExtraPath())
                         f.write("open %s\n" % localVol)
                 f.write('tile\n')
                 f.close()
                 view.append(ChimeraView(cmdFile))
             else:
-                view.append(ChimeraClientView(volumes[0]))
+                view.append(ChimeraView(volumes[0]))
         else:
             showInfo('Info', "Chimera plugin is not installed. Please, "
                              "install it to display the volume",
                      self.getTkRoot())
 
         return view
```

### Comparing `scipion-em-cryosparc2-4.0.4/cryosparc2/wizards.py` & `scipion-em-cryosparc2-4.0.5/cryosparc2/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/PKG-INFO` & `scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.4
+Version: 4.0.5
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
```

### Comparing `scipion-em-cryosparc2-4.0.4/scipion_em_cryosparc2.egg-info/SOURCES.txt` & `scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.4/setup.py` & `scipion-em-cryosparc2-4.0.5/setup.py`

 * *Files identical despite different names*


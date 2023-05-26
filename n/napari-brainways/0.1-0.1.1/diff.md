# Comparing `tmp/napari_brainways-0.1.tar.gz` & `tmp/napari_brainways-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_brainways-0.1.tar", last modified: Fri May 26 10:50:40 2023, max compression
+gzip compressed data, was "napari_brainways-0.1.1.tar", last modified: Fri May 26 13:58:20 2023, max compression
```

## Comparing `napari_brainways-0.1.tar` & `napari_brainways-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.483196 napari_brainways-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.475196 napari_brainways-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.479196 napari_brainways-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-26 10:50:14.000000 napari_brainways-0.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 10:50:14.000000 napari_brainways-0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.479196 napari_brainways-0.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-26 10:50:14.000000 napari_brainways-0.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 10:50:14.000000 napari_brainways-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-26 10:50:14.000000 napari_brainways-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 10:50:14.000000 napari_brainways-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-26 10:50:40.483196 napari_brainways-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 10:50:14.000000 napari_brainways-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.479196 napari_brainways-0.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-05-26 10:50:14.000000 napari_brainways-0.1/data/test_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 10:50:14.000000 napari_brainways-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 10:50:40.483196 napari_brainways-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 10:50:14.000000 napari_brainways-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.475196 napari_brainways-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.479196 napari_brainways-0.1/src/napari_brainways/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.483196 napari_brainways-0.1/src/napari_brainways/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 10:50:40.000000 napari_brainways-0.1/src/napari_brainways/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/brainways_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.483196 napari_brainways-0.1/src/napari_brainways/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.483196 napari_brainways-0.1/src/napari_brainways/controllers/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/_tests/test_tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/controllers/tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/napari_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.483196 napari_brainways-0.1/src/napari_brainways/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.483196 napari_brainways-0.1/src/napari_brainways/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.483196 napari_brainways-0.1/src/napari_brainways/widgets/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/_tests/test_registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/affine_2d_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/cell_detector_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/cell_viewer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/create_subject_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/tps_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    21920 2023-05-26 10:50:14.000000 napari_brainways-0.1/src/napari_brainways/widgets/workflow_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:50:40.479196 napari_brainways-0.1/src/napari_brainways.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-26 10:50:40.000000 napari_brainways-0.1/src/napari_brainways.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-26 10:50:40.000000 napari_brainways-0.1/src/napari_brainways.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:50:40.000000 napari_brainways-0.1/src/napari_brainways.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 10:50:40.000000 napari_brainways-0.1/src/napari_brainways.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 10:50:40.000000 napari_brainways-0.1/src/napari_brainways.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 10:50:40.000000 napari_brainways-0.1/src/napari_brainways.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 10:50:14.000000 napari_brainways-0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.581213 napari_brainways-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.565213 napari_brainways-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.573213 napari_brainways-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.573213 napari_brainways-0.1.1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 13:58:20.581213 napari_brainways-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.573213 napari_brainways-0.1.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/data/test_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 13:58:20.581213 napari_brainways-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.569213 napari_brainways-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.577213 napari_brainways-0.1.1/src/napari_brainways/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.577213 napari_brainways-0.1.1/src/napari_brainways/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 13:58:20.000000 napari_brainways-0.1.1/src/napari_brainways/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/brainways_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.577213 napari_brainways-0.1.1/src/napari_brainways/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.577213 napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/controllers/tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/napari_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.577213 napari_brainways-0.1.1/src/napari_brainways/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.581213 napari_brainways-0.1.1/src/napari_brainways/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.581213 napari_brainways-0.1.1/src/napari_brainways/widgets/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/_tests/test_registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/affine_2d_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/cell_detector_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/cell_viewer_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/create_subject_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/tps_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/src/napari_brainways/widgets/workflow_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:58:20.577213 napari_brainways-0.1.1/src/napari_brainways.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 13:58:20.000000 napari_brainways-0.1.1/src/napari_brainways.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-26 13:58:20.000000 napari_brainways-0.1.1/src/napari_brainways.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:58:20.000000 napari_brainways-0.1.1/src/napari_brainways.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 13:58:20.000000 napari_brainways-0.1.1/src/napari_brainways.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 13:58:20.000000 napari_brainways-0.1.1/src/napari_brainways.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 13:58:20.000000 napari_brainways-0.1.1/src/napari_brainways.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 13:57:56.000000 napari_brainways-0.1.1/tox.ini
```

### Comparing `napari_brainways-0.1/.github/workflows/test_and_deploy.yml` & `napari_brainways-0.1.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/.gitignore` & `napari_brainways-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/.napari/DESCRIPTION.md` & `napari_brainways-0.1.1/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/.pre-commit-config.yaml` & `napari_brainways-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/LICENSE` & `napari_brainways-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/PKG-INFO` & `napari_brainways-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_brainways
-Version: 0.1
+Version: 0.1.1
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1/README.md` & `napari_brainways-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/data/test_data.npz` & `napari_brainways-0.1.1/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/setup.cfg` & `napari_brainways-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/_sample_data.py` & `napari_brainways-0.1.1/src/napari_brainways/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/_tests/test_reader.py` & `napari_brainways-0.1.1/src/napari_brainways/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/_tests/test_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/brainways_ui.py` & `napari_brainways-0.1.1/src/napari_brainways/brainways_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,15 @@
                 image=self._image, params=self.current_params
             )
 
     def _open_step(self):
         self.current_step.open()
         self.current_step.show(self.current_params, self._image)
         self.widget.hide_progress_bar()
+        self.widget.update_enabled_steps()
         self._set_title()
 
     def _set_title(self, valid_document_index: Optional[int] = None):
         if valid_document_index is None:
             valid_document_index = self._current_valid_document_index
         _, document = self.current_subject.valid_documents[valid_document_index]
         self.viewer.title = (
@@ -277,14 +278,23 @@
         image_index = min(
             max(image_index, 0), len(self.current_subject.valid_documents) - 1
         )
         if not force and self._current_valid_document_index == image_index:
             return None
 
         self._current_valid_document_index = image_index
+
+        if not self.current_step.enabled(self.current_params):
+            self.current_step.close()
+            for step_index in reversed(range(self._current_step_index)):
+                if self.current_step.enabled(self.current_params):
+                    break
+                self._current_step_index = step_index
+            self.widget.set_step(self._current_step_index)
+
         self.widget.set_image_index(image_index + 1)
         self.widget.show_progress_bar()
 
         worker = create_worker(self._open_image)
         worker.returned.connect(self._open_step)
         worker.start()
         return worker
@@ -323,20 +333,20 @@
         run_async: bool = True,
     ) -> FunctionWorker | None:
         if not force and self._current_step_index == step_index:
             return
         if save_subject:
             self.save_subject()
         self.current_step.close()
+        self.widget.set_step(step_index)
         self._current_step_index = step_index
         if run_async:
             worker = create_worker(self._load_step_default_params)
             worker.returned.connect(self._open_step)
             worker.start()
-            self.widget.set_step(step_index)
             self.widget.show_progress_bar()
             return worker
         else:
             self._load_step_default_params()
             self._open_step()
 
     def prev_step(self, _=None) -> FunctionWorker | None:
```

### Comparing `napari_brainways-0.1/src/napari_brainways/conftest.py` & `napari_brainways-0.1.1/src/napari_brainways/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import replace
 from typing import Tuple
 
+from brainways.pipeline.atlas_registration import AtlasRegistrationParams
+from brainways.project.info_classes import BrainwaysParams
 from brainways.utils.test_utils import randomly_modified_params
 from pytest import fixture
 from pytestqt.qtbot import QtBot
 
 from napari_brainways.brainways_ui import BrainwaysUI
 from napari_brainways.controllers.affine_2d_controller import Affine2DController
 
@@ -65,7 +67,19 @@
         angle=modified_affine_params.angle,
         tx=modified_affine_params.tx,
         ty=modified_affine_params.ty,
         sx=modified_affine_params.sx,
         sy=modified_affine_params.sy,
     )
     assert controller.params == modified_params
+
+
+def test_enabled_false_by_default():
+    params = BrainwaysParams()
+    enabled = Affine2DController.enabled(params)
+    assert enabled is False
+
+
+def test_enabled_when_has_atlas():
+    params = BrainwaysParams(atlas=AtlasRegistrationParams())
+    enabled = Affine2DController.enabled(params)
+    assert enabled is True
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/_tests/test_tps_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/_tests/test_tps_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from dataclasses import replace
 from typing import Tuple
 from unittest.mock import patch
 
 import numpy as np
 import numpy.testing
 import pytest
+from brainways.pipeline.affine_2d import AffineTransform2DParams
 from brainways.pipeline.brainways_params import TPSTransformParams
+from brainways.project.info_classes import BrainwaysParams
 from pytest import fixture
 from pytestqt.qtbot import QtBot
 
 from napari_brainways.brainways_ui import BrainwaysUI
 from napari_brainways.controllers.tps_controller import TpsController
 from napari_brainways.test_utils import randomly_modified_params, worker_join
 
@@ -219,7 +221,19 @@
         tps=TPSTransformParams(np.random.rand(10, 2), np.random.rand(10, 2)),
     )
     controller.show(next_params1, from_ui=True)
     controller.previous_params()
     controller.show(next_params2, from_ui=True)
     controller.next_params()
     assert controller.params == next_params2
+
+
+def test_enabled_false_by_default():
+    params = BrainwaysParams()
+    enabled = TpsController.enabled(params)
+    assert enabled is False
+
+
+def test_enabled_with_affine_params():
+    params = BrainwaysParams(affine=AffineTransform2DParams())
+    enabled = TpsController.enabled(params)
+    assert enabled is True
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/affine_2d_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/affine_2d_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,18 @@
     def show_help(self, _=None):
         self.widget.show_help(key_bindings=self._key_bindings)
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
         return params.affine is not None
 
+    @staticmethod
+    def enabled(params: BrainwaysParams) -> bool:
+        return params.atlas is not None
+
     def default_params(
         self, image: np.ndarray, params: BrainwaysParams
     ) -> BrainwaysParams:
         return self.run_model(image=image, params=params)
 
     def run_model(self, image: np.ndarray, params: BrainwaysParams) -> BrainwaysParams:
         affine_params = self.pipeline.find_2d_affine_transform(
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/annotation_viewer_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/annotation_viewer_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     def run_model(self, image: np.ndarray, params: BrainwaysParams) -> BrainwaysParams:
         return params
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
         return True
 
+    @staticmethod
+    def enabled(params: BrainwaysParams) -> bool:
+        return params.tps is not None
+
     def open(self) -> None:
         if self._is_open:
             return
 
         self.input_layer = self.ui.viewer.add_image(np.zeros((10, 10)), name="Image")
         self.annotations_layer = self.ui.viewer.add_labels(
             np.zeros((10, 10), np.int32), name="Annotations"
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/base.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,19 @@
         ...
 
     @staticmethod
     @abstractmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
         ...
 
+    @staticmethod
+    @abstractmethod
+    def enabled(params: BrainwaysParams) -> bool:
+        ...
+
     def pipeline_loaded(self) -> None:
         pass
 
     @abstractmethod
     def run_model(self, image: np.ndarray, params: BrainwaysParams) -> BrainwaysParams:
         ...
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/cell_3d_viewer_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/cell_3d_viewer_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,18 @@
     ) -> BrainwaysParams:
         return params
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
         return True
 
+    @staticmethod
+    def enabled(params: BrainwaysParams) -> bool:
+        return params.tps is not None
+
     def run_model(self, image: np.ndarray, params: BrainwaysParams) -> BrainwaysParams:
         return params
 
     def _load_full_res_image(self):
         self._image = self.ui.current_subject.read_highres_image(
             self.ui.current_document
         )
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/cell_detector_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/cell_detector_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     def name(self) -> str:
         return "Cell Detection"
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
         return params.cell is not None
 
+    @staticmethod
+    def enabled(params: BrainwaysParams) -> bool:
+        return True
+
     def default_params(
         self, image: np.ndarray, params: BrainwaysParams
     ) -> BrainwaysParams:
         preview_bb = self.selected_bounding_box(
             image, point=(0.5 * image.shape[0], 0.5 * image.shape[1])
         )
         return replace(
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/registration_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/registration_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,18 @@
             self.ui.viewer.keymap.pop(key)
         self._key_bindings = None
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
         return params.atlas is not None
 
+    @staticmethod
+    def enabled(params: BrainwaysParams) -> bool:
+        return True
+
     def pipeline_loaded(self):
         self.widget.update_model(ap_min=0, ap_max=self.pipeline.atlas.shape[0] - 1)
 
     def default_params(
         self, image: np.ndarray, params: BrainwaysParams
     ) -> BrainwaysParams:
         if self.model_available():
@@ -142,15 +146,15 @@
     def on_run_model_button_click(self):
         if self.model_available():
             params = self.run_model(image=self._image, params=self._params)
             self.show(params)
 
     def model_available(self) -> bool:
         model_supports_atlas = (
-            self.ui.current_subject.atlas.brainglobe_atlas.atlas_name
+            self.ui.project.pipeline.atlas.brainglobe_atlas.atlas_name
             == "whs_sd_rat_39um"
         )
         return BRAINWAYS_REG_MODEL_AVAILABLE and model_supports_atlas
 
     def show(
         self,
         params: BrainwaysParams,
```

### Comparing `napari_brainways-0.1/src/napari_brainways/controllers/tps_controller.py` & `napari_brainways-0.1.1/src/napari_brainways/controllers/tps_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,18 @@
     def show_help(self, _=None):
         self.widget.show_help(key_bindings=self._key_bindings)
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
         return params.tps is not None
 
+    @staticmethod
+    def enabled(params: BrainwaysParams) -> bool:
+        return params.affine is not None
+
     def run_model(self, image: np.ndarray, params: BrainwaysParams) -> BrainwaysParams:
         affine_image = self.pipeline.transform_image(
             image=image, params=params, until_step=PipelineStep.AFFINE_2D
         )
         atlas_slice = self.pipeline.get_atlas_slice(params)
         return self.pipeline.tps.find_registration_params(
             image=affine_image, atlas_slice=atlas_slice, params=params
```

### Comparing `napari_brainways-0.1/src/napari_brainways/napari.yaml` & `napari_brainways-0.1.1/src/napari_brainways/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/napari_reader.py` & `napari_brainways-0.1.1/src/napari_brainways/napari_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/resources/logo.png` & `napari_brainways-0.1.1/src/napari_brainways/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/test_utils.py` & `napari_brainways-0.1.1/src/napari_brainways/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/utils.py` & `napari_brainways-0.1.1/src/napari_brainways/utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/_tests/test_create_project_dialog.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/_tests/test_create_project_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/_tests/test_registration_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/_tests/test_registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/affine_2d_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/affine_2d_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/cell_detector_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/cell_detector_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/cell_viewer_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/cell_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/create_subject_dialog.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/create_subject_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/registration_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/tps_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/tps_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1/src/napari_brainways/widgets/workflow_widget.py` & `napari_brainways-0.1.1/src/napari_brainways/widgets/workflow_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from pathlib import Path
 from typing import Callable, List, Union
 
 import importlib_resources
 import PIL.Image
 from bg_atlasapi.list_atlases import get_all_atlases_lastversions
+from brainways.pipeline.brainways_params import BrainwaysParams
 from brainways.project.brainways_project import BrainwaysProject
 from brainways.project.info_classes import ExcelMode, ProjectSettings
 from brainways.utils.cell_detection_importer.utils import (
     cell_detection_importer_types,
     get_cell_detection_importer,
 )
 from magicgui import magicgui
@@ -192,14 +193,15 @@
             return
         self._prev_path = str(Path(path).parent)
         self.controller.open_project_async(Path(path))
 
     def on_project_changed(self, n_subjects: int):
         self.project_buttons.project_opened()
         self.subject_navigation.project_opened(n_subjects)
+        self.step_buttons.update_enabled(self.controller.current_params)
         self.set_step(0)
 
     def on_subject_changed(self):
         self.image_navigation.max = self.controller.subject_size
         self.subject_controls.show()
 
     def select_subject(self, value: int):
@@ -369,14 +371,17 @@
         self.progress_bar.max = max_value
         self.header_section.show_progress()
 
     def hide_progress_bar(self):
         self.all_widgets.setEnabled(True)
         self.header_section.hide_progress()
 
+    def update_enabled_steps(self):
+        self.step_buttons.update_enabled(self.controller.current_params)
+
 
 class TitledGroupBox(QWidget):
     def __init__(
         self,
         title: Union[str, QLabel],
         widgets: List[QWidget | None],
         layout: str = "vertical",
@@ -571,28 +576,33 @@
 
     def project_closed(self, n_subjects: int):
         self.visible = False
 
 
 class StepButtons(TitledGroupBox):
     def __init__(self, steps: List[Controller], clicked: Callable, title: str):
+        self.steps = steps
         self.buttons = []
         for i, step in enumerate(steps):
             button = QPushButton(step.name)
             button.clicked.connect(functools.partial(clicked, step_index=i))
             button.clicked.connect(functools.partial(self.set_step, step_index=i))
             button.setCheckable(True)
             self.buttons.append(button)
 
         super().__init__(title=title, widgets=self.buttons)
 
     def set_step(self, step_index: int):
         for i, button in enumerate(self.buttons):
             button.setChecked(i == step_index)
 
+    def update_enabled(self, params: BrainwaysParams):
+        for step, button in zip(self.steps, self.buttons):
+            button.setEnabled(step.enabled(params))
+
 
 class StepControls(TitledGroupBox):
     def __init__(self, steps: List[Controller]):
         self.steps = steps
         self.title = QLabel("")
         self.widgets = [step.widget for step in steps]
         super().__init__(title=self.title, widgets=self.widgets)
```

### Comparing `napari_brainways-0.1/src/napari_brainways.egg-info/PKG-INFO` & `napari_brainways-0.1.1/src/napari_brainways.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-brainways
-Version: 0.1
+Version: 0.1.1
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1/src/napari_brainways.egg-info/SOURCES.txt` & `napari_brainways-0.1.1/src/napari_brainways.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 src/napari_brainways/controllers/annotation_viewer_controller.py
 src/napari_brainways/controllers/base.py
 src/napari_brainways/controllers/cell_3d_viewer_controller.py
 src/napari_brainways/controllers/cell_detector_controller.py
 src/napari_brainways/controllers/registration_controller.py
 src/napari_brainways/controllers/tps_controller.py
 src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
+src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
+src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
+src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
+src/napari_brainways/controllers/_tests/test_registration_controller.py
 src/napari_brainways/controllers/_tests/test_tps_controller.py
 src/napari_brainways/resources/logo.png
 src/napari_brainways/widgets/__init__.py
 src/napari_brainways/widgets/affine_2d_widget.py
 src/napari_brainways/widgets/cell_detector_widget.py
 src/napari_brainways/widgets/cell_viewer_widget.py
 src/napari_brainways/widgets/create_subject_dialog.py
```

### Comparing `napari_brainways-0.1/tox.ini` & `napari_brainways-0.1.1/tox.ini`

 * *Files identical despite different names*


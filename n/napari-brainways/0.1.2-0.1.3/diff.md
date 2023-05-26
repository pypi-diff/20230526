# Comparing `tmp/napari_brainways-0.1.2.tar.gz` & `tmp/napari_brainways-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_brainways-0.1.2.tar", last modified: Fri May 26 15:20:01 2023, max compression
+gzip compressed data, was "napari_brainways-0.1.3.tar", last modified: Fri May 26 15:40:39 2023, max compression
```

## Comparing `napari_brainways-0.1.2.tar` & `napari_brainways-0.1.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.234473 napari_brainways-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.222473 napari_brainways-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.222473 napari_brainways-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.226473 napari_brainways-0.1.2/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 15:20:01.234473 napari_brainways-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.226473 napari_brainways-0.1.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/data/test_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 15:20:01.234473 napari_brainways-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.222473 napari_brainways-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.226473 napari_brainways-0.1.2/src/napari_brainways/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.230473 napari_brainways-0.1.2/src/napari_brainways/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 15:20:01.000000 napari_brainways-0.1.2/src/napari_brainways/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/brainways_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.230473 napari_brainways-0.1.2/src/napari_brainways/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.230473 napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/controllers/tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/napari_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.230473 napari_brainways-0.1.2/src/napari_brainways/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.234473 napari_brainways-0.1.2/src/napari_brainways/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.234473 napari_brainways-0.1.2/src/napari_brainways/widgets/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/_tests/test_registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/affine_2d_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/cell_detector_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/cell_viewer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/create_subject_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/tps_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/src/napari_brainways/widgets/workflow_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:20:01.226473 napari_brainways-0.1.2/src/napari_brainways.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 15:20:01.000000 napari_brainways-0.1.2/src/napari_brainways.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-26 15:20:01.000000 napari_brainways-0.1.2/src/napari_brainways.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:20:01.000000 napari_brainways-0.1.2/src/napari_brainways.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 15:20:01.000000 napari_brainways-0.1.2/src/napari_brainways.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 15:20:01.000000 napari_brainways-0.1.2/src/napari_brainways.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:20:01.000000 napari_brainways-0.1.2/src/napari_brainways.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 15:19:37.000000 napari_brainways-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.867291 napari_brainways-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/data/test_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.867291 napari_brainways-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/src/napari_brainways/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/src/napari_brainways/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/brainways_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/napari_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/affine_2d_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/cell_detector_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/cell_viewer_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/create_subject_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/tps_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/workflow_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/src/napari_brainways.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/tox.ini
```

### Comparing `napari_brainways-0.1.2/.github/workflows/test_and_deploy.yml` & `napari_brainways-0.1.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/.gitignore` & `napari_brainways-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/.napari/DESCRIPTION.md` & `napari_brainways-0.1.3/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/.pre-commit-config.yaml` & `napari_brainways-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/LICENSE` & `napari_brainways-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/PKG-INFO` & `napari_brainways-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_brainways
-Version: 0.1.2
+Version: 0.1.3
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.2/README.md` & `napari_brainways-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/data/test_data.npz` & `napari_brainways-0.1.3/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/setup.cfg` & `napari_brainways-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/_sample_data.py` & `napari_brainways-0.1.3/src/napari_brainways/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/_tests/test_reader.py` & `napari_brainways-0.1.3/src/napari_brainways/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/_tests/test_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/brainways_ui.py` & `napari_brainways-0.1.3/src/napari_brainways/brainways_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,15 @@
         self._set_title()
         self._register_keybinds()
         self.widget.on_subject_changed()
         for step in self.steps:
             step.pipeline_loaded()
         self.current_step.open()
         self.current_step.show(self.current_params, self._image)
+        self.widget.update_enabled_steps()
         self.widget.hide_progress_bar()
 
     def _on_progress_returned(self):
         self.widget.hide_progress_bar()
 
     def persist_current_params(self):
         self.current_document = replace(
```

### Comparing `napari_brainways-0.1.2/src/napari_brainways/conftest.py` & `napari_brainways-0.1.3/src/napari_brainways/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/_tests/test_tps_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/affine_2d_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/annotation_viewer_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/base.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/base.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/cell_3d_viewer_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/cell_detector_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/cell_detector_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/registration_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/registration_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/controllers/tps_controller.py` & `napari_brainways-0.1.3/src/napari_brainways/controllers/tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/napari.yaml` & `napari_brainways-0.1.3/src/napari_brainways/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/napari_reader.py` & `napari_brainways-0.1.3/src/napari_brainways/napari_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/resources/logo.png` & `napari_brainways-0.1.3/src/napari_brainways/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/test_utils.py` & `napari_brainways-0.1.3/src/napari_brainways/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/utils.py` & `napari_brainways-0.1.3/src/napari_brainways/utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/_tests/test_create_project_dialog.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_create_project_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/_tests/test_registration_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/affine_2d_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/affine_2d_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/cell_detector_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/cell_detector_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/cell_viewer_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/cell_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/create_subject_dialog.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/create_subject_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/registration_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/tps_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/tps_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/src/napari_brainways/widgets/workflow_widget.py` & `napari_brainways-0.1.3/src/napari_brainways/widgets/workflow_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,14 @@
             return
         self._prev_path = str(Path(path).parent)
         self.controller.open_project_async(Path(path))
 
     def on_project_changed(self, n_subjects: int):
         self.project_buttons.project_opened()
         self.subject_navigation.project_opened(n_subjects)
-        if n_subjects > 0:
-            self.step_buttons.update_enabled(self.controller.current_params)
         self.set_step(0)
 
     def on_subject_changed(self):
         self.image_navigation.max = self.controller.subject_size
         self.subject_controls.show()
 
     def select_subject(self, value: int):
```

### Comparing `napari_brainways-0.1.2/src/napari_brainways.egg-info/PKG-INFO` & `napari_brainways-0.1.3/src/napari_brainways.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-brainways
-Version: 0.1.2
+Version: 0.1.3
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.2/src/napari_brainways.egg-info/SOURCES.txt` & `napari_brainways-0.1.3/src/napari_brainways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.2/tox.ini` & `napari_brainways-0.1.3/tox.ini`

 * *Files identical despite different names*


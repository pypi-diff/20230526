# Comparing `tmp/brainways-0.1.tar.gz` & `tmp/brainways-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainways-0.1.tar", last modified: Fri May 26 08:27:19 2023, max compression
+gzip compressed data, was "brainways-0.1.1.tar", last modified: Fri May 26 13:54:23 2023, max compression
```

## Comparing `brainways-0.1.tar` & `brainways-0.1.1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.749876 brainways-0.1/
--rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1/.editorconfig
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.729876 brainways-0.1/.github/
--rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1/.gitignore
--rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1/.pre-commit-config.yaml
--rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1/.travis.yml
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1/AUTHORS.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1/CONTRIBUTING.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1/HISTORY.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1/LICENSE
--rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1/MANIFEST.in
--rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1/Makefile
--rw-rw-r--   0 ben       (1001) ben       (1001)     2341 2023-05-26 08:27:19.749876 brainways-0.1/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1/README.rst
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.729876 brainways-0.1/data/
--rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1/data/test_data.npz
--rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1/data/test_image.jpg
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.733876 brainways-0.1/docs/
--rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1/docs/Makefile
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.725876 brainways-0.1/docs/_build/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.725876 brainways-0.1/docs/_build/html/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.733876 brainways-0.1/docs/_build/html/_static/
--rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1/docs/authors.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.elastix.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.pipeline.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.project.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1/docs/brainways.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.scripts.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.transforms.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.utils.atlas.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.utils.cell_detection_importer.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.utils.czi.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.utils.io_utils.file_iterators.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.utils.io_utils.readers.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.utils.io_utils.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1/docs/brainways.utils.rst
--rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1/docs/conf.py
--rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1/docs/contributing.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1/docs/history.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1/docs/index.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1/docs/installation.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1/docs/make.bat
--rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1/docs/modules.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1/docs/readme.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1/docs/usage.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1/pyproject.toml
--rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1/requirements_dev.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-05-26 08:27:19.749876 brainways-0.1/setup.cfg
--rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1/setup.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.725876 brainways-0.1/src/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.733876 brainways-0.1/src/brainways/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1/src/brainways/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      155 2023-05-26 08:27:19.000000 brainways-0.1/src/brainways/_version.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7068 2022-11-30 13:46:38.000000 brainways-0.1/src/brainways/conftest.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.733876 brainways-0.1/src/brainways/elastix/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1/src/brainways/elastix/Par0033bspline.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1/src/brainways/elastix/Par0033similarity.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1/src/brainways/elastix/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.733876 brainways-0.1/src/brainways/elastix/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1/src/brainways/elastix/_tests/test_elastix.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1/src/brainways/elastix/elastix.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.737876 brainways-0.1/src/brainways/pipeline/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1/src/brainways/pipeline/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.737876 brainways-0.1/src/brainways/pipeline/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1/src/brainways/pipeline/_tests/test_atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1/src/brainways/pipeline/_tests/test_brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1/src/brainways/pipeline/affine_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1/src/brainways/pipeline/atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1231 2023-01-25 12:05:30.000000 brainways-0.1/src/brainways/pipeline/brainways_params.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1/src/brainways/pipeline/brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4123 2023-04-30 11:04:32.000000 brainways-0.1/src/brainways/pipeline/cell_detector.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1/src/brainways/pipeline/tps.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.737876 brainways-0.1/src/brainways/project/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1/src/brainways/project/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.737876 brainways-0.1/src/brainways/project/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1/src/brainways/project/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      615 2022-11-23 13:20:41.000000 brainways-0.1/src/brainways/project/_tests/conftest.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1951 2022-11-24 12:49:33.000000 brainways-0.1/src/brainways/project/_tests/test_brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8844 2022-11-23 13:20:41.000000 brainways-0.1/src/brainways/project/_tests/test_brainways_subject.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8262 2023-05-18 10:57:16.000000 brainways-0.1/src/brainways/project/brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    18817 2023-05-07 14:18:30.000000 brainways-0.1/src/brainways/project/brainways_subject.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1277 2023-05-17 07:54:03.000000 brainways-0.1/src/brainways/project/info_classes.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.741876 brainways-0.1/src/brainways/scripts/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1/src/brainways/scripts/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.741876 brainways-0.1/src/brainways/scripts/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1/src/brainways/scripts/_tests/test_cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1/src/brainways/scripts/batch_create_thumbnails.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1/src/brainways/scripts/cell_detection.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1/src/brainways/scripts/cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1/src/brainways/scripts/create_excel.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1/src/brainways/scripts/create_excel_colabelling.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1/src/brainways/scripts/create_reg_model_data.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1/src/brainways/scripts/display_area.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1/src/brainways/scripts/import_cell_detections_keren.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1/src/brainways/scripts/import_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1/src/brainways/scripts/move_images.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.741876 brainways-0.1/src/brainways/transforms/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1/src/brainways/transforms/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.741876 brainways-0.1/src/brainways/transforms/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1/src/brainways/transforms/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1/src/brainways/transforms/_tests/test_affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1/src/brainways/transforms/_tests/test_depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1/src/brainways/transforms/_tests/test_tps_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1/src/brainways/transforms/affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1/src/brainways/transforms/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1/src/brainways/transforms/compose.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1/src/brainways/transforms/depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1/src/brainways/transforms/image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1/src/brainways/transforms/tps_transform.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1/src/brainways/utils/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1/src/brainways/utils/_imports.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1/src/brainways/utils/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1/src/brainways/utils/_tests/test_cell_count_summary.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1/src/brainways/utils/_tests/test_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1/src/brainways/utils/_tests/test_image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/atlas/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1/src/brainways/utils/atlas/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/atlas/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1/src/brainways/utils/atlas/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1/src/brainways/utils/atlas/_tests/test_slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4263 2022-12-11 16:13:39.000000 brainways-0.1/src/brainways/utils/atlas/brainways_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1/src/brainways/utils/atlas/slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1/src/brainways/utils/cell_count_summary.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/cell_detection_importer/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/cell_detection_importer/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1/src/brainways/utils/cell_detection_importer/utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1/src/brainways/utils/cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1/src/brainways/utils/config.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/czi/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1/src/brainways/utils/czi/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1/src/brainways/utils/czi/czi_to_jpg.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1/src/brainways/utils/dataclasses.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     9024 2023-05-24 15:16:48.000000 brainways-0.1/src/brainways/utils/image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/io_utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1/src/brainways/utils/io_utils/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.745876 brainways-0.1/src/brainways/utils/io_utils/file_iterators/
--rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1/src/brainways/utils/io_utils/file_iterators/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1/src/brainways/utils/io_utils/file_iterators/image_entry.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1/src/brainways/utils/io_utils/file_iterators/path.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1/src/brainways/utils/io_utils/file_iterators/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1/src/brainways/utils/io_utils/image_path.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.749876 brainways-0.1/src/brainways/utils/io_utils/readers/
--rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1/src/brainways/utils/io_utils/readers/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.749876 brainways-0.1/src/brainways/utils/io_utils/readers/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1/src/brainways/utils/io_utils/readers/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1/src/brainways/utils/io_utils/readers/czi_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1/src/brainways/utils/io_utils/readers/qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1/src/brainways/utils/paths.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1/src/brainways/utils/preprocess.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1/src/brainways/utils/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1/src/brainways/utils/test_utils.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 08:27:19.733876 brainways-0.1/src/brainways.egg-info/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2341 2023-05-26 08:27:19.000000 brainways-0.1/src/brainways.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)     5332 2023-05-26 08:27:19.000000 brainways-0.1/src/brainways.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-05-26 08:27:19.000000 brainways-0.1/src/brainways.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-05-26 08:27:19.000000 brainways-0.1/src/brainways.egg-info/entry_points.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-05-26 08:27:19.000000 brainways-0.1/src/brainways.egg-info/requires.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-05-26 08:27:19.000000 brainways-0.1/src/brainways.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1/tox.ini
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.1/.editorconfig
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.938592 brainways-0.1.1/.github/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.1/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.1/.gitignore
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.1/.travis.yml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.1/AUTHORS.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.1/HISTORY.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.1/LICENSE
+-rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.1/MANIFEST.in
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.1/Makefile
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-05-26 13:54:23.958592 brainways-0.1.1/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.1/README.rst
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/data/
+-rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.1/data/test_data.npz
+-rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.1/data/test_image.jpg
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/docs/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/Makefile
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.934592 brainways-0.1.1/docs/_build/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.934592 brainways-0.1.1/docs/_build/html/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/docs/_build/html/_static/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/authors.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.elastix.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.pipeline.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.project.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.1/docs/brainways.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.scripts.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.transforms.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.atlas.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.cell_detection_importer.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.czi.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.io_utils.file_iterators.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.io_utils.readers.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.io_utils.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.rst
+-rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.1/docs/conf.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/contributing.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/history.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/index.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/installation.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/make.bat
+-rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.1/docs/modules.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/readme.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/usage.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.1/pyproject.toml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.1/requirements_dev.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-05-26 13:54:23.958592 brainways-0.1.1/setup.cfg
+-rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.1/setup.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.934592 brainways-0.1.1/src/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/src/brainways/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.1/src/brainways/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways/_version.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7068 2022-11-30 13:46:38.000000 brainways-0.1.1/src/brainways/conftest.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/elastix/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.1/src/brainways/elastix/Par0033bspline.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.1/src/brainways/elastix/Par0033similarity.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.1/src/brainways/elastix/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/elastix/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.1/src/brainways/elastix/_tests/test_elastix.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.1/src/brainways/elastix/elastix.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/pipeline/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/pipeline/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/pipeline/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.1/src/brainways/pipeline/_tests/test_atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.1/src/brainways/pipeline/_tests/test_brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.1/src/brainways/pipeline/affine_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.1/src/brainways/pipeline/atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1231 2023-01-25 12:05:30.000000 brainways-0.1.1/src/brainways/pipeline/brainways_params.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.1/src/brainways/pipeline/brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4123 2023-04-30 11:04:32.000000 brainways-0.1.1/src/brainways/pipeline/cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.1/src/brainways/pipeline/tps.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/project/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/project/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/project/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.1/src/brainways/project/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      615 2022-11-23 13:20:41.000000 brainways-0.1.1/src/brainways/project/_tests/conftest.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1951 2022-11-24 12:49:33.000000 brainways-0.1.1/src/brainways/project/_tests/test_brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8844 2022-11-23 13:20:41.000000 brainways-0.1.1/src/brainways/project/_tests/test_brainways_subject.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8262 2023-05-18 10:57:16.000000 brainways-0.1.1/src/brainways/project/brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    18817 2023-05-07 14:18:30.000000 brainways-0.1.1/src/brainways/project/brainways_subject.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1277 2023-05-17 07:54:03.000000 brainways-0.1.1/src/brainways/project/info_classes.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/scripts/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.1/src/brainways/scripts/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/scripts/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.1/src/brainways/scripts/_tests/test_cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.1/src/brainways/scripts/batch_create_thumbnails.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.1/src/brainways/scripts/cell_detection.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.1/src/brainways/scripts/cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.1/src/brainways/scripts/create_excel.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.1/src/brainways/scripts/create_excel_colabelling.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.1/src/brainways/scripts/create_reg_model_data.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.1/src/brainways/scripts/display_area.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.1/src/brainways/scripts/import_cell_detections_keren.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.1/src/brainways/scripts/import_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.1/src/brainways/scripts/move_images.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/transforms/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.1/src/brainways/transforms/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/transforms/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.1/src/brainways/transforms/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_tps_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.1/src/brainways/transforms/affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.1/src/brainways/transforms/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.1/src/brainways/transforms/compose.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.1/src/brainways/transforms/image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.1/src/brainways/transforms/tps_transform.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.1/src/brainways/utils/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.1/src/brainways/utils/_imports.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.1/src/brainways/utils/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.1/src/brainways/utils/_tests/test_cell_count_summary.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.1/src/brainways/utils/_tests/test_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/utils/_tests/test_image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/atlas/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.1/src/brainways/utils/atlas/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/atlas/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.1/src/brainways/utils/atlas/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.1/src/brainways/utils/atlas/_tests/test_slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4263 2022-12-11 16:13:39.000000 brainways-0.1.1/src/brainways/utils/atlas/brainways_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.1/src/brainways/utils/atlas/slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.1/src/brainways/utils/cell_count_summary.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/cell_detection_importer/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.1/src/brainways/utils/cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.1/src/brainways/utils/config.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/czi/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.1/src/brainways/utils/czi/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/utils/czi/czi_to_jpg.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.1/src/brainways/utils/dataclasses.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.1/src/brainways/utils/image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.1/src/brainways/utils/io_utils/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/image_entry.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/path.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.1/src/brainways/utils/io_utils/image_path.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/readers/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/readers/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/czi_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.1/src/brainways/utils/paths.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/utils/preprocess.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.1/src/brainways/utils/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.1/src/brainways/utils/test_utils.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways.egg-info/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5332 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/entry_points.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/top_level.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.1/tox.ini
```

### Comparing `brainways-0.1/.gitignore` & `brainways-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `brainways-0.1/.pre-commit-config.yaml` & `brainways-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainways-0.1/.travis.yml` & `brainways-0.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `brainways-0.1/CONTRIBUTING.rst` & `brainways-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/LICENSE` & `brainways-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brainways-0.1/Makefile` & `brainways-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1/PKG-INFO` & `brainways-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1
+Version: 0.1.1
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1/README.rst` & `brainways-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/data/test_data.npz` & `brainways-0.1.1/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `brainways-0.1/data/test_image.jpg` & `brainways-0.1.1/data/test_image.jpg`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/Makefile` & `brainways-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.pipeline.rst` & `brainways-0.1.1/docs/brainways.pipeline.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.project.rst` & `brainways-0.1.1/docs/brainways.project.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.scripts.rst` & `brainways-0.1.1/docs/brainways.scripts.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.transforms.rst` & `brainways-0.1.1/docs/brainways.transforms.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.utils.atlas.rst` & `brainways-0.1.1/docs/brainways.utils.atlas.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.utils.cell_detection_importer.rst` & `brainways-0.1.1/docs/brainways.utils.cell_detection_importer.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.utils.io_utils.file_iterators.rst` & `brainways-0.1.1/docs/brainways.utils.io_utils.file_iterators.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.utils.io_utils.readers.rst` & `brainways-0.1.1/docs/brainways.utils.io_utils.readers.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.utils.io_utils.rst` & `brainways-0.1.1/docs/brainways.utils.io_utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/brainways.utils.rst` & `brainways-0.1.1/docs/brainways.utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/conf.py` & `brainways-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/installation.rst` & `brainways-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1/docs/make.bat` & `brainways-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `brainways-0.1/setup.cfg` & `brainways-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/conftest.py` & `brainways-0.1.1/src/brainways/conftest.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/elastix/Par0033bspline.txt` & `brainways-0.1.1/src/brainways/elastix/Par0033bspline.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/elastix/Par0033similarity.txt` & `brainways-0.1.1/src/brainways/elastix/Par0033similarity.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/elastix/_tests/test_elastix.py` & `brainways-0.1.1/src/brainways/elastix/_tests/test_elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/elastix/elastix.py` & `brainways-0.1.1/src/brainways/elastix/elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/pipeline/_tests/test_brainways_pipeline.py` & `brainways-0.1.1/src/brainways/pipeline/_tests/test_brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/pipeline/affine_2d.py` & `brainways-0.1.1/src/brainways/pipeline/affine_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/pipeline/atlas_registration.py` & `brainways-0.1.1/src/brainways/pipeline/atlas_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/pipeline/brainways_params.py` & `brainways-0.1.1/src/brainways/pipeline/brainways_params.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/pipeline/brainways_pipeline.py` & `brainways-0.1.1/src/brainways/pipeline/brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/pipeline/cell_detector.py` & `brainways-0.1.1/src/brainways/pipeline/cell_detector.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/pipeline/tps.py` & `brainways-0.1.1/src/brainways/pipeline/tps.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/project/_tests/conftest.py` & `brainways-0.1.1/src/brainways/project/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/project/_tests/test_brainways_project.py` & `brainways-0.1.1/src/brainways/project/_tests/test_brainways_project.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/project/_tests/test_brainways_subject.py` & `brainways-0.1.1/src/brainways/project/_tests/test_brainways_subject.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/project/brainways_project.py` & `brainways-0.1.1/src/brainways/project/brainways_project.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/project/brainways_subject.py` & `brainways-0.1.1/src/brainways/project/brainways_subject.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/project/info_classes.py` & `brainways-0.1.1/src/brainways/project/info_classes.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/_tests/test_cli.py` & `brainways-0.1.1/src/brainways/scripts/_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/batch_create_thumbnails.py` & `brainways-0.1.1/src/brainways/scripts/batch_create_thumbnails.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/cell_detection.py` & `brainways-0.1.1/src/brainways/scripts/cell_detection.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/cli.py` & `brainways-0.1.1/src/brainways/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/create_excel.py` & `brainways-0.1.1/src/brainways/scripts/create_excel.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/create_excel_colabelling.py` & `brainways-0.1.1/src/brainways/scripts/create_excel_colabelling.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/create_reg_model_data.py` & `brainways-0.1.1/src/brainways/scripts/create_reg_model_data.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/display_area.py` & `brainways-0.1.1/src/brainways/scripts/display_area.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/import_cell_detections_keren.py` & `brainways-0.1.1/src/brainways/scripts/import_cell_detections_keren.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/import_cells.py` & `brainways-0.1.1/src/brainways/scripts/import_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/scripts/move_images.py` & `brainways-0.1.1/src/brainways/scripts/move_images.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/_tests/test_affine_transform_2d.py` & `brainways-0.1.1/src/brainways/transforms/_tests/test_affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/_tests/test_depth_registration.py` & `brainways-0.1.1/src/brainways/transforms/_tests/test_depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/_tests/test_image_to_atlas_transform.py` & `brainways-0.1.1/src/brainways/transforms/_tests/test_image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/_tests/test_tps_transform.py` & `brainways-0.1.1/src/brainways/transforms/_tests/test_tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/affine_transform_2d.py` & `brainways-0.1.1/src/brainways/transforms/affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/compose.py` & `brainways-0.1.1/src/brainways/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/depth_registration.py` & `brainways-0.1.1/src/brainways/transforms/depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/image_to_atlas_transform.py` & `brainways-0.1.1/src/brainways/transforms/image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/transforms/tps_transform.py` & `brainways-0.1.1/src/brainways/transforms/tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/_imports.py` & `brainways-0.1.1/src/brainways/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/_tests/test_cell_count_summary.py` & `brainways-0.1.1/src/brainways/utils/_tests/test_cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/_tests/test_cells.py` & `brainways-0.1.1/src/brainways/utils/_tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/_tests/test_image.py` & `brainways-0.1.1/src/brainways/utils/_tests/test_image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/atlas/_tests/test_slice_atlas.py` & `brainways-0.1.1/src/brainways/utils/atlas/_tests/test_slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/atlas/brainways_atlas.py` & `brainways-0.1.1/src/brainways/utils/atlas/brainways_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/atlas/slice_atlas.py` & `brainways-0.1.1/src/brainways/utils/atlas/slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cell_count_summary.py` & `brainways-0.1.1/src/brainways/utils/cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt` & `brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py` & `brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py` & `brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py` & `brainways-0.1.1/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py` & `brainways-0.1.1/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cell_detection_importer/utils.py` & `brainways-0.1.1/src/brainways/utils/cell_detection_importer/utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/cells.py` & `brainways-0.1.1/src/brainways/utils/cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/config.py` & `brainways-0.1.1/src/brainways/utils/config.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/czi/czi_to_jpg.py` & `brainways-0.1.1/src/brainways/utils/czi/czi_to_jpg.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/dataclasses.py` & `brainways-0.1.1/src/brainways/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/image.py` & `brainways-0.1.1/src/brainways/utils/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     return image
 
 
 def brain_mask(image: np.ndarray):
     # quantize image to black and white
     h, w = image.shape[:2]
     image_flat = image.reshape((h * w, 1))
-    min_pixel_value, max_pixel_value = np.quantile(image, (0, 0.5))
+    min_pixel_value, max_pixel_value = np.quantile(image, (0, 0.85))
     image_flat = np.clip(image_flat, min_pixel_value, max_pixel_value)
     kmeans = MiniBatchKMeans(n_init="auto", n_clusters=2, batch_size=2048)
     labels = kmeans.fit_predict(image_flat)
     labels_order = kmeans.cluster_centers_.flatten().argsort()
     quantized = labels_order[labels].astype("uint8").reshape((h, w))
 
     if (quantized == 0).all():
```

### Comparing `brainways-0.1/src/brainways/utils/io_utils/file_iterators/qupath.py` & `brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/io_utils/image_path.py` & `brainways-0.1.1/src/brainways/utils/io_utils/image_path.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/io_utils/readers/__init__.py` & `brainways-0.1.1/src/brainways/utils/io_utils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/io_utils/readers/aicsimageio_reader.py` & `brainways-0.1.1/src/brainways/utils/io_utils/readers/aicsimageio_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/io_utils/readers/base.py` & `brainways-0.1.1/src/brainways/utils/io_utils/readers/base.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/io_utils/readers/czi_reader.py` & `brainways-0.1.1/src/brainways/utils/io_utils/readers/czi_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/io_utils/readers/qupath_reader.py` & `brainways-0.1.1/src/brainways/utils/io_utils/readers/qupath_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/preprocess.py` & `brainways-0.1.1/src/brainways/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/qupath.py` & `brainways-0.1.1/src/brainways/utils/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways/utils/test_utils.py` & `brainways-0.1.1/src/brainways/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1/src/brainways.egg-info/PKG-INFO` & `brainways-0.1.1/src/brainways.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1
+Version: 0.1.1
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1/src/brainways.egg-info/SOURCES.txt` & `brainways-0.1.1/src/brainways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1/tox.ini` & `brainways-0.1.1/tox.ini`

 * *Files identical despite different names*


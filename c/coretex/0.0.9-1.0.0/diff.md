# Comparing `tmp/coretex-0.0.9.tar.gz` & `tmp/coretex-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-0.0.9.tar", last modified: Tue Feb 14 14:03:55 2023, max compression
+gzip compressed data, was "coretex-1.0.0.tar", last modified: Fri May 26 00:03:11 2023, max compression
```

## Comparing `coretex-0.0.9.tar` & `coretex-1.0.0.tar`

### file list

```diff
@@ -1,149 +1,179 @@
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.925225 coretex-0.0.9/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      805 2023-02-14 14:03:55.921226 coretex-0.0.9/PKG-INFO
--rw-r--r--   0 jenkins    (113) jenkins    (119)       57 2023-02-10 09:27:35.000000 coretex-0.0.9/README.md
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1200 2023-02-14 14:03:49.000000 coretex-0.0.9/pyproject.toml
--rw-r--r--   0 jenkins    (113) jenkins    (119)       38 2023-02-14 14:03:55.925225 coretex-0.0.9/setup.cfg
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.901227 coretex-0.0.9/src/
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.905227 coretex-0.0.9/src/coretex/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       40 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/__init__.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/cache/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       97 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/cache/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     5462 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/cache/cache_module.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/codable/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       67 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/codable/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     6538 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/codable/codable.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      658 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/codable/descriptor.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/context/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       50 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/context/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     3550 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/context/experiment_context.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/coretex/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      139 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/__init__.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/coretex/annotation/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       21 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/annotation/__init__.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/coretex/annotation/image/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      170 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/annotation/image/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1619 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/annotation/image/bbox.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2524 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/annotation/image/classes_format.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2805 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/annotation/image/coretex_format.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/coretex/conversion/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       31 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2768 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/base_converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      703 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1444 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converter_processor_factory.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex/coretex/conversion/converters/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      385 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     3660 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/city_scape_converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     3672 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/coco_converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2707 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/create_ml_converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     4891 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2566 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.913226 coretex-0.0.9/src/coretex/coretex/conversion/converters/pascal/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       54 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/pascal/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)    10756 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2512 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      964 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/pascal/shared.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2961 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/voc_converter.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     4849 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.913226 coretex-0.0.9/src/coretex/coretex/dataset/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      477 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/__init__.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.913226 coretex-0.0.9/src/coretex/coretex/dataset/custom_dataset/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       95 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/custom_dataset/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)       34 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/custom_dataset/base.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      472 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      310 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1893 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/dataset.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.913226 coretex-0.0.9/src/coretex/coretex/dataset/image_dataset/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      154 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_dataset/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1366 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_dataset/base.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2285 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      842 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     8170 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.913226 coretex-0.0.9/src/coretex/coretex/dataset/image_segmentation_dataset/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      141 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      455 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      309 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1420 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/local_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     3737 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/network_dataset.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.913226 coretex-0.0.9/src/coretex/coretex/dataset/object_detection_dataset/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      130 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/object_detection_dataset/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      296 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/object_detection_dataset/local_object_detection_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      447 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/object_detection_dataset/object_detection_dataset.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      329 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/dataset/utils.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/experiment/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      103 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/experiment/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     3834 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/experiment/artifact.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     7016 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/experiment/experiment.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1300 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/experiment/status.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/item/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      431 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      299 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/any_local_item.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/item/custom_item/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       83 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/custom_item/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1053 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/custom_item/custom_item.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      138 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/custom_item/custom_item_data.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      244 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/custom_item/local_custom_item.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/item/image_item/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      131 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_item/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      215 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_item/image_format.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2056 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_item/image_item.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1611 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_item/image_item_data.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      962 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_item/local_image_item.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/item/image_segmentation_item/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      129 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_segmentation_item/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      726 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_segmentation_item/image_segmentation_item.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      137 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/image_segmentation_item/local_image_segmentation_item.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1808 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/item.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      773 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/local_item.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2090 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/network_item.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/item/object_detection_item/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      121 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/object_detection_item/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      135 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/object_detection_item/local_object_detection_item.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      718 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/item/object_detection_item/object_detection_item.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/model/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       25 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/model/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     4606 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/model/model.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.917226 coretex-0.0.9/src/coretex/coretex/project/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      100 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/project/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1911 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/project/base.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1705 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/project/project.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      388 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/project/project_task.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1189 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/coretex/project/workspace.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.921226 coretex-0.0.9/src/coretex/folder_management/
--rw-r--r--   0 jenkins    (113) jenkins    (119)       42 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/folder_management/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2373 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/folder_management/folder_manager.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.921226 coretex-0.0.9/src/coretex/logging/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      486 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/logging/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1257 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/logging/log.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1777 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/logging/log_severity.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     4889 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/logging/logger.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.921226 coretex-0.0.9/src/coretex/networking/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      238 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/networking/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)    11426 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/networking/network_manager.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     4491 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/networking/network_object.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2258 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/networking/network_response.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      122 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/networking/request_type.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     5459 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/networking/requests_manager.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.921226 coretex-0.0.9/src/coretex/qiime2/
--rw-r--r--   0 jenkins    (113) jenkins    (119)     7678 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/qiime2/__init__.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.921226 coretex-0.0.9/src/coretex/threading/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      110 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/threading/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      306 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/threading/stoppable_thread.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1179 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.921226 coretex-0.0.9/src/coretex/utils/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      153 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/utils/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1303 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/utils/console_progress_bar.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)       96 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/utils/date.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2885 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/utils/file.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      258 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/utils/number.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.921226 coretex-0.0.9/src/coretex/workspace/
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2126 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/workspace/__init__.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1061 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/workspace/base.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     1567 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/workspace/heartbeat.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)     2529 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/workspace/local.py
--rw-r--r--   0 jenkins    (113) jenkins    (119)      669 2023-02-10 09:27:35.000000 coretex-0.0.9/src/coretex/workspace/remote.py
-drwxr-xr-x   0 jenkins    (113) jenkins    (119)        0 2023-02-14 14:03:55.909226 coretex-0.0.9/src/coretex.egg-info/
--rw-r--r--   0 jenkins    (113) jenkins    (119)      805 2023-02-14 14:03:55.000000 coretex-0.0.9/src/coretex.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (113) jenkins    (119)     5389 2023-02-14 14:03:55.000000 coretex-0.0.9/src/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (113) jenkins    (119)        1 2023-02-14 14:03:55.000000 coretex-0.0.9/src/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (113) jenkins    (119)      152 2023-02-14 14:03:55.000000 coretex-0.0.9/src/coretex.egg-info/requires.txt
--rw-r--r--   0 jenkins    (113) jenkins    (119)        8 2023-02-14 14:03:55.000000 coretex-0.0.9/src/coretex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.304675 coretex-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-05-26 00:02:58.000000 coretex-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-26 00:03:11.304675 coretex-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-26 00:02:58.000000 coretex-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-26 00:02:58.000000 coretex-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:03:11.304675 coretex-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.272674 coretex-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.276674 coretex-1.0.0/src/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.276674 coretex-1.0.0/src/coretex/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/cache/cache_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/codable/descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/network_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.288674 coretex-1.0.0/src/coretex/coretex/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/executing_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.288674 coretex-1.0.0/src/coretex/coretex/experiment/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.288674 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/coretex/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/space_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/folder_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/folder_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/folder_management/folder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/requests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.304675 coretex-1.0.0/src/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/console_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.276674 coretex-1.0.0/src/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/top_level.txt
```

### Comparing `coretex-0.0.9/pyproject.toml` & `coretex-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coretex"
-version = "0.0.9"
+version = "1.0.0"
 authors = [
-  { name="Igor Perić", email="igor@coretex.ai" },
+  { name="Duško Mirković", email="dmirkovic@coretex.ai" },
 ]
 maintainers = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
-  { name="Alex Maslennikov", email="alex@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
   { name="Darko Zarić", email="dzaric@coretex.ai" },
   { name="Bogdan Tintor", email="btintor@coretex.ai" },
+  { name="Alex Maslennikov", email="alex@coretex.ai" },
   { name="Igor Perić", email="igor@coretex.ai" },
 ]
 description = "A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -27,19 +27,23 @@
 dependencies = [
   "requests",
   "inflection",
   "pillow",
   "numpy",
   "scikit-image",
   "shapely",
-  "opencv-python",
-  "tensorflow==2.8",
-  "tensorflowjs",
-  "torch",
   "protobuf~=3.19.0",
   "typed-argument-parser",
-  "termcolor"
+  "termcolor",
+  "typing-extensions",
+  "psutil",
+  "py3nvml",
 ]
 
 [project.urls]
 "Homepage" = "https://coretex.ai"
-"Documentation" = "https://docs.coretex.ai/1.0.0/"
+"Documentation" = "https://docs.coretex.ai/"
+"Python API" = "https://coretexpylib.coretex.ai/"
+"Source" = "https://github.com/coretex-ai/coretexpylib"
+
+[tool.setuptools.package-data]
+"*" = ["py.typed"]
```

### Comparing `coretex-0.0.9/src/coretex/codable/codable.py` & `coretex-1.0.0/src/coretex/codable/codable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,45 @@
+#     Copyright (C) 2023  BioMech LLC
+
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import Any, Optional, Type, Dict, Tuple
+from typing_extensions import Self
 from datetime import datetime
 from enum import Enum
-from typing import Any, Optional, TypeVar, Type, Dict, Tuple
 from uuid import UUID
 
 import inflection
 
 from .descriptor import KeyDescriptor
 from ..utils.date import DATE_FORMAT
 
 
-T = TypeVar("T", bound="Codable")
+def processDate(value: str, datetimeType: Type[datetime]) -> datetime:
+    """
+        Converts the date to a format used by Coretex
 
+        Returns
+        -------
+        datetime -> object whose datetime is represented using the Coretex datetime format
+    """
 
-def processDate(value: str, datetimeType: Type[datetime]) -> datetime:
     try:
         return datetimeType.strptime(value, DATE_FORMAT)
     except:
         # Python's datetime library requires UTC minutes to always
         # be present in the date in either of those 2 formats:
         # - +HHMM
         # - +HH:MM
@@ -26,23 +49,30 @@
         # so we need to handle the first case where minutes
         # are not present by adding them manually
         return datetimeType.strptime(f"{value}00", DATE_FORMAT)
 
 
 class Codable:
 
+    """
+        Class whose subclasses can be serialized/deserialized into/from a JSON format object
+    """
+
     @classmethod
     def _keyDescriptors(cls) -> Dict[str, KeyDescriptor]:
         """
-            Defines how to translate json key names and json values to python
-            and vice versa
-
-            Returns:
-            list[KeyDescriptor] -> List of objects describing translation
+            Defines a custom mapping for python objects to json field
+            Key of the dictionary represents a name of the field in python
+            Value of the dictionary represents how should the object be serialized/deserialized
+
+            Returns
+            -------
+            Dict[str, KeyDescriptor] -> Dictionary of objects describing translation
         """
+
         return {}
 
     @classmethod
     def __keyDescriptorByJsonName(cls, jsonName: str) -> Tuple[Optional[str], Optional[KeyDescriptor]]:
         for key, value in cls._keyDescriptors().items():
             if value.jsonName == jsonName:
                 return key, value
@@ -64,19 +94,27 @@
         if descriptor is None or descriptor.jsonName is None:
             return inflection.underscore(key)
 
         return descriptor.jsonName
 
     def _encodeValue(self, key: str, value: Any) -> Any:
         """
-            Used to change json field value
+            Encodes python value into a json property
+            Custom field serialization can be implemented by overriding this method
 
-            Parameters:
-            key: str -> python object variable name
-            value: Any -> json object represented as an object from standard python library
+            Parameters
+            ----------
+            key : str
+                python object variable name
+            value : Any
+                json object represented as an object from standard python library
+
+            Returns
+            -------
+            Any -> encoded value of the object
         """
 
         descriptor = self.__class__.__keyDescriptorByPythonName(key)
 
         if descriptor is None or descriptor.pythonType is None:
             return value
 
@@ -105,18 +143,22 @@
             return value.strftime(DATE_FORMAT)
 
         return value
 
     def encode(self) -> Dict[str, Any]:
         """
             Encodes python object into dictionary which contains
-            only values representable by standard python library
+            only values representable by standard python library/types
+
+            Returns
+            -------
+            Dict[str, Any] -> encoded object which can be serialized into json string
         """
 
-        encodedObject: dict[str, Any] = {}
+        encodedObject: Dict[str, Any] = {}
 
         for key, value in self.__dict__.items():
             descriptor = self.__class__.__keyDescriptorByPythonName(key)
 
             # skip ignored fields for encoding
             if descriptor is not None and not descriptor.isEncodable:
                 # print(f">> [Coretex] Skipping encoding for field: {key}")
@@ -138,14 +180,30 @@
         if descriptorKey is None:
             return inflection.camelize(key, False)
 
         return descriptorKey
 
     @classmethod
     def _decodeValue(cls, key: str, value: Any) -> Any:
+        """
+            Decodes a value of a single json field
+            Custom logic can be implemented by overriding this method
+
+            Parameters
+            ----------
+            key : str
+                name of the json field
+            value : Any
+                value of the json field
+
+            Returns
+            -------
+            Any -> decoded value of the json field
+        """
+
         _, descriptor = cls.__keyDescriptorByJsonName(key)
 
         if descriptor is None or descriptor.pythonType is None:
             return value
 
         if issubclass(descriptor.pythonType, Enum):
             if descriptor.isList() and descriptor.collectionType is not None:
@@ -170,29 +228,54 @@
                 return descriptor.collectionType([processDate(element, descriptor.pythonType) for element in value])
 
             return processDate(value, descriptor.pythonType)
 
         return value
 
     def _updateFields(self, encodedObject: Dict[str, Any]) -> None:
+        """
+            Updates the properties of object with new values
+
+            Parameters
+            ----------
+            encodedObject : Dict[str, Any]
+                json encoded object
+        """
+
         for key, value in encodedObject.items():
             _, descriptor = self.__class__.__keyDescriptorByJsonName(key)
 
             # skip ignored fields for deserialization
             if descriptor is not None and not descriptor.isDecodable:
                 # print(f">> [Coretex] Skipping decoding for field: {key}")
                 continue
 
             decodedKey = self.__decodeKey(key)
             self.__dict__[decodedKey] = self._decodeValue(key, value)
 
     def onDecode(self) -> None:
+        """
+            Callback which is called once the object has been decoded
+        """
+
         pass
 
     @classmethod
-    def decode(cls: Type[T], encodedObject: Dict[str, Any]) -> T:
+    def decode(cls, encodedObject: Dict[str, Any]) -> Self:
+        """
+            Decodes the json object into a python object
+
+            Parameters
+            ----------
+            encodedObject : Dict[str, Any]
+                json encoded object
+
+            Returns
+            -------
+            Self -> Decoded python object
+        """
         obj = cls()
 
         obj._updateFields(encodedObject)
         obj.onDecode()
 
         return obj
```

### Comparing `coretex-0.0.9/src/coretex/context/experiment_context.py` & `coretex-1.0.0/src/coretex/project/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,121 @@
-from __future__ import annotations
+#     Copyright (C) 2023  BioMech LLC
 
-from typing import Final, Any, Generic, Optional, Type, TypeVar
+#     This file is part of Coretex.ai  
 
-import os
-import json
-
-from ..coretex import Experiment, Model, ProjectTask
-from ..coretex.dataset import *
-
-
-T = TypeVar("T", bound = "NetworkDataset")
-
-
-class ContextBuilder(Generic[T]):
-
-    def __init__(self, experimentId: int) -> None:
-        self.experimentId: Final = experimentId
-
-        self.__datasetType: Optional[Type[T]] = None
-
-    def setDatasetType(self, datasetType: Optional[Type[T]]) -> ContextBuilder:
-        self.__datasetType = datasetType
-        return self
-
-    def __getDatasetType(self, experiment: Experiment) -> Type[T]:
-        if self.__datasetType is not None:
-            return self.__datasetType
-
-        if experiment.projectTask == ProjectTask.other:
-            return CustomDataset  # type: ignore
-
-        if experiment.projectTask == ProjectTask.imageSegmentation:
-            return ImageSegmentationDataset  # type: ignore
-
-        if experiment.projectTask == ProjectTask.objectDetection:
-            return ObjectDetectionDataset  # type: ignore
-
-        raise ValueError(f">> [Coretex] ProjectTask ({experiment.projectTask}) not supported")
-
-    def build(self) -> ExperimentContext[T]:
-        experiment = Experiment.fetchById(self.experimentId)
-        if experiment is None:
-            raise Exception(f">> [Coretex] Experiment (ID: {self.experimentId}) not found")
-
-        if not os.path.exists("experiment.config"):
-            raise FileNotFoundError(">> [Coretex] (experiment.config) file not found")
-
-        with open("experiment.config", "r") as configFile:
-            config: dict[str, Any] = {}
-            configContent = json.load(configFile)
-
-            # load parameters array as key => value pairs
-            if "parameters" in configContent:
-                parameters = configContent["parameters"]
-
-                if not isinstance(parameters, list):
-                    raise ValueError(">> [Coretex] Invalid experiment.config file. Property 'parameters' must be an array")
-
-                for parameter in parameters:
-                    config[parameter["name"]] = parameter["value"]
-
-            dataset = self.__getDatasetType(experiment).fetchById(config["dataset"])
-            if dataset is None:
-                raise Exception(f">> [Coretex] Dataset (ID: {config['dataset']}) not found")
-
-        return ExperimentContext(experiment, dataset, config)
-
-
-class ExperimentContext(Generic[T]):
-
-    __instance: Optional[ExperimentContext] = None
-
-    @classmethod
-    def instance(cls) -> ExperimentContext:
-        if cls.__instance is None:
-            raise ValueError(">> [Coretex] Invalid context access")
-
-        return cls.__instance
-
-    def __init__(self, experiment: Experiment, dataset: T, config: dict[str, Any]):
-        self.experiment: Final = experiment
-        self.dataset: Final = dataset
-        self.config: Final = config
-
-    @classmethod
-    def create(cls, experimentId: int, datasetType: Optional[Type[T]] = None) -> ExperimentContext:
-        if cls.__instance is not None:
-            raise ValueError(">> [Coretex] Context already exists")
-
-        cls.__instance = ContextBuilder(experimentId).setDatasetType(datasetType).build()  # type: ignore
-        return cls.__instance
-
-    @classmethod
-    def destroy(cls) -> None:
-        if cls.__instance is None:
-            raise ValueError(">> [Coretex] Context already destroyed")
-
-        cls.__instance = None
-
-    def createModel(self) -> Model:
-        return Model(self.experiment)
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import Callable, Optional, Type, TypeVar, Tuple, List
+from enum import IntEnum
+
+import logging
+import sys
+
+from .remote import processRemote
+from .local import processLocal
+from ..coretex import ExperimentStatus, NetworkDataset, ExecutingExperiment, MetricType
+from ..logging import LogHandler, initializeLogger, LogSeverity
+from ..networking import RequestFailedError
+from ..folder_management import FolderManager
+
+
+DatasetType = TypeVar("DatasetType", bound = "NetworkDataset")
+
+
+class ExecutionType(IntEnum):
+     # TODO: NYI on backend
+
+     local = 1
+     remote = 2
+
+
+def _prepareForExecution(
+     experimentId: int,
+     datasetType: Optional[Type[DatasetType]] = None,
+     metrics: Optional[List[Tuple[str, str, MetricType, str, MetricType]]] = None
+) -> None:
+     experiment = ExecutingExperiment.startExecuting(experimentId, datasetType)
+
+     logPath = FolderManager.instance().logs / f"{experimentId}.log"
+     customLogHandler = LogHandler.instance()
+     customLogHandler.currentExperimentId = experimentId
+
+     # if logLevel exists apply it, otherwise default to info
+     severity = LogSeverity.info
+     logLevel = experiment.parameters.get("logLevel")
+
+     if logLevel is not None:
+          severity = LogSeverity(logLevel)
+
+     initializeLogger(severity, logPath)
+
+     experiment.updateStatus(
+          status = ExperimentStatus.inProgress,
+          message = "Executing project."
+     )
+
+     if metrics is not None:
+          experiment.createMetrics(metrics)
+
+          if len(ExecutingExperiment.current().metrics) > 0:
+               logging.getLogger("coretexpylib").info(">> [Coretex] Metrics successfully created.")
+
+
+def initializeProject(
+     mainFunction: Callable[[ExecutingExperiment], None],
+     datasetType: Optional[Type[DatasetType]] = None,
+     metrics: Optional[List[Tuple[str, str, MetricType, str, MetricType]]] = None,
+     args: Optional[List[str]] = None
+) -> None:
+     """
+          Initializes and starts the python project as
+          Coretex experiment
+
+          Parameters
+          ----------
+          mainFunction : Callable[[ExecutingExperiment], None]
+               entry point function
+          datasetType : Optional[Type[DatasetType]]
+               Custom dataset if there is any (Not required)
+          metrics : Optional[List[Tuple[str, str, MetricType, str, MetricType]]]
+               list of metrics that will be created for executing Experiment
+          args : Optional[List[str]]
+               list of command line arguments, if None sys.argv will be used
+     """
+
+     try:
+          experimentId, callback = processRemote(args)
+     except:
+          experimentId, callback = processLocal(args)
+
+     try:
+          _prepareForExecution(experimentId, datasetType, metrics)
+
+          callback.onStart()
+
+          logging.getLogger("coretexpylib").info("Experiment execution started")
+          mainFunction(ExecutingExperiment.current())
+
+          callback.onSuccess()
+     except RequestFailedError:
+          callback.onNetworkConnectionLost()
+     except KeyboardInterrupt:
+          callback.onKeyboardInterrupt()
+     except BaseException as ex:
+          callback.onException(ex)
+
+          # sys.exit is ok here, finally block is guaranteed to execute
+          # due to how sys.exit is implemented (it internally raises SystemExit exception)
+          sys.exit(1)
+     finally:
+          callback.onCleanUp()
```

### Comparing `coretex-0.0.9/src/coretex/coretex/conversion/converters/city_scape_converter.py` & `coretex-1.0.0/src/coretex/coretex/conversion/converters/city_scape_converter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,25 @@
-from typing import Any, Optional
+#     Copyright (C) 2023  BioMech LLC
+
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import Any, Optional, List, Set, Dict
 from pathlib import Path
 
 import glob
 import os
 import json
 import logging
 
@@ -10,28 +27,24 @@
 
 from ..base_converter import BaseConverter
 from ...annotation import CoretexImageAnnotation, CoretexSegmentationInstance, BBox
 
 
 class CityScapeConverter(BaseConverter):
 
-    """
-        Represents the Converter from City Scape Format to Cortex Format
-    """
-
-    def __init__(self, datasetName: str, projectId: int, datasetPath: str) -> None:
-        super().__init__(datasetName, projectId, datasetPath)
+    def __init__(self, datasetName: str, spaceId: int, datasetPath: str) -> None:
+        super().__init__(datasetName, spaceId, datasetPath)
 
         self.__baseImagePath = os.path.join(datasetPath, "leftImg8bit_trainvaltest", "leftImg8bit")
         self.__baseAnnotationsPaths = [
             os.path.join(datasetPath, "gtFine_trainvaltest", "gtFine", "train"),
             os.path.join(datasetPath, "gtFine_trainvaltest", "gtFine", "val")
         ]
 
-        self.__imagePaths: list[str] = []
+        self.__imagePaths: List[str] = []
         self.__imagePaths.extend(glob.glob(f"{self.__baseImagePath}/train/*/*.png"))
         self.__imagePaths.extend(glob.glob(f"{self.__baseImagePath}/val/*/*.png"))
 
     def __annotationPathFor(self, imagePath: str) -> str:
         # Extract last 2 components of imagePath
         annotationName = os.path.sep.join(Path(imagePath).parts[-2:])
 
@@ -42,32 +55,32 @@
             annotationPath = os.path.join(annotationsPath, annotationName)
 
             if os.path.exists(annotationPath):
                 return annotationPath
 
         raise RuntimeError
 
-    def _dataSource(self) -> list[str]:
+    def _dataSource(self) -> List[str]:
         return self.__imagePaths
 
-    def _extractLabels(self) -> set[str]:
-        labels: set[str] = set()
+    def _extractLabels(self) -> Set[str]:
+        labels: Set[str] = set()
 
         for imagePath in self.__imagePaths:
             annotationPath = self.__annotationPathFor(imagePath)
 
             with open(annotationPath, mode="r") as annotationFile:
-                annotationData: dict[str, Any] = json.load(annotationFile)
+                annotationData: Dict[str, Any] = json.load(annotationFile)
 
                 for obj in annotationData["objects"]:
                     labels.add(obj["label"])
 
         return labels
 
-    def __extractInstance(self, obj: dict[str, Any]) -> Optional[CoretexSegmentationInstance]:
+    def __extractInstance(self, obj: Dict[str, Any]) -> Optional[CoretexSegmentationInstance]:
         label = obj["label"]
 
         coretexClass = self._dataset.classByName(label)
         if coretexClass is None:
             logging.getLogger("coretexpylib").info(f">> [Coretex] Class: ({label}) is not a part of dataset")
             return None
 
@@ -75,15 +88,15 @@
 
         return CoretexSegmentationInstance.create(
             coretexClass.classIds[0],
             BBox.fromPoly(polygon),
             [polygon]
         )
 
-    def __extractImageAnnotation(self, imagePath: str, annotationData: dict[str, Any]) -> None:
+    def __extractImageAnnotation(self, imagePath: str, annotationData: Dict[str, Any]) -> None:
         imageName = Path(imagePath).stem
         width = annotationData["imgWidth"]
         height = annotationData["imgHeight"]
 
         coretexAnnotation = CoretexImageAnnotation.create(imageName, width, height, [])
 
         for obj in annotationData["objects"]:
@@ -95,9 +108,9 @@
 
         self._saveImageAnnotationPair(imagePath, coretexAnnotation)
 
     def _extractSingleAnnotation(self, imagePath: str) -> None:
         annotationPath = self.__annotationPathFor(imagePath)
 
         with open(annotationPath, mode="r") as annotationFile:
-            annotationData: dict[str, Any] = json.load(annotationFile)
+            annotationData: Dict[str, Any] = json.load(annotationFile)
             self.__extractImageAnnotation(imagePath, annotationData)
```

### Comparing `coretex-0.0.9/src/coretex/coretex/conversion/converters/coco_converter.py` & `coretex-1.0.0/src/coretex/coretex/conversion/converters/coco_converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,82 @@
-from typing import Any, Final, Optional
+#     Copyright (C) 2023  BioMech LLC
+
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import Any, Final, Optional, List, Dict, Set
 
 import glob
 import os
 import json
 import logging
 
 from ..base_converter import BaseConverter
 from ...annotation import CoretexImageAnnotation, CoretexSegmentationInstance, BBox
 
 
 class _CocoImageAnnotationData:
 
-    def __init__(self, data: dict[str, Any], imageInfo: dict[str, Any]) -> None:
+    def __init__(self, data: Dict[str, Any], imageInfo: Dict[str, Any]) -> None:
         self.data = data
         self.imageInfo = imageInfo
 
 
 class COCOConverter(BaseConverter):
 
-    """
-        Represents the Converter from COCO Format to Cortex Format
-    """
-
-    def __init__(self, datasetName: str, projectId: int, datasetPath: str) -> None:
-        super().__init__(datasetName, projectId, datasetPath)
+    def __init__(self, datasetName: str, spaceId: int, datasetPath: str) -> None:
+        super().__init__(datasetName, spaceId, datasetPath)
 
         self.__imagesPath: Final = os.path.join(datasetPath, "images")
 
         annotationsPath = os.path.join(datasetPath, "annotations")
         self.__fileNames: Final = glob.glob(os.path.join(annotationsPath, "*.json"))
 
-    def _dataSource(self) -> list[_CocoImageAnnotationData]:
-        fullAnnotationData: list[_CocoImageAnnotationData] = []
+    def _dataSource(self) -> List[_CocoImageAnnotationData]:
+        fullAnnotationData: List[_CocoImageAnnotationData] = []
 
         for fileName in self.__fileNames:
             with open(fileName) as jsonFile:
                 data = json.load(jsonFile)
 
                 fullAnnotationData.extend([
                     _CocoImageAnnotationData(data, imageInfo)
                     for imageInfo in data["images"]
                 ])
 
         return fullAnnotationData
 
-    def _extractLabels(self) -> set[str]:
-        labels: set[str] = set()
+    def _extractLabels(self) -> Set[str]:
+        labels: Set[str] = set()
 
         for fileName in self.__fileNames:
             with open(fileName) as jsonFile:
                 data = json.load(jsonFile)
 
                 for category in data["categories"]:
                     labels.add(category["name"])
 
         return labels
 
     def __extractInstance(
         self,
-        categories: list[dict[str, Any]],
-        annotation: dict[str, Any]
+        categories: List[Dict[str, Any]],
+        annotation: Dict[str, Any]
     ) -> Optional[CoretexSegmentationInstance]:
 
         label: Optional[str] = None
 
         for category in categories:
             if category["id"] == annotation["category_id"]:
                 label = category["name"]
```

### Comparing `coretex-0.0.9/src/coretex/coretex/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.0/src/coretex/coretex/conversion/converters/human_segmentation_converter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,25 @@
-from __future__ import annotations
+#     Copyright (C) 2023  BioMech LLC
 
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import List, Set
 from pathlib import Path
 
 import os
 
 from PIL import Image
 from shapely.geometry import Polygon
 
@@ -12,16 +28,16 @@
 
 from ..base_converter import BaseConverter
 from ...annotation import CoretexImageAnnotation, CoretexSegmentationInstance, ImageDatasetClass, BBox
 
 
 class HumanSegmentationConverter(BaseConverter):
 
-    def __init__(self, datasetName: str, projectId: int, datasetPath: str) -> None:
-        super().__init__(datasetName, projectId, datasetPath)
+    def __init__(self, datasetName: str, spaceId: int, datasetPath: str) -> None:
+        super().__init__(datasetName, spaceId, datasetPath)
 
         self.__imagesPath = os.path.join(datasetPath, "images")
         self.__annotationsPath = os.path.join(datasetPath, "annotations")
 
         self.__imageNames = list(filter(
             lambda path: path.endswith("jpg"),
             os.listdir(self.__imagesPath))
@@ -39,21 +55,21 @@
     def __humanClass(self) -> ImageDatasetClass:
         coretexClass = self._dataset.classByName("human")
         if coretexClass is None:
             raise ValueError(f">> [Coretex] Class: (human) is not a part of dataset")
 
         return coretexClass
 
-    def _dataSource(self) -> list[str]:
+    def _dataSource(self) -> List[str]:
         return self.__imageNames
 
-    def _extractLabels(self) -> set[str]:
+    def _extractLabels(self) -> Set[str]:
         return set(["background", "human"])
 
-    def __extractPolygons(self, annotationPath: str, imageWidth: int, imageHeight: int) -> list[list[float]]:
+    def __extractPolygons(self, annotationPath: str, imageWidth: int, imageHeight: int) -> List[List[float]]:
         maskImage = Image.open(annotationPath)
         if maskImage is None:
             return []
 
         maskImage = maskImage.resize((imageWidth, imageHeight), Image.ANTIALIAS)
         subMaskArray = np.asarray(maskImage, dtype = np.uint8)
 
@@ -61,15 +77,15 @@
         subMaskArray[:, 0] = 0
         subMaskArray[0, :] = 0
         subMaskArray[:, -1] = 0
         subMaskArray[-1, :] = 0
 
         contours = skimage.measure.find_contours(subMaskArray, 0.5)
 
-        segmentations: list[list[float]] = []
+        segmentations: List[List[float]] = []
         for contour in contours:
             for i in range(len(contour)):
                 row, col = contour[i]
                 contour[i] = (col - 1, row - 1)
 
             # Make a polygon and simplify it
             poly = Polygon(contour)
@@ -84,20 +100,20 @@
                 segmentations.append(segmentation)
 
         # sorts polygons by size, descending
         segmentations.sort(key=len, reverse=True)
 
         return segmentations
 
-    def __extractInstances(self, annotationPath: str, imageWidth: int, imageHeight: int) -> list[CoretexSegmentationInstance]:
+    def __extractInstances(self, annotationPath: str, imageWidth: int, imageHeight: int) -> List[CoretexSegmentationInstance]:
         polygons = self.__extractPolygons(annotationPath, imageWidth, imageHeight)
         if len(polygons) == 0:
             return []
 
-        instances: list[CoretexSegmentationInstance] = []
+        instances: List[CoretexSegmentationInstance] = []
 
         largestBBox = BBox.fromPoly(polygons[0])
         firstPolygon = Polygon(np.array(polygons[0]).reshape((-1, 2)))
 
         backgroundBoundingBox = BBox(0, 0, imageWidth, imageHeight)
         instances.append(CoretexSegmentationInstance.create(
             self.__backgroundClass.classIds[0],
```

### Comparing `coretex-0.0.9/src/coretex/coretex/conversion/converters/label_me_converter.py` & `coretex-1.0.0/src/coretex/coretex/conversion/converters/create_ml_converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,94 @@
-from typing import Any, Optional
-from pathlib import Path
+#     Copyright (C) 2023  BioMech LLC
+
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import Any, Optional, List, Set, Dict
 
 import os
 import json
 import glob
 import logging
 
-import numpy as np
+from PIL import Image
 
 from ..base_converter import BaseConverter
-from ...annotation import CoretexImageAnnotation, CoretexSegmentationInstance, BBox
+from ...annotation import CoretexSegmentationInstance, CoretexImageAnnotation, BBox
 
 
-class LabelMeConverter(BaseConverter):
+class CreateMLConverter(BaseConverter):
 
-    """
-        Represents the Converter from LabelMe Format to Cortex Format
-    """
-
-    def __init__(self, datasetName: str, projectId: int, datasetPath: str) -> None:
-        super().__init__(datasetName, projectId, datasetPath)
+    def __init__(self, datasetName: str, spaceId: int, datasetPath: str) -> None:
+        super().__init__(datasetName, spaceId, datasetPath)
 
         self.__imagesPath = os.path.join(datasetPath, "images")
 
         annotations = os.path.join(datasetPath, "annotations")
         self.__fileNames = glob.glob(os.path.join(annotations, "*.json"))
 
-    def _dataSource(self) -> list[str]:
+    def _dataSource(self) -> List[str]:
         return self.__fileNames
 
-    def _extractLabels(self) -> set[str]:
-        labels: set[str] = set()
+    def _extractLabels(self) -> Set[str]:
+        labels: Set[str] = set()
 
         for fileName in self.__fileNames:
             with open(fileName) as jsonFile:
-                data = json.load(jsonFile)
+                data = json.load(jsonFile)[0]
 
-                for shape in data["shapes"]:
-                    labels.add(shape["label"])
+                for annotation in data["annotations"]:
+                    labels.add(annotation["label"])
 
         return labels
 
-    def __extractInstance(self, shape: dict[str, Any]) -> Optional[CoretexSegmentationInstance]:
-        label = shape["label"]
+    def __extractBBox(self, bbox: Dict[str, float]) -> BBox:
+        return BBox(
+            bbox["x"] - bbox["width"] / 2,
+            bbox["y"] - bbox["height"] / 2,
+            bbox["width"],
+            bbox["height"]
+        )
+
+    def __extractInstance(self, annotation: Dict[str, Any]) -> Optional[CoretexSegmentationInstance]:
+        label = annotation["label"]
 
         coretexClass = self._dataset.classByName(label)
         if coretexClass is None:
             logging.getLogger("coretexpylib").info(f">> [Coretex] Class: ({label}) is not a part of dataset")
             return None
 
-        points: list[float] = np.array(shape["points"]).flatten().tolist()
-        bbox = BBox.fromPoly(points)
-
-        return CoretexSegmentationInstance.create(coretexClass.classIds[0], bbox, [points])
+        bbox = self.__extractBBox(annotation["coordinates"])
+        return CoretexSegmentationInstance.create(coretexClass.classIds[0], bbox, [bbox.polygon])
 
-    def __extractImageAnnotation(self, imageAnnotation: dict[str, Any]) -> None:
-        imageName = Path(imageAnnotation["imagePath"]).stem
-        imageName = f"{imageName}.jpg"
+    def __extractImageAnnotation(self, imageAnnotation: Dict[str, Any]) -> None:
+        imageName = imageAnnotation["image"]
+        image = Image.open(f"{self.__imagesPath}/{imageName}")
 
-        width = imageAnnotation["imageWidth"]
-        height = imageAnnotation["imageHeight"]
+        coretexAnnotation = CoretexImageAnnotation.create(imageName, image.width, image.height, [])
 
-        coretexAnnotation = CoretexImageAnnotation.create(imageName, width, height, [])
-
-        for shape in imageAnnotation["shapes"]:
-            instance = self.__extractInstance(shape)
+        for annotation in imageAnnotation["annotations"]:
+            instance = self.__extractInstance(annotation)
             if instance is None:
                 continue
 
             coretexAnnotation.instances.append(instance)
 
         self._saveImageAnnotationPair(os.path.join(self.__imagesPath, imageName), coretexAnnotation)
 
     def _extractSingleAnnotation(self, fileName: str) -> None:
         with open(fileName) as jsonFile:
-            data = json.load(jsonFile)
+            data = json.load(jsonFile)[0]
+
             self.__extractImageAnnotation(data)
```

### Comparing `coretex-0.0.9/src/coretex/coretex/conversion/converters/voc_converter.py` & `coretex-1.0.0/src/coretex/coretex/conversion/converters/voc_converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,51 @@
-from typing import Optional
+#     Copyright (C) 2023  BioMech LLC
+
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import Optional, List, Set
 
 import os
 import logging
 import glob
 import xml.etree.ElementTree as ET
 
 from .pascal.shared import getTag, getBoxes, toFloat
 from ..base_converter import BaseConverter
 from ...annotation import CoretexImageAnnotation, CoretexSegmentationInstance, BBox
 
 
 class VOCConverter(BaseConverter):
 
-    def __init__(self, datasetName: str, projectId: int, datasetPath: str) -> None:
-        super().__init__(datasetName, projectId, datasetPath)
+    def __init__(self, datasetName: str, spaceId: int, datasetPath: str) -> None:
+        super().__init__(datasetName, spaceId, datasetPath)
 
         self.__imagesPath = os.path.join(datasetPath, "images")
 
         annotations = os.path.join(datasetPath, "annotations")
         self.__fileNames = glob.glob(os.path.join(annotations, "*.xml"))
 
-    def _dataSource(self) -> list[str]:
+    def _dataSource(self) -> List[str]:
         return self.__fileNames
 
-    def _extractLabels(self) -> set[str]:
-        labels: set[str] = set()
+    def _extractLabels(self) -> Set[str]:
+        labels: Set[str] = set()
 
         for filename in self.__fileNames:
             tree = ET.parse(filename)
             root = tree.getroot()
             objects = root.findall("object")
 
             for obj in objects:
```

### Comparing `coretex-0.0.9/src/coretex/coretex/dataset/image_dataset/image_dataset.py` & `coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/image_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,86 @@
-from __future__ import annotations
+#     Copyright (C) 2023  BioMech LLC
 
-from typing import TypeVar, Type, Optional
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from typing import TypeVar, Type, Optional, Dict, List
 
 from .base import BaseImageDataset
 from ..network_dataset import NetworkDataset
-from ...item import ImageItem
+from ...sample import ImageSample
 from ...annotation import ImageDatasetClass, ImageDatasetClasses
-from ....codable import KeyDescriptor
-from ....networking import NetworkManager, RequestType
+from ....codable import KeyDescriptor, Codable
+from ....networking import networkManager, RequestType
 
 
 DatasetType = TypeVar("DatasetType", bound = "ImageDataset")
-ItemType = TypeVar("ItemType", bound = "ImageItem")
+SampleType = TypeVar("SampleType", bound = "ImageSample")
+
 
+class ClassDistribution(Codable):
 
-class ImageDataset(BaseImageDataset[ItemType], NetworkDataset[ItemType]):  # type: ignore
+    name: str
+    color: str
+    count: int
+
+
+class ImageDataset(BaseImageDataset[SampleType], NetworkDataset[SampleType]):  # type: ignore
+
+    """
+        Represents the Image Dataset class \n
+        Includes functionality for working with Image Datasets
+        that are uploaded to Coretex.ai
+    """
+
+    classDistribution: List[ClassDistribution]
 
     @classmethod
-    def _keyDescriptors(cls) -> dict[str, KeyDescriptor]:
+    def _keyDescriptors(cls) -> Dict[str, KeyDescriptor]:
         descriptors = super()._keyDescriptors()
 
-        descriptors["items"] = KeyDescriptor("sessions", ImageItem, list)
+        descriptors["samples"] = KeyDescriptor("sessions", ImageSample, list)
         descriptors["classes"] = KeyDescriptor("classes", ImageDatasetClass, ImageDatasetClasses)
+        descriptors["classDistribution"] = KeyDescriptor("class_distribution", ClassDistribution, list)
 
         return descriptors
 
     @classmethod
-    def fetchById(cls: Type[DatasetType], objectId: int, queryParameters: Optional[list[str]] = None) -> Optional[DatasetType]:
+    def fetchById(cls: Type[DatasetType], objectId: int, queryParameters: Optional[List[str]] = None) -> Optional[DatasetType]:
         obj = super().fetchById(objectId, queryParameters)
         if obj is None:
             return None
 
-        response = NetworkManager.instance().genericJSONRequest(
+        response = networkManager.genericJSONRequest(
             endpoint=f"annotation-class?dataset_id={obj.id}",
             requestType=RequestType.get,
         )
 
         if not response.hasFailed():
             obj.classes = cls._decodeValue("classes", response.json)
             obj._writeClassesToFile()
 
         return obj
 
     def saveClasses(self, classes: ImageDatasetClasses) -> bool:
-        """
-            Saves provided classes (including their color) to dataset.
-            ImageDataset.classes property will be updated on successful save
-
-            Parameters:
-            classes: list[ImageDatasetClass] -> list of classes
-
-            Returns:
-            True if dataset classes were saved, False if failed to save dataset classes
-        """
-
         parameters = {
             "dataset_id": self.id,
             "classes": [clazz.encode() for clazz in classes]
         }
 
-        response = NetworkManager.instance().genericJSONRequest("annotation-class", RequestType.post, parameters)
+        response = networkManager.genericJSONRequest("annotation-class", RequestType.post, parameters)
         if not response.hasFailed():
             return super().saveClasses(classes)
 
         return not response.hasFailed()
```

### Comparing `coretex-0.0.9/src/coretex/networking/network_manager.py` & `coretex-1.0.0/src/coretex/networking/network_manager_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,237 @@
-from __future__ import annotations
-from pathlib import Path
+#     Copyright (C) 2023  BioMech LLC
 
-from typing import Optional, Any
-from threading import Lock
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+from pathlib import Path
+from typing import Optional, Any, Dict
+from abc import ABC, abstractmethod
+from importlib.metadata import version as getLibraryVersion
 
-import os
 import json
+import logging
+import os
+import platform
 
 from .requests_manager import RequestsManager
 from .request_type import RequestType
 from .network_response import HttpCode, NetworkResponse
 
 
-class NetworkManager:
+class NetworkManagerBase(ABC):
 
-    __instanceLock = Lock()
-    __instance: Optional[NetworkManager] = None
-
-    @classmethod
-    def instance(cls) -> NetworkManager:
-        if cls.__instance is None:
-            with cls.__instanceLock:
-                if cls.__instance is None:
-                    cls.__instance = cls()
-
-        return cls.__instance
+    MAX_RETRY_COUNT = 3
 
     def __init__(self) -> None:
-        self.__requestManager = RequestsManager(
-            baseURL = "{0}api/v1/".format(os.environ["SERVER_IP"]),
-            connectionTimeout = 20,
-            readTimeout = 30
-        )
-
-        self.__apiToken: Optional[str] = None
-        self.__refreshToken: Optional[str] = None
-        self.__agentID: Optional[int] = None
+        self._requestManager = RequestsManager(self.serverUrl(), 20, 30)
 
         # Override NetworkManager to update values
         self.loginEndpoint: str = "user/login"
         self.refreshEndpoint: str = "user/refresh"
 
         self.apiTokenHeaderField: str = "api-token"
-        self.agentIDHeaderField: str = "User-Agent"
 
         self.apiTokenKey: str = "token"
         self.refreshTokenKey: str = "refresh_token"
 
+    @classmethod
+    def serverUrl(cls) -> str:
+        serverUrl = os.environ["CTX_API_URL"]
+        return f"{serverUrl}api/v1/"
+
+    @property
+    @abstractmethod
+    def _apiToken(self) -> Optional[str]:
+        pass
+
+    @_apiToken.setter
+    @abstractmethod
+    def _apiToken(self, value: Optional[str]) -> None:
+        pass
+
     @property
-    def agentID(self) -> Optional[int]:
-        return self.__agentID
+    @abstractmethod
+    def _refreshToken(self) -> Optional[str]:
+        pass
+
+    @_refreshToken.setter
+    @abstractmethod
+    def _refreshToken(self, value: Optional[str]) -> None:
+        pass
 
-    @agentID.setter
-    def agentID(self, agentID: int) -> None:
-        self.__agentID = agentID
+    @property
+    def userAgent(self) -> str:
+        coretexpylibVersion = getLibraryVersion("coretex")
+        return f"coretexpylib;{coretexpylibVersion};python;{platform.python_version()}"
+
+    @property
+    def hasStoredCredentials(self) -> bool:
+        """
+            To use this functions call it using coretex.networking.networkManager
 
-    def __requestHeader(self) -> dict[str, str]:
+            Raises
+            ------
+            NotImplementedError
+        """
+
+        raise NotImplementedError
+
+    def _requestHeader(self) -> Dict[str, str]:
         header = {
             "Content-Type": "application/json",
             "Accept": "*/*",
             "Cache-Control": "no-cache",
             "Accept-Encoding": "gzip, deflate",
             "Content-Length": "0",
             "Connection": "keep-alive",
-            "cache-control": "no-cache"
+            "cache-control": "no-cache",
+            "X-User-Agent": self.userAgent
         }
 
-        if self.__apiToken is not None:
-            header[self.apiTokenHeaderField] = self.__apiToken
-
-        if self.__agentID is not None:
-            header[self.agentIDHeaderField] = str(self.__agentID)
+        if self._apiToken is not None:
+            header[self.apiTokenHeaderField] = self._apiToken
 
         return header
 
+    def _authenticate(self) -> NetworkResponse:
+        # authenticate using credentials stored in requests.Session.auth
+
+        response = self._requestManager.post(
+            endpoint = self.loginEndpoint,
+            headers = self._requestHeader()
+        )
+
+        if self.apiTokenKey in response.json:
+            self._apiToken = response.json[self.apiTokenKey]
+
+        if self.refreshTokenKey in response.json:
+            self._refreshToken = response.json[self.refreshTokenKey]
+
+        return response
+
+    def authenticate(self, username: str, password: str, storeCredentials: bool = True) -> NetworkResponse:
+        """
+            Authenticates user with provided credentials
+
+            Parameters
+            ----------
+            username : str
+                Coretex.ai username
+            password : str
+                Coretex.ai password
+            storeCredentials : bool
+                If true credentials will be stored in User object for reuse,
+                ignored for all managers except coretex.networking.networkManager
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object containing the full response info
+
+            Example
+            -------
+            >>> from coretex.networking import networkManager
+            \b
+            >>> response = networkManager.authenticate(username = "dummy@coretex.ai", password = "123456")
+            >>> if response.hasFailed():
+                    print("Failed to authenticate")
+        """
+
+        self._requestManager.setAuth(username, password)
+
+        # authenticate using credentials stored in requests.Session.auth
+        return self._authenticate()
+
+    def authenticateWithStoredCredentials(self) -> NetworkResponse:
+        """
+            To use this functions call it using coretex.networking.networkManager
+
+            Raises
+            ------
+            NotImplementedError
+        """
+
+        raise NotImplementedError
+
+    def authenticateWithRefreshToken(self, token: str) -> NetworkResponse:
+        """
+            Authenticates user with provided refresh token
+
+            Parameters
+            ----------
+            token : str
+                refresh token
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object containing the full response info
+        """
+
+        self._refreshToken = token
+        return self.refreshToken()
+
     def genericDownload(
         self,
         endpoint: str,
         destination: str,
-        parameters: Optional[dict[str, Any]] = None,
+        parameters: Optional[Dict[str, Any]] = None,
         retryCount: int = 0
     ) -> NetworkResponse:
         """
             Downloads file to the given destination
 
-            Parameters:
-            endpoint: str -> API endpoint
-            destination: str -> path to save file
-            parameters: Optional[dict[str, Any]] -> request parameters (not required)
-            retryCount: int -> number of function calls if request has failed
+            Parameters
+            ----------
+            endpoint : str
+                API endpoint
+            destination : str
+                path to save file
+            parameters : Optional[dict[str, Any]]
+                request parameters (not required)
+            retryCount : int
+                number of function calls if request has failed
 
-            Returns:
+            Returns
+            -------
             NetworkResponse as response content to request
+
+            Example
+            -------
+            >>> from coretex import networkManager
+            \b
+            >>> response = networkManager.genericDownload(
+                    endpoint = "dummyObject/download",
+                    destination = "path/to/destination/folder"
+                )
+            >>> if response.hasFailed():
+                    print("Failed to download the file")
         """
 
-        headers = self.__requestHeader()
+        headers = self._requestHeader()
 
         if parameters is None:
             parameters = {}
 
-        response = self.__requestManager.get(
-            endpoint = endpoint,
-            headers = headers,
-            jsonObject = parameters
-        )
+        response = self._requestManager.get(endpoint, headers, jsonObject = parameters)
 
         if self.shouldRetry(retryCount, response):
-            print(">> [MLService] Retry count: {0}".format(retryCount))
-
-            if self.__apiToken is not None:
-                headers[self.apiTokenHeaderField] = self.__apiToken
-
-            return self.genericDownload(
-                endpoint = endpoint,
-                destination = destination,
-                parameters = parameters,
-                retryCount = retryCount + 1
-            )
+            print(">> [Coretex] Retry count: {0}".format(retryCount))
+            return self.genericDownload(endpoint, destination, parameters, retryCount + 1)
 
         if response.raw.ok:
             destinationPath = Path(destination)
             if destinationPath.is_dir():
                 raise RuntimeError(">> [Coretex] Destination is a directory not a file")
 
             if destinationPath.exists():
@@ -133,221 +244,212 @@
 
         return response
 
     def genericUpload(
         self,
         endpoint: str,
         files: Any,
-        parameters: Optional[dict[str, Any]] = None,
+        parameters: Optional[Dict[str, Any]] = None,
         retryCount: int = 0
     ) -> NetworkResponse:
         """
             Uploads files to Cortex.ai
 
-            Parameters:
-            endpoint: str -> API endpoint
-            files: Any -> files
-            parameters: Optional[dict[str, Any]] -> request parameters (not required)
-            retryCount: int -> number of function calls if request has failed
-
-            Returns:
-            NetworkResponse as response content to request
+            Parameters
+            ----------
+            endpoint : str
+                API endpoint
+            files : Any
+                files
+            parameters : Optional[dict[str, Any]]
+                request parameters (not required)
+            retryCount : int
+                number of function calls if request has failed
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object containing the full response info
+
+            Example
+            -------
+            >>> from coretex import networkManager
+            \b
+            >>> localFilePath = "path/to/file/filename.ext"
+            >>> with open(localFilePath, "rb") as file:
+                    files = [
+                        ("file", ("filename.ext", file, "application/zip"))
+                    ]
+            \b
+                    response = networkManager.genericUpload(
+                        endpoint = "dummy/upload",
+                        files = files,
+                    )
+            >>> if response.hasFailed():
+                    print("Failed to upload the file")
         """
 
-        headers = self.__requestHeader()
+        headers = self._requestHeader()
         del headers['Content-Type']
 
         if parameters is None:
             parameters = {}
 
-        networkResponse = self.__requestManager.genericRequest(
-            requestType = RequestType.post,
-            endpoint = endpoint,
-            headers = headers,
-            data = parameters,
-            files = files
-        )
+        networkResponse = self._requestManager.genericRequest(RequestType.post, endpoint, headers, parameters, files)
 
         if self.shouldRetry(retryCount, networkResponse):
-            print(">> [MLService] Retry count: {0}".format(retryCount))
-
-            if self.__apiToken is not None:
-                headers[self.apiTokenHeaderField] = self.__apiToken
-
-            return self.genericUpload(
-                endpoint = endpoint,
-                files = files,
-                parameters = parameters,
-                retryCount = retryCount + 1
-            )
+            print(">> [Coretex] Retry count: {0}".format(retryCount))
+            return self.genericUpload(endpoint, files, parameters, retryCount + 1)
 
         return networkResponse
 
     def genericDelete(
         self,
         endpoint: str
     ) -> NetworkResponse:
         """
             Deletes Cortex.ai objects
 
-            Parameters:
-            endpoint: str -> API endpoint
-
-            Returns:
-            NetworkResponse as response content to request
+            Parameters
+            ----------
+            endpoint : str
+                API endpoint
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object containing the full response info
+
+            Example
+            -------
+            >>> from coretex import networkManager
+            \b
+            >>> response = networkManager.genericDelete(
+                    endpoint = "dummyObject/delete"
+                )
+            >>> if response.hasFailed():
+                    print("Failed to delete the object")
         """
 
-        headers = self.__requestHeader()
-
-        return self.__requestManager.genericRequest(
-            requestType = RequestType.delete,
-            endpoint = endpoint,
-            headers = headers
-        )
+        return self._requestManager.genericRequest(RequestType.delete, endpoint, self._requestHeader())
 
     def genericJSONRequest(
         self,
         endpoint: str,
         requestType: RequestType,
-        parameters: Optional[dict[str, Any]] = None,
-        headers: Optional[dict[str, str]] = None,
+        parameters: Optional[Dict[str, Any]] = None,
+        headers: Optional[Dict[str, str]] = None,
         retryCount: int = 0
     ) -> NetworkResponse:
         """
             Sends generic http request with specified parameters
 
-            Parameters:
-            endpoint: str -> API endpoint
-            requestType: RequestType -> request type
-            parameters: Optional[dict[str, Any]] -> request parameters (not required)
-            headers: Optional[dict[str, str]] -> headers (not required)
-            retryCount: int -> number of function calls if request has failed
-
-            Returns:
-            NetworkResponse as response content to request
+            Parameters
+            ----------
+            endpoint : str
+                API endpoint
+            requestType : RequestType
+                request type
+            parameters : Optional[dict[str, Any]]
+                request parameters (not required)
+            headers : Optional[dict[str, str]]
+                headers (not required)
+            retryCount : int
+                number of function calls if request has failed
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object containing the full response info
+
+            Example
+            -------
+            >>> from coretex import networkManager
+            \b
+            >>> response = networkManager.genericJSONRequest(
+                    endpoint = "dummy/add",
+                    requestType = RequestType.post,
+                    parameters = {
+                        "object_id": 1,
+                    }
+                )
+            >>> if response.hasFailed():
+                    print("Failed to add the object")
         """
 
         if headers is None:
-            headers = self.__requestHeader()
+            headers = self._requestHeader()
 
         if parameters is None:
             parameters = {}
 
-        networkResponse = self.__requestManager.genericRequest(
-            requestType = requestType,
-            endpoint = endpoint,
-            headers = headers,
-            data = json.dumps(parameters)
-        )
+        networkResponse = self._requestManager.genericRequest(requestType, endpoint, headers, json.dumps(parameters))
 
         if self.shouldRetry(retryCount, networkResponse):
-            print(">> [MLService] Retry count: {0}".format(retryCount))
-
-            if self.__apiToken is not None:
-                headers[self.apiTokenHeaderField] = self.__apiToken
-
-            return self.genericJSONRequest(
-                endpoint,
-                requestType,
-                parameters,
-                headers,
-                retryCount + 1
-            )
+            print(">> [Coretex] Retry count: {0}".format(retryCount))
+            return self.genericJSONRequest(endpoint, requestType, parameters, headers, retryCount + 1)
 
         return networkResponse
 
-    def __authenticate(self) -> NetworkResponse:
-        # authenticate using credentials stored in requests.Session.auth
-
-        response = self.__requestManager.post(
-            endpoint = self.loginEndpoint,
-            headers = self.__requestHeader()
-        )
-
-        if self.apiTokenKey in response.json:
-            self.__apiToken = response.json[self.apiTokenKey]
-
-        if self.refreshTokenKey in response.json:
-            self.__refreshToken = response.json[self.refreshTokenKey]
-
-        if not response.hasFailed():
-            print(">> [MLService] Login successful")
-
-        return response
-
-    def authenticate(self, username: str, password: str) -> NetworkResponse:
-        self.__requestManager.setAuth(username, password)
-
-        # authenticate using credentials stored in requests.Session.auth
-        return self.__authenticate()
-
-    def authenticateWithRefreshToken(self, token: str) -> None:
-        """
-            Authenticates user with provided refresh token
-        """
-
-        self.__refreshToken = token
-        self.refreshToken()
-
-    def refreshToken(self) -> None:
+    def refreshToken(self) -> NetworkResponse:
         """
             Uses refresh token functionality to fetch new API access token
+
+            Returns
+            -------
+            NetworkResponse -> NetworkResponse object containing the full response info
         """
 
-        headers = self.__requestHeader()
+        headers = self._requestHeader()
 
-        if self.__refreshToken is not None:
-            headers[self.apiTokenHeaderField] = self.__refreshToken
+        if self._refreshToken is not None:
+            headers[self.apiTokenHeaderField] = self._refreshToken
 
-        networkResponse = self.__requestManager.genericRequest(
+        networkResponse = self._requestManager.genericRequest(
             requestType = RequestType.post,
             endpoint = self.refreshEndpoint,
             headers = headers
         )
 
-        if networkResponse.hasFailed():
-            # the following logic should be removed as part of CTX-1659
-            # it is needed for node authentication when refresh token issued on startup expires
-
-            # if refresh failed try to login again
-            # authResponse = self.authenticate(username = "agent1", password = "Qwebnm11.")
-            if not self.__requestManager.isAuthSet:
-                raise RuntimeError(">> [Coretex] Cannot login on user/refresh failure. Credentials not available")
-
-            authResponse = self.__authenticate()
-            if authResponse.hasFailed():
-                # if both login and refresh failed, something is seriously wrong
-                raise RuntimeError(">> [Coretex] Failed to login during on user/refresh failure")
-
-            # the following line should be commented out as part of CTX-1659
-            # as both node and workspace will use the same refresh token which duration will be enough to cover long running experiments
-            # raise RuntimeError(">> [MLService] Failed to do API token refresh")
-        elif self.apiTokenKey in networkResponse.json:
-            self.__apiToken = networkResponse.json[self.apiTokenKey]
-            print(">> [Coretex] API token refresh was successful. API token updated")
+        if self.apiTokenKey in networkResponse.json:
+            self._apiToken = networkResponse.json[self.apiTokenKey]
+            logging.getLogger("coretexpylib").debug(">> [Coretex] API token refresh was successful. API token updated")
+
+        return networkResponse
 
     def shouldRetry(self, retryCount: int, response: NetworkResponse) -> bool:
         """
             Checks if network request should be repeated based on the number of repetitions
             as well as the response from previous repetition
 
-            Parameters:
-            retryCount: int -> number of repeated function calls
-            response: NetworkResponse -> generated response after sending the request
-
-            Returns:
-            True if the function call needs to be repeated, False if function was called 3 times or if request has not failed
+            Parameters
+            ----------
+            retryCount : int
+                number of repeated function calls
+            response : NetworkResponse
+                generated response after sending the request
+
+            Returns
+            -------
+            bool -> True if the function call needs to be repeated,
+            False if function was called 3 times or if request has not failed
         """
 
         # Limit retry count to 3 times
-        if retryCount == 3:
+        if retryCount == NetworkManagerBase.MAX_RETRY_COUNT:
             return False
 
         # If we get unauthorized maybe API token is expired
         if response.isUnauthorized():
-            self.refreshToken()
-            return True
+            refreshTokenResponse = self.refreshToken()
+            return not refreshTokenResponse.hasFailed()
 
         return (
             response.statusCode == HttpCode.internalServerError or
             response.statusCode == HttpCode.serviceUnavailable
         )
+
+    def reset(self) -> None:
+        """
+            Removes api and refresh token
+        """
+
+        self._apiToken = None
+        self._refreshToken = None
+        self._requestManager.reset()
```

### Comparing `coretex-0.0.9/src/coretex/networking/network_object.py` & `coretex-1.0.0/src/coretex/coretex/sample/network_sample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,140 @@
-from typing import Type, TypeVar, Optional, Any, Dict, List
+#     Copyright (C) 2023  BioMech LLC
 
-import inflection
+#     This file is part of Coretex.ai  
 
-from .request_type import RequestType
-from .network_manager import NetworkManager
-from ..codable import Codable
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
 
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
 
-T = TypeVar("T", bound="NetworkObject")
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-DEFAULT_PAGE_SIZE = 100
+from typing import Any, TypeVar, Optional, Generic, Dict, Union
+from typing_extensions import Self
+from pathlib import Path
 
+import os
 
-class NetworkObject(Codable):
-    """
-        Base class for every Coretex object representation in python
-    """
-
-    id: int
-    isDeleted: bool
-
-    # Required init
-    def __init__(self) -> None:
-        pass
-
-    @classmethod
-    def _endpoint(cls) -> str:
-        """
-            Returns:
-            Coretex.ai object endpoint for a given class
-        """
+from .sample import Sample
+from ..space import SpaceTask
+from ...codable import KeyDescriptor
+from ...networking import NetworkObject, networkManager
+from ...folder_management import FolderManager
+from ...utils import guessMimeType
 
-        return inflection.underscore(cls.__name__)
 
-    def __eq__(self, __o: object) -> bool:
-        """
-            Checks if the NetworkObjects which have id property
-            defined are equal
+SampleDataType = TypeVar("SampleDataType")
 
-            Parameter:
-            __o: object -> object to which we are comparing self
 
-            Returns:
-            True if ids are present and equal, False in any other case
-        """
+class NetworkSample(Generic[SampleDataType], Sample[SampleDataType], NetworkObject):
 
-        # check if object parent class matches
-        if isinstance(__o, NetworkObject):
-            return self.id == __o.id
+    """
+        Represents a base class for all Sample classes which are
+        comunicating with Coretex.ai
+    """
 
-        return NotImplemented
+    isLocked: bool
+    spaceTask: SpaceTask
 
-    def __hash__(self) -> int:
+    @property
+    def path(self) -> str:
         """
-            Returns:
-            hash of all the items defined on the self.__dict__ object
+            Returns
+            -------
+            str -> path for network sample
         """
 
-        return hash(tuple(sorted(self.__dict__.items())))
+        return os.path.join(FolderManager.instance().samplesFolder, str(self.id))
 
-    def refresh(self, jsonObject: Optional[Dict[str, Any]] = None) -> bool:
+    @property
+    def zipPath(self) -> str:
+        """
+            Returns
+            -------
+            str -> zip path for network sample
         """
-            Updates objects fields to a provided value if set, otherwise
-            fetches the object from the API and updates the values
-            using the fetched object
 
-            Parameters:
-            jsonObject: Optional[dict[str, Any]] -> A serialized json object to
-            which the values should be updated, if provided
+        return f"{self.path}.zip"
 
-            Returns:
-            True if the update was successful, False otherwise
-        """
+    @classmethod
+    def _keyDescriptors(cls) -> Dict[str, KeyDescriptor]:
+        descriptors = super()._keyDescriptors()
+        descriptors["spaceTask"] = KeyDescriptor("project_task", SpaceTask)
 
-        # Update from json if it exists
-        if jsonObject is not None:
-            self._updateFields(jsonObject)
-            return True
+        return descriptors
 
-        # Fetch from server otherwise
-        obj = self.__class__.fetchById(self.id)
-        if obj is None:
-            return False
-
-        for key, value in obj.__dict__.items():
-            self.__dict__[key] = value
-
-        return True
-
-    def update(self, parameters: Dict[str, Any]) -> bool:
-        if self.isDeleted:
-            return False
-
-        return not NetworkManager.instance().genericJSONRequest(
-            endpoint=f"{self.__class__._endpoint()}/{self.id}",
-            requestType=RequestType.put,
-            parameters=parameters
-        ).hasFailed()
-
-    def delete(self) -> bool:
-        if self.isDeleted:
-            return False
-
-        return not NetworkManager.instance().genericDelete(
-            f"{self.__class__._endpoint()}/{self.id}"
-        ).hasFailed()
+    @classmethod
+    def _endpoint(cls) -> str:
+        return "session"
 
     @classmethod
-    def create(cls: Type[T], parameters: Dict[str, Any]) -> Optional[T]:
-        response = NetworkManager.instance().genericJSONRequest(
-            endpoint=cls._endpoint(),
-            requestType=RequestType.post,
-            parameters=parameters
-        )
+    def _createSample(
+        cls,
+        parameters: Dict[str, Any],
+        filePath: Union[Path, str],
+        mimeType: Optional[str] = None
+    ) -> Optional[Self]:
+        """
+            Uploads sample to Coretex.ai
 
-        if response.hasFailed():
-            return None
+            Parametrs
+            ---------
+            endpoint : str
+                API endpoint
+            parameters : Dict[str, Any]
+                parameters which will be sent as request body
+            filePath : str
+                path to sample
+            mimeType : Optional[str]
+                mimeType (not required)
 
-        return cls.decode(response.json)
+            Returns
+            -------
+            Optional[Self] -> created sample object if request
+            was successful, None otherwise
+        """
 
-    @classmethod
-    def fetchAll(cls: Type[T], queryParameters: Optional[List[str]]=None, pageSize: int=DEFAULT_PAGE_SIZE) -> List[T]:
-        if queryParameters is None:
-            queryParameters = [f"page_size={pageSize}"]
-        else:
-            queryParameters.append(f"page_size={pageSize}")
+        if isinstance(filePath, str):
+            filePath = Path(filePath)
 
-        formattedQueryParameters = "&".join(queryParameters)
-        endpoint = f"{cls._endpoint()}?{formattedQueryParameters}"
+        if mimeType is None:
+            mimeType = guessMimeType(str(filePath))
 
-        response = NetworkManager.instance().genericJSONRequest(endpoint, RequestType.get)
+        with filePath.open("rb") as sampleFile:
+            files = [
+                ("file", (filePath.stem, sampleFile, mimeType))
+            ]
 
-        if response.hasFailed():
-            return []
+            response = networkManager.genericUpload("session/import", files, parameters)
+            if response.hasFailed():
+                return None
 
-        objects: list[T] = []
+            return cls.decode(response.json)
 
-        for obj in response.json:
-            objects.append(cls.decode(obj))
+    def download(self, ignoreCache: bool = False) -> bool:
+        """
+            Downloads sample from Coretex.ai
 
-        return objects
+            Returns
+            -------
+            bool -> False if response is failed, True otherwise
+        """
 
-    @classmethod
-    def fetchById(cls: Type[T], objectId: int, queryParameters: Optional[List[str]]=None) -> Optional[T]:
-        endpoint = f"{cls._endpoint()}/{objectId}"
-        if queryParameters is not None:
-            formattedQueryParameters = "&".join(queryParameters)
-            endpoint = f"{endpoint}?{formattedQueryParameters}"
+        if os.path.exists(self.zipPath) and not ignoreCache:
+            return True
 
-        response = NetworkManager.instance().genericJSONRequest(endpoint, RequestType.get)
+        response = networkManager.genericDownload(
+            endpoint = f"{self.__class__._endpoint()}/export?id={self.id}",
+            destination = self.zipPath
+        )
 
-        if response.hasFailed():
-            return None
+        return not response.hasFailed()
 
-        return cls.decode(response.json)
+    def load(self) -> SampleDataType:
+        return super().load()  # type: ignore
```

### Comparing `coretex-0.0.9/src/coretex/qiime2/__init__.py` & `coretex-1.0.0/src/coretex/qiime2/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,69 @@
+#     Copyright (C) 2023  BioMech LLC
+
+#     This file is part of Coretex.ai  
+
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
+
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
+
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 from typing import List
 from pathlib import Path
 
 import subprocess
 import logging
 
 
 class QiimeCommandException(Exception):
     pass
 
 
-def logProcessOutput(output: bytes) -> None:
-    line = output.decode("UTF-8")
-    if line.strip() == "":
-        return
+def logProcessOutput(output: bytes, severity: int) -> None:
+    decoded = output.decode("UTF-8")
 
-    logging.getLogger("coretexpylib").info(line)
+    for line in decoded.split("\n"):
+        # skip empty lines
+        if line.strip() == "":
+            continue
+
+        # ignoring type for now, has to be fixed in coretexpylib
+        logging.getLogger("coretexpylib").log(severity, line)
 
 
 def QiimeCommand(args: List[str]) -> None:
     process = subprocess.Popen(
         args,
         shell = False,
         cwd = Path(__file__).parent,
         stdout = subprocess.PIPE,
         stderr = subprocess.PIPE
     )
 
-    # stdout, stderr = process.communicate()
-    while code := process.poll() is None:
-        stdout = process.stdout
-        if stdout is not None:
-            logProcessOutput(stdout.readline())
-
-        stderr = process.stderr
-        if stderr is not None:
-            logProcessOutput(stderr.readline())
+    stdout, stderr = process.communicate()
+
+    if len(stdout) > 0:
+        logProcessOutput(stdout, logging.INFO)
+
+    if len(stderr) > 0:
+        severity = logging.CRITICAL
+        if process.returncode == 0:
+            severity = logging.WARNING
+
+        logProcessOutput(stderr, severity)
 
-    if code != 0:
+    if process.returncode != 0:
         raise QiimeCommandException
 
 
 def toolsImport(sequenceType: str, inputPath: str, outputPath: str) -> None:
     QiimeCommand([
         "qiime", "tools", "import",
         "--type", sequenceType,
```

### Comparing `coretex-0.0.9/src/coretex/workspace/local.py` & `coretex-1.0.0/src/coretex/project/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from typing import Any, Dict, List, Tuple
+#     Copyright (C) 2023  BioMech LLC
 
-import json
-import logging
-import traceback
-
-from tap import Tap
+#     This file is part of Coretex.ai  
 
-from .base import WorkspaceCallback
-from ..coretex import Experiment, ExperimentStatus
-from ..networking import NetworkManager
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU Affero General Public License as
+#     published by the Free Software Foundation, either version 3 of the
+#     License, or (at your option) any later version.
 
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU Affero General Public License for more details.
 
-class LocalWorkspaceCallback(WorkspaceCallback):
-
-    def onSuccess(self) -> None:
-        super().onSuccess()
+#     You should have received a copy of the GNU Affero General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-        self._experiment.updateStatus(ExperimentStatus.completedWithSuccess)
+from typing import Final
+from typing_extensions import Self
 
-    def onException(self, exception: BaseException) -> None:
-        super().onException(exception)
+import sys
+import logging
+import multiprocessing
 
-        self._experiment.updateStatus(ExperimentStatus.completedWithError)
+from ..coretex import Experiment
+from ..folder_management import FolderManager
+from ..logging import LogHandler
 
-        exceptionStackTrace = "".join(traceback.format_exception(
-            type(exception),
-            exception,
-            exception.__traceback__
-        ))
+from .calculate_metrics import uploadMetricsWorker
 
-        for line in exceptionStackTrace.split("\n"):
-            if len(line.strip()) == 0:
-                continue
 
-            logging.getLogger("coretexpylib").fatal(line)
+class ProjectCallback:
 
+    def __init__(self, experiment: Experiment, refreshToken: str) -> None:
+        self._experiment: Final = experiment
 
-class LocalArgumentParser(Tap):
+        self.__outputStream, self.__inputStream = multiprocessing.Pipe()
 
-    username: str
-    password: str
+        self.process = multiprocessing.Process(
+            target = uploadMetricsWorker,
+            args = (self.__outputStream, refreshToken, self._experiment.id)
+        )
 
-    datasetId: int
-    subProjectId: int
-    description: str
+    @classmethod
+    def create(cls, experimentId: int, refreshToken: str) -> Self:
+        experiment = Experiment.fetchById(experimentId)
+        if experiment is None:
+            raise ValueError
 
-    def configure(self) -> None:
-        self.add_argument("--username", type = str)
-        self.add_argument("--password", type = str)
+        return cls(experiment, refreshToken)
 
-        self.add_argument("--datasetId", type = int)
-        self.add_argument("--subProjectId", type = int)
-        self.add_argument("--description", nargs = "?", type = str, default = "")
+    def onStart(self) -> None:
+        self.process.start()
 
+        result = self.__inputStream.recv()
+        if result["code"] != 0:
+            raise RuntimeError(result["message"])
 
-def loadLocalParameters() -> List[Dict[str, Any]]:
-    with open("experiment.config", "r") as configFile:
-        configContent = json.load(configFile)
+        logging.getLogger("coretexpylib").info(result["message"])
 
-        if "parameters" in configContent:
-            parameters: List[Dict[str, Any]] = configContent["parameters"]
+    def onSuccess(self) -> None:
+        pass
 
-    return parameters
+    def onKeyboardInterrupt(self) -> None:
+        pass
 
+    def onException(self, exception: BaseException) -> None:
+        logging.getLogger("coretexpylib").debug(exception, exc_info = True)
+        logging.getLogger("coretexpylib").critical(str(exception))
 
-def processLocal() -> Tuple[int, WorkspaceCallback]:
-    parser = LocalArgumentParser().parse_args()
+    def onNetworkConnectionLost(self) -> None:
+        FolderManager.instance().clearTempFiles()
 
-    NetworkManager.instance().authenticate(parser.username, parser.password)
-    parameters = loadLocalParameters()
+        sys.exit(1)
 
-    experiment = Experiment.startCustomExperiment(
-        parser.datasetId,
-        parser.subProjectId,
-        # Dummy Local service ID, hardcoded as it is only a temporary solution,
-        # backend will add a new ExperimentType (local) which does not require a specific
-        # machine to run
-        43,
-        parser.description,
-        parameters=parameters
-    )
+    def onCleanUp(self) -> None:
+        logging.getLogger("coretexpylib").info("Experiment execution finished")
+        self.process.kill()
 
-    if experiment is None:
-        raise RuntimeError(">> [Coretex] Failed to create experiment")
+        try:
+            from py3nvml import py3nvml
+            py3nvml.nvmlShutdown()
+        except:
+            pass
 
-    experiment.updateStatus(ExperimentStatus.preparingToStart)
+        LogHandler.instance().flushLogs()
+        LogHandler.instance().reset()
 
-    return experiment.id, LocalWorkspaceCallback(experiment)
+        FolderManager.instance().clearTempFiles()
```

### Comparing `coretex-0.0.9/src/coretex.egg-info/SOURCES.txt` & `coretex-1.0.0/src/coretex.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+LICENSE
 README.md
 pyproject.toml
 src/coretex/__init__.py
+src/coretex/_configuration.py
+src/coretex/_logger.py
+src/coretex/py.typed
 src/coretex.egg-info/PKG-INFO
 src/coretex.egg-info/SOURCES.txt
 src/coretex.egg-info/dependency_links.txt
 src/coretex.egg-info/requires.txt
 src/coretex.egg-info/top_level.txt
 src/coretex/cache/__init__.py
 src/coretex/cache/cache_module.py
 src/coretex/codable/__init__.py
 src/coretex/codable/codable.py
 src/coretex/codable/descriptor.py
-src/coretex/context/__init__.py
-src/coretex/context/experiment_context.py
 src/coretex/coretex/__init__.py
 src/coretex/coretex/annotation/__init__.py
 src/coretex/coretex/annotation/image/__init__.py
 src/coretex/coretex/annotation/image/bbox.py
 src/coretex/coretex/annotation/image/classes_format.py
 src/coretex/coretex/annotation/image/coretex_format.py
 src/coretex/coretex/conversion/__init__.py
@@ -36,79 +38,105 @@
 src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
 src/coretex/coretex/conversion/converters/pascal/shared.py
 src/coretex/coretex/dataset/__init__.py
 src/coretex/coretex/dataset/dataset.py
 src/coretex/coretex/dataset/local_dataset.py
 src/coretex/coretex/dataset/network_dataset.py
 src/coretex/coretex/dataset/utils.py
+src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
 src/coretex/coretex/dataset/custom_dataset/__init__.py
 src/coretex/coretex/dataset/custom_dataset/base.py
 src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
 src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
 src/coretex/coretex/dataset/image_dataset/__init__.py
 src/coretex/coretex/dataset/image_dataset/base.py
 src/coretex/coretex/dataset/image_dataset/image_dataset.py
 src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
 src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
 src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
 src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
 src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
-src/coretex/coretex/dataset/object_detection_dataset/__init__.py
-src/coretex/coretex/dataset/object_detection_dataset/local_object_detection_dataset.py
-src/coretex/coretex/dataset/object_detection_dataset/object_detection_dataset.py
 src/coretex/coretex/experiment/__init__.py
 src/coretex/coretex/experiment/artifact.py
+src/coretex/coretex/experiment/executing_experiment.py
 src/coretex/coretex/experiment/experiment.py
+src/coretex/coretex/experiment/parameters.py
 src/coretex/coretex/experiment/status.py
-src/coretex/coretex/item/__init__.py
-src/coretex/coretex/item/any_local_item.py
-src/coretex/coretex/item/item.py
-src/coretex/coretex/item/local_item.py
-src/coretex/coretex/item/network_item.py
-src/coretex/coretex/item/custom_item/__init__.py
-src/coretex/coretex/item/custom_item/custom_item.py
-src/coretex/coretex/item/custom_item/custom_item_data.py
-src/coretex/coretex/item/custom_item/local_custom_item.py
-src/coretex/coretex/item/image_item/__init__.py
-src/coretex/coretex/item/image_item/image_format.py
-src/coretex/coretex/item/image_item/image_item.py
-src/coretex/coretex/item/image_item/image_item_data.py
-src/coretex/coretex/item/image_item/local_image_item.py
-src/coretex/coretex/item/image_segmentation_item/__init__.py
-src/coretex/coretex/item/image_segmentation_item/image_segmentation_item.py
-src/coretex/coretex/item/image_segmentation_item/local_image_segmentation_item.py
-src/coretex/coretex/item/object_detection_item/__init__.py
-src/coretex/coretex/item/object_detection_item/local_object_detection_item.py
-src/coretex/coretex/item/object_detection_item/object_detection_item.py
+src/coretex/coretex/experiment/metrics/__init__.py
+src/coretex/coretex/experiment/metrics/metric.py
+src/coretex/coretex/experiment/metrics/metric_factory.py
+src/coretex/coretex/experiment/metrics/metric_type.py
+src/coretex/coretex/experiment/metrics/utils.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
 src/coretex/coretex/model/__init__.py
 src/coretex/coretex/model/model.py
-src/coretex/coretex/project/__init__.py
-src/coretex/coretex/project/base.py
-src/coretex/coretex/project/project.py
-src/coretex/coretex/project/project_task.py
-src/coretex/coretex/project/workspace.py
+src/coretex/coretex/sample/__init__.py
+src/coretex/coretex/sample/any_local_sample.py
+src/coretex/coretex/sample/local_sample.py
+src/coretex/coretex/sample/network_sample.py
+src/coretex/coretex/sample/sample.py
+src/coretex/coretex/sample/computer_vision_sample/__init__.py
+src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+src/coretex/coretex/sample/custom_sample/__init__.py
+src/coretex/coretex/sample/custom_sample/custom_sample.py
+src/coretex/coretex/sample/custom_sample/custom_sample_data.py
+src/coretex/coretex/sample/custom_sample/local_custom_sample.py
+src/coretex/coretex/sample/image_sample/__init__.py
+src/coretex/coretex/sample/image_sample/image_format.py
+src/coretex/coretex/sample/image_sample/image_sample.py
+src/coretex/coretex/sample/image_sample/image_sample_data.py
+src/coretex/coretex/sample/image_sample/local_image_sample.py
+src/coretex/coretex/sample/image_segmentation_sample/__init__.py
+src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+src/coretex/coretex/space/__init__.py
+src/coretex/coretex/space/base.py
+src/coretex/coretex/space/project.py
+src/coretex/coretex/space/space.py
+src/coretex/coretex/space/space_task.py
 src/coretex/folder_management/__init__.py
 src/coretex/folder_management/folder_manager.py
 src/coretex/logging/__init__.py
 src/coretex/logging/log.py
 src/coretex/logging/log_severity.py
 src/coretex/logging/logger.py
 src/coretex/networking/__init__.py
+src/coretex/networking/chunk_upload_session.py
 src/coretex/networking/network_manager.py
+src/coretex/networking/network_manager_base.py
 src/coretex/networking/network_object.py
 src/coretex/networking/network_response.py
 src/coretex/networking/request_type.py
 src/coretex/networking/requests_manager.py
+src/coretex/networking/user_data.py
+src/coretex/nlp/__init__.py
+src/coretex/nlp/text.py
+src/coretex/nlp/token.py
+src/coretex/nlp/transcriber.py
+src/coretex/nlp/transcription.py
+src/coretex/nlp/utils.py
+src/coretex/project/__init__.py
+src/coretex/project/base.py
+src/coretex/project/calculate_metrics.py
+src/coretex/project/heartbeat.py
+src/coretex/project/local.py
+src/coretex/project/remote.py
 src/coretex/qiime2/__init__.py
+src/coretex/qiime2/utils.py
 src/coretex/threading/__init__.py
-src/coretex/threading/stoppable_thread.py
 src/coretex/threading/threaded_data_processor.py
 src/coretex/utils/__init__.py
 src/coretex/utils/console_progress_bar.py
 src/coretex/utils/date.py
 src/coretex/utils/file.py
-src/coretex/utils/number.py
-src/coretex/workspace/__init__.py
-src/coretex/workspace/base.py
-src/coretex/workspace/heartbeat.py
-src/coretex/workspace/local.py
-src/coretex/workspace/remote.py
+src/coretex/utils/number.py
```


# Comparing `tmp/datavision_beeyard_sdk-12.0.0.tar.gz` & `tmp/datavision_beeyard_sdk-12.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datavision_beeyard_sdk-12.0.0.tar", max compression
+gzip compressed data, was "datavision_beeyard_sdk-12.2.0.tar", max compression
```

## Comparing `datavision_beeyard_sdk-12.0.0.tar` & `datavision_beeyard_sdk-12.2.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0       90 2022-12-02 16:43:42.126544 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/__init__.py
--rw-r--r--   0        0        0       48 2022-12-02 16:43:42.126891 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.126891 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/__init__.py
--rw-r--r--   0        0        0      547 2022-12-02 16:43:42.127891 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/add_properties.py
--rw-r--r--   0        0        0      544 2022-12-02 16:43:42.128891 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/add_references.py
--rw-r--r--   0        0        0      523 2022-12-02 16:43:42.129891 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/add_tags.py
--rw-r--r--   0        0        0      385 2022-12-02 16:43:42.130893 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/aggregate_cells.py
--rw-r--r--   0        0        0      954 2022-12-02 16:43:42.132061 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/create_cell.py
--rw-r--r--   0        0        0      299 2022-12-02 16:43:42.133185 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/list_referenced_cells.py
--rw-r--r--   0        0        0      526 2022-12-02 16:43:42.134185 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/modify_cell_description.py
--rw-r--r--   0        0        0      561 2022-12-02 16:43:42.135187 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/modify_property.py
--rw-r--r--   0        0        0      296 2022-12-02 16:43:42.136185 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/read_cell.py
--rw-r--r--   0        0        0      268 2022-12-02 16:43:42.137186 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/remove_cell.py
--rw-r--r--   0        0        0      341 2022-12-02 16:43:42.137978 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/remove_properties.py
--rw-r--r--   0        0        0      341 2022-12-02 16:43:42.139356 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/remove_references.py
--rw-r--r--   0        0        0      529 2022-12-02 16:43:42.139356 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/remove_tags.py
--rw-r--r--   0        0        0      733 2022-12-02 16:43:42.141120 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/search_cells.py
--rw-r--r--   0        0        0      536 2022-12-02 16:43:42.141120 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/update_tags.py
--rw-r--r--   0        0        0      812 2022-12-02 16:43:42.142359 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/upload_cell.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.142359 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/document/__init__.py
--rw-r--r--   0        0        0      456 2022-12-02 16:43:42.143362 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/document/add_documents.py
--rw-r--r--   0        0        0      641 2022-12-02 16:43:42.144395 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/document/modify_document.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.145394 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/event/__init__.py
--rw-r--r--   0        0        0      386 2022-12-02 16:43:42.146360 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/event/aggregate_events.py
--rw-r--r--   0        0        0      278 2022-12-02 16:43:42.147304 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/event/read_event.py
--rw-r--r--   0        0        0      670 2022-12-02 16:43:42.147304 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/event/search_events.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.148304 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/__init__.py
--rw-r--r--   0        0        0      418 2022-12-02 16:43:42.149334 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/add_files.py
--rw-r--r--   0        0        0      622 2022-12-02 16:43:42.149334 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/add_properties.py
--rw-r--r--   0        0        0      447 2022-12-02 16:43:42.150334 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/modify_file.py
--rw-r--r--   0        0        0      636 2022-12-02 16:43:42.151335 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/modify_property.py
--rw-r--r--   0        0        0      322 2022-12-02 16:43:42.152335 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/read_file.py
--rw-r--r--   0        0        0      357 2022-12-02 16:43:42.153335 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/remove_files.py
--rw-r--r--   0        0        0      408 2022-12-02 16:43:42.153335 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/remove_properties.py
--rw-r--r--   0        0        0      611 2022-12-02 16:43:42.154336 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/update_tags.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.155368 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/health/__init__.py
--rw-r--r--   0        0        0      240 2022-12-02 16:43:42.155368 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/health/get_liveness.py
--rw-r--r--   0        0        0      242 2022-12-02 16:43:42.156335 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/health/get_readiness.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.157335 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/image/__init__.py
--rw-r--r--   0        0        0      444 2022-12-02 16:43:42.157528 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/image/add_images.py
--rw-r--r--   0        0        0      342 2022-12-02 16:43:42.158562 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/image/create_image_thumbnail.py
--rw-r--r--   0        0        0      339 2022-12-02 16:43:42.159629 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/image/read_image_thumbnail.py
--rw-r--r--   0        0        0      544 2022-12-02 16:43:42.159629 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/image/upload_image_thumbnail.py
--rw-r--r--   0        0        0        0 2023-03-21 14:58:46.464255 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/license/__init__.py
--rw-r--r--   0        0        0      274 2023-03-21 15:56:06.368253 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/license/get_license.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.160662 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/__init__.py
--rw-r--r--   0        0        0      455 2022-12-02 16:43:42.160662 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/add_overlays.py
--rw-r--r--   0        0        0      604 2022-12-02 16:43:42.161630 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/add_shapes.py
--rw-r--r--   0        0        0      555 2022-12-02 16:43:42.162662 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/modify_mask.py
--rw-r--r--   0        0        0      669 2022-12-02 16:43:42.163985 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/modify_overlay.py
--rw-r--r--   0        0        0      264 2022-12-02 16:43:42.165020 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/read_overlays.py
--rw-r--r--   0        0        0      389 2022-12-02 16:43:42.166124 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/read_shape.py
--rw-r--r--   0        0        0      464 2022-12-02 16:43:42.167132 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/remove_layers.py
--rw-r--r--   0        0        0      441 2022-12-02 16:43:42.167132 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/remove_shapes.py
--rw-r--r--   0        0        0      555 2022-12-02 16:43:42.168167 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/rename_layer.py
--rw-r--r--   0        0        0      617 2022-12-02 16:43:42.169134 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/upload_mask.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.169134 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/statistics/__init__.py
--rw-r--r--   0        0        0      373 2022-12-02 16:43:42.170172 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/statistics/compute_cell_stats_per_workspace.py
--rw-r--r--   0        0        0      623 2022-12-02 16:43:42.171168 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/statistics/compute_file_stats.py
--rw-r--r--   0        0        0      388 2022-12-02 16:43:42.172165 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/statistics/compute_shape_stats.py
--rw-r--r--   0        0        0      378 2022-12-02 16:43:42.173166 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/statistics/compute_tag_stats.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.174167 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/version/__init__.py
--rw-r--r--   0        0        0      239 2022-12-02 16:43:42.174349 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/version/read_version.py
--rw-r--r--   0        0        0        0 2022-12-02 16:43:42.174349 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/__init__.py
--rw-r--r--   0        0        0      627 2022-12-02 16:43:42.175794 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_favorite_queries.py
--rw-r--r--   0        0        0      600 2022-12-02 16:43:42.176989 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_or_replace_favorite_query.py
--rw-r--r--   0        0        0      449 2022-12-02 16:43:42.176989 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_or_replace_shape_template.py
--rw-r--r--   0        0        0      450 2022-12-02 16:43:42.178023 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_shape_templates.py
--rw-r--r--   0        0        0      794 2022-12-02 16:43:42.179026 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_tag_templates.py
--rw-r--r--   0        0        0      521 2022-12-02 16:43:42.180126 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/create_workspace.py
--rw-r--r--   0        0        0      674 2022-12-02 16:43:42.180126 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/modify_favorite_query.py
--rw-r--r--   0        0        0      620 2022-12-02 16:43:42.181160 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/modify_shape_template.py
--rw-r--r--   0        0        0      439 2022-12-02 16:43:42.182160 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/modify_workspace.py
--rw-r--r--   0        0        0      314 2022-12-02 16:43:42.183162 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/read_workspace.py
--rw-r--r--   0        0        0      450 2022-12-02 16:43:42.184160 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/remove_favorite_queries.py
--rw-r--r--   0        0        0      426 2022-12-02 16:43:42.184368 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/remove_shape_templates.py
--rw-r--r--   0        0        0      637 2022-12-02 16:43:42.185401 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/remove_tag_templates.py
--rw-r--r--   0        0        0      311 2022-12-02 16:43:42.186406 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/remove_workspace.py
--rw-r--r--   0        0        0      673 2022-12-02 16:43:42.187401 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/search_workspaces.py
--rw-r--r--   0        0        0     5358 2023-03-21 15:56:15.596148 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/automation.py
--rw-r--r--   0        0        0     9824 2022-12-02 16:43:42.188871 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/client.py
--rw-r--r--   0        0        0      509 2023-01-13 17:07:50.854724 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/exceptions.py
--rw-r--r--   0        0        0      851 2022-12-02 16:43:42.189871 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/__init__.py
--rw-r--r--   0        0        0     1298 2022-12-02 16:43:42.190579 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/add_documents_multipart_data.py
--rw-r--r--   0        0        0     1298 2022-12-02 16:43:42.190579 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/add_files_multipart_data.py
--rw-r--r--   0        0        0     1295 2022-12-02 16:43:42.191618 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/add_images_multipart_data.py
--rw-r--r--   0        0        0      781 2022-12-02 16:43:42.192690 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/favorite_query_dto.py
--rw-r--r--   0        0        0     2762 2022-12-02 16:43:42.193697 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/filter.py
--rw-r--r--   0        0        0      266 2022-12-02 16:43:42.194696 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/modify_cell_input_dto.py
--rw-r--r--   0        0        0      813 2022-12-02 16:43:42.195925 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/modify_document_input_dto.py
--rw-r--r--   0        0        0      470 2022-12-02 16:43:42.195925 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/modify_overlay_multipart_data.py
--rw-r--r--   0        0        0      939 2022-12-02 16:43:42.196925 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/property_dto.py
--rw-r--r--   0        0        0      915 2022-12-02 16:43:42.198103 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/reference_dto.py
--rw-r--r--   0        0        0      965 2022-12-02 16:43:42.199164 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/tag_dto.py
--rw-r--r--   0        0        0      597 2022-12-02 16:43:42.200176 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/tag_template_dto.py
--rw-r--r--   0        0        0     1030 2022-12-02 16:43:42.200176 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/update_tags_dto.py
--rw-r--r--   0        0        0      347 2022-12-02 16:43:42.201213 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/upload_cell_multipart_data.py
--rw-r--r--   0        0        0      902 2022-12-02 16:43:42.202177 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/upload_mask_multipart_data.py
--rw-r--r--   0        0        0      795 2022-12-02 16:43:42.203177 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/workspace_descriptor_dto.py
--rw-r--r--   0        0        0     3152 2023-01-13 17:07:49.968375 datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/types.py
--rw-r--r--   0        0        0      919 2023-04-04 13:45:56.597199 datavision_beeyard_sdk-12.0.0/pyproject.toml
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 datavision_beeyard_sdk-12.0.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2022-12-02 16:43:42.126544 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2022-12-02 16:43:42.126891 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.126891 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/__init__.py
+-rw-r--r--   0        0        0      547 2022-12-02 16:43:42.127891 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/add_properties.py
+-rw-r--r--   0        0        0      544 2022-12-02 16:43:42.128891 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/add_references.py
+-rw-r--r--   0        0        0      523 2022-12-02 16:43:42.129891 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/add_tags.py
+-rw-r--r--   0        0        0      385 2022-12-02 16:43:42.130893 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/aggregate_cells.py
+-rw-r--r--   0        0        0      954 2022-12-02 16:43:42.132061 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/create_cell.py
+-rw-r--r--   0        0        0      299 2022-12-02 16:43:42.133185 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/list_referenced_cells.py
+-rw-r--r--   0        0        0      526 2022-12-02 16:43:42.134185 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/modify_cell_description.py
+-rw-r--r--   0        0        0      561 2022-12-02 16:43:42.135187 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/modify_property.py
+-rw-r--r--   0        0        0      296 2022-12-02 16:43:42.136185 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/read_cell.py
+-rw-r--r--   0        0        0      268 2022-12-02 16:43:42.137186 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/remove_cell.py
+-rw-r--r--   0        0        0      341 2022-12-02 16:43:42.137978 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/remove_properties.py
+-rw-r--r--   0        0        0      341 2022-12-02 16:43:42.139356 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/remove_references.py
+-rw-r--r--   0        0        0      529 2022-12-02 16:43:42.139356 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/remove_tags.py
+-rw-r--r--   0        0        0      733 2022-12-02 16:43:42.141120 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/search_cells.py
+-rw-r--r--   0        0        0      536 2022-12-02 16:43:42.141120 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/update_tags.py
+-rw-r--r--   0        0        0      812 2022-12-02 16:43:42.142359 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/upload_cell.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.142359 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/document/__init__.py
+-rw-r--r--   0        0        0      456 2022-12-02 16:43:42.143362 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/document/add_documents.py
+-rw-r--r--   0        0        0      641 2022-12-02 16:43:42.144395 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/document/modify_document.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.145394 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/event/__init__.py
+-rw-r--r--   0        0        0      386 2022-12-02 16:43:42.146360 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/event/aggregate_events.py
+-rw-r--r--   0        0        0      278 2022-12-02 16:43:42.147304 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/event/read_event.py
+-rw-r--r--   0        0        0      670 2022-12-02 16:43:42.147304 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/event/search_events.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.148304 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/__init__.py
+-rw-r--r--   0        0        0      418 2022-12-02 16:43:42.149334 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/add_files.py
+-rw-r--r--   0        0        0      622 2022-12-02 16:43:42.149334 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/add_properties.py
+-rw-r--r--   0        0        0      447 2022-12-02 16:43:42.150334 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/modify_file.py
+-rw-r--r--   0        0        0      636 2022-12-02 16:43:42.151335 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/modify_property.py
+-rw-r--r--   0        0        0      322 2022-12-02 16:43:42.152335 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/read_file.py
+-rw-r--r--   0        0        0      357 2022-12-02 16:43:42.153335 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/remove_files.py
+-rw-r--r--   0        0        0      408 2022-12-02 16:43:42.153335 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/remove_properties.py
+-rw-r--r--   0        0        0      611 2022-12-02 16:43:42.154336 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/update_tags.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.155368 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/health/__init__.py
+-rw-r--r--   0        0        0      240 2022-12-02 16:43:42.155368 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/health/get_liveness.py
+-rw-r--r--   0        0        0      242 2022-12-02 16:43:42.156335 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/health/get_readiness.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.157335 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/image/__init__.py
+-rw-r--r--   0        0        0      444 2022-12-02 16:43:42.157528 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/image/add_images.py
+-rw-r--r--   0        0        0      342 2022-12-02 16:43:42.158562 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/image/create_image_thumbnail.py
+-rw-r--r--   0        0        0      339 2022-12-02 16:43:42.159629 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/image/read_image_thumbnail.py
+-rw-r--r--   0        0        0      544 2022-12-02 16:43:42.159629 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/image/upload_image_thumbnail.py
+-rw-r--r--   0        0        0        0 2023-03-21 14:58:46.464255 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/license/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-21 15:56:06.368253 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/license/get_license.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.160662 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/__init__.py
+-rw-r--r--   0        0        0      455 2022-12-02 16:43:42.160662 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/add_overlays.py
+-rw-r--r--   0        0        0      604 2022-12-02 16:43:42.161630 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/add_shapes.py
+-rw-r--r--   0        0        0      555 2022-12-02 16:43:42.162662 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/modify_mask.py
+-rw-r--r--   0        0        0      669 2022-12-02 16:43:42.163985 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/modify_overlay.py
+-rw-r--r--   0        0        0      264 2022-12-02 16:43:42.165020 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/read_overlays.py
+-rw-r--r--   0        0        0      389 2022-12-02 16:43:42.166124 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/read_shape.py
+-rw-r--r--   0        0        0      464 2022-12-02 16:43:42.167132 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/remove_layers.py
+-rw-r--r--   0        0        0      441 2022-12-02 16:43:42.167132 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/remove_shapes.py
+-rw-r--r--   0        0        0      555 2022-12-02 16:43:42.168167 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/rename_layer.py
+-rw-r--r--   0        0        0      617 2022-12-02 16:43:42.169134 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/upload_mask.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.169134 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/statistics/__init__.py
+-rw-r--r--   0        0        0      537 2023-05-25 11:47:08.496082 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/statistics/compute_cell_stats_per_workspace.py
+-rw-r--r--   0        0        0      623 2022-12-02 16:43:42.171168 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/statistics/compute_file_stats.py
+-rw-r--r--   0        0        0      388 2022-12-02 16:43:42.172165 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/statistics/compute_shape_stats.py
+-rw-r--r--   0        0        0      378 2022-12-02 16:43:42.173166 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/statistics/compute_tag_stats.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.174167 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/version/__init__.py
+-rw-r--r--   0        0        0      239 2022-12-02 16:43:42.174349 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/version/read_version.py
+-rw-r--r--   0        0        0        0 2022-12-02 16:43:42.174349 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/__init__.py
+-rw-r--r--   0        0        0      627 2022-12-02 16:43:42.175794 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_favorite_queries.py
+-rw-r--r--   0        0        0      600 2022-12-02 16:43:42.176989 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_or_replace_favorite_query.py
+-rw-r--r--   0        0        0      449 2022-12-02 16:43:42.176989 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_or_replace_shape_template.py
+-rw-r--r--   0        0        0      450 2022-12-02 16:43:42.178023 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_shape_templates.py
+-rw-r--r--   0        0        0      794 2022-12-02 16:43:42.179026 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_tag_templates.py
+-rw-r--r--   0        0        0      521 2022-12-02 16:43:42.180126 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0      674 2022-12-02 16:43:42.180126 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/modify_favorite_query.py
+-rw-r--r--   0        0        0      620 2022-12-02 16:43:42.181160 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/modify_shape_template.py
+-rw-r--r--   0        0        0      439 2022-12-02 16:43:42.182160 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/modify_workspace.py
+-rw-r--r--   0        0        0      314 2022-12-02 16:43:42.183162 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/read_workspace.py
+-rw-r--r--   0        0        0      450 2022-12-02 16:43:42.184160 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/remove_favorite_queries.py
+-rw-r--r--   0        0        0      426 2022-12-02 16:43:42.184368 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/remove_shape_templates.py
+-rw-r--r--   0        0        0      637 2022-12-02 16:43:42.185401 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/remove_tag_templates.py
+-rw-r--r--   0        0        0      311 2022-12-02 16:43:42.186406 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/remove_workspace.py
+-rw-r--r--   0        0        0      673 2022-12-02 16:43:42.187401 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/search_workspaces.py
+-rw-r--r--   0        0        0     5358 2023-03-21 15:56:15.596148 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/automation.py
+-rw-r--r--   0        0        0     9873 2023-05-26 07:35:41.858917 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/client.py
+-rw-r--r--   0        0        0      509 2023-01-13 17:07:50.854724 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/exceptions.py
+-rw-r--r--   0        0        0      851 2022-12-02 16:43:42.189871 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/__init__.py
+-rw-r--r--   0        0        0     1298 2022-12-02 16:43:42.190579 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/add_documents_multipart_data.py
+-rw-r--r--   0        0        0     1298 2022-12-02 16:43:42.190579 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/add_files_multipart_data.py
+-rw-r--r--   0        0        0     1295 2022-12-02 16:43:42.191618 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/add_images_multipart_data.py
+-rw-r--r--   0        0        0      781 2022-12-02 16:43:42.192690 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/favorite_query_dto.py
+-rw-r--r--   0        0        0     2762 2022-12-02 16:43:42.193697 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/filter.py
+-rw-r--r--   0        0        0      266 2022-12-02 16:43:42.194696 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/modify_cell_input_dto.py
+-rw-r--r--   0        0        0      813 2022-12-02 16:43:42.195925 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/modify_document_input_dto.py
+-rw-r--r--   0        0        0      470 2022-12-02 16:43:42.195925 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/modify_overlay_multipart_data.py
+-rw-r--r--   0        0        0      939 2022-12-02 16:43:42.196925 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/property_dto.py
+-rw-r--r--   0        0        0      915 2022-12-02 16:43:42.198103 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/reference_dto.py
+-rw-r--r--   0        0        0      965 2022-12-02 16:43:42.199164 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/tag_dto.py
+-rw-r--r--   0        0        0      597 2022-12-02 16:43:42.200176 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/tag_template_dto.py
+-rw-r--r--   0        0        0     1030 2022-12-02 16:43:42.200176 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/update_tags_dto.py
+-rw-r--r--   0        0        0      347 2022-12-02 16:43:42.201213 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/upload_cell_multipart_data.py
+-rw-r--r--   0        0        0      902 2022-12-02 16:43:42.202177 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/upload_mask_multipart_data.py
+-rw-r--r--   0        0        0      795 2022-12-02 16:43:42.203177 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/workspace_descriptor_dto.py
+-rw-r--r--   0        0        0     3152 2023-01-13 17:07:49.968375 datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/types.py
+-rw-r--r--   0        0        0      910 2023-05-26 08:07:41.047980 datavision_beeyard_sdk-12.2.0/pyproject.toml
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 datavision_beeyard_sdk-12.2.0/PKG-INFO
```

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/add_properties.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/add_properties.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/add_references.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/add_references.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/add_tags.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/add_tags.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/create_cell.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/create_cell.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/modify_cell_description.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/modify_cell_description.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/modify_property.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/modify_property.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/remove_tags.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/remove_tags.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/search_cells.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/search_cells.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/update_tags.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/update_tags.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/cell/upload_cell.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/cell/upload_cell.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/document/modify_document.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/document/modify_document.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/event/search_events.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/event/search_events.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/add_properties.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/add_properties.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/modify_property.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/modify_property.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/file/update_tags.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/file/update_tags.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/image/upload_image_thumbnail.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/image/upload_image_thumbnail.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/add_shapes.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/add_shapes.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/modify_mask.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/modify_mask.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/modify_overlay.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/modify_overlay.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/rename_layer.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/rename_layer.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/overlay/upload_mask.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/overlay/upload_mask.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/statistics/compute_file_stats.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/statistics/compute_file_stats.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_favorite_queries.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_favorite_queries.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_or_replace_favorite_query.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_or_replace_favorite_query.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/add_tag_templates.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/add_tag_templates.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/create_workspace.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/modify_favorite_query.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/modify_favorite_query.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/modify_shape_template.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/modify_shape_template.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/remove_tag_templates.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/remove_tag_templates.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/api/workspace/search_workspaces.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/api/workspace/search_workspaces.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/automation.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/automation.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/client.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,30 @@
         max_waiting_time_ms=0,
         client_id="byard",
         client_secret="",
         login_url=None,
         use_token=False,
         token=None,
     ):
-        self.base_url = base_url
+        self.base_url = base_url[:-1] if base_url.endswith("/") else base_url
         self.username = username
         self.password = password
         self.grant_type = grant_type
         self.delay = max_waiting_time_ms
         self.endpoint_auth: str = "/oauth/token/"
         self.client_id = client_id
         self.client_secret = client_secret
         self.login_url = login_url
         if use_token:
-            self.token_headers = token
+            if isinstance(token, dict):
+                self.token_headers = token
+            elif "Authorization" in token:
+                self.token_headers = {"Authorization": f"Bearer {token.split(' ')[2]}"}
+            else:
+                self.token_headers = {"Authorization": f"Bearer {token}"}
         else:
             self.authenticate()
 
     def authenticate(self):
         if self.grant_type == "password":
             data = {
                 "grant_type": self.grant_type,
@@ -49,26 +54,20 @@
                 "client_id": self.client_id,
                 "client_secret": self.client_secret,
             }
             header = {}
         else:
             raise Exception(f"Grant type '{self.grant_type}' not recognized")
         if self.login_url is None:
-            self.base_url = (
-                self.base_url[:-1] if self.base_url.endswith("/") else self.base_url
-            )
             response = httpx.post(
                 f"{self.base_url}{self.endpoint_auth}".replace("hive", "id"),
                 data=data,
                 headers=header,
             )
         else:
-            self.login_url = (
-                self.login_url[:-1] if self.login_url.endswith("/") else self.login_url
-            )
             response = httpx.post(
                 f"{self.login_url}{self.endpoint_auth}",
                 data=data,
                 headers=header,
             )
         if response.status_code not in range(200, 300):
             raise Exception("Bad authenticate response")
```

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/__init__.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/add_documents_multipart_data.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/add_documents_multipart_data.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/add_files_multipart_data.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/add_files_multipart_data.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/add_images_multipart_data.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/add_images_multipart_data.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/favorite_query_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/favorite_query_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/filter.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/filter.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/modify_document_input_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/modify_document_input_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/property_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/property_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/reference_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/reference_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/tag_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/tag_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/tag_template_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/tag_template_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/update_tags_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/update_tags_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/upload_mask_multipart_data.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/upload_mask_multipart_data.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/models/workspace_descriptor_dto.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/models/workspace_descriptor_dto.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/datavision_beeyard_sdk/types.py` & `datavision_beeyard_sdk-12.2.0/datavision_beeyard_sdk/types.py`

 * *Files identical despite different names*

### Comparing `datavision_beeyard_sdk-12.0.0/pyproject.toml` & `datavision_beeyard_sdk-12.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "datavision-beeyard-sdk"
-version = "12.0.0"
+version = "12.2.0"
 description = "BeeYard Python SDK"
 authors = ["DataVision <support@datavision.software>"]
 license = "MIT"
 homepage = "https://docs.beeyard.services/docs/reference/sdk/python/"
 keywords = ["python", "sdk", "beeyard"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = ">=0.15.4,<0.19.0"
 attrs = "^21.2.0"
+httpx = "^0.24.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 Pillow = "^8.3.2"
 flake8 = "^3.9.2"
 ipykernel = "^6.5.1"
 torch = "^1.11.0"
```

### Comparing `datavision_beeyard_sdk-12.0.0/PKG-INFO` & `datavision_beeyard_sdk-12.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: datavision-beeyard-sdk
-Version: 12.0.0
+Version: 12.2.0
 Summary: BeeYard Python SDK
 Home-page: https://docs.beeyard.services/docs/reference/sdk/python/
 License: MIT
 Keywords: python,sdk,beeyard
 Author: DataVision
 Author-email: support@datavision.software
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: attrs (>=21.2.0,<22.0.0)
-Requires-Dist: httpx (>=0.15.4,<0.19.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
```


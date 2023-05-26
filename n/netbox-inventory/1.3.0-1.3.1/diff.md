# Comparing `tmp/netbox-inventory-1.3.0.tar.gz` & `tmp/netbox-inventory-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.3.0.tar", last modified: Wed May  3 08:04:19 2023, max compression
+gzip compressed data, was "netbox-inventory-1.3.1.tar", last modified: Fri May 26 18:19:55 2023, max compression
```

## Comparing `netbox-inventory-1.3.0.tar` & `netbox-inventory-1.3.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.881295 netbox-inventory-1.3.0/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.881295 netbox-inventory-1.3.0/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/forms/reassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.877294 netbox-inventory-1.3.0/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.885295 netbox-inventory-1.3.0/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:04:19.881295 netbox-inventory-1.3.0/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 08:04:19.000000 netbox-inventory-1.3.0/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 08:04:02.000000 netbox-inventory-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:04:19.889295 netbox-inventory-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.043877 netbox-inventory-1.3.1/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/setup.cfg
```

### Comparing `netbox-inventory-1.3.0/LICENSE` & `netbox-inventory-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/PKG-INFO` & `netbox-inventory-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.3.0
+Version: 1.3.1
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox-inventory-1.3.0/README.md` & `netbox-inventory-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/__init__.py` & `netbox-inventory-1.3.1/netbox_inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/analyzers.py` & `netbox-inventory-1.3.1/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.3.1/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/api/serializers.py` & `netbox-inventory-1.3.1/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/api/urls.py` & `netbox-inventory-1.3.1/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/api/views.py` & `netbox-inventory-1.3.1/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/filtersets.py` & `netbox-inventory-1.3.1/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/forms/assign.py` & `netbox-inventory-1.3.1/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.3.1/netbox_inventory/forms/bulk.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/forms/bulk_add.py` & `netbox-inventory-1.3.1/netbox_inventory/forms/bulk_add.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/forms/create.py` & `netbox-inventory-1.3.1/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/forms/filters.py` & `netbox-inventory-1.3.1/netbox_inventory/forms/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/forms/models.py` & `netbox-inventory-1.3.1/netbox_inventory/forms/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/forms/reassign.py` & `netbox-inventory-1.3.1/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.3.1/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.3.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.3.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/models.py` & `netbox-inventory-1.3.1/netbox_inventory/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/navigation.py` & `netbox-inventory-1.3.1/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/search.py` & `netbox-inventory-1.3.1/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/signals.py` & `netbox-inventory-1.3.1/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tables.py` & `netbox-inventory-1.3.1/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/template_content.py` & `netbox-inventory-1.3.1/netbox_inventory/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files 8% similar despite different names*

```diff
@@ -75,41 +75,37 @@
       <div class="card">
         <h5 class="card-header">Asset count by type & status</h5>
         <div class="card-body">
           <table class="table table-hover object-list table-striped">
           <thead>
             <tr>
               <th>Inventory Item Type</th>
-              <th>Status</th>
-              <th>Count</th>
+              <th>Status - Count</th>
             </tr>
           </thead>
           <tbody>
-            {% for tsc in type_status_counts %}
+            {% for tsc in type_status_objects %}
             <tr>
-            {% ifchanged tsc.inventoryitem_type %}
               <td>
                 <a href="{% url 'plugins:netbox_inventory:inventoryitemtype' tsc.inventoryitem_type %}">
                   {{ tsc.inventoryitem_type__manufacturer__name }} {{ tsc.inventoryitem_type__model }}
                 </a>
               </td>
-            {% else %}
-              <td>&nbsp;</td>
-            {% endifchanged %}
-              <td>
-                {% badge value=tsc.label bg_color=tsc.color %}
-              </td>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ tsc.inventoryitem_type }}&status={{ tsc.status }}">
-                  {{ tsc.count }}
-                </a>
+              <td style="max-width:400px;">
+                <div class="d-flex" style="overflow:auto;">
+                  {% for status in tsc.status_list %}
+                    <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ tsc.inventoryitem_type }}&status={{ status.status }}" class="w-100 me-2">
+                      {% badge value=status.label|add:' - '|add:status.count bg_color=status.color|add:' w-100' %}
+                    </a>
+                  {% endfor %}
+                </div>
               </td>
             </tr>
             {% empty %}
-            <tr><td class="text-center text-muted" colspan="3">— No assets found —</td></tr>
+            <tr><td class="text-center text-muted" colspan="2">— No assets found —</td></tr>
             {% endfor %}
           </tbody>
           </table>
         </div>
       </div>
   
     </div>
```

#### html2text {}

```diff
@@ -12,19 +12,20 @@
 Assets {{_asset_table.rows|length_}}
 {% include 'inc/panels/custom_fields.html' %}
 ** Asset count by status **
 Status                                       Count
 {% badge value=sc.label bg_color=sc.color %} {{_sc.count_}}
 â No assets found â
 ** Asset count by type & status **
-Inventory Item Type                        Status Count
-{                                                 {% badge           {
-{                                                value=tsc.label    {
-tsc.inventoryitem_type__manufacturer__name        bg_color=tsc.color tsc.count
-}}_{{_tsc.inventoryitem_type__model_}}            %}                 }}
+Inventory Item Type                        Status - Count
+{                                          {% for status in tsc.status_list %}
+{                                          {%_badge_value=status.label|add:'_-
+tsc.inventoryitem_type__manufacturer__name '|add:status.count
+}}_{{_tsc.inventoryitem_type__model_}}     bg_color=status.color|add:'_w-100'
+                                           %} {% endfor %}
 â No assets found â
 ** Child Groups **
 {% render_table child_groups_table 'inc/table.html' %}
 {% if perms.netbox_inventory.add_inventoryitemgroup %}
 _Add_Group
 {% endif %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
```

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
-      {% include 'inc/panels/contacts.html' %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Supplied Assets</h5>
         <div class="card-body table-responsive">
```

#### html2text {}

```diff
@@ -8,12 +8,12 @@
 ** Supplier **
 Name        {{ object.name }}
 Description {{ object.description }}
 Purchases   {{_purchase_count_}}
 Assets      {{_asset_count_}}
 {% include 'inc/panels/tags.html' %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
-comments.html' %} {% include 'inc/panels/contacts.html' %}
+comments.html' %}
 ** Supplied Assets **
 {% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
 with paginator=asset_table.paginator page=asset_table.page %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_create.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/custom.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/settings.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.3.1/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.3.0"
+        assert __version__ == "1.3.1"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.3.0/netbox_inventory/urls.py` & `netbox-inventory-1.3.1/netbox_inventory/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from django.urls import path
+from django.urls import include, path
 
 from netbox.views.generic import ObjectChangeLogView, ObjectJournalView
+from utilities.urls import get_model_urls
 from . import models, views
 
 
 urlpatterns = (
 
     # Assets
     path('assets/', views.AssetListView.as_view(), name='asset_list'),
@@ -29,18 +30,15 @@
     # Suppliers
     path('suppliers/', views.SupplierListView.as_view(), name='supplier_list'),
     path('suppliers/add/', views.SupplierEditView.as_view(), name='supplier_add'),
     path('suppliers/import/', views.SupplierBulkImportView.as_view(), name='supplier_import'),
     path('suppliers/edit/', views.SupplierBulkEditView.as_view(), name='supplier_bulk_edit'),
     path('suppliers/delete/', views.SupplierBulkDeleteView.as_view(), name='supplier_bulk_delete'),
     path('suppliers/<int:pk>', views.SupplierView.as_view(), name='supplier'),
-    path('suppliers/<int:pk>/edit/', views.SupplierEditView.as_view(), name='supplier_edit'),
-    path('suppliers/<int:pk>/delete/', views.SupplierDeleteView.as_view(), name='supplier_delete'),
-    path('suppliers/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='supplier_changelog', kwargs={'model': models.Supplier}),
-    path('suppliers/<int:pk>/journal/', ObjectJournalView.as_view(), name='supplier_journal', kwargs={'model': models.Supplier}),
+    path('suppliers/<int:pk>/', include(get_model_urls('netbox_inventory', 'supplier'))),
 
     # Purchases
     path('purchases/', views.PurchaseListView.as_view(), name='purchase_list'),
     path('purchases/add/', views.PurchaseEditView.as_view(), name='purchase_add'),
     path('purchases/import/', views.PurchaseBulkImportView.as_view(), name='purchase_import'),
     path('purchases/edit/', views.PurchaseBulkEditView.as_view(), name='purchase_bulk_edit'),
     path('purchases/delete/', views.PurchaseBulkDeleteView.as_view(), name='purchase_bulk_delete'),
```

### Comparing `netbox-inventory-1.3.0/netbox_inventory/utils.py` & `netbox-inventory-1.3.1/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/asset.py` & `netbox-inventory-1.3.1/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.3.1/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.3.1/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/asset_reassign.py` & `netbox-inventory-1.3.1/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.3.1/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/purchase.py` & `netbox-inventory-1.3.1/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/supplier.py` & `netbox-inventory-1.3.1/netbox_inventory/views/supplier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from netbox.views import generic
+from tenancy.views import ObjectContactsView
 from utilities.utils import count_related
+from utilities.views import register_model_view
 from .. import filtersets, forms, models, tables
 
 __all__ = (
     'SupplierView',
     'SupplierListView',
     'SupplierEditView',
     'SupplierDeleteView',
     'SupplierBulkImportView',
     'SupplierBulkEditView',
     'SupplierBulkDeleteView',
+    'SupplierContactsView',
 )
 
+
 class SupplierView(generic.ObjectView):
     queryset = models.Supplier.objects.all()
 
     def get_extra_context(self, request, instance):
         supplier_assets = models.Asset.objects.restrict(request.user, 'view').filter(
             purchase__supplier=instance
         )
@@ -25,29 +29,32 @@
 
         return {
             'asset_table': asset_table,
             'asset_count': models.Asset.objects.filter(purchase__supplier=instance).count(),
             'purchase_count': models.Purchase.objects.filter(supplier=instance).count(),
         }
 
+
 class SupplierListView(generic.ObjectListView):
     queryset = models.Supplier.objects.annotate(
         purchase_count=count_related(models.Purchase, 'supplier'),
         asset_count=count_related(models.Asset, 'purchase__supplier'),
     )
     table = tables.SupplierTable
     filterset = filtersets.SupplierFilterSet
     filterset_form = forms.SupplierFilterForm
 
 
+@register_model_view(models.Supplier, 'edit')
 class SupplierEditView(generic.ObjectEditView):
     queryset = models.Supplier.objects.all()
     form = forms.SupplierForm
 
 
+@register_model_view(models.Supplier, 'delete')
 class SupplierDeleteView(generic.ObjectDeleteView):
     queryset = models.Supplier.objects.all()
 
 
 class SupplierBulkImportView(generic.BulkImportView):
     queryset = models.Supplier.objects.all()
     model_form = forms.SupplierImportForm
@@ -59,7 +66,12 @@
     table = tables.SupplierTable
     form = forms.SupplierBulkEditForm
 
 
 class SupplierBulkDeleteView(generic.BulkDeleteView):
     queryset = models.Supplier.objects.all()
     table = tables.SupplierTable
+
+
+@register_model_view(models.Supplier, 'contacts')
+class SupplierContactsView(ObjectContactsView):
+    queryset = models.Supplier.objects.all()
```

### Comparing `netbox-inventory-1.3.0/netbox_inventory/views/tabs.py` & `netbox-inventory-1.3.1/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.3.1/netbox_inventory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.3.0
+Version: 1.3.1
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox-inventory-1.3.0/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.3.1/netbox_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.0/pyproject.toml` & `netbox-inventory-1.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


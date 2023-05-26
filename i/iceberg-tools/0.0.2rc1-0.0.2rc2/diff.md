# Comparing `tmp/iceberg_tools-0.0.2rc1.tar.gz` & `tmp/iceberg_tools-0.0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg_tools-0.0.2rc1.tar", last modified: Thu May 25 21:08:48 2023, max compression
+gzip compressed data, was "iceberg_tools-0.0.2rc2.tar", last modified: Fri May 26 00:30:26 2023, max compression
```

## Comparing `iceberg_tools-0.0.2rc1.tar` & `iceberg_tools-0.0.2rc2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:48.002102 iceberg_tools-0.0.2rc1/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2656 2023-05-25 21:08:48.001793 iceberg_tools-0.0.2rc1/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1941 2023-05-25 21:06:29.000000 iceberg_tools-0.0.2rc1/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.963109 iceberg_tools-0.0.2rc1/iceberg_tools/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 16:19:26.000000 iceberg_tools-0.0.2rc1/iceberg_tools/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.967984 iceberg_tools-0.0.2rc1/iceberg_tools/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142      482 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/iceberg_tools/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4329 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/iceberg_tools/cli/data.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5607 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/iceberg_tools/cli/schema.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.970180 iceberg_tools-0.0.2rc1/iceberg_tools/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-25 15:58:53.000000 iceberg_tools-0.0.2rc1/iceberg_tools/data/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.970579 iceberg_tools-0.0.2rc1/iceberg_tools/data/migrator/
--rw-r--r--   0 walsbr   (320923486) 1971611142    12261 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/iceberg_tools/data/migrator/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6137 2023-05-25 19:18:02.000000 iceberg_tools-0.0.2rc1/iceberg_tools/data/pfb.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.975499 iceberg_tools-0.0.2rc1/iceberg_tools/data/simplifier/
--rw-r--r--   0 walsbr   (320923486) 1971611142    25734 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/iceberg_tools/data/simplifier/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142   123504 2023-05-23 18:08:13.000000 iceberg_tools-0.0.2rc1/iceberg_tools/data/simplifier/oid_lookup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.978474 iceberg_tools-0.0.2rc1/iceberg_tools/schema/
--rw-r--r--   0 walsbr   (320923486) 1971611142     9512 2023-05-25 19:25:02.000000 iceberg_tools-0.0.2rc1/iceberg_tools/schema/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1348 2023-05-13 22:22:19.000000 iceberg_tools-0.0.2rc1/iceberg_tools/schema/bmeg.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    19847 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/iceberg_tools/schema/gen3.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4157 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/iceberg_tools/schema/gen3_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6840 2023-05-25 15:57:02.000000 iceberg_tools-0.0.2rc1/iceberg_tools/util.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.966338 iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2656 2023-05-25 21:08:47.000000 iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2140 2023-05-25 21:08:47.000000 iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-25 21:08:47.000000 iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       51 2023-05-25 21:08:47.000000 iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      146 2023-05-25 21:08:47.000000 iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-05-25 21:08:47.000000 iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-25 21:08:48.002165 iceberg_tools-0.0.2rc1/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5682 2023-05-25 21:08:32.000000 iceberg_tools-0.0.2rc1/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.960427 iceberg_tools-0.0.2rc1/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.979143 iceberg_tools-0.0.2rc1/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:03.000000 iceberg_tools-0.0.2rc1/tests/integration/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.993426 iceberg_tools-0.0.2rc1/tests/integration/bmeg/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1834 2023-05-15 20:39:46.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      967 2023-05-15 20:24:40.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      782 2023-05-15 20:39:22.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_edge_load_granular_reference.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2736 2023-05-15 20:39:04.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_edge_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1449 2023-05-15 20:38:41.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_invalid_edges.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      255 2023-05-15 20:24:59.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_lathe_lint.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      662 2023-05-15 20:38:23.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_negative_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      829 2023-05-23 20:22:18.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      330 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_schema_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1140 2023-05-15 20:38:10.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_spot_check_embedded_type.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      731 2023-05-15 20:37:50.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_trivial_edge_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      888 2023-05-15 20:37:28.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      340 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_yaml_anonymous_schemas.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:47.994532 iceberg_tools-0.0.2rc1/tests/integration/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-23 23:15:41.000000 iceberg_tools-0.0.2rc1/tests/integration/data/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4897 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/tests/integration/data/test_pfb.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:48.000494 iceberg_tools-0.0.2rc1/tests/integration/gen3/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 18:03:42.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      616 2023-05-18 20:08:55.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      911 2023-05-15 20:20:57.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_codeable_concept.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      451 2023-05-15 20:17:07.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_embedded_types.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-14 12:07:10.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_identifiers.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      171 2023-05-12 18:57:49.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_individual_yaml.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-05-12 18:56:56.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_keys.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      979 2023-05-23 19:23:34.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_primitive.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      469 2023-05-15 20:06:10.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_quantities.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      517 2023-05-18 20:10:27.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_research_study_has_project.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      155 2023-05-24 00:59:54.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1832 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_simplify_medication.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1744 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_simplify_task.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       34 2023-05-18 20:08:09.000000 iceberg_tools-0.0.2rc1/tests/integration/gen3/test_task.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-25 21:08:48.001462 iceberg_tools-0.0.2rc1/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:24.000000 iceberg_tools-0.0.2rc1/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      176 2023-05-15 20:40:27.000000 iceberg_tools-0.0.2rc1/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 iceberg_tools-0.0.2rc1/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3144 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/tests/unit/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1080 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc1/tests/unit/test_simplify.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.309278 iceberg_tools-0.0.2rc2/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2862 2023-05-26 00:30:26.308979 iceberg_tools-0.0.2rc2/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2126 2023-05-26 00:28:26.000000 iceberg_tools-0.0.2rc2/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.170302 iceberg_tools-0.0.2rc2/iceberg_tools/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 16:19:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.175709 iceberg_tools-0.0.2rc2/iceberg_tools/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      482 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4423 2023-05-25 22:36:19.000000 iceberg_tools-0.0.2rc2/iceberg_tools/cli/data.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5607 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/cli/schema.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.192399 iceberg_tools-0.0.2rc2/iceberg_tools/data/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-25 15:58:53.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.192783 iceberg_tools-0.0.2rc2/iceberg_tools/data/migrator/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12270 2023-05-25 22:13:53.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/migrator/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6137 2023-05-25 19:18:02.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/pfb.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.193969 iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    25714 2023-05-25 22:21:05.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142   123504 2023-05-23 18:08:13.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/oid_lookup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.196129 iceberg_tools-0.0.2rc2/iceberg_tools/schema/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9512 2023-05-25 19:25:02.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1348 2023-05-13 22:22:19.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/bmeg.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    19847 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4157 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3_validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6840 2023-05-25 15:57:02.000000 iceberg_tools-0.0.2rc2/iceberg_tools/util.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.174693 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2862 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2140 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       84 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      146 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-26 00:30:26.309360 iceberg_tools-0.0.2rc2/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5751 2023-05-26 00:29:56.000000 iceberg_tools-0.0.2rc2/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.157916 iceberg_tools-0.0.2rc2/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.196574 iceberg_tools-0.0.2rc2/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:03.000000 iceberg_tools-0.0.2rc2/tests/integration/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.282095 iceberg_tools-0.0.2rc2/tests/integration/bmeg/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1834 2023-05-15 20:39:46.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      967 2023-05-15 20:24:40.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      782 2023-05-15 20:39:22.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_load_granular_reference.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2736 2023-05-15 20:39:04.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1449 2023-05-15 20:38:41.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_invalid_edges.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      255 2023-05-15 20:24:59.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_lathe_lint.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      662 2023-05-15 20:38:23.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_negative_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      829 2023-05-23 20:22:18.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      330 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_schema_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1140 2023-05-15 20:38:10.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_spot_check_embedded_type.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      731 2023-05-15 20:37:50.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_edge_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      888 2023-05-15 20:37:28.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      340 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_yaml_anonymous_schemas.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.288288 iceberg_tools-0.0.2rc2/tests/integration/data/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-23 23:15:41.000000 iceberg_tools-0.0.2rc2/tests/integration/data/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4897 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/integration/data/test_pfb.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.306702 iceberg_tools-0.0.2rc2/tests/integration/gen3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 18:03:42.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      616 2023-05-18 20:08:55.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      911 2023-05-15 20:20:57.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_codeable_concept.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      451 2023-05-15 20:17:07.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_embedded_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-14 12:07:10.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_identifiers.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      171 2023-05-12 18:57:49.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_individual_yaml.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-05-12 18:56:56.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_keys.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      979 2023-05-23 19:23:34.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_primitive.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      469 2023-05-15 20:06:10.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_quantities.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      517 2023-05-18 20:10:27.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_research_study_has_project.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      155 2023-05-24 00:59:54.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1832 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_medication.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1744 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_task.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142       34 2023-05-18 20:08:09.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_task.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.308466 iceberg_tools-0.0.2rc2/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:24.000000 iceberg_tools-0.0.2rc2/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      176 2023-05-15 20:40:27.000000 iceberg_tools-0.0.2rc2/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 iceberg_tools-0.0.2rc2/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3144 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/unit/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1080 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/unit/test_simplify.py
```

### Comparing `iceberg_tools-0.0.2rc1/PKG-INFO` & `iceberg_tools-0.0.2rc2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 Metadata-Version: 2.1
 Name: iceberg_tools
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
-Author: Ellrott Lab
+Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
-Keywords: gen3 bioinformatics graph
+Keywords: FHIR PFB gen3 bioinformatics graph
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
 # iceberg-schema-tools
-Create and maintain central iceberg schema.
+Create and maintain central iceberg schema.  Render and validate FHIR data.
 
 ## Overview
 
-![image](https://user-images.githubusercontent.com/47808/233504556-498adff7-428d-4fa3-b534-937802cb6af4.png)
+![image](docs/figure-5.png)
 
 
 Code that generates the base schema from FHIR goes here.  Additional tools are provided to lints, validates and visualize the schema.
 
 Note: The actual schemas are stored in [iceberg](https://github.com/bmeg/iceberg)
 
 
 ## Setup
 
 ```
-python3 -m venv venv
-source venv/bin/activate
-pip install -r requirements.txt
-pip install -e .
+pip install iceberg-tools
 ```
 
 
 ## Use
 
 ```
 $ iceberg schema
@@ -70,44 +67,43 @@
   validate       Check FHIR data for validity and ACED conventions.
   validate-gen3  Check Gen3 data for validity and ACED conventions.
   pfb            Write simplified FHIR files to a PFB.
   migrate        Migrate from FHIR R4B to R5.0.
 
 ```
 
+> Note: `pfb_fhir` and `iceberg` are synonymous in this context.
 
-## Testing
+## Examples
 
-```
-pip install -r requirements-dev.txt
-pytest --cov
----
-86%
-
-```
+The commands:
+```commandline
+pfb_fhir data simplify  tests/fixtures/simplify/study/ tmp/simplified
+pfb_fhir data pfb tmp/simplified/ tmp/study.pfb
+tree tmp
 
-## Contributing
-
-```
-pre-commit install
 ```
 
-## Distribution
-
-- PyPi
+Will generate the following output:
+```commandline
+INFO:'Records with relationships': 59413
+INFO:'Records': 59460
+tmp
+├── simplified
+│   ├── Condition.ndjson
+│   ├── DocumentReference.ndjson
+│   ├── Encounter.ndjson
+│   ├── MedicationAdministration.ndjson
+│   ├── Observation.ndjson
+│   ├── Patient.ndjson
+│   ├── ResearchStudy.ndjson
+│   ├── ResearchSubject.ndjson
+│   ├── Specimen.ndjson
+│   └── Task.ndjson
+└── study.pfb
 
 ```
-# update pypi
-
-# pypi credentials - see https://twine.readthedocs.io/en/stable/#environment-variables
-
-export TWINE_USERNAME=  #  the username to use for authentication to the repository.
-export TWINE_PASSWORD=  # the password to use for authentication to the repository.
 
-# this could be maintained as so: export $(cat .env | xargs)
-
-rm -r dist/
-python3  setup.py sdist bdist_wheel
-twine upload dist/*
-```
+## Contributing
+See [CONTRIBUTING.md](docs/CONTRIBUTING.md) for developer notes.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/cli/data.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/cli/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,17 @@
     [_ for _ in pfb_writer.transform_directory(path)]
 
     inspection = pfb_writer.inspect()
     if len(inspection.errors) > 0:
         logger.error(inspection.warnings)
     if len(inspection.warnings) > 0:
         logger.warning(inspection.warnings)
+    if len(inspection.info) > 0:
+        for _ in inspection.info:
+            logger.info(_)
 
 
 @cli.command('migrate')
 @click.argument('path')
 @click.argument('output_path')
 @click.option('--validate', default=True, is_flag=True, show_default=True,
               help="Validate after migration")
```

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/cli/schema.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/cli/schema.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/data/migrator/__init__.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/data/migrator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 def _is_resource(resource):
     """Return True if resource is a FHIR resource."""
     return 'resourceType' in resource
 
 
 def migrate_bundles(output_path, path, validate):
     """Migrate bundles."""
-    for input_file in path.glob('*.json'):   # TODO: see util directory_reader
+    for input_file in path.glob('**/*.json'):   # TODO: see util directory_reader
         with open(input_file, "rb") as fp:
             resource = orjson.loads(fp.read())
             if not _is_resource(resource):
                 logger.warning(f"Not a FHIR resource {input_file}")
                 continue
             if not _is_bundle(resource):
                 continue
@@ -260,15 +260,15 @@
         with open(output_file, "wb") as fp:
             fp.write(orjson.dumps(bundle_))
         logger.info(f'Migrated {input_file} to {output_file}')
 
 
 def migrate_resources(output_path, path, validate):
     """Migrate single resource per file."""
-    for input_file in path.glob('*.json'):  # TODO: see util directory_reader
+    for input_file in path.glob('**/*.json'):  # TODO: see util directory_reader
         with open(input_file, "rb") as fp:
             resource = orjson.loads(fp.read())
             if not _is_resource(resource):
                 logger.warning(f"Not a FHIR resource {input_file}")
                 continue
             if _is_bundle(resource):
                 continue
@@ -288,15 +288,15 @@
         if parse_result.exception is not None:
             if 'resourceType' not in str(parse_result.exception):
                 logger.warning(f"{input_file} has exception {parse_result.exception}")
 
 
 def migrate_ndjson(output_path, path, validate):
     """Migrate ndjson files, not expecting bundles."""
-    for input_file in path.glob('*.ndjson'):  # TODO: see util directory_reader
+    for input_file in path.glob('**/*.ndjson'):  # TODO: see util directory_reader
         with open(input_file, "r") as fp:
             output_file = output_path / input_file.name
             with open(output_file, "wb") as out_fp:
                 for line in fp.readlines():
                     resource = orjson.loads(line)
                     _ = migrate_resource(resource)
                     logging_validator(_, input_file, validate)
```

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/data/pfb.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/data/pfb.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/data/simplifier/__init__.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,15 @@
         with open(schema_path, "rb") as fp_:
             schemas = orjson.loads(fp_.read())
     else:
         schemas = requests.get(schema_path).json()
     assert schemas, f"No schema found at {schema_path}"
 
     with SimplifierContextManager():
-        with EmitterContextManager(output_path, verbose=True) as emitter:
+        with EmitterContextManager(output_path) as emitter:
             for parse_result in directory_reader(directory_path=input_path, pattern=pattern,
                                                  validate=False):
                 if parse_result.exception is not None:
                     if 'resourceType' not in str(parse_result.exception):
                         logger.error(f"{parse_result.path} has exception {parse_result.exception}")
                     continue
                 resource = parse_result.resource
@@ -628,25 +628,25 @@
         logger.warning(f"{parse_result.path} {reference} {parse_result.offset}")
         logger.warning(f"\t{simplified}")
         logger.warning({k: validate_simplified_value(v) for k, v in simplified.items()})
     assert all_ok
 
 
 @click.command('simplify')
-@click.argument('input_path')
+@click.argument('path')
 @click.argument('output_path')
 @click.option('--pattern', required=True, default="**/*.*", show_default=True,
               help='File name pattern')
 @click.option('--schema_path', required=True,
               default='https://aced-public.s3.us-west-2.amazonaws.com/aced.json',
               show_default=True,
               help='Path to gen3 schema json.  (Accepts file path for schema development)'
               )
 @click.option('--dialect',
-              default='FHIR',
+              default='GEN3',
               type=click.Choice(['FHIR', 'GEN3'], case_sensitive=False),
               help='GEN3: adds common properties, FHIR: passthrough'
               )
 def cli(path, pattern, output_path, schema_path, dialect):
     """Renders Gen3 friendly flattened records.
 
     PATH: Path containing bundles (*.json) or resources (*.ndjson)
```

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/data/simplifier/oid_lookup.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/oid_lookup.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/schema/__init__.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/schema/bmeg.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/schema/bmeg.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/schema/gen3.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/schema/gen3_validator.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3_validator.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools/util.py` & `iceberg_tools-0.0.2rc2/iceberg_tools/util.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/PKG-INFO` & `iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 Metadata-Version: 2.1
 Name: iceberg-tools
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
-Author: Ellrott Lab
+Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
-Keywords: gen3 bioinformatics graph
+Keywords: FHIR PFB gen3 bioinformatics graph
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
 # iceberg-schema-tools
-Create and maintain central iceberg schema.
+Create and maintain central iceberg schema.  Render and validate FHIR data.
 
 ## Overview
 
-![image](https://user-images.githubusercontent.com/47808/233504556-498adff7-428d-4fa3-b534-937802cb6af4.png)
+![image](docs/figure-5.png)
 
 
 Code that generates the base schema from FHIR goes here.  Additional tools are provided to lints, validates and visualize the schema.
 
 Note: The actual schemas are stored in [iceberg](https://github.com/bmeg/iceberg)
 
 
 ## Setup
 
 ```
-python3 -m venv venv
-source venv/bin/activate
-pip install -r requirements.txt
-pip install -e .
+pip install iceberg-tools
 ```
 
 
 ## Use
 
 ```
 $ iceberg schema
@@ -70,44 +67,43 @@
   validate       Check FHIR data for validity and ACED conventions.
   validate-gen3  Check Gen3 data for validity and ACED conventions.
   pfb            Write simplified FHIR files to a PFB.
   migrate        Migrate from FHIR R4B to R5.0.
 
 ```
 
+> Note: `pfb_fhir` and `iceberg` are synonymous in this context.
 
-## Testing
+## Examples
 
-```
-pip install -r requirements-dev.txt
-pytest --cov
----
-86%
-
-```
+The commands:
+```commandline
+pfb_fhir data simplify  tests/fixtures/simplify/study/ tmp/simplified
+pfb_fhir data pfb tmp/simplified/ tmp/study.pfb
+tree tmp
 
-## Contributing
-
-```
-pre-commit install
 ```
 
-## Distribution
-
-- PyPi
+Will generate the following output:
+```commandline
+INFO:'Records with relationships': 59413
+INFO:'Records': 59460
+tmp
+├── simplified
+│   ├── Condition.ndjson
+│   ├── DocumentReference.ndjson
+│   ├── Encounter.ndjson
+│   ├── MedicationAdministration.ndjson
+│   ├── Observation.ndjson
+│   ├── Patient.ndjson
+│   ├── ResearchStudy.ndjson
+│   ├── ResearchSubject.ndjson
+│   ├── Specimen.ndjson
+│   └── Task.ndjson
+└── study.pfb
 
 ```
-# update pypi
-
-# pypi credentials - see https://twine.readthedocs.io/en/stable/#environment-variables
-
-export TWINE_USERNAME=  #  the username to use for authentication to the repository.
-export TWINE_PASSWORD=  # the password to use for authentication to the repository.
 
-# this could be maintained as so: export $(cat .env | xargs)
-
-rm -r dist/
-python3  setup.py sdist bdist_wheel
-twine upload dist/*
-```
+## Contributing
+See [CONTRIBUTING.md](docs/CONTRIBUTING.md) for developer notes.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iceberg_tools-0.0.2rc1/iceberg_tools.egg-info/SOURCES.txt` & `iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/setup.py` & `iceberg_tools-0.0.2rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='iceberg_tools',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2rc1',  # Required
+    version='0.0.2rc2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='FHIR schemas tools for bioinformatics.',
     # Optional
 
@@ -59,15 +59,15 @@
     long_description_content_type='text/markdown',  # Optional (see note above)
 
     # Project's main homepage.
     url='https://github.com/bmeg/iceberg-schema-tools',  # Optional
 
     # This should be your name or the name of the organization which owns the
     # project.
-    author='Ellrott Lab',  # Optional
+    author='https://ellrottlab.org/',  # Optional
 
 
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
@@ -83,27 +83,27 @@
         'Programming Language :: Python :: 3.9',
     ],
 
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
-    keywords='gen3 bioinformatics graph',  # Optional
+    keywords='FHIR PFB gen3 bioinformatics graph',  # Optional
 
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
 
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),  # Required
 
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. If you
     # do not support Python 2, you can simplify this to '>=3.5' or similar, see
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires='>=3.6, <4',
+    python_requires='>=3.9, <4',
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
@@ -119,15 +119,16 @@
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
 
     entry_points={
         'console_scripts': [
-            'iceberg = iceberg_tools.cli:cli'
+            'iceberg = iceberg_tools.cli:cli',
+            'pfb_fhir = iceberg_tools.cli:cli'
         ],
     },
 
     include_package_data=True,
 
     # List additional URLs that are relevant to your project as a dict.
     #
```

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/__init__.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/conftest.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/conftest.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_edge_load_granular_reference.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_load_granular_reference.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_edge_validator.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_validator.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_invalid_edges.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_invalid_edges.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_negative_trivial_vertex_load.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_negative_trivial_vertex_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_schema.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_schema.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_spot_check_embedded_type.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_spot_check_embedded_type.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_trivial_edge_load.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_edge_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/bmeg/test_trivial_vertex_load.py` & `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_vertex_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/data/test_pfb.py` & `iceberg_tools-0.0.2rc2/tests/integration/data/test_pfb.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/gen3/conftest.py` & `iceberg_tools-0.0.2rc2/tests/integration/gen3/conftest.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/gen3/test_codeable_concept.py` & `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_codeable_concept.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/gen3/test_primitive.py` & `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_primitive.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/gen3/test_research_study_has_project.py` & `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_research_study_has_project.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/gen3/test_simplify_medication.py` & `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_medication.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/integration/gen3/test_simplify_task.py` & `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_task.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/unit/test_coding_conventions.py` & `iceberg_tools-0.0.2rc2/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/unit/test_schema.py` & `iceberg_tools-0.0.2rc2/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc1/tests/unit/test_simplify.py` & `iceberg_tools-0.0.2rc2/tests/unit/test_simplify.py`

 * *Files identical despite different names*


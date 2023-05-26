# Comparing `tmp/loqusdb-2.6.9.tar.gz` & `tmp/loqusdb-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loqusdb-2.6.9.tar", last modified: Wed May 25 15:06:07 2022, max compression
+gzip compressed data, was "loqusdb-2.7.0.tar", last modified: Fri May 26 08:02:35 2023, max compression
```

## Comparing `loqusdb-2.6.9.tar` & `loqusdb-2.7.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.870260 loqusdb-2.6.9/
--rw-r--r--   0 runner    (1001) docker     (116)     1537 2022-05-25 15:05:57.000000 loqusdb-2.6.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)      191 2022-05-25 15:05:57.000000 loqusdb-2.6.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)     1054 2022-05-25 15:05:57.000000 loqusdb-2.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      208 2022-05-25 15:05:57.000000 loqusdb-2.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5624 2022-05-25 15:06:07.870260 loqusdb-2.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4795 2022-05-25 15:05:57.000000 loqusdb-2.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.850261 loqusdb-2.6.9/loqusdb/
--rw-r--r--   0 runner    (1001) docker     (116)     1658 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      397 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.854261 loqusdb-2.6.9/loqusdb/build_models/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/build_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4255 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/build_models/case.py
--rw-r--r--   0 runner    (1001) docker     (116)     1021 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/build_models/profile_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)     6552 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/build_models/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.854261 loqusdb-2.6.9/loqusdb/commands/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1384 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/annotate.py
--rw-r--r--   0 runner    (1001) docker     (116)     3176 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1979 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     3254 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/export.py
--rw-r--r--   0 runner    (1001) docker     (116)      779 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/identity.py
--rw-r--r--   0 runner    (1001) docker     (116)     4226 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/load.py
--rw-r--r--   0 runner    (1001) docker     (116)     3336 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/load_profile.py
--rw-r--r--   0 runner    (1001) docker     (116)      667 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1492 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/restore.py
--rw-r--r--   0 runner    (1001) docker     (116)     3206 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (116)     5111 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/view.py
--rw-r--r--   0 runner    (1001) docker     (116)      553 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/commands/wipe.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.854261 loqusdb-2.6.9/loqusdb/constants/
--rw-r--r--   0 runner    (1001) docker     (116)     1645 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.858260 loqusdb-2.6.9/loqusdb/exceptions/
--rw-r--r--   0 runner    (1001) docker     (116)       88 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       92 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/exceptions/case.py
--rw-r--r--   0 runner    (1001) docker     (116)       98 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/exceptions/profile.py
--rw-r--r--   0 runner    (1001) docker     (116)       95 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/exceptions/vcf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1691 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/log.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.858260 loqusdb-2.6.9/loqusdb/models/
--rw-r--r--   0 runner    (1001) docker     (116)      139 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1660 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/models/case.py
--rw-r--r--   0 runner    (1001) docker     (116)      511 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (116)      409 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/models/profile_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)     1068 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/models/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.858260 loqusdb-2.6.9/loqusdb/plugins/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.858260 loqusdb-2.6.9/loqusdb/plugins/mongo/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/plugins/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2593 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/plugins/mongo/adapter.py
--rw-r--r--   0 runner    (1001) docker     (116)     3119 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/plugins/mongo/case.py
--rw-r--r--   0 runner    (1001) docker     (116)      600 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/plugins/mongo/profile_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)    12955 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/plugins/mongo/structural_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)     8715 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/plugins/mongo/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.862260 loqusdb-2.6.9/loqusdb/resources/
--rw-r--r--   0 runner    (1001) docker     (116)      639 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.862260 loqusdb-2.6.9/loqusdb/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2646 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/annotate.py
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/case.py
--rw-r--r--   0 runner    (1001) docker     (116)     4843 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     8065 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (116)     1113 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/migrate.py
--rw-r--r--   0 runner    (1001) docker     (116)     9164 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (116)     4426 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/update.py
--rw-r--r--   0 runner    (1001) docker     (116)     2088 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/variant.py
--rw-r--r--   0 runner    (1001) docker     (116)     5175 2022-05-25 15:05:57.000000 loqusdb-2.6.9/loqusdb/utils/vcf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.850261 loqusdb-2.6.9/loqusdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5624 2022-05-25 15:06:07.000000 loqusdb-2.6.9/loqusdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2832 2022-05-25 15:06:07.000000 loqusdb-2.6.9/loqusdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-25 15:06:07.000000 loqusdb-2.6.9/loqusdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       59 2022-05-25 15:06:07.000000 loqusdb-2.6.9/loqusdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      201 2022-05-25 15:06:07.000000 loqusdb-2.6.9/loqusdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-05-25 15:06:07.000000 loqusdb-2.6.9/loqusdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-05-25 15:06:07.870260 loqusdb-2.6.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     2789 2022-05-25 15:05:57.000000 loqusdb-2.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.862260 loqusdb-2.6.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.862260 loqusdb-2.6.9/tests/build_models/
--rw-r--r--   0 runner    (1001) docker     (116)     4404 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/build_models/test_build_case.py
--rw-r--r--   0 runner    (1001) docker     (116)      537 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/build_models/test_build_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)     1360 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/build_models/test_is_greater.py
--rw-r--r--   0 runner    (1001) docker     (116)    10488 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.866260 loqusdb-2.6.9/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (116)    59626 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/643594.clinical.SV.vcf
--rw-r--r--   0 runner    (1001) docker     (116)   413153 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/643594.clinical.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/double_variant.vcf
--rwxr-xr-x   0 runner    (1001) docker     (116)      130 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/funny_trio.ped
--rw-r--r--   0 runner    (1001) docker     (116)     5421 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/profile_snv.vcf
--rwxr-xr-x   0 runner    (1001) docker     (116)      148 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/recessive_trio.ped
--rw-r--r--   0 runner    (1001) docker     (116)    59618 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/test.SV.vcf
--rw-r--r--   0 runner    (1001) docker     (116)     2393 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/test.vcf
--rw-r--r--   0 runner    (1001) docker     (116)      652 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/test.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (116)      267 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/test.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/fixtures/unsorted.vcf
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.866260 loqusdb-2.6.9/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (116)     8095 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/functional/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.846261 loqusdb-2.6.9/tests/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.870260 loqusdb-2.6.9/tests/plugins/mongo/
--rw-r--r--   0 runner    (1001) docker     (116)     4271 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/plugins/mongo/test_case_operations.py
--rw-r--r--   0 runner    (1001) docker     (116)      199 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/plugins/mongo/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (116)      738 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/plugins/mongo/test_flask_extension.py
--rw-r--r--   0 runner    (1001) docker     (116)     1029 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/plugins/mongo/test_get_sv.py
--rw-r--r--   0 runner    (1001) docker     (116)     2670 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/plugins/mongo/test_load_svs.py
--rw-r--r--   0 runner    (1001) docker     (116)     9687 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/plugins/mongo/test_variant_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.870260 loqusdb-2.6.9/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (116)     1317 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_case.py
--rw-r--r--   0 runner    (1001) docker     (116)     1872 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (116)      845 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_delete_family.py
--rw-r--r--   0 runner    (1001) docker     (116)     2171 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_delete_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)      329 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_get_family.py
--rw-r--r--   0 runner    (1001) docker     (116)     1473 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_load_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     2376 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_load_family.py
--rw-r--r--   0 runner    (1001) docker     (116)     6278 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_load_variants.py
--rw-r--r--   0 runner    (1001) docker     (116)     1177 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (116)     2658 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/utils/test_profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-25 15:06:07.870260 loqusdb-2.6.9/tests/vcf_tools/
--rw-r--r--   0 runner    (1001) docker     (116)     1155 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/vcf_tools/test_check_par.py
--rw-r--r--   0 runner    (1001) docker     (116)     1966 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/vcf_tools/test_check_vcf.py
--rw-r--r--   0 runner    (1001) docker     (116)     4375 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/vcf_tools/test_format_sv_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)     3647 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/vcf_tools/test_format_variant.py
--rw-r--r--   0 runner    (1001) docker     (116)     1563 2022-05-25 15:05:57.000000 loqusdb-2.6.9/tests/vcf_tools/test_vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-26 08:02:26.000000 loqusdb-2.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 08:02:26.000000 loqusdb-2.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-26 08:02:26.000000 loqusdb-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 08:02:26.000000 loqusdb-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-26 08:02:35.085550 loqusdb-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-26 08:02:26.000000 loqusdb-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.077550 loqusdb-2.7.0/loqusdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      397 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/build_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/profile_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/load_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/wipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/profile_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/plugins/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/profile_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/structural_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.077550 loqusdb-2.7.0/loqusdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:02:35.085550 loqusdb-2.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-05-26 08:02:26.000000 loqusdb-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/tests/build_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/build_models/test_build_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/build_models/test_build_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/build_models/test_is_greater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    59626 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/643594.clinical.SV.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)   413153 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/643594.clinical.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/double_variant.vcf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/funny_trio.ped
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/profile_snv.vcf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/recessive_trio.ped
+-rw-r--r--   0 runner    (1001) docker     (123)    59618 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.SV.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/unsorted.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/functional/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.077550 loqusdb-2.7.0/tests/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/plugins/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_case_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_flask_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_get_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_load_svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_variant_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_delete_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_delete_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_get_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_load_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_load_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_load_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/vcf_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_check_par.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_check_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_format_sv_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_format_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_vcf.py
```

### Comparing `loqusdb-2.6.9/CHANGELOG.md` & `loqusdb-2.7.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/LICENSE` & `loqusdb-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/PKG-INFO` & `loqusdb-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loqusdb
-Version: 2.6.9
+Version: 2.7.0
 Summary: Store observations of vcf variants in a mongodb
 Home-page: https://github.com/moonso/loqusdb
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.com
 License: MIT
 Keywords: vcf,variants
 Platform: UNKNOWN
```

### Comparing `loqusdb-2.6.9/README.md` & `loqusdb-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/__init__.py` & `loqusdb-2.7.0/loqusdb/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/build_models/case.py` & `loqusdb-2.7.0/loqusdb/build_models/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/build_models/profile_variant.py` & `loqusdb-2.7.0/loqusdb/build_models/profile_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/build_models/variant.py` & `loqusdb-2.7.0/loqusdb/build_models/variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,27 +135,27 @@
     coordinates["end"] = end
     coordinates["sv_length"] = sv_len
     coordinates["sv_type"] = sv_type
 
     return coordinates
 
 
-def build_variant(variant, case_obj, case_id=None, gq_treshold=None, genome_build=None):
+def build_variant(variant, case_obj, case_id=None, gq_threshold=None, gq_qual=False, genome_build=None):
     """Return a Variant object
 
     Take a cyvcf2 formated variant line and return a models.Variant.
 
     If criterias are not fullfilled, eg. variant have no gt call or quality
-    is below gq treshold then return None.
+    is below gq threshold then return None.
 
     Args:
         variant(cyvcf2.Variant)
         case_obj(Case): We need the case object to check individuals sex
         case_id(str): The case id
-        gq_treshold(int): Genotype Quality treshold
+        gq_threshold(int): Genotype Quality threshold
 
     Return:
         formated_variant(models.Variant): A variant dictionary
     """
     variant_obj = None
 
     sv = False
@@ -184,16 +184,22 @@
         found_variant = True
     else:
         found_variant = False
         for ind_obj in case_obj["individuals"]:
             ind_id = ind_obj["ind_id"]
             # Get the index position for the individual in the VCF
             ind_pos = ind_obj["ind_index"]
-            gq = int(variant.gt_quals[ind_pos])
-            if gq_treshold and gq < gq_treshold:
+
+            if gq_qual:
+                gq = int(variant.QUAL)
+
+            if not gq_qual:
+                gq = int(variant.gt_quals[ind_pos])
+
+            if gq_threshold and gq < gq_threshold:
                 continue
 
             genotype = GENOTYPE_MAP[variant.gt_types[ind_pos]]
 
             if genotype in ["het", "hom_alt"]:
                 LOG.debug("Found variant")
                 found_variant = True
```

### Comparing `loqusdb-2.6.9/loqusdb/commands/__init__.py` & `loqusdb-2.7.0/loqusdb/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/annotate.py` & `loqusdb-2.7.0/loqusdb/commands/annotate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/cli.py` & `loqusdb-2.7.0/loqusdb/commands/cli.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/delete.py` & `loqusdb-2.7.0/loqusdb/commands/delete.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/export.py` & `loqusdb-2.7.0/loqusdb/commands/export.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/identity.py` & `loqusdb-2.7.0/loqusdb/commands/identity.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/load.py` & `loqusdb-2.7.0/loqusdb/commands/load.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     "-s",
     "--skip-case-id",
     is_flag=True,
     show_default=True,
     help="Do not store case information on variants",
 )
 @click.option("--ensure-index", is_flag=True, help="Make sure that the indexes are in place")
-@click.option("--gq-treshold", default=20, show_default=True, help="Treshold to consider variant")
+@click.option("--gq-threshold", default=20, show_default=True, help="Threshold to consider variant")
+@click.option("--qual-gq", is_flag=True, default=False, show_default=True, help="Use QUAL tag instead of GQ value for quality filter")
 @click.option(
     "--max-window",
     "-m",
     default=2000,
     show_default=True,
     help="Specify the maximum window size for svs",
 )
@@ -85,21 +86,22 @@
 def load(
     ctx,
     variant_file,
     sv_variants,
     family_file,
     family_type,
     skip_case_id,
-    gq_treshold,
+    gq_threshold,
     case_id,
     ensure_index,
     max_window,
     check_profile,
     hard_threshold,
     soft_threshold,
+    qual_gq
 ):
     """Load the variants of a case
 
     A variant is loaded if it is observed in any individual of a case
     If no family file is provided all individuals in vcf file will be considered.
     """
     if not (family_file or case_id):
@@ -132,15 +134,16 @@
             adapter=adapter,
             variant_file=variant_path,
             sv_file=variant_sv_path,
             family_file=family_file,
             family_type=family_type,
             skip_case_id=skip_case_id,
             case_id=case_id,
-            gq_treshold=gq_treshold,
+            gq_threshold=gq_threshold,
+            qual_gq=qual_gq,
             max_window=max_window,
             profile_file=variant_profile_path,
             hard_threshold=hard_threshold,
             soft_threshold=soft_threshold,
             genome_build=genome_build,
         )
     except (SyntaxError, CaseError, IOError) as error:
```

### Comparing `loqusdb-2.6.9/loqusdb/commands/load_profile.py` & `loqusdb-2.7.0/loqusdb/commands/load_profile.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/migrate.py` & `loqusdb-2.7.0/loqusdb/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/restore.py` & `loqusdb-2.7.0/loqusdb/commands/restore.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/update.py` & `loqusdb-2.7.0/loqusdb/commands/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "-s",
     "--skip-case-id",
     is_flag=True,
     show_default=True,
     help="Do not store case information on variants",
 )
 @click.option("--ensure-index", is_flag=True, help="Make sure that the indexes are in place")
-@click.option("--gq-treshold", default=20, show_default=True, help="Treshold to consider variant")
+@click.option("--gq-threshold", default=20, show_default=True, help="Threshold to consider variant")
 @click.option(
     "--max-window",
     "-m",
     default=2000,
     show_default=True,
     help="Specify the maximum window size for svs",
 )
@@ -59,15 +59,15 @@
 def update(
     ctx,
     variant_file,
     sv_variants,
     family_file,
     family_type,
     skip_case_id,
-    gq_treshold,
+    gq_threshold,
     case_id,
     ensure_index,
     max_window,
 ):
     """Load the variants of a case
 
     A variant is loaded if it is observed in any individual of a case
@@ -98,15 +98,15 @@
             adapter=adapter,
             variant_file=variant_path,
             sv_file=variant_sv_path,
             family_file=family_file,
             family_type=family_type,
             skip_case_id=skip_case_id,
             case_id=case_id,
-            gq_treshold=gq_treshold,
+            gq_threshold=gq_threshold,
             max_window=max_window,
         )
     except (SyntaxError, CaseError, IOError, VcfError) as error:
         LOG.warning(error)
         ctx.abort()
 
     LOG.info("Nr variants inserted: %s", nr_inserted)
```

### Comparing `loqusdb-2.6.9/loqusdb/commands/view.py` & `loqusdb-2.7.0/loqusdb/commands/view.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/commands/wipe.py` & `loqusdb-2.7.0/loqusdb/commands/wipe.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/constants/__init__.py` & `loqusdb-2.7.0/loqusdb/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/log.py` & `loqusdb-2.7.0/loqusdb/log.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/models/case.py` & `loqusdb-2.7.0/loqusdb/models/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/models/variant.py` & `loqusdb-2.7.0/loqusdb/models/variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/plugins/mongo/adapter.py` & `loqusdb-2.7.0/loqusdb/plugins/mongo/adapter.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/plugins/mongo/case.py` & `loqusdb-2.7.0/loqusdb/plugins/mongo/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/plugins/mongo/profile_variant.py` & `loqusdb-2.7.0/loqusdb/plugins/mongo/profile_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/plugins/mongo/structural_variant.py` & `loqusdb-2.7.0/loqusdb/plugins/mongo/structural_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/plugins/mongo/variant.py` & `loqusdb-2.7.0/loqusdb/plugins/mongo/variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/resources/__init__.py` & `loqusdb-2.7.0/loqusdb/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/utils/annotate.py` & `loqusdb-2.7.0/loqusdb/utils/annotate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/utils/case.py` & `loqusdb-2.7.0/loqusdb/utils/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/utils/delete.py` & `loqusdb-2.7.0/loqusdb/utils/delete.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/utils/load.py` & `loqusdb-2.7.0/loqusdb/utils/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 def load_database(
     adapter,
     variant_file=None,
     sv_file=None,
     family_file=None,
     family_type="ped",
     skip_case_id=False,
-    gq_treshold=None,
+    gq_threshold=None,
+    qual_gq=False,
     case_id=None,
     max_window=3000,
     profile_file=None,
     hard_threshold=0.95,
     soft_threshold=0.9,
     genome_build=None,
 ):
@@ -44,15 +45,16 @@
     Args:
           adapter: Connection to database
           variant_file(str): Path to variant file
           sv_file(str): Path to sv variant file
           family_file(str): Path to family file
           family_type(str): Format of family file
           skip_case_id(bool): If no case information should be added to variants
-          gq_treshold(int): If only quality variants should be considered
+          gq_threshold(int): If only quality variants should be considered
+          qual_gq(bool): Use QUAL field instead of GQ format tag to gate quality
           case_id(str): If different case id than the one in family file should be used
           max_window(int): Specify the max size for sv windows
           check_profile(bool): Does profile check if True
           hard_threshold(float): Rejects load if hamming distance above this is found
           soft_threshold(float): Stores similar samples if hamming distance above this is found
 
     Returns:
@@ -83,21 +85,21 @@
     if profile_file:
         profiles = get_profiles(adapter, profile_file)
         ###Check if any profile already exists
         matches = profile_match(
             adapter, profiles, hard_threshold=hard_threshold, soft_threshold=soft_threshold
         )
 
-    # If a gq treshold is used the variants needs to have GQ
+    # If a gq threshold is used the variants needs to have GQ
     for _vcf_file in vcf_files:
         # Get a cyvcf2.VCF object
         vcf = get_vcf(_vcf_file)
 
-        if gq_treshold and not vcf.contains("GQ"):
-            LOG.warning("Set gq-treshold to 0 or add info to vcf {0}".format(_vcf_file))
+        if gq_threshold and not vcf.contains("GQ") and not qual_gq:
+            LOG.warning("Set gq-threshold to 0 or add info to vcf {0}".format(_vcf_file))
             raise SyntaxError("GQ is not defined in vcf header")
 
     # Get a ped_parser.Family object from family file
     family = None
     family_id = None
     if family_file:
         LOG.info("Loading family from %s", family_file)
@@ -139,15 +141,16 @@
         vcf_obj = get_vcf(case_obj[file_type])
         try:
             nr_inserted += load_variants(
                 adapter=adapter,
                 vcf_obj=vcf_obj,
                 case_obj=case_obj,
                 skip_case_id=skip_case_id,
-                gq_treshold=gq_treshold,
+                gq_threshold=gq_threshold,
+                qual_gq=qual_gq,
                 max_window=max_window,
                 variant_type=variant_type,
                 genome_build=genome_build,
             )
         except Exception as err:
             # If something went wrong do a rollback
             LOG.warning(err)
@@ -185,28 +188,29 @@
 
 
 def load_variants(
     adapter,
     vcf_obj,
     case_obj,
     skip_case_id=False,
-    gq_treshold=None,
+    gq_threshold=None,
+    qual_gq=False,
     max_window=3000,
     variant_type="snv",
     genome_build=None,
 ):
     """Load variants for a family into the database.
 
     Args:
         adapter (loqusdb.plugins.Adapter): initialized plugin
         case_obj(Case): dict with case information
         nr_variants(int)
         skip_case_id (bool): whether to include the case id on variant level
                              or not
-        gq_treshold(int)
+        gq_threshold(int)
         max_window(int): Specify the max size for sv windows
         variant_type(str): 'sv' or 'snv'
 
     Returns:
         nr_inserted(int)
     """
     if variant_type == "snv":
@@ -218,15 +222,15 @@
     case_id = case_obj["case_id"]
     if skip_case_id:
         case_id = None
     # Loop over the variants in the vcf
     with click.progressbar(vcf_obj, label="Inserting variants", length=nr_variants) as bar:
 
         variants = (
-            build_variant(variant, case_obj, case_id, gq_treshold, genome_build=genome_build)
+            build_variant(variant, case_obj, case_id, gq_threshold, qual_gq, genome_build=genome_build)
             for variant in bar
         )
 
     if variant_type == "sv":
         for sv_variant in variants:
             if not sv_variant:
                 continue
```

### Comparing `loqusdb-2.6.9/loqusdb/utils/migrate.py` & `loqusdb-2.7.0/loqusdb/utils/migrate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/utils/profiling.py` & `loqusdb-2.7.0/loqusdb/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/utils/update.py` & `loqusdb-2.7.0/loqusdb/utils/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 def update_database(
     adapter,
     variant_file=None,
     sv_file=None,
     family_file=None,
     family_type="ped",
     skip_case_id=False,
-    gq_treshold=None,
+    gq_threshold=None,
     case_id=None,
     max_window=3000,
 ):
     """Update a case in the database
 
     Args:
           adapter: Connection to database
           variant_file(str): Path to variant file
           sv_file(str): Path to sv variant file
           family_file(str): Path to family file
           family_type(str): Format of family file
           skip_case_id(bool): If no case information should be added to variants
-          gq_treshold(int): If only quality variants should be considered
+          gq_threshold(int): If only quality variants should be considered
           case_id(str): If different case id than the one in family file should be used
           max_window(int): Specify the max size for sv windows
 
     Returns:
           nr_inserted(int)
     """
     vcf_files = []
@@ -63,22 +63,22 @@
     sv_individuals = None
     if sv_file:
         vcf_info = check_vcf(sv_file, "sv")
         nr_sv_variants = vcf_info["nr_variants"]
         vcf_files.append(sv_file)
         sv_individuals = vcf_info["individuals"]
 
-    # If a gq treshold is used the variants needs to have GQ
+    # If a gq threshold is used the variants needs to have GQ
     for _vcf_file in vcf_files:
         # Get a cyvcf2.VCF object
         vcf = get_vcf(_vcf_file)
 
-        if gq_treshold:
+        if gq_threshold:
             if not vcf.contains("GQ"):
-                LOG.warning("Set gq-treshold to 0 or add info to vcf {0}".format(_vcf_file))
+                LOG.warning("Set gq-threshold to 0 or add info to vcf {0}".format(_vcf_file))
                 raise SyntaxError("GQ is not defined in vcf header")
 
     # Get a ped_parser.Family object from family file
     family = None
     family_id = None
     if family_file:
         with open(family_file, "r") as family_lines:
@@ -123,15 +123,15 @@
         vcf_obj = get_vcf(case_obj[file_type])
         try:
             nr_inserted += load_variants(
                 adapter=adapter,
                 vcf_obj=vcf_obj,
                 case_obj=case_obj,
                 skip_case_id=skip_case_id,
-                gq_treshold=gq_treshold,
+                gq_threshold=gq_threshold,
                 max_window=max_window,
                 variant_type=variant_type,
             )
         except Exception as err:
             # If something went wrong do a rollback
             LOG.warning(err)
             delete(
```

### Comparing `loqusdb-2.6.9/loqusdb/utils/variant.py` & `loqusdb-2.7.0/loqusdb/utils/variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb/utils/vcf.py` & `loqusdb-2.7.0/loqusdb/utils/vcf.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/loqusdb.egg-info/PKG-INFO` & `loqusdb-2.7.0/loqusdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loqusdb
-Version: 2.6.9
+Version: 2.7.0
 Summary: Store observations of vcf variants in a mongodb
 Home-page: https://github.com/moonso/loqusdb
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.com
 License: MIT
 Keywords: vcf,variants
 Platform: UNKNOWN
```

### Comparing `loqusdb-2.6.9/loqusdb.egg-info/SOURCES.txt` & `loqusdb-2.7.0/loqusdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/setup.py` & `loqusdb-2.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,27 @@
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pip install twine
 """Based on https://github.com/kennethreitz/setup.py"""
 
 import io
 import os
 
-from pip._internal.network.session import PipSession
-from pip._internal.req import parse_requirements
 from setuptools import find_packages, setup
 
 # Package meta-data.
 NAME = "loqusdb"
 DESCRIPTION = "Store observations of vcf variants in a mongodb"
 URL = "https://github.com/moonso/loqusdb"
 EMAIL = "mans.magnusson@scilifelab.com"
 AUTHOR = "Måns Magnusson"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "2.6.9"
-
-requirements = [
-    requirement.requirement
-    for requirement in parse_requirements(filename="./requirements.txt", session=PipSession())
-]
+VERSION = "2.7.0"
 
+with open('requirements.txt') as f:
+    install_requires = f.read().strip().split('\n')
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
@@ -64,15 +59,15 @@
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=("tests",)),
     entry_points={
         "console_scripts": ["loqusdb = loqusdb.__main__:base_command"],
     },
-    install_requires=requirements,
+    install_requires=install_requires,
     include_package_data=True,
     license="MIT",
     keywords=["vcf", "variants"],
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: MIT License",
```

### Comparing `loqusdb-2.6.9/tests/build_models/test_build_case.py` & `loqusdb-2.7.0/tests/build_models/test_build_case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/build_models/test_build_variant.py` & `loqusdb-2.7.0/tests/build_models/test_build_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/build_models/test_is_greater.py` & `loqusdb-2.7.0/tests/build_models/test_is_greater.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/conftest.py` & `loqusdb-2.7.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 @pytest.fixture(scope="function")
 def variant_obj(request, het_variant, ind_positions, individuals):
     return build_variant(
         variant=het_variant,
         individuals=individuals,
         ind_positions=ind_positions,
         case_id="test",
-        gq_treshold=None,
+        gq_threshold=None,
     )
 
 
 ### CYVCF2 variants
 ### SNVs:
 @pytest.fixture(scope="function")
 def hem_variant(request):
```

### Comparing `loqusdb-2.6.9/tests/fixtures/643594.clinical.SV.vcf` & `loqusdb-2.7.0/tests/fixtures/643594.clinical.SV.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/fixtures/643594.clinical.vcf.gz` & `loqusdb-2.7.0/tests/fixtures/643594.clinical.vcf.gz`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/fixtures/double_variant.vcf` & `loqusdb-2.7.0/tests/fixtures/double_variant.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/fixtures/profile_snv.vcf` & `loqusdb-2.7.0/tests/fixtures/profile_snv.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/fixtures/test.SV.vcf` & `loqusdb-2.7.0/tests/fixtures/test.SV.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/fixtures/test.vcf` & `loqusdb-2.7.0/tests/fixtures/test.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/fixtures/test.vcf.gz` & `loqusdb-2.7.0/tests/fixtures/test.vcf.gz`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/fixtures/unsorted.vcf` & `loqusdb-2.7.0/tests/fixtures/unsorted.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/functional/test_cli.py` & `loqusdb-2.7.0/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/plugins/mongo/test_case_operations.py` & `loqusdb-2.7.0/tests/plugins/mongo/test_case_operations.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/plugins/mongo/test_flask_extension.py` & `loqusdb-2.7.0/tests/plugins/mongo/test_flask_extension.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/plugins/mongo/test_get_sv.py` & `loqusdb-2.7.0/tests/plugins/mongo/test_get_sv.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/plugins/mongo/test_load_svs.py` & `loqusdb-2.7.0/tests/plugins/mongo/test_load_svs.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/plugins/mongo/test_variant_operations.py` & `loqusdb-2.7.0/tests/plugins/mongo/test_variant_operations.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_case.py` & `loqusdb-2.7.0/tests/utils/test_case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_delete.py` & `loqusdb-2.7.0/tests/utils/test_delete.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_delete_family.py` & `loqusdb-2.7.0/tests/utils/test_delete_family.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_delete_variant.py` & `loqusdb-2.7.0/tests/utils/test_delete_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_load_database.py` & `loqusdb-2.7.0/tests/utils/test_load_database.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_load_family.py` & `loqusdb-2.7.0/tests/utils/test_load_family.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_load_variants.py` & `loqusdb-2.7.0/tests/utils/test_load_variants.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_migrate.py` & `loqusdb-2.7.0/tests/utils/test_migrate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/utils/test_profiling.py` & `loqusdb-2.7.0/tests/utils/test_profiling.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/vcf_tools/test_check_par.py` & `loqusdb-2.7.0/tests/vcf_tools/test_check_par.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/vcf_tools/test_check_vcf.py` & `loqusdb-2.7.0/tests/vcf_tools/test_check_vcf.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/vcf_tools/test_format_sv_variant.py` & `loqusdb-2.7.0/tests/vcf_tools/test_format_sv_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.6.9/tests/vcf_tools/test_format_variant.py` & `loqusdb-2.7.0/tests/vcf_tools/test_format_variant.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,30 +21,30 @@
     assert formated_variant["homozygote"] == 0
 
 
 def test_format_variant_no_gq(variant_no_gq, case_obj):
     ## GIVEN a variant without GQ
     variant = variant_no_gq
     case_id = case_obj["case_id"]
-    ## WHEN parsing the variant using a GQ treshold
+    ## WHEN parsing the variant using a GQ threshold
     formated_variant = build_variant(
-        variant=variant, case_obj=case_obj, case_id=case_id, gq_treshold=20
+        variant=variant, case_obj=case_obj, case_id=case_id, gq_threshold=20
     )
     ## THEN assert that None is returned since requirements are not fulfilled
     assert formated_variant is None
 
 
 def test_format_variant_chr_prefix(variant_chr, case_obj):
     ## GIVEN a variant with 'chr' prefix in chromosome name
     variant = variant_chr
     assert variant.CHROM.startswith("chr")
     case_id = case_obj["case_id"]
-    ## WHEN parsing the variant using a GQ treshold
+    ## WHEN parsing the variant using a GQ threshold
     formated_variant = build_variant(
-        variant=variant, case_obj=case_obj, case_id=case_id, gq_treshold=20
+        variant=variant, case_obj=case_obj, case_id=case_id, gq_threshold=20
     )
     ## THEN assert that the 'chr' part has been stripped away
     assert formated_variant["chrom"] == variant.CHROM[3:]
 
 
 def test_format_variant_no_family_id(het_variant, case_obj):
     ## GIVEN a parsed variant
```

### Comparing `loqusdb-2.6.9/tests/vcf_tools/test_vcf.py` & `loqusdb-2.7.0/tests/vcf_tools/test_vcf.py`

 * *Files identical despite different names*


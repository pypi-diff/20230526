# Comparing `tmp/loqusdb-2.7.0.tar.gz` & `tmp/loqusdb-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loqusdb-2.7.0.tar", last modified: Fri May 26 08:02:35 2023, max compression
+gzip compressed data, was "loqusdb-2.7.1.tar", last modified: Fri May 26 14:16:55 2023, max compression
```

## Comparing `loqusdb-2.7.0.tar` & `loqusdb-2.7.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-26 08:02:26.000000 loqusdb-2.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 08:02:26.000000 loqusdb-2.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-26 08:02:26.000000 loqusdb-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 08:02:26.000000 loqusdb-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-26 08:02:35.085550 loqusdb-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-26 08:02:26.000000 loqusdb-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.077550 loqusdb-2.7.0/loqusdb/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      397 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/build_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/profile_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/build_models/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/load_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/view.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/commands/wipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/case.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/exceptions/vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/models/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/case.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/profile_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/models/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/plugins/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/case.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/profile_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/structural_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/plugins/mongo/variant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/loqusdb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-26 08:02:26.000000 loqusdb-2.7.0/loqusdb/utils/vcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.077550 loqusdb-2.7.0/loqusdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 08:02:35.000000 loqusdb-2.7.0/loqusdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:02:35.085550 loqusdb-2.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-05-26 08:02:26.000000 loqusdb-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.081550 loqusdb-2.7.0/tests/build_models/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/build_models/test_build_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/build_models/test_build_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/build_models/test_is_greater.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    59626 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/643594.clinical.SV.vcf
--rw-r--r--   0 runner    (1001) docker     (123)   413153 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/643594.clinical.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/double_variant.vcf
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/funny_trio.ped
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/profile_snv.vcf
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/recessive_trio.ped
--rw-r--r--   0 runner    (1001) docker     (123)    59618 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.SV.vcf
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.vcf
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/test.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/fixtures/unsorted.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/functional/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.077550 loqusdb-2.7.0/tests/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/plugins/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_case_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_flask_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_get_sv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_load_svs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/plugins/mongo/test_variant_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_delete_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_delete_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_get_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_load_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_load_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_load_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/utils/test_profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:35.085550 loqusdb-2.7.0/tests/vcf_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_check_par.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_check_vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_format_sv_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_format_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-26 08:02:26.000000 loqusdb-2.7.0/tests/vcf_tools/test_vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.232870 loqusdb-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-26 14:16:45.000000 loqusdb-2.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 14:16:45.000000 loqusdb-2.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-26 14:16:45.000000 loqusdb-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 14:16:45.000000 loqusdb-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-26 14:16:55.232870 loqusdb-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-26 14:16:45.000000 loqusdb-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.224870 loqusdb-2.7.1/loqusdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      397 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.224870 loqusdb-2.7.1/loqusdb/build_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/build_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/build_models/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/build_models/profile_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/build_models/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.224870 loqusdb-2.7.1/loqusdb/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/load_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/commands/wipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.224870 loqusdb-2.7.1/loqusdb/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.224870 loqusdb-2.7.1/loqusdb/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/exceptions/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/exceptions/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/exceptions/vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.224870 loqusdb-2.7.1/loqusdb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/models/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/models/profile_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/models/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/loqusdb/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/loqusdb/plugins/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/plugins/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/plugins/mongo/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/plugins/mongo/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/plugins/mongo/profile_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/plugins/mongo/structural_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/plugins/mongo/variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/loqusdb/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/loqusdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-26 14:16:45.000000 loqusdb-2.7.1/loqusdb/utils/vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.224870 loqusdb-2.7.1/loqusdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-26 14:16:55.000000 loqusdb-2.7.1/loqusdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-26 14:16:55.000000 loqusdb-2.7.1/loqusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:16:55.000000 loqusdb-2.7.1/loqusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 14:16:55.000000 loqusdb-2.7.1/loqusdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-26 14:16:55.000000 loqusdb-2.7.1/loqusdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 14:16:55.000000 loqusdb-2.7.1/loqusdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:16:55.232870 loqusdb-2.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-05-26 14:16:45.000000 loqusdb-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/tests/build_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/build_models/test_build_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/build_models/test_build_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/build_models/test_is_greater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    59626 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/643594.clinical.SV.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)   413153 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/643594.clinical.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/double_variant.vcf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/funny_trio.ped
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/profile_snv.vcf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/recessive_trio.ped
+-rw-r--r--   0 runner    (1001) docker     (123)    59618 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/test.SV.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/test.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/test.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/test.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/fixtures/unsorted.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.228870 loqusdb-2.7.1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/functional/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.220870 loqusdb-2.7.1/tests/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.232870 loqusdb-2.7.1/tests/plugins/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/plugins/mongo/test_case_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/plugins/mongo/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/plugins/mongo/test_flask_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/plugins/mongo/test_get_sv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/plugins/mongo/test_load_svs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/plugins/mongo/test_variant_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.232870 loqusdb-2.7.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_delete_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_delete_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_get_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_load_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_load_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_load_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/utils/test_profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:16:55.232870 loqusdb-2.7.1/tests/vcf_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/vcf_tools/test_check_par.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/vcf_tools/test_check_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/vcf_tools/test_format_sv_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/vcf_tools/test_format_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-26 14:16:45.000000 loqusdb-2.7.1/tests/vcf_tools/test_vcf.py
```

### Comparing `loqusdb-2.7.0/CHANGELOG.md` & `loqusdb-2.7.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/LICENSE` & `loqusdb-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/PKG-INFO` & `loqusdb-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loqusdb
-Version: 2.7.0
+Version: 2.7.1
 Summary: Store observations of vcf variants in a mongodb
 Home-page: https://github.com/moonso/loqusdb
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.com
 License: MIT
 Keywords: vcf,variants
 Platform: UNKNOWN
```

### Comparing `loqusdb-2.7.0/README.md` & `loqusdb-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/__init__.py` & `loqusdb-2.7.1/loqusdb/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/build_models/case.py` & `loqusdb-2.7.1/loqusdb/build_models/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/build_models/profile_variant.py` & `loqusdb-2.7.1/loqusdb/build_models/profile_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/build_models/variant.py` & `loqusdb-2.7.1/loqusdb/build_models/variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/__init__.py` & `loqusdb-2.7.1/loqusdb/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/annotate.py` & `loqusdb-2.7.1/loqusdb/commands/annotate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/cli.py` & `loqusdb-2.7.1/loqusdb/commands/cli.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/delete.py` & `loqusdb-2.7.1/loqusdb/commands/delete.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/export.py` & `loqusdb-2.7.1/loqusdb/commands/export.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/identity.py` & `loqusdb-2.7.1/loqusdb/commands/identity.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/load.py` & `loqusdb-2.7.1/loqusdb/commands/load.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/load_profile.py` & `loqusdb-2.7.1/loqusdb/commands/load_profile.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/migrate.py` & `loqusdb-2.7.1/loqusdb/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/restore.py` & `loqusdb-2.7.1/loqusdb/commands/restore.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/update.py` & `loqusdb-2.7.1/loqusdb/commands/update.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/view.py` & `loqusdb-2.7.1/loqusdb/commands/view.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/commands/wipe.py` & `loqusdb-2.7.1/loqusdb/commands/wipe.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/constants/__init__.py` & `loqusdb-2.7.1/loqusdb/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/log.py` & `loqusdb-2.7.1/loqusdb/log.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/models/case.py` & `loqusdb-2.7.1/loqusdb/models/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/models/variant.py` & `loqusdb-2.7.1/loqusdb/models/variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/plugins/mongo/adapter.py` & `loqusdb-2.7.1/loqusdb/plugins/mongo/adapter.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/plugins/mongo/case.py` & `loqusdb-2.7.1/loqusdb/plugins/mongo/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/plugins/mongo/profile_variant.py` & `loqusdb-2.7.1/loqusdb/plugins/mongo/profile_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/plugins/mongo/structural_variant.py` & `loqusdb-2.7.1/loqusdb/plugins/mongo/structural_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/plugins/mongo/variant.py` & `loqusdb-2.7.1/loqusdb/plugins/mongo/variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/resources/__init__.py` & `loqusdb-2.7.1/loqusdb/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/annotate.py` & `loqusdb-2.7.1/loqusdb/utils/annotate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/case.py` & `loqusdb-2.7.1/loqusdb/utils/case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/delete.py` & `loqusdb-2.7.1/loqusdb/utils/delete.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/load.py` & `loqusdb-2.7.1/loqusdb/utils/load.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/migrate.py` & `loqusdb-2.7.1/loqusdb/utils/migrate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/profiling.py` & `loqusdb-2.7.1/loqusdb/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/update.py` & `loqusdb-2.7.1/loqusdb/utils/update.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/variant.py` & `loqusdb-2.7.1/loqusdb/utils/variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb/utils/vcf.py` & `loqusdb-2.7.1/loqusdb/utils/vcf.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/loqusdb.egg-info/PKG-INFO` & `loqusdb-2.7.1/loqusdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loqusdb
-Version: 2.7.0
+Version: 2.7.1
 Summary: Store observations of vcf variants in a mongodb
 Home-page: https://github.com/moonso/loqusdb
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.com
 License: MIT
 Keywords: vcf,variants
 Platform: UNKNOWN
```

### Comparing `loqusdb-2.7.0/loqusdb.egg-info/SOURCES.txt` & `loqusdb-2.7.1/loqusdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/setup.py` & `loqusdb-2.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Package meta-data.
 NAME = "loqusdb"
 DESCRIPTION = "Store observations of vcf variants in a mongodb"
 URL = "https://github.com/moonso/loqusdb"
 EMAIL = "mans.magnusson@scilifelab.com"
 AUTHOR = "Måns Magnusson"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "2.7.0"
+VERSION = "2.7.1"
 
 with open('requirements.txt') as f:
     install_requires = f.read().strip().split('\n')
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
```

### Comparing `loqusdb-2.7.0/tests/build_models/test_build_case.py` & `loqusdb-2.7.1/tests/build_models/test_build_case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/build_models/test_build_variant.py` & `loqusdb-2.7.1/tests/build_models/test_build_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/build_models/test_is_greater.py` & `loqusdb-2.7.1/tests/build_models/test_is_greater.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/conftest.py` & `loqusdb-2.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/643594.clinical.SV.vcf` & `loqusdb-2.7.1/tests/fixtures/643594.clinical.SV.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/643594.clinical.vcf.gz` & `loqusdb-2.7.1/tests/fixtures/643594.clinical.vcf.gz`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/double_variant.vcf` & `loqusdb-2.7.1/tests/fixtures/double_variant.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/profile_snv.vcf` & `loqusdb-2.7.1/tests/fixtures/profile_snv.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/test.SV.vcf` & `loqusdb-2.7.1/tests/fixtures/test.SV.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/test.vcf` & `loqusdb-2.7.1/tests/fixtures/test.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/test.vcf.gz` & `loqusdb-2.7.1/tests/fixtures/test.vcf.gz`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/fixtures/unsorted.vcf` & `loqusdb-2.7.1/tests/fixtures/unsorted.vcf`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/functional/test_cli.py` & `loqusdb-2.7.1/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/plugins/mongo/test_case_operations.py` & `loqusdb-2.7.1/tests/plugins/mongo/test_case_operations.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/plugins/mongo/test_flask_extension.py` & `loqusdb-2.7.1/tests/plugins/mongo/test_flask_extension.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/plugins/mongo/test_get_sv.py` & `loqusdb-2.7.1/tests/plugins/mongo/test_get_sv.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/plugins/mongo/test_load_svs.py` & `loqusdb-2.7.1/tests/plugins/mongo/test_load_svs.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/plugins/mongo/test_variant_operations.py` & `loqusdb-2.7.1/tests/plugins/mongo/test_variant_operations.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_case.py` & `loqusdb-2.7.1/tests/utils/test_case.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_delete.py` & `loqusdb-2.7.1/tests/utils/test_delete.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_delete_family.py` & `loqusdb-2.7.1/tests/utils/test_delete_family.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_delete_variant.py` & `loqusdb-2.7.1/tests/utils/test_delete_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_load_database.py` & `loqusdb-2.7.1/tests/utils/test_load_database.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_load_family.py` & `loqusdb-2.7.1/tests/utils/test_load_family.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_load_variants.py` & `loqusdb-2.7.1/tests/utils/test_load_variants.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_migrate.py` & `loqusdb-2.7.1/tests/utils/test_migrate.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/utils/test_profiling.py` & `loqusdb-2.7.1/tests/utils/test_profiling.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/vcf_tools/test_check_par.py` & `loqusdb-2.7.1/tests/vcf_tools/test_check_par.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/vcf_tools/test_check_vcf.py` & `loqusdb-2.7.1/tests/vcf_tools/test_check_vcf.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/vcf_tools/test_format_sv_variant.py` & `loqusdb-2.7.1/tests/vcf_tools/test_format_sv_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/vcf_tools/test_format_variant.py` & `loqusdb-2.7.1/tests/vcf_tools/test_format_variant.py`

 * *Files identical despite different names*

### Comparing `loqusdb-2.7.0/tests/vcf_tools/test_vcf.py` & `loqusdb-2.7.1/tests/vcf_tools/test_vcf.py`

 * *Files identical despite different names*


# Comparing `tmp/impala_shell-4.3.0a2.tar.gz` & `tmp/impala_shell-4.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wenzhe/projects/impala/shell/dist/impala_shell-4.3.0a2.tar", last modified: Thu Apr 13 20:54:10 2023, max compression
+gzip compressed data, was "/home/wenzhe/projects/impala/shell/dist/impala_shell-4.3.0a3.tar", last modified: Thu May 25 22:17:36 2023, max compression
```

## Comparing `impala_shell-4.3.0a2.tar` & `impala_shell-4.3.0a3.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/PKG-INFO
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    59759 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/LICENSE.txt
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Exprs/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Exprs/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    59637 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Exprs/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Exprs/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2157 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/shell_exceptions.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Metrics/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Metrics/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1755 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Metrics/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Metrics/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/ResourceProfile/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ResourceProfile/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4395 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ResourceProfile/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ResourceProfile/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/fb303/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/fb303/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      961 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/fb303/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       53 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/fb303/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69618 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/fb303/FacebookService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1765 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/value_converter.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Status/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Status/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3396 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Status/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Status/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/SqlConstraints/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/SqlConstraints/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4200 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/SqlConstraints/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/SqlConstraints/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Partitions/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Partitions/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3917 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Partitions/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Partitions/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Descriptors/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Descriptors/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    32802 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Descriptors/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Descriptors/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/ImpalaInternalService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      396 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaInternalService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    38764 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaInternalService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaInternalService/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1433 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/compatibility.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2393 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/impala_shell_config_defaults.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    69741 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/impala_client.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2085 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/cookie_util.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      986 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/impala_build_version.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    16188 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaHttpClient.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/hive_metastore/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1841 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/hive_metastore/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  1133584 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/hive_metastore/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  2093003 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/hive_metastore/ThriftHiveMetastore.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       57 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/hive_metastore/__init__.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    93752 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/impala_shell.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/BackendGflags/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/BackendGflags/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    83607 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/BackendGflags/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/BackendGflags/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Frontend/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Frontend/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   257204 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Frontend/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Frontend/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Zip/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Zip/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3234 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Zip/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Zip/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/TCLIService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1055 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/TCLIService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   136485 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/TCLIService/TCLIService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   244075 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/TCLIService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       49 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/TCLIService/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/PlanNodes/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/PlanNodes/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   171088 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/PlanNodes/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/PlanNodes/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/JniCatalog/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      412 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/JniCatalog/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   254619 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/JniCatalog/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/JniCatalog/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/ImpalaService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    51193 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaService/ImpalaHiveServer2Service.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69323 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaService/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    47740 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ImpalaService/ImpalaService.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    21118 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/option_parser.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Logging/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Logging/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6111 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Logging/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Logging/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/DataSinks/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/DataSinks/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    37237 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/DataSinks/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/DataSinks/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/MetricDefs/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   127227 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/MetricDefs/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5039 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/MetricDefs/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/MetricDefs/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/StatestoreService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/StatestoreService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     8032 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/StatestoreService/StatestoreService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    52057 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/StatestoreService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/StatestoreService/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    13898 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/StatestoreService/StatestoreSubscriber.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     8485 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/shell_output.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/CatalogObjects/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      398 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogObjects/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   204572 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogObjects/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogObjects/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/NetworkTest/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/NetworkTest/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7640 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/NetworkTest/NetworkTestService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4553 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/NetworkTest/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       56 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/NetworkTest/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/CatalogService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    57260 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogService/CatalogService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      432 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   155237 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogService/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/parquet/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/parquet/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   184091 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/parquet/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/parquet/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2072 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/ExecStats/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ExecStats/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    20911 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ExecStats/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ExecStats/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/LineageGraph/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/LineageGraph/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    17384 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/LineageGraph/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/LineageGraph/__init__.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6399 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/thrift_printer.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Planner/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Planner/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    23434 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Planner/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Planner/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/ExternalDataSource/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ExternalDataSource/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    36903 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ExternalDataSource/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ExternalDataSource/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/CatalogInternalService/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogInternalService/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7882 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogInternalService/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/CatalogInternalService/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Types/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Types/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    43325 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Types/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Types/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/beeswaxd/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/beeswaxd/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    27060 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/beeswaxd/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    82393 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/beeswaxd/BeeswaxService.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/beeswaxd/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/RuntimeProfile/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/RuntimeProfile/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    73406 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/RuntimeProfile/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/RuntimeProfile/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Query/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      413 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Query/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   147695 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Query/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Query/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/ErrorCodes/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    12746 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ErrorCodes/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    18611 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ErrorCodes/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/ErrorCodes/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Data/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Data/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    19140 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Data/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Data/__init__.py
--rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)     6552 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/TSSLSocketWithWildcardSAN.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell/Results/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Results/constants.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6110 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Results/ttypes.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell/Results/__init__.py
-drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell.egg-info/
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell.egg-info/PKG-INFO
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        1 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5215 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/impala_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       78 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell.egg-info/entry_points.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell.egg-info/requires.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       13 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/impala_shell.egg-info/top_level.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6129 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/setup.py
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        7 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/version.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2442 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/README.md
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       97 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/MANIFEST.in
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-04-13 20:54:09.000000 impala_shell-4.3.0a2/requirements.txt
--rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       38 2023-04-13 20:54:10.000000 impala_shell-4.3.0a2/setup.cfg
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/PKG-INFO
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    58107 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/LICENSE.txt
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Exprs/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Exprs/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    59637 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Exprs/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Exprs/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2157 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/shell_exceptions.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Metrics/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Metrics/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1755 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Metrics/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Metrics/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4395 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ResourceProfile/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/fb303/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      961 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       53 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69618 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/fb303/FacebookService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1765 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/value_converter.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Status/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Status/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3396 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Status/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Status/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4200 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/SqlConstraints/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Partitions/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Partitions/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3917 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Partitions/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Partitions/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    32802 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Descriptors/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      396 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    38764 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1433 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/compatibility.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2393 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_shell_config_defaults.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    70102 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_client.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2085 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/cookie_util.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      986 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_build_version.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    17002 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaHttpClient.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1841 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  1141856 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)  2099744 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/ThriftHiveMetastore.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       57 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/hive_metastore/__init__.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    96419 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/impala_shell.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    83607 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/BackendGflags/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Frontend/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Frontend/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   257862 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Frontend/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Frontend/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Zip/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Zip/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3234 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Zip/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Zip/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     1055 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   136485 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/TCLIService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   244075 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       49 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TCLIService/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   171160 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/PlanNodes/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      412 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   255110 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/JniCatalog/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    51193 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaHiveServer2Service.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    69461 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    47740 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaService.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)    21476 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/option_parser.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Logging/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Logging/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6111 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Logging/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Logging/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    37237 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/DataSinks/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   127227 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5039 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/MetricDefs/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     8032 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    52057 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       79 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    13898 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreSubscriber.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     9123 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/shell_output.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      398 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   204572 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogObjects/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7640 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/NetworkTestService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     4553 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       56 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/NetworkTest/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    57260 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/CatalogService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      432 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   155237 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogService/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/parquet/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/parquet/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   184091 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/parquet/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/parquet/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2072 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    20911 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExecStats/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    17384 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/LineageGraph/__init__.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6399 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/thrift_printer.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Planner/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Planner/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    23434 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Planner/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Planner/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    36903 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ExternalDataSource/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     7882 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/CatalogInternalService/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Types/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Types/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    43325 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Types/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Types/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    27060 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    82393 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/BeeswaxService.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       52 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/beeswaxd/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    73406 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/RuntimeProfile/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Query/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      451 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Query/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)   148375 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Query/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Query/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    12746 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    18611 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/ErrorCodes/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Data/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Data/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)    19140 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Data/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Data/__init__.py
+-rwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)     6552 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/TSSLSocketWithWildcardSAN.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell/Results/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      370 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Results/constants.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6110 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Results/ttypes.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       34 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/impala_shell/Results/__init__.py
+drwxrwxr-x   0 wenzhe    (1000) wenzhe    (1000)        0 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     3913 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        1 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     5215 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       78 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/requires.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       13 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/impala_shell.egg-info/top_level.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     6129 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/setup.py
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)        7 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/version.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)     2442 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/README.md
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       97 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/MANIFEST.in
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)      164 2023-05-25 22:17:35.000000 impala_shell-4.3.0a3/requirements.txt
+-rw-rw-r--   0 wenzhe    (1000) wenzhe    (1000)       38 2023-05-25 22:17:36.000000 impala_shell-4.3.0a3/setup.cfg
```

### Comparing `impala_shell-4.3.0a2/PKG-INFO` & `impala_shell-4.3.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impala_shell
-Version: 4.3.0a2
+Version: 4.3.0a3
 Summary: Impala Shell
 Home-page: https://impala.apache.org/
 Author: Impala Dev
 Author-email: dev@impala.apache.org
 License: Apache Software License
 Description: # Impala Interactive Shell
```

### Comparing `impala_shell-4.3.0a2/LICENSE.txt` & `impala_shell-4.3.0a3/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -697,48 +697,14 @@
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  THE SOFTWARE.
 
 --------------------------------------------------------------------------------
 
-cmake_modules/FindJNI.cmake: 3-clause BSD
-
- Copyright 2001-2009 Kitware, Inc.
-
- Redistribution and use in source and binary forms, with or without
- modification, are permitted provided that the following conditions
- are met:
-
- * Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-
- * Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
-
- * Neither the names of Kitware, Inc., the Insight Software Consortium,
-   nor the names of their contributors may be used to endorse or promote
-   products derived from this software without specific prior written
-   permission.
-
- THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
- LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
- A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
- HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
- SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
- LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
- DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
- THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
- (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
- OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
---------------------------------------------------------------------------------
-
 be/src/kudu/util (some portions): 3-clause BSD license
 
 Some portions of this module are derived from code from LevelDB
 ( https://github.com/google/leveldb ):
 
   Copyright (c) 2011 The LevelDB Authors. All rights reserved.
```

### Comparing `impala_shell-4.3.0a2/impala_shell/Exprs/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Exprs/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/shell_exceptions.py` & `impala_shell-4.3.0a3/impala_shell/shell_exceptions.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Metrics/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Metrics/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/ResourceProfile/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/ResourceProfile/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/fb303/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/fb303/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/fb303/FacebookService.py` & `impala_shell-4.3.0a3/impala_shell/fb303/FacebookService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/value_converter.py` & `impala_shell-4.3.0a3/impala_shell/value_converter.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Status/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Status/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/SqlConstraints/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/SqlConstraints/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Partitions/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Partitions/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Descriptors/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Descriptors/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/ImpalaInternalService/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/ImpalaInternalService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/compatibility.py` & `impala_shell-4.3.0a3/impala_shell/compatibility.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/impala_shell_config_defaults.py` & `impala_shell-4.3.0a3/impala_shell/impala_shell_config_defaults.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/impala_client.py` & `impala_shell-4.3.0a3/impala_shell/impala_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import operator
 import re
 import sasl
 import socket
 import ssl
 import sys
 import time
+import traceback
 from datetime import datetime
 import uuid
 
 from beeswaxd import BeeswaxService
 from beeswaxd.BeeswaxService import QueryState
 from ExecStats.ttypes import TExecStats
 from ImpalaService import ImpalaService, ImpalaHiveServer2Service
@@ -130,15 +131,16 @@
   for methods that are expected to be implemented in the subclasses.
   TODO: when beeswax support is removed, merge this with ImpalaHS2Client."""
   def __init__(self, impalad, fetch_size, kerberos_host_fqdn, use_kerberos=False,
                kerberos_service_name="impala", use_ssl=False, ca_cert=None, user=None,
                ldap_password=None, use_ldap=False, client_connect_timeout_ms=60000,
                verbose=True, use_http_base_transport=False, http_path=None,
                http_cookie_names=None, http_socket_timeout_s=None, value_converter=None,
-               connect_max_tries=4, rpc_stdout=False, rpc_file=None, http_tracing=True):
+               connect_max_tries=4, rpc_stdout=False, rpc_file=None, http_tracing=True,
+               jwt=None):
     self.connected = False
     self.impalad_host = impalad[0]
     self.impalad_port = int(impalad[1])
     self.kerberos_host_fqdn = kerberos_host_fqdn
     self.imp_service = None
     self.transport = None
     self.use_kerberos = use_kerberos
@@ -153,14 +155,15 @@
     self.default_query_options = {}
     self.query_option_levels = {}
     self.fetch_size = fetch_size
     self.use_http_base_transport = use_http_base_transport
     self.http_path = http_path
     self.http_cookie_names = http_cookie_names
     self.http_tracing = http_tracing
+    self.jwt = jwt
     # This is set from ImpalaShell's signal handler when a query is cancelled
     # from command line via CTRL+C. It is used to suppress error messages of
     # query cancellation.
     self.is_query_cancelled = False
     self.verbose = verbose
     # This is set in connect(). It's used in constructing the retried query link after
     # we parse the retried query id.
@@ -420,14 +423,16 @@
       user_passwd = "{0}:{1}".format(self.user, self.ldap_password)
       if sys.version_info.major < 3 or \
           sys.version_info.major == 3 and sys.version_info.minor == 0:
         auth = base64.encodestring(user_passwd.encode()).decode().strip('\n')
       else:
         auth = base64.encodebytes(user_passwd.encode()).decode().strip('\n')
       transport.setLdapAuth(auth)
+    elif self.jwt is not None:
+      transport.setJwtAuth(self.jwt)
     elif self.use_kerberos or self.kerberos_host_fqdn:
       # Set the Kerberos service
       if self.kerberos_host_fqdn is not None:
         kerb_host = self.kerberos_host_fqdn.split(':')[0].encode('ascii', 'ignore')
       else:
         kerb_host = self.impalad_host
       kerb_service = "{0}@{1}".format(self.kerberos_service_name, kerb_host)
@@ -1253,17 +1258,17 @@
     a rpc call.  Handles both the 'rpc_stdout' and 'rpc_file' command line arguments."""
     if self.rpc_stdout or self.rpc_file is not None:
       end_time = datetime.now()
       duration = end_time - start_time
 
       def print_end_to_file(fh):
         self._print_line_separator(fh)
-        fh.write("[{0}] RPC CALL FINISHED:\n".format(datetime.now()))
+        fh.write("[{0}] RPC CALL FINISHED:\n".format(end_time))
         fh.write("OPERATION: {0}\nDETAILS:\n".format(rpc_func.__name__))
-        fh.write("  * Time:   {0}ms\n".format(duration.microseconds / 1000))
+        fh.write("  * Time:   {0}ms\n".format(duration.total_seconds() * 1000))
         fh.write("  * Result: {0}\n".format(result))
         if rpc_output is not None:
           fh.write("\nRPC RESPONSE:\n")
           self.thrift_printer.print_obj(rpc_output, fh)
         self._print_line_separator(fh)
 
       if self.rpc_stdout:
@@ -1588,7 +1593,11 @@
       if suppress_error_on_cancel and self.is_query_cancelled:
         raise QueryCancelledByShellException()
       else:
         if "BeeswaxException" in str(e):
           raise RPCException("ERROR: %s" % e.message)
         if "QueryNotFoundException" in str(e):
           raise QueryStateException('Error: Stale query handle')
+        # Print more details for other kinds of exceptions
+        print('Caught exception {0}, type={1}'.format(str(e), type(e)), file=sys.stderr)
+        traceback.print_exc()
+        raise Exception("Encountered unknown exception")
```

### Comparing `impala_shell-4.3.0a2/impala_shell/cookie_util.py` & `impala_shell-4.3.0a3/impala_shell/cookie_util.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/impala_build_version.py` & `impala_shell-4.3.0a3/impala_shell/impala_build_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 def get_version():
-  return "4.3.0a2"
+  return "4.3.0a3"
 
 def get_git_hash():
-  return "32aeeecc078015263a1282f631acde4df6bd789c"
+  return "ee300a1af09514af5650b0b14b90afc8d23d54b1"
 
 def get_build_date():
-  return "Thu Apr 13 13:00:31 PDT 2023"
+  return "Thu May 25 15:04:10 PDT 2023"
```

### Comparing `impala_shell-4.3.0a2/impala_shell/ImpalaHttpClient.py` & `impala_shell-4.3.0a3/impala_shell/ImpalaHttpClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,26 @@
     # Add the 'Authorization' header to request even if the auth cookie is
     # present to avoid a round trip in case the cookie is expired when server
     # receive the request. Since the 'auth' value is calculated once, so it
     # won't cause a performance issue.
     custom_headers['Authorization'] = "Basic " + self.__basic_auth
     return custom_headers
 
+  def getCustomHeadersWithBearerAuth(self, cookie_header, has_auth_cookie):
+    custom_headers = {}
+    if cookie_header:
+      # Add cookies to HTTP header.
+      custom_headers['Cookie'] = cookie_header
+    # Add the 'Authorization' header to request even if the auth cookie is
+    # present to avoid a round trip in case the cookie is expired when server
+    # receive the request. Since the 'auth' value is calculated once, so it
+    # won't cause a performance issue.
+    custom_headers['Authorization'] = "Bearer {0}".format(self.__bearer_token)
+    return custom_headers
+
   def getCustomHeadersWithNegotiateAuth(self, cookie_header, has_auth_cookie):
     import kerberos
     custom_headers = {}
     if cookie_header:
       # Add cookies to HTTP header.
       custom_headers['Cookie'] = cookie_header
     # For GSSAPI over http we need to dynamically generate custom request headers.
@@ -213,14 +225,20 @@
 
   # Set function to generate customized HTTP headers for Ldap authorization.
   def setLdapAuth(self, basic_auth):
     # auth mechanism: LDAP
     self.__basic_auth = basic_auth
     self.__get_custom_headers_func = self.getCustomHeadersWithBasicAuth
 
+  # Set function to generate customized HTTP headers for JWT authorization.
+  def setJwtAuth(self, jwt):
+    # auth mechanism: JWT
+    self.__bearer_token = jwt
+    self.__get_custom_headers_func = self.getCustomHeadersWithBearerAuth
+
   # Set function to generate customized HTTP headers for Kerberos authorization.
   def setKerberosAuth(self, kerb_service):
     # auth mechanism: GSSAPI
     self.__kerb_service = kerb_service
     self.__get_custom_headers_func = self.getCustomHeadersWithNegotiateAuth
 
   # Set function to generate customized HTTP headers without authorization.
```

### Comparing `impala_shell-4.3.0a2/impala_shell/hive_metastore/constants.py` & `impala_shell-4.3.0a3/impala_shell/hive_metastore/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from thrift.Thrift import TType, TMessageType, TFrozenDict, TException, TApplicationException
 from thrift.protocol.TProtocol import TProtocolException
 from thrift.TRecursive import fix_spec
 
 from .ttypes import *
 DDL_TIME = "transient_lastDdlTime"
-HMS_API = "1.2.24"
+HMS_API = "1.2.26"
 ACCESSTYPE_NONE = 1
 ACCESSTYPE_READONLY = 2
 ACCESSTYPE_WRITEONLY = 4
 ACCESSTYPE_READWRITE = 8
 HIVE_FILTER_FIELD_OWNER = "hive_filter_field_owner__"
 HIVE_FILTER_FIELD_PARAMS = "hive_filter_field_params__"
 HIVE_FILTER_FIELD_LAST_ACCESS = "hive_filter_field_last_access__"
```

### Comparing `impala_shell-4.3.0a2/impala_shell/hive_metastore/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/hive_metastore/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -14992,27 +14992,29 @@
      - tablename
      - partitionname
      - type
      - runas
      - properties
      - initiatorId
      - initiatorVersion
+     - poolName
 
     """
 
 
-    def __init__(self, dbname=None, tablename=None, partitionname=None, type=None, runas=None, properties=None, initiatorId=None, initiatorVersion=None,):
+    def __init__(self, dbname=None, tablename=None, partitionname=None, type=None, runas=None, properties=None, initiatorId=None, initiatorVersion=None, poolName=None,):
         self.dbname = dbname
         self.tablename = tablename
         self.partitionname = partitionname
         self.type = type
         self.runas = runas
         self.properties = properties
         self.initiatorId = initiatorId
         self.initiatorVersion = initiatorVersion
+        self.poolName = poolName
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -15061,14 +15063,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.STRING:
                     self.initiatorVersion = iprot.readString()
                 else:
                     iprot.skip(ftype)
+            elif fid == 9:
+                if ftype == TType.STRING:
+                    self.poolName = iprot.readString()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -15107,14 +15114,18 @@
             oprot.writeFieldBegin('initiatorId', TType.STRING, 7)
             oprot.writeString(self.initiatorId)
             oprot.writeFieldEnd()
         if self.initiatorVersion is not None:
             oprot.writeFieldBegin('initiatorVersion', TType.STRING, 8)
             oprot.writeString(self.initiatorVersion)
             oprot.writeFieldEnd()
+        if self.poolName is not None:
+            oprot.writeFieldBegin('poolName', TType.STRING, 9)
+            oprot.writeString(self.poolName)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.dbname is None:
             raise TProtocolException(message='Required field dbname is unset!')
         if self.tablename is None:
@@ -15150,19 +15161,20 @@
      - workerId
      - start
      - highestWriteId
      - errorMessage
      - hasoldabort
      - enqueueTime
      - retryRetention
+     - poolname
 
     """
 
 
-    def __init__(self, id=None, dbname=None, tablename=None, partitionname=None, type=None, runas=None, properties=None, toomanyaborts=None, state=None, workerId=None, start=None, highestWriteId=None, errorMessage=None, hasoldabort=None, enqueueTime=None, retryRetention=None,):
+    def __init__(self, id=None, dbname=None, tablename=None, partitionname=None, type=None, runas=None, properties=None, toomanyaborts=None, state=None, workerId=None, start=None, highestWriteId=None, errorMessage=None, hasoldabort=None, enqueueTime=None, retryRetention=None, poolname=None,):
         self.id = id
         self.dbname = dbname
         self.tablename = tablename
         self.partitionname = partitionname
         self.type = type
         self.runas = runas
         self.properties = properties
@@ -15171,14 +15183,15 @@
         self.workerId = workerId
         self.start = start
         self.highestWriteId = highestWriteId
         self.errorMessage = errorMessage
         self.hasoldabort = hasoldabort
         self.enqueueTime = enqueueTime
         self.retryRetention = retryRetention
+        self.poolname = poolname
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -15261,14 +15274,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 16:
                 if ftype == TType.I64:
                     self.retryRetention = iprot.readI64()
                 else:
                     iprot.skip(ftype)
+            elif fid == 17:
+                if ftype == TType.STRING:
+                    self.poolname = iprot.readString()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -15335,14 +15353,18 @@
             oprot.writeFieldBegin('enqueueTime', TType.I64, 15)
             oprot.writeI64(self.enqueueTime)
             oprot.writeFieldEnd()
         if self.retryRetention is not None:
             oprot.writeFieldBegin('retryRetention', TType.I64, 16)
             oprot.writeI64(self.retryRetention)
             oprot.writeFieldEnd()
+        if self.poolname is not None:
+            oprot.writeFieldBegin('poolname', TType.STRING, 17)
+            oprot.writeString(self.poolname)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.id is None:
             raise TProtocolException(message='Required field id is unset!')
         if self.dbname is None:
@@ -15805,35 +15827,52 @@
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
 class ShowCompactRequest(object):
+    """
+    Attributes:
+     - poolName
+
+    """
 
 
+    def __init__(self, poolName=None,):
+        self.poolName = poolName
+
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.poolName = iprot.readString()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ShowCompactRequest')
+        if self.poolName is not None:
+            oprot.writeFieldBegin('poolName', TType.STRING, 1)
+            oprot.writeString(self.poolName)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -15866,19 +15905,20 @@
      - id
      - errorMessage
      - enqueueTime
      - workerVersion
      - initiatorId
      - initiatorVersion
      - cleanerStart
+     - poolName
 
     """
 
 
-    def __init__(self, dbname=None, tablename=None, partitionname=None, type=None, state=None, workerid=None, start=None, runAs=None, hightestTxnId=None, metaInfo=None, endTime=None, hadoopJobId="None", id=None, errorMessage=None, enqueueTime=None, workerVersion=None, initiatorId=None, initiatorVersion=None, cleanerStart=None,):
+    def __init__(self, dbname=None, tablename=None, partitionname=None, type=None, state=None, workerid=None, start=None, runAs=None, hightestTxnId=None, metaInfo=None, endTime=None, hadoopJobId="None", id=None, errorMessage=None, enqueueTime=None, workerVersion=None, initiatorId=None, initiatorVersion=None, cleanerStart=None, poolName=None,):
         self.dbname = dbname
         self.tablename = tablename
         self.partitionname = partitionname
         self.type = type
         self.state = state
         self.workerid = workerid
         self.start = start
@@ -15890,14 +15930,15 @@
         self.id = id
         self.errorMessage = errorMessage
         self.enqueueTime = enqueueTime
         self.workerVersion = workerVersion
         self.initiatorId = initiatorId
         self.initiatorVersion = initiatorVersion
         self.cleanerStart = cleanerStart
+        self.poolName = poolName
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -15995,14 +16036,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 19:
                 if ftype == TType.I64:
                     self.cleanerStart = iprot.readI64()
                 else:
                     iprot.skip(ftype)
+            elif fid == 20:
+                if ftype == TType.STRING:
+                    self.poolName = iprot.readString()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -16081,14 +16127,18 @@
             oprot.writeFieldBegin('initiatorVersion', TType.STRING, 18)
             oprot.writeString(self.initiatorVersion)
             oprot.writeFieldEnd()
         if self.cleanerStart is not None:
             oprot.writeFieldBegin('cleanerStart', TType.I64, 19)
             oprot.writeI64(self.cleanerStart)
             oprot.writeFieldEnd()
+        if self.poolName is not None:
+            oprot.writeFieldBegin('poolName', TType.STRING, 20)
+            oprot.writeString(self.poolName)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.dbname is None:
             raise TProtocolException(message='Required field dbname is unset!')
         if self.tablename is None:
@@ -16350,21 +16400,23 @@
 
 
 class FindNextCompactRequest(object):
     """
     Attributes:
      - workerId
      - workerVersion
+     - poolName
 
     """
 
 
-    def __init__(self, workerId=None, workerVersion=None,):
+    def __init__(self, workerId=None, workerVersion=None, poolName=None,):
         self.workerId = workerId
         self.workerVersion = workerVersion
+        self.poolName = poolName
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -16377,14 +16429,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.workerVersion = iprot.readString()
                 else:
                     iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
+                    self.poolName = iprot.readString()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -16395,14 +16452,18 @@
             oprot.writeFieldBegin('workerId', TType.STRING, 1)
             oprot.writeString(self.workerId)
             oprot.writeFieldEnd()
         if self.workerVersion is not None:
             oprot.writeFieldBegin('workerVersion', TType.STRING, 2)
             oprot.writeString(self.workerVersion)
             oprot.writeFieldEnd()
+        if self.poolName is not None:
+            oprot.writeFieldBegin('poolName', TType.STRING, 3)
+            oprot.writeString(self.poolName)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -17785,14 +17846,161 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class WriteNotificationLogBatchRequest(object):
+    """
+    Attributes:
+     - catalog
+     - db
+     - table
+     - requestList
+
+    """
+
+
+    def __init__(self, catalog=None, db=None, table=None, requestList=None,):
+        self.catalog = catalog
+        self.db = db
+        self.table = table
+        self.requestList = requestList
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.catalog = iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.db = iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
+                    self.table = iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.requestList = []
+                    (_etype863, _size860) = iprot.readListBegin()
+                    for _i864 in range(_size860):
+                        _elem865 = WriteNotificationLogRequest()
+                        _elem865.read(iprot)
+                        self.requestList.append(_elem865)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('WriteNotificationLogBatchRequest')
+        if self.catalog is not None:
+            oprot.writeFieldBegin('catalog', TType.STRING, 1)
+            oprot.writeString(self.catalog)
+            oprot.writeFieldEnd()
+        if self.db is not None:
+            oprot.writeFieldBegin('db', TType.STRING, 2)
+            oprot.writeString(self.db)
+            oprot.writeFieldEnd()
+        if self.table is not None:
+            oprot.writeFieldBegin('table', TType.STRING, 3)
+            oprot.writeString(self.table)
+            oprot.writeFieldEnd()
+        if self.requestList is not None:
+            oprot.writeFieldBegin('requestList', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.requestList))
+            for iter866 in self.requestList:
+                iter866.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        if self.catalog is None:
+            raise TProtocolException(message='Required field catalog is unset!')
+        if self.db is None:
+            raise TProtocolException(message='Required field db is unset!')
+        if self.table is None:
+            raise TProtocolException(message='Required field table is unset!')
+        if self.requestList is None:
+            raise TProtocolException(message='Required field requestList is unset!')
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class WriteNotificationLogBatchResponse(object):
+
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('WriteNotificationLogBatchResponse')
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class MetadataPpdResult(object):
     """
     Attributes:
      - metadata
      - includeBitset
 
     """
@@ -17878,20 +18086,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.metadata = {}
-                    (_ktype861, _vtype862, _size860) = iprot.readMapBegin()
-                    for _i864 in range(_size860):
-                        _key865 = iprot.readI64()
-                        _val866 = MetadataPpdResult()
-                        _val866.read(iprot)
-                        self.metadata[_key865] = _val866
+                    (_ktype868, _vtype869, _size867) = iprot.readMapBegin()
+                    for _i871 in range(_size867):
+                        _key872 = iprot.readI64()
+                        _val873 = MetadataPpdResult()
+                        _val873.read(iprot)
+                        self.metadata[_key872] = _val873
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.BOOL:
                     self.isSupported = iprot.readBool()
                 else:
@@ -17905,17 +18113,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetFileMetadataByExprResult')
         if self.metadata is not None:
             oprot.writeFieldBegin('metadata', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.STRUCT, len(self.metadata))
-            for kiter867, viter868 in self.metadata.items():
-                oprot.writeI64(kiter867)
-                viter868.write(oprot)
+            for kiter874, viter875 in self.metadata.items():
+                oprot.writeI64(kiter874)
+                viter875.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.isSupported is not None:
             oprot.writeFieldBegin('isSupported', TType.BOOL, 2)
             oprot.writeBool(self.isSupported)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -17965,18 +18173,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.fileIds = []
-                    (_etype872, _size869) = iprot.readListBegin()
-                    for _i873 in range(_size869):
-                        _elem874 = iprot.readI64()
-                        self.fileIds.append(_elem874)
+                    (_etype879, _size876) = iprot.readListBegin()
+                    for _i880 in range(_size876):
+                        _elem881 = iprot.readI64()
+                        self.fileIds.append(_elem881)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.expr = iprot.readBinary()
                 else:
@@ -18000,16 +18208,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetFileMetadataByExprRequest')
         if self.fileIds is not None:
             oprot.writeFieldBegin('fileIds', TType.LIST, 1)
             oprot.writeListBegin(TType.I64, len(self.fileIds))
-            for iter875 in self.fileIds:
-                oprot.writeI64(iter875)
+            for iter882 in self.fileIds:
+                oprot.writeI64(iter882)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.expr is not None:
             oprot.writeFieldBegin('expr', TType.STRING, 2)
             oprot.writeBinary(self.expr)
             oprot.writeFieldEnd()
         if self.doGetFooters is not None:
@@ -18063,19 +18271,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.metadata = {}
-                    (_ktype877, _vtype878, _size876) = iprot.readMapBegin()
-                    for _i880 in range(_size876):
-                        _key881 = iprot.readI64()
-                        _val882 = iprot.readBinary()
-                        self.metadata[_key881] = _val882
+                    (_ktype884, _vtype885, _size883) = iprot.readMapBegin()
+                    for _i887 in range(_size883):
+                        _key888 = iprot.readI64()
+                        _val889 = iprot.readBinary()
+                        self.metadata[_key888] = _val889
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.BOOL:
                     self.isSupported = iprot.readBool()
                 else:
@@ -18089,17 +18297,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetFileMetadataResult')
         if self.metadata is not None:
             oprot.writeFieldBegin('metadata', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.STRING, len(self.metadata))
-            for kiter883, viter884 in self.metadata.items():
-                oprot.writeI64(kiter883)
-                oprot.writeBinary(viter884)
+            for kiter890, viter891 in self.metadata.items():
+                oprot.writeI64(kiter890)
+                oprot.writeBinary(viter891)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.isSupported is not None:
             oprot.writeFieldBegin('isSupported', TType.BOOL, 2)
             oprot.writeBool(self.isSupported)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -18143,18 +18351,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.fileIds = []
-                    (_etype888, _size885) = iprot.readListBegin()
-                    for _i889 in range(_size885):
-                        _elem890 = iprot.readI64()
-                        self.fileIds.append(_elem890)
+                    (_etype895, _size892) = iprot.readListBegin()
+                    for _i896 in range(_size892):
+                        _elem897 = iprot.readI64()
+                        self.fileIds.append(_elem897)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -18163,16 +18371,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetFileMetadataRequest')
         if self.fileIds is not None:
             oprot.writeFieldBegin('fileIds', TType.LIST, 1)
             oprot.writeListBegin(TType.I64, len(self.fileIds))
-            for iter891 in self.fileIds:
-                oprot.writeI64(iter891)
+            for iter898 in self.fileIds:
+                oprot.writeI64(iter898)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.fileIds is None:
@@ -18254,28 +18462,28 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.fileIds = []
-                    (_etype895, _size892) = iprot.readListBegin()
-                    for _i896 in range(_size892):
-                        _elem897 = iprot.readI64()
-                        self.fileIds.append(_elem897)
+                    (_etype902, _size899) = iprot.readListBegin()
+                    for _i903 in range(_size899):
+                        _elem904 = iprot.readI64()
+                        self.fileIds.append(_elem904)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.metadata = []
-                    (_etype901, _size898) = iprot.readListBegin()
-                    for _i902 in range(_size898):
-                        _elem903 = iprot.readBinary()
-                        self.metadata.append(_elem903)
+                    (_etype908, _size905) = iprot.readListBegin()
+                    for _i909 in range(_size905):
+                        _elem910 = iprot.readBinary()
+                        self.metadata.append(_elem910)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I32:
                     self.type = iprot.readI32()
                 else:
@@ -18289,23 +18497,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('PutFileMetadataRequest')
         if self.fileIds is not None:
             oprot.writeFieldBegin('fileIds', TType.LIST, 1)
             oprot.writeListBegin(TType.I64, len(self.fileIds))
-            for iter904 in self.fileIds:
-                oprot.writeI64(iter904)
+            for iter911 in self.fileIds:
+                oprot.writeI64(iter911)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.metadata is not None:
             oprot.writeFieldBegin('metadata', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.metadata))
-            for iter905 in self.metadata:
-                oprot.writeBinary(iter905)
+            for iter912 in self.metadata:
+                oprot.writeBinary(iter912)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.type is not None:
             oprot.writeFieldBegin('type', TType.I32, 3)
             oprot.writeI32(self.type)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -18389,18 +18597,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.fileIds = []
-                    (_etype909, _size906) = iprot.readListBegin()
-                    for _i910 in range(_size906):
-                        _elem911 = iprot.readI64()
-                        self.fileIds.append(_elem911)
+                    (_etype916, _size913) = iprot.readListBegin()
+                    for _i917 in range(_size913):
+                        _elem918 = iprot.readI64()
+                        self.fileIds.append(_elem918)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -18409,16 +18617,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ClearFileMetadataRequest')
         if self.fileIds is not None:
             oprot.writeFieldBegin('fileIds', TType.LIST, 1)
             oprot.writeListBegin(TType.I64, len(self.fileIds))
-            for iter912 in self.fileIds:
-                oprot.writeI64(iter912)
+            for iter919 in self.fileIds:
+                oprot.writeI64(iter919)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.fileIds is None:
@@ -18609,19 +18817,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.functions = []
-                    (_etype916, _size913) = iprot.readListBegin()
-                    for _i917 in range(_size913):
-                        _elem918 = Function()
-                        _elem918.read(iprot)
-                        self.functions.append(_elem918)
+                    (_etype923, _size920) = iprot.readListBegin()
+                    for _i924 in range(_size920):
+                        _elem925 = Function()
+                        _elem925.read(iprot)
+                        self.functions.append(_elem925)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -18630,16 +18838,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetAllFunctionsResponse')
         if self.functions is not None:
             oprot.writeFieldBegin('functions', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.functions))
-            for iter919 in self.functions:
-                iter919.write(oprot)
+            for iter926 in self.functions:
+                iter926.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -18675,18 +18883,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype923, _size920) = iprot.readListBegin()
-                    for _i924 in range(_size920):
-                        _elem925 = iprot.readI32()
-                        self.values.append(_elem925)
+                    (_etype930, _size927) = iprot.readListBegin()
+                    for _i931 in range(_size927):
+                        _elem932 = iprot.readI32()
+                        self.values.append(_elem932)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -18695,16 +18903,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ClientCapabilities')
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 1)
             oprot.writeListBegin(TType.I32, len(self.values))
-            for iter926 in self.values:
-                oprot.writeI32(iter926)
+            for iter933 in self.values:
+                oprot.writeI32(iter933)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.values is None:
@@ -18746,18 +18954,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.fieldList = []
-                    (_etype930, _size927) = iprot.readListBegin()
-                    for _i931 in range(_size927):
-                        _elem932 = iprot.readString()
-                        self.fieldList.append(_elem932)
+                    (_etype937, _size934) = iprot.readListBegin()
+                    for _i938 in range(_size934):
+                        _elem939 = iprot.readString()
+                        self.fieldList.append(_elem939)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.includeParamKeyPattern = iprot.readString()
                 else:
@@ -18776,16 +18984,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetProjectionsSpec')
         if self.fieldList is not None:
             oprot.writeFieldBegin('fieldList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.fieldList))
-            for iter933 in self.fieldList:
-                oprot.writeString(iter933)
+            for iter940 in self.fieldList:
+                oprot.writeString(iter940)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.includeParamKeyPattern is not None:
             oprot.writeFieldBegin('includeParamKeyPattern', TType.STRING, 2)
             oprot.writeString(self.includeParamKeyPattern)
             oprot.writeFieldEnd()
         if self.excludeParamKeyPattern is not None:
@@ -18880,18 +19088,18 @@
                 if ftype == TType.BOOL:
                     self.getColumnStats = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.LIST:
                     self.processorCapabilities = []
-                    (_etype937, _size934) = iprot.readListBegin()
-                    for _i938 in range(_size934):
-                        _elem939 = iprot.readString()
-                        self.processorCapabilities.append(_elem939)
+                    (_etype944, _size941) = iprot.readListBegin()
+                    for _i945 in range(_size941):
+                        _elem946 = iprot.readString()
+                        self.processorCapabilities.append(_elem946)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
                 if ftype == TType.STRING:
                     self.processorIdentifier = iprot.readString()
                 else:
@@ -18944,16 +19152,16 @@
         if self.getColumnStats is not None:
             oprot.writeFieldBegin('getColumnStats', TType.BOOL, 7)
             oprot.writeBool(self.getColumnStats)
             oprot.writeFieldEnd()
         if self.processorCapabilities is not None:
             oprot.writeFieldBegin('processorCapabilities', TType.LIST, 8)
             oprot.writeListBegin(TType.STRING, len(self.processorCapabilities))
-            for iter940 in self.processorCapabilities:
-                oprot.writeString(iter940)
+            for iter947 in self.processorCapabilities:
+                oprot.writeString(iter947)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorIdentifier is not None:
             oprot.writeFieldBegin('processorIdentifier', TType.STRING, 9)
             oprot.writeString(self.processorIdentifier)
             oprot.writeFieldEnd()
         if self.engine is not None:
@@ -19099,18 +19307,18 @@
                 if ftype == TType.STRING:
                     self.dbName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.tblNames = []
-                    (_etype944, _size941) = iprot.readListBegin()
-                    for _i945 in range(_size941):
-                        _elem946 = iprot.readString()
-                        self.tblNames.append(_elem946)
+                    (_etype951, _size948) = iprot.readListBegin()
+                    for _i952 in range(_size948):
+                        _elem953 = iprot.readString()
+                        self.tblNames.append(_elem953)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRUCT:
                     self.capabilities = ClientCapabilities()
                     self.capabilities.read(iprot)
@@ -19120,18 +19328,18 @@
                 if ftype == TType.STRING:
                     self.catName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.processorCapabilities = []
-                    (_etype950, _size947) = iprot.readListBegin()
-                    for _i951 in range(_size947):
-                        _elem952 = iprot.readString()
-                        self.processorCapabilities.append(_elem952)
+                    (_etype957, _size954) = iprot.readListBegin()
+                    for _i958 in range(_size954):
+                        _elem959 = iprot.readString()
+                        self.processorCapabilities.append(_elem959)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.STRING:
                     self.processorIdentifier = iprot.readString()
                 else:
@@ -19160,31 +19368,31 @@
         if self.dbName is not None:
             oprot.writeFieldBegin('dbName', TType.STRING, 1)
             oprot.writeString(self.dbName)
             oprot.writeFieldEnd()
         if self.tblNames is not None:
             oprot.writeFieldBegin('tblNames', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.tblNames))
-            for iter953 in self.tblNames:
-                oprot.writeString(iter953)
+            for iter960 in self.tblNames:
+                oprot.writeString(iter960)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.capabilities is not None:
             oprot.writeFieldBegin('capabilities', TType.STRUCT, 3)
             self.capabilities.write(oprot)
             oprot.writeFieldEnd()
         if self.catName is not None:
             oprot.writeFieldBegin('catName', TType.STRING, 4)
             oprot.writeString(self.catName)
             oprot.writeFieldEnd()
         if self.processorCapabilities is not None:
             oprot.writeFieldBegin('processorCapabilities', TType.LIST, 5)
             oprot.writeListBegin(TType.STRING, len(self.processorCapabilities))
-            for iter954 in self.processorCapabilities:
-                oprot.writeString(iter954)
+            for iter961 in self.processorCapabilities:
+                oprot.writeString(iter961)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorIdentifier is not None:
             oprot.writeFieldBegin('processorIdentifier', TType.STRING, 6)
             oprot.writeString(self.processorIdentifier)
             oprot.writeFieldEnd()
         if self.projectionSpec is not None:
@@ -19234,19 +19442,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.tables = []
-                    (_etype958, _size955) = iprot.readListBegin()
-                    for _i959 in range(_size955):
-                        _elem960 = Table()
-                        _elem960.read(iprot)
-                        self.tables.append(_elem960)
+                    (_etype965, _size962) = iprot.readListBegin()
+                    for _i966 in range(_size962):
+                        _elem967 = Table()
+                        _elem967.read(iprot)
+                        self.tables.append(_elem967)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -19255,16 +19463,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetTablesResult')
         if self.tables is not None:
             oprot.writeFieldBegin('tables', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.tables))
-            for iter961 in self.tables:
-                iter961.write(oprot)
+            for iter968 in self.tables:
+                iter968.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.tables is None:
@@ -19339,18 +19547,18 @@
                 if ftype == TType.I32:
                     self.limit = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.processorCapabilities = []
-                    (_etype965, _size962) = iprot.readListBegin()
-                    for _i966 in range(_size962):
-                        _elem967 = iprot.readString()
-                        self.processorCapabilities.append(_elem967)
+                    (_etype972, _size969) = iprot.readListBegin()
+                    for _i973 in range(_size969):
+                        _elem974 = iprot.readString()
+                        self.processorCapabilities.append(_elem974)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRING:
                     self.processorIdentifier = iprot.readString()
                 else:
@@ -19384,16 +19592,16 @@
         if self.limit is not None:
             oprot.writeFieldBegin('limit', TType.I32, 5)
             oprot.writeI32(self.limit)
             oprot.writeFieldEnd()
         if self.processorCapabilities is not None:
             oprot.writeFieldBegin('processorCapabilities', TType.LIST, 6)
             oprot.writeListBegin(TType.STRING, len(self.processorCapabilities))
-            for iter968 in self.processorCapabilities:
-                oprot.writeString(iter968)
+            for iter975 in self.processorCapabilities:
+                oprot.writeString(iter975)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorIdentifier is not None:
             oprot.writeFieldBegin('processorIdentifier', TType.STRING, 7)
             oprot.writeString(self.processorIdentifier)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -19457,28 +19665,28 @@
                 if ftype == TType.I32:
                     self.accessType = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.requiredReadCapabilities = []
-                    (_etype972, _size969) = iprot.readListBegin()
-                    for _i973 in range(_size969):
-                        _elem974 = iprot.readString()
-                        self.requiredReadCapabilities.append(_elem974)
+                    (_etype979, _size976) = iprot.readListBegin()
+                    for _i980 in range(_size976):
+                        _elem981 = iprot.readString()
+                        self.requiredReadCapabilities.append(_elem981)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.requiredWriteCapabilities = []
-                    (_etype978, _size975) = iprot.readListBegin()
-                    for _i979 in range(_size975):
-                        _elem980 = iprot.readString()
-                        self.requiredWriteCapabilities.append(_elem980)
+                    (_etype985, _size982) = iprot.readListBegin()
+                    for _i986 in range(_size982):
+                        _elem987 = iprot.readString()
+                        self.requiredWriteCapabilities.append(_elem987)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -19495,23 +19703,23 @@
         if self.accessType is not None:
             oprot.writeFieldBegin('accessType', TType.I32, 2)
             oprot.writeI32(self.accessType)
             oprot.writeFieldEnd()
         if self.requiredReadCapabilities is not None:
             oprot.writeFieldBegin('requiredReadCapabilities', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.requiredReadCapabilities))
-            for iter981 in self.requiredReadCapabilities:
-                oprot.writeString(iter981)
+            for iter988 in self.requiredReadCapabilities:
+                oprot.writeString(iter988)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.requiredWriteCapabilities is not None:
             oprot.writeFieldBegin('requiredWriteCapabilities', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.requiredWriteCapabilities))
-            for iter982 in self.requiredWriteCapabilities:
-                oprot.writeString(iter982)
+            for iter989 in self.requiredWriteCapabilities:
+                oprot.writeString(iter989)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.tblName is None:
@@ -19565,18 +19773,18 @@
                 if ftype == TType.STRING:
                     self.catalogName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.processorCapabilities = []
-                    (_etype986, _size983) = iprot.readListBegin()
-                    for _i987 in range(_size983):
-                        _elem988 = iprot.readString()
-                        self.processorCapabilities.append(_elem988)
+                    (_etype993, _size990) = iprot.readListBegin()
+                    for _i994 in range(_size990):
+                        _elem995 = iprot.readString()
+                        self.processorCapabilities.append(_elem995)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRING:
                     self.processorIdentifier = iprot.readString()
                 else:
@@ -19598,16 +19806,16 @@
         if self.catalogName is not None:
             oprot.writeFieldBegin('catalogName', TType.STRING, 2)
             oprot.writeString(self.catalogName)
             oprot.writeFieldEnd()
         if self.processorCapabilities is not None:
             oprot.writeFieldBegin('processorCapabilities', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.processorCapabilities))
-            for iter989 in self.processorCapabilities:
-                oprot.writeString(iter989)
+            for iter996 in self.processorCapabilities:
+                oprot.writeString(iter996)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorIdentifier is not None:
             oprot.writeFieldBegin('processorIdentifier', TType.STRING, 4)
             oprot.writeString(self.processorIdentifier)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -20803,52 +21011,52 @@
                     self.plan = WMResourcePlan()
                     self.plan.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.pools = []
-                    (_etype993, _size990) = iprot.readListBegin()
-                    for _i994 in range(_size990):
-                        _elem995 = WMPool()
-                        _elem995.read(iprot)
-                        self.pools.append(_elem995)
+                    (_etype1000, _size997) = iprot.readListBegin()
+                    for _i1001 in range(_size997):
+                        _elem1002 = WMPool()
+                        _elem1002.read(iprot)
+                        self.pools.append(_elem1002)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.mappings = []
-                    (_etype999, _size996) = iprot.readListBegin()
-                    for _i1000 in range(_size996):
-                        _elem1001 = WMMapping()
-                        _elem1001.read(iprot)
-                        self.mappings.append(_elem1001)
+                    (_etype1006, _size1003) = iprot.readListBegin()
+                    for _i1007 in range(_size1003):
+                        _elem1008 = WMMapping()
+                        _elem1008.read(iprot)
+                        self.mappings.append(_elem1008)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.triggers = []
-                    (_etype1005, _size1002) = iprot.readListBegin()
-                    for _i1006 in range(_size1002):
-                        _elem1007 = WMTrigger()
-                        _elem1007.read(iprot)
-                        self.triggers.append(_elem1007)
+                    (_etype1012, _size1009) = iprot.readListBegin()
+                    for _i1013 in range(_size1009):
+                        _elem1014 = WMTrigger()
+                        _elem1014.read(iprot)
+                        self.triggers.append(_elem1014)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.poolTriggers = []
-                    (_etype1011, _size1008) = iprot.readListBegin()
-                    for _i1012 in range(_size1008):
-                        _elem1013 = WMPoolTrigger()
-                        _elem1013.read(iprot)
-                        self.poolTriggers.append(_elem1013)
+                    (_etype1018, _size1015) = iprot.readListBegin()
+                    for _i1019 in range(_size1015):
+                        _elem1020 = WMPoolTrigger()
+                        _elem1020.read(iprot)
+                        self.poolTriggers.append(_elem1020)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -20861,37 +21069,37 @@
         if self.plan is not None:
             oprot.writeFieldBegin('plan', TType.STRUCT, 1)
             self.plan.write(oprot)
             oprot.writeFieldEnd()
         if self.pools is not None:
             oprot.writeFieldBegin('pools', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.pools))
-            for iter1014 in self.pools:
-                iter1014.write(oprot)
+            for iter1021 in self.pools:
+                iter1021.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.mappings is not None:
             oprot.writeFieldBegin('mappings', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.mappings))
-            for iter1015 in self.mappings:
-                iter1015.write(oprot)
+            for iter1022 in self.mappings:
+                iter1022.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.triggers is not None:
             oprot.writeFieldBegin('triggers', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.triggers))
-            for iter1016 in self.triggers:
-                iter1016.write(oprot)
+            for iter1023 in self.triggers:
+                iter1023.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.poolTriggers is not None:
             oprot.writeFieldBegin('poolTriggers', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.poolTriggers))
-            for iter1017 in self.poolTriggers:
-                iter1017.write(oprot)
+            for iter1024 in self.poolTriggers:
+                iter1024.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.plan is None:
@@ -21293,19 +21501,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.resourcePlans = []
-                    (_etype1021, _size1018) = iprot.readListBegin()
-                    for _i1022 in range(_size1018):
-                        _elem1023 = WMResourcePlan()
-                        _elem1023.read(iprot)
-                        self.resourcePlans.append(_elem1023)
+                    (_etype1028, _size1025) = iprot.readListBegin()
+                    for _i1029 in range(_size1025):
+                        _elem1030 = WMResourcePlan()
+                        _elem1030.read(iprot)
+                        self.resourcePlans.append(_elem1030)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -21314,16 +21522,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('WMGetAllResourcePlanResponse')
         if self.resourcePlans is not None:
             oprot.writeFieldBegin('resourcePlans', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.resourcePlans))
-            for iter1024 in self.resourcePlans:
-                iter1024.write(oprot)
+            for iter1031 in self.resourcePlans:
+                iter1031.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -21578,28 +21786,28 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.errors = []
-                    (_etype1028, _size1025) = iprot.readListBegin()
-                    for _i1029 in range(_size1025):
-                        _elem1030 = iprot.readString()
-                        self.errors.append(_elem1030)
+                    (_etype1035, _size1032) = iprot.readListBegin()
+                    for _i1036 in range(_size1032):
+                        _elem1037 = iprot.readString()
+                        self.errors.append(_elem1037)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.warnings = []
-                    (_etype1034, _size1031) = iprot.readListBegin()
-                    for _i1035 in range(_size1031):
-                        _elem1036 = iprot.readString()
-                        self.warnings.append(_elem1036)
+                    (_etype1041, _size1038) = iprot.readListBegin()
+                    for _i1042 in range(_size1038):
+                        _elem1043 = iprot.readString()
+                        self.warnings.append(_elem1043)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -21608,23 +21816,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('WMValidateResourcePlanResponse')
         if self.errors is not None:
             oprot.writeFieldBegin('errors', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.errors))
-            for iter1037 in self.errors:
-                oprot.writeString(iter1037)
+            for iter1044 in self.errors:
+                oprot.writeString(iter1044)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.warnings is not None:
             oprot.writeFieldBegin('warnings', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.warnings))
-            for iter1038 in self.warnings:
-                oprot.writeString(iter1038)
+            for iter1045 in self.warnings:
+                oprot.writeString(iter1045)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -22118,19 +22326,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.triggers = []
-                    (_etype1042, _size1039) = iprot.readListBegin()
-                    for _i1043 in range(_size1039):
-                        _elem1044 = WMTrigger()
-                        _elem1044.read(iprot)
-                        self.triggers.append(_elem1044)
+                    (_etype1049, _size1046) = iprot.readListBegin()
+                    for _i1050 in range(_size1046):
+                        _elem1051 = WMTrigger()
+                        _elem1051.read(iprot)
+                        self.triggers.append(_elem1051)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -22139,16 +22347,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('WMGetTriggersForResourePlanResponse')
         if self.triggers is not None:
             oprot.writeFieldBegin('triggers', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.triggers))
-            for iter1045 in self.triggers:
-                iter1045.write(oprot)
+            for iter1052 in self.triggers:
+                iter1052.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -23164,19 +23372,19 @@
                 if ftype == TType.I64:
                     self.createdAt = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.cols = []
-                    (_etype1049, _size1046) = iprot.readListBegin()
-                    for _i1050 in range(_size1046):
-                        _elem1051 = FieldSchema()
-                        _elem1051.read(iprot)
-                        self.cols.append(_elem1051)
+                    (_etype1056, _size1053) = iprot.readListBegin()
+                    for _i1057 in range(_size1053):
+                        _elem1058 = FieldSchema()
+                        _elem1058.read(iprot)
+                        self.cols.append(_elem1058)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.I32:
                     self.state = iprot.readI32()
                 else:
@@ -23228,16 +23436,16 @@
         if self.createdAt is not None:
             oprot.writeFieldBegin('createdAt', TType.I64, 3)
             oprot.writeI64(self.createdAt)
             oprot.writeFieldEnd()
         if self.cols is not None:
             oprot.writeFieldBegin('cols', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.cols))
-            for iter1052 in self.cols:
-                iter1052.write(oprot)
+            for iter1059 in self.cols:
+                iter1059.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.state is not None:
             oprot.writeFieldBegin('state', TType.I32, 5)
             oprot.writeI32(self.state)
             oprot.writeFieldEnd()
         if self.description is not None:
@@ -23445,19 +23653,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemaVersions = []
-                    (_etype1056, _size1053) = iprot.readListBegin()
-                    for _i1057 in range(_size1053):
-                        _elem1058 = SchemaVersionDescriptor()
-                        _elem1058.read(iprot)
-                        self.schemaVersions.append(_elem1058)
+                    (_etype1063, _size1060) = iprot.readListBegin()
+                    for _i1064 in range(_size1060):
+                        _elem1065 = SchemaVersionDescriptor()
+                        _elem1065.read(iprot)
+                        self.schemaVersions.append(_elem1065)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -23466,16 +23674,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('FindSchemasByColsResp')
         if self.schemaVersions is not None:
             oprot.writeFieldBegin('schemaVersions', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemaVersions))
-            for iter1059 in self.schemaVersions:
-                iter1059.write(oprot)
+            for iter1066 in self.schemaVersions:
+                iter1066.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -23891,84 +24099,84 @@
                     self.envContext = EnvironmentContext()
                     self.envContext.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.primaryKeys = []
-                    (_etype1063, _size1060) = iprot.readListBegin()
-                    for _i1064 in range(_size1060):
-                        _elem1065 = SQLPrimaryKey()
-                        _elem1065.read(iprot)
-                        self.primaryKeys.append(_elem1065)
+                    (_etype1070, _size1067) = iprot.readListBegin()
+                    for _i1071 in range(_size1067):
+                        _elem1072 = SQLPrimaryKey()
+                        _elem1072.read(iprot)
+                        self.primaryKeys.append(_elem1072)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.foreignKeys = []
-                    (_etype1069, _size1066) = iprot.readListBegin()
-                    for _i1070 in range(_size1066):
-                        _elem1071 = SQLForeignKey()
-                        _elem1071.read(iprot)
-                        self.foreignKeys.append(_elem1071)
+                    (_etype1076, _size1073) = iprot.readListBegin()
+                    for _i1077 in range(_size1073):
+                        _elem1078 = SQLForeignKey()
+                        _elem1078.read(iprot)
+                        self.foreignKeys.append(_elem1078)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.uniqueConstraints = []
-                    (_etype1075, _size1072) = iprot.readListBegin()
-                    for _i1076 in range(_size1072):
-                        _elem1077 = SQLUniqueConstraint()
-                        _elem1077.read(iprot)
-                        self.uniqueConstraints.append(_elem1077)
+                    (_etype1082, _size1079) = iprot.readListBegin()
+                    for _i1083 in range(_size1079):
+                        _elem1084 = SQLUniqueConstraint()
+                        _elem1084.read(iprot)
+                        self.uniqueConstraints.append(_elem1084)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.notNullConstraints = []
-                    (_etype1081, _size1078) = iprot.readListBegin()
-                    for _i1082 in range(_size1078):
-                        _elem1083 = SQLNotNullConstraint()
-                        _elem1083.read(iprot)
-                        self.notNullConstraints.append(_elem1083)
+                    (_etype1088, _size1085) = iprot.readListBegin()
+                    for _i1089 in range(_size1085):
+                        _elem1090 = SQLNotNullConstraint()
+                        _elem1090.read(iprot)
+                        self.notNullConstraints.append(_elem1090)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.defaultConstraints = []
-                    (_etype1087, _size1084) = iprot.readListBegin()
-                    for _i1088 in range(_size1084):
-                        _elem1089 = SQLDefaultConstraint()
-                        _elem1089.read(iprot)
-                        self.defaultConstraints.append(_elem1089)
+                    (_etype1094, _size1091) = iprot.readListBegin()
+                    for _i1095 in range(_size1091):
+                        _elem1096 = SQLDefaultConstraint()
+                        _elem1096.read(iprot)
+                        self.defaultConstraints.append(_elem1096)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.LIST:
                     self.checkConstraints = []
-                    (_etype1093, _size1090) = iprot.readListBegin()
-                    for _i1094 in range(_size1090):
-                        _elem1095 = SQLCheckConstraint()
-                        _elem1095.read(iprot)
-                        self.checkConstraints.append(_elem1095)
+                    (_etype1100, _size1097) = iprot.readListBegin()
+                    for _i1101 in range(_size1097):
+                        _elem1102 = SQLCheckConstraint()
+                        _elem1102.read(iprot)
+                        self.checkConstraints.append(_elem1102)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
                 if ftype == TType.LIST:
                     self.processorCapabilities = []
-                    (_etype1099, _size1096) = iprot.readListBegin()
-                    for _i1100 in range(_size1096):
-                        _elem1101 = iprot.readString()
-                        self.processorCapabilities.append(_elem1101)
+                    (_etype1106, _size1103) = iprot.readListBegin()
+                    for _i1107 in range(_size1103):
+                        _elem1108 = iprot.readString()
+                        self.processorCapabilities.append(_elem1108)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 10:
                 if ftype == TType.STRING:
                     self.processorIdentifier = iprot.readString()
                 else:
@@ -23990,58 +24198,58 @@
         if self.envContext is not None:
             oprot.writeFieldBegin('envContext', TType.STRUCT, 2)
             self.envContext.write(oprot)
             oprot.writeFieldEnd()
         if self.primaryKeys is not None:
             oprot.writeFieldBegin('primaryKeys', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.primaryKeys))
-            for iter1102 in self.primaryKeys:
-                iter1102.write(oprot)
+            for iter1109 in self.primaryKeys:
+                iter1109.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.foreignKeys is not None:
             oprot.writeFieldBegin('foreignKeys', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.foreignKeys))
-            for iter1103 in self.foreignKeys:
-                iter1103.write(oprot)
+            for iter1110 in self.foreignKeys:
+                iter1110.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.uniqueConstraints is not None:
             oprot.writeFieldBegin('uniqueConstraints', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.uniqueConstraints))
-            for iter1104 in self.uniqueConstraints:
-                iter1104.write(oprot)
+            for iter1111 in self.uniqueConstraints:
+                iter1111.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.notNullConstraints is not None:
             oprot.writeFieldBegin('notNullConstraints', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.notNullConstraints))
-            for iter1105 in self.notNullConstraints:
-                iter1105.write(oprot)
+            for iter1112 in self.notNullConstraints:
+                iter1112.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.defaultConstraints is not None:
             oprot.writeFieldBegin('defaultConstraints', TType.LIST, 7)
             oprot.writeListBegin(TType.STRUCT, len(self.defaultConstraints))
-            for iter1106 in self.defaultConstraints:
-                iter1106.write(oprot)
+            for iter1113 in self.defaultConstraints:
+                iter1113.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.checkConstraints is not None:
             oprot.writeFieldBegin('checkConstraints', TType.LIST, 8)
             oprot.writeListBegin(TType.STRUCT, len(self.checkConstraints))
-            for iter1107 in self.checkConstraints:
-                iter1107.write(oprot)
+            for iter1114 in self.checkConstraints:
+                iter1114.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorCapabilities is not None:
             oprot.writeFieldBegin('processorCapabilities', TType.LIST, 9)
             oprot.writeListBegin(TType.STRING, len(self.processorCapabilities))
-            for iter1108 in self.processorCapabilities:
-                oprot.writeString(iter1108)
+            for iter1115 in self.processorCapabilities:
+                oprot.writeString(iter1115)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorIdentifier is not None:
             oprot.writeFieldBegin('processorIdentifier', TType.STRING, 10)
             oprot.writeString(self.processorIdentifier)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -24120,19 +24328,19 @@
                 if ftype == TType.STRING:
                     self.locationUri = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.MAP:
                     self.parameters = {}
-                    (_ktype1110, _vtype1111, _size1109) = iprot.readMapBegin()
-                    for _i1113 in range(_size1109):
-                        _key1114 = iprot.readString()
-                        _val1115 = iprot.readString()
-                        self.parameters[_key1114] = _val1115
+                    (_ktype1117, _vtype1118, _size1116) = iprot.readMapBegin()
+                    for _i1120 in range(_size1116):
+                        _key1121 = iprot.readString()
+                        _val1122 = iprot.readString()
+                        self.parameters[_key1121] = _val1122
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.privileges = PrincipalPrivilegeSet()
                     self.privileges.read(iprot)
@@ -24194,17 +24402,17 @@
         if self.locationUri is not None:
             oprot.writeFieldBegin('locationUri', TType.STRING, 3)
             oprot.writeString(self.locationUri)
             oprot.writeFieldEnd()
         if self.parameters is not None:
             oprot.writeFieldBegin('parameters', TType.MAP, 4)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.parameters))
-            for kiter1116, viter1117 in self.parameters.items():
-                oprot.writeString(kiter1116)
-                oprot.writeString(viter1117)
+            for kiter1123, viter1124 in self.parameters.items():
+                oprot.writeString(kiter1123)
+                oprot.writeString(viter1124)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.privileges is not None:
             oprot.writeFieldBegin('privileges', TType.STRUCT, 5)
             self.privileges.write(oprot)
             oprot.writeFieldEnd()
         if self.ownerName is not None:
@@ -24924,19 +25132,19 @@
                 if ftype == TType.STRING:
                     self.tableName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.partitions = []
-                    (_etype1121, _size1118) = iprot.readListBegin()
-                    for _i1122 in range(_size1118):
-                        _elem1123 = Partition()
-                        _elem1123.read(iprot)
-                        self.partitions.append(_elem1123)
+                    (_etype1128, _size1125) = iprot.readListBegin()
+                    for _i1129 in range(_size1125):
+                        _elem1130 = Partition()
+                        _elem1130.read(iprot)
+                        self.partitions.append(_elem1130)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.environmentContext = EnvironmentContext()
                     self.environmentContext.read(iprot)
@@ -24973,16 +25181,16 @@
         if self.tableName is not None:
             oprot.writeFieldBegin('tableName', TType.STRING, 3)
             oprot.writeString(self.tableName)
             oprot.writeFieldEnd()
         if self.partitions is not None:
             oprot.writeFieldBegin('partitions', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.partitions))
-            for iter1124 in self.partitions:
-                iter1124.write(oprot)
+            for iter1131 in self.partitions:
+                iter1131.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.environmentContext is not None:
             oprot.writeFieldBegin('environmentContext', TType.STRUCT, 5)
             self.environmentContext.write(oprot)
             oprot.writeFieldEnd()
         if self.writeId is not None:
@@ -25105,18 +25313,18 @@
                 if ftype == TType.STRING:
                     self.tableName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.partVals = []
-                    (_etype1128, _size1125) = iprot.readListBegin()
-                    for _i1129 in range(_size1125):
-                        _elem1130 = iprot.readString()
-                        self.partVals.append(_elem1130)
+                    (_etype1135, _size1132) = iprot.readListBegin()
+                    for _i1136 in range(_size1132):
+                        _elem1137 = iprot.readString()
+                        self.partVals.append(_elem1137)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.newPart = Partition()
                     self.newPart.read(iprot)
@@ -25158,16 +25366,16 @@
         if self.tableName is not None:
             oprot.writeFieldBegin('tableName', TType.STRING, 3)
             oprot.writeString(self.tableName)
             oprot.writeFieldEnd()
         if self.partVals is not None:
             oprot.writeFieldBegin('partVals', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.partVals))
-            for iter1131 in self.partVals:
-                oprot.writeString(iter1131)
+            for iter1138 in self.partVals:
+                oprot.writeString(iter1138)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.newPart is not None:
             oprot.writeFieldBegin('newPart', TType.STRUCT, 5)
             self.newPart.write(oprot)
             oprot.writeFieldEnd()
         if self.validWriteIdList is not None:
@@ -25320,18 +25528,18 @@
                 if ftype == TType.STRING:
                     self.validWriteIdList = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.LIST:
                     self.processorCapabilities = []
-                    (_etype1135, _size1132) = iprot.readListBegin()
-                    for _i1136 in range(_size1132):
-                        _elem1137 = iprot.readString()
-                        self.processorCapabilities.append(_elem1137)
+                    (_etype1142, _size1139) = iprot.readListBegin()
+                    for _i1143 in range(_size1139):
+                        _elem1144 = iprot.readString()
+                        self.processorCapabilities.append(_elem1144)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
                 if ftype == TType.STRING:
                     self.processorIdentifier = iprot.readString()
                 else:
@@ -25373,16 +25581,16 @@
         if self.validWriteIdList is not None:
             oprot.writeFieldBegin('validWriteIdList', TType.STRING, 7)
             oprot.writeString(self.validWriteIdList)
             oprot.writeFieldEnd()
         if self.processorCapabilities is not None:
             oprot.writeFieldBegin('processorCapabilities', TType.LIST, 8)
             oprot.writeListBegin(TType.STRING, len(self.processorCapabilities))
-            for iter1138 in self.processorCapabilities:
-                oprot.writeString(iter1138)
+            for iter1145 in self.processorCapabilities:
+                oprot.writeString(iter1145)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorIdentifier is not None:
             oprot.writeFieldBegin('processorIdentifier', TType.STRING, 9)
             oprot.writeString(self.processorIdentifier)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -25475,18 +25683,18 @@
                 if ftype == TType.I32:
                     self.filterMode = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.LIST:
                     self.filters = []
-                    (_etype1142, _size1139) = iprot.readListBegin()
-                    for _i1143 in range(_size1139):
-                        _elem1144 = iprot.readString()
-                        self.filters.append(_elem1144)
+                    (_etype1149, _size1146) = iprot.readListBegin()
+                    for _i1150 in range(_size1146):
+                        _elem1151 = iprot.readString()
+                        self.filters.append(_elem1151)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -25499,16 +25707,16 @@
         if self.filterMode is not None:
             oprot.writeFieldBegin('filterMode', TType.I32, 7)
             oprot.writeI32(self.filterMode)
             oprot.writeFieldEnd()
         if self.filters is not None:
             oprot.writeFieldBegin('filters', TType.LIST, 8)
             oprot.writeListBegin(TType.STRING, len(self.filters))
-            for iter1145 in self.filters:
-                oprot.writeString(iter1145)
+            for iter1152 in self.filters:
+                oprot.writeString(iter1152)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -25544,19 +25752,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.partitionSpec = []
-                    (_etype1149, _size1146) = iprot.readListBegin()
-                    for _i1150 in range(_size1146):
-                        _elem1151 = PartitionSpec()
-                        _elem1151.read(iprot)
-                        self.partitionSpec.append(_elem1151)
+                    (_etype1156, _size1153) = iprot.readListBegin()
+                    for _i1157 in range(_size1153):
+                        _elem1158 = PartitionSpec()
+                        _elem1158.read(iprot)
+                        self.partitionSpec.append(_elem1158)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -25565,16 +25773,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetPartitionsResponse')
         if self.partitionSpec is not None:
             oprot.writeFieldBegin('partitionSpec', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.partitionSpec))
-            for iter1152 in self.partitionSpec:
-                iter1152.write(oprot)
+            for iter1159 in self.partitionSpec:
+                iter1159.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -25655,18 +25863,18 @@
                 if ftype == TType.STRING:
                     self.user = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.groupNames = []
-                    (_etype1156, _size1153) = iprot.readListBegin()
-                    for _i1157 in range(_size1153):
-                        _elem1158 = iprot.readString()
-                        self.groupNames.append(_elem1158)
+                    (_etype1163, _size1160) = iprot.readListBegin()
+                    for _i1164 in range(_size1160):
+                        _elem1165 = iprot.readString()
+                        self.groupNames.append(_elem1165)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.projectionSpec = GetProjectionsSpec()
                     self.projectionSpec.read(iprot)
@@ -25677,18 +25885,18 @@
                     self.filterSpec = GetPartitionsFilterSpec()
                     self.filterSpec.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 9:
                 if ftype == TType.LIST:
                     self.processorCapabilities = []
-                    (_etype1162, _size1159) = iprot.readListBegin()
-                    for _i1163 in range(_size1159):
-                        _elem1164 = iprot.readString()
-                        self.processorCapabilities.append(_elem1164)
+                    (_etype1169, _size1166) = iprot.readListBegin()
+                    for _i1170 in range(_size1166):
+                        _elem1171 = iprot.readString()
+                        self.processorCapabilities.append(_elem1171)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 10:
                 if ftype == TType.STRING:
                     self.processorIdentifier = iprot.readString()
                 else:
@@ -25727,31 +25935,31 @@
         if self.user is not None:
             oprot.writeFieldBegin('user', TType.STRING, 5)
             oprot.writeString(self.user)
             oprot.writeFieldEnd()
         if self.groupNames is not None:
             oprot.writeFieldBegin('groupNames', TType.LIST, 6)
             oprot.writeListBegin(TType.STRING, len(self.groupNames))
-            for iter1165 in self.groupNames:
-                oprot.writeString(iter1165)
+            for iter1172 in self.groupNames:
+                oprot.writeString(iter1172)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.projectionSpec is not None:
             oprot.writeFieldBegin('projectionSpec', TType.STRUCT, 7)
             self.projectionSpec.write(oprot)
             oprot.writeFieldEnd()
         if self.filterSpec is not None:
             oprot.writeFieldBegin('filterSpec', TType.STRUCT, 8)
             self.filterSpec.write(oprot)
             oprot.writeFieldEnd()
         if self.processorCapabilities is not None:
             oprot.writeFieldBegin('processorCapabilities', TType.LIST, 9)
             oprot.writeListBegin(TType.STRING, len(self.processorCapabilities))
-            for iter1166 in self.processorCapabilities:
-                oprot.writeString(iter1166)
+            for iter1173 in self.processorCapabilities:
+                oprot.writeString(iter1173)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.processorIdentifier is not None:
             oprot.writeFieldBegin('processorIdentifier', TType.STRING, 10)
             oprot.writeString(self.processorIdentifier)
             oprot.writeFieldEnd()
         if self.validWriteIdList is not None:
@@ -25912,19 +26120,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.fields = []
-                    (_etype1170, _size1167) = iprot.readListBegin()
-                    for _i1171 in range(_size1167):
-                        _elem1172 = FieldSchema()
-                        _elem1172.read(iprot)
-                        self.fields.append(_elem1172)
+                    (_etype1177, _size1174) = iprot.readListBegin()
+                    for _i1178 in range(_size1174):
+                        _elem1179 = FieldSchema()
+                        _elem1179.read(iprot)
+                        self.fields.append(_elem1179)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -25933,16 +26141,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetFieldsResponse')
         if self.fields is not None:
             oprot.writeFieldBegin('fields', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.fields))
-            for iter1173 in self.fields:
-                iter1173.write(oprot)
+            for iter1180 in self.fields:
+                iter1180.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.fields is None:
@@ -26097,19 +26305,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.fields = []
-                    (_etype1177, _size1174) = iprot.readListBegin()
-                    for _i1178 in range(_size1174):
-                        _elem1179 = FieldSchema()
-                        _elem1179.read(iprot)
-                        self.fields.append(_elem1179)
+                    (_etype1184, _size1181) = iprot.readListBegin()
+                    for _i1185 in range(_size1181):
+                        _elem1186 = FieldSchema()
+                        _elem1186.read(iprot)
+                        self.fields.append(_elem1186)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -26118,16 +26326,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetSchemaResponse')
         if self.fields is not None:
             oprot.writeFieldBegin('fields', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.fields))
-            for iter1180 in self.fields:
-                iter1180.write(oprot)
+            for iter1187 in self.fields:
+                iter1187.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.fields is None:
@@ -26190,18 +26398,18 @@
                 if ftype == TType.STRING:
                     self.tblName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.partVals = []
-                    (_etype1184, _size1181) = iprot.readListBegin()
-                    for _i1185 in range(_size1181):
-                        _elem1186 = iprot.readString()
-                        self.partVals.append(_elem1186)
+                    (_etype1191, _size1188) = iprot.readListBegin()
+                    for _i1192 in range(_size1188):
+                        _elem1193 = iprot.readString()
+                        self.partVals.append(_elem1193)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRING:
                     self.validWriteIdList = iprot.readString()
                 else:
@@ -26232,16 +26440,16 @@
         if self.tblName is not None:
             oprot.writeFieldBegin('tblName', TType.STRING, 3)
             oprot.writeString(self.tblName)
             oprot.writeFieldEnd()
         if self.partVals is not None:
             oprot.writeFieldBegin('partVals', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.partVals))
-            for iter1187 in self.partVals:
-                oprot.writeString(iter1187)
+            for iter1194 in self.partVals:
+                oprot.writeString(iter1194)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.validWriteIdList is not None:
             oprot.writeFieldBegin('validWriteIdList', TType.STRING, 5)
             oprot.writeString(self.validWriteIdList)
             oprot.writeFieldEnd()
         if self.id is not None:
@@ -26467,19 +26675,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.partitions = []
-                    (_etype1191, _size1188) = iprot.readListBegin()
-                    for _i1192 in range(_size1188):
-                        _elem1193 = Partition()
-                        _elem1193.read(iprot)
-                        self.partitions.append(_elem1193)
+                    (_etype1198, _size1195) = iprot.readListBegin()
+                    for _i1199 in range(_size1195):
+                        _elem1200 = Partition()
+                        _elem1200.read(iprot)
+                        self.partitions.append(_elem1200)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -26488,16 +26696,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('PartitionsResponse')
         if self.partitions is not None:
             oprot.writeFieldBegin('partitions', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.partitions))
-            for iter1194 in self.partitions:
-                iter1194.write(oprot)
+            for iter1201 in self.partitions:
+                iter1201.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.partitions is None:
@@ -26562,18 +26770,18 @@
                 if ftype == TType.STRING:
                     self.tblName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.partValues = []
-                    (_etype1198, _size1195) = iprot.readListBegin()
-                    for _i1199 in range(_size1195):
-                        _elem1200 = iprot.readString()
-                        self.partValues.append(_elem1200)
+                    (_etype1205, _size1202) = iprot.readListBegin()
+                    for _i1206 in range(_size1202):
+                        _elem1207 = iprot.readString()
+                        self.partValues.append(_elem1207)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.I16:
                     self.maxParts = iprot.readI16()
                 else:
@@ -26609,16 +26817,16 @@
         if self.tblName is not None:
             oprot.writeFieldBegin('tblName', TType.STRING, 3)
             oprot.writeString(self.tblName)
             oprot.writeFieldEnd()
         if self.partValues is not None:
             oprot.writeFieldBegin('partValues', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.partValues))
-            for iter1201 in self.partValues:
-                oprot.writeString(iter1201)
+            for iter1208 in self.partValues:
+                oprot.writeString(iter1208)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.maxParts is not None:
             oprot.writeFieldBegin('maxParts', TType.I16, 5)
             oprot.writeI16(self.maxParts)
             oprot.writeFieldEnd()
         if self.validWriteIdList is not None:
@@ -26670,18 +26878,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.names = []
-                    (_etype1205, _size1202) = iprot.readListBegin()
-                    for _i1206 in range(_size1202):
-                        _elem1207 = iprot.readString()
-                        self.names.append(_elem1207)
+                    (_etype1212, _size1209) = iprot.readListBegin()
+                    for _i1213 in range(_size1209):
+                        _elem1214 = iprot.readString()
+                        self.names.append(_elem1214)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -26690,16 +26898,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetPartitionNamesPsResponse')
         if self.names is not None:
             oprot.writeFieldBegin('names', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.names))
-            for iter1208 in self.names:
-                oprot.writeString(iter1208)
+            for iter1215 in self.names:
+                oprot.writeString(iter1215)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.names is None:
@@ -26768,18 +26976,18 @@
                 if ftype == TType.STRING:
                     self.tblName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.partVals = []
-                    (_etype1212, _size1209) = iprot.readListBegin()
-                    for _i1213 in range(_size1209):
-                        _elem1214 = iprot.readString()
-                        self.partVals.append(_elem1214)
+                    (_etype1219, _size1216) = iprot.readListBegin()
+                    for _i1220 in range(_size1216):
+                        _elem1221 = iprot.readString()
+                        self.partVals.append(_elem1221)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.I16:
                     self.maxParts = iprot.readI16()
                 else:
@@ -26788,18 +26996,18 @@
                 if ftype == TType.STRING:
                     self.userName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.groupNames = []
-                    (_etype1218, _size1215) = iprot.readListBegin()
-                    for _i1219 in range(_size1215):
-                        _elem1220 = iprot.readString()
-                        self.groupNames.append(_elem1220)
+                    (_etype1225, _size1222) = iprot.readListBegin()
+                    for _i1226 in range(_size1222):
+                        _elem1227 = iprot.readString()
+                        self.groupNames.append(_elem1227)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.STRING:
                     self.validWriteIdList = iprot.readString()
                 else:
@@ -26830,31 +27038,31 @@
         if self.tblName is not None:
             oprot.writeFieldBegin('tblName', TType.STRING, 3)
             oprot.writeString(self.tblName)
             oprot.writeFieldEnd()
         if self.partVals is not None:
             oprot.writeFieldBegin('partVals', TType.LIST, 4)
             oprot.writeListBegin(TType.STRING, len(self.partVals))
-            for iter1221 in self.partVals:
-                oprot.writeString(iter1221)
+            for iter1228 in self.partVals:
+                oprot.writeString(iter1228)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.maxParts is not None:
             oprot.writeFieldBegin('maxParts', TType.I16, 5)
             oprot.writeI16(self.maxParts)
             oprot.writeFieldEnd()
         if self.userName is not None:
             oprot.writeFieldBegin('userName', TType.STRING, 6)
             oprot.writeString(self.userName)
             oprot.writeFieldEnd()
         if self.groupNames is not None:
             oprot.writeFieldBegin('groupNames', TType.LIST, 7)
             oprot.writeListBegin(TType.STRING, len(self.groupNames))
-            for iter1222 in self.groupNames:
-                oprot.writeString(iter1222)
+            for iter1229 in self.groupNames:
+                oprot.writeString(iter1229)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.validWriteIdList is not None:
             oprot.writeFieldBegin('validWriteIdList', TType.STRING, 8)
             oprot.writeString(self.validWriteIdList)
             oprot.writeFieldEnd()
         if self.id is not None:
@@ -26902,19 +27110,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.partitions = []
-                    (_etype1226, _size1223) = iprot.readListBegin()
-                    for _i1227 in range(_size1223):
-                        _elem1228 = Partition()
-                        _elem1228.read(iprot)
-                        self.partitions.append(_elem1228)
+                    (_etype1233, _size1230) = iprot.readListBegin()
+                    for _i1234 in range(_size1230):
+                        _elem1235 = Partition()
+                        _elem1235.read(iprot)
+                        self.partitions.append(_elem1235)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -26923,16 +27131,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetPartitionsPsWithAuthResponse')
         if self.partitions is not None:
             oprot.writeFieldBegin('partitions', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.partitions))
-            for iter1229 in self.partitions:
-                iter1229.write(oprot)
+            for iter1236 in self.partitions:
+                iter1236.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.partitions is None:
@@ -27088,19 +27296,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.replicationMetricList = []
-                    (_etype1233, _size1230) = iprot.readListBegin()
-                    for _i1234 in range(_size1230):
-                        _elem1235 = ReplicationMetrics()
-                        _elem1235.read(iprot)
-                        self.replicationMetricList.append(_elem1235)
+                    (_etype1240, _size1237) = iprot.readListBegin()
+                    for _i1241 in range(_size1237):
+                        _elem1242 = ReplicationMetrics()
+                        _elem1242.read(iprot)
+                        self.replicationMetricList.append(_elem1242)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -27109,16 +27317,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ReplicationMetricList')
         if self.replicationMetricList is not None:
             oprot.writeFieldBegin('replicationMetricList', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.replicationMetricList))
-            for iter1236 in self.replicationMetricList:
-                iter1236.write(oprot)
+            for iter1243 in self.replicationMetricList:
+                iter1243.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.replicationMetricList is None:
@@ -27235,18 +27443,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.excludeTxnTypes = []
-                    (_etype1240, _size1237) = iprot.readListBegin()
-                    for _i1241 in range(_size1237):
-                        _elem1242 = iprot.readI32()
-                        self.excludeTxnTypes.append(_elem1242)
+                    (_etype1247, _size1244) = iprot.readListBegin()
+                    for _i1248 in range(_size1244):
+                        _elem1249 = iprot.readI32()
+                        self.excludeTxnTypes.append(_elem1249)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -27255,16 +27463,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('GetOpenTxnsRequest')
         if self.excludeTxnTypes is not None:
             oprot.writeFieldBegin('excludeTxnTypes', TType.LIST, 1)
             oprot.writeListBegin(TType.I32, len(self.excludeTxnTypes))
-            for iter1243 in self.excludeTxnTypes:
-                oprot.writeI32(iter1243)
+            for iter1250 in self.excludeTxnTypes:
+                oprot.writeI32(iter1250)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -30350,14 +30558,15 @@
     (2, TType.STRING, 'tablename', None, None, ),  # 2
     (3, TType.STRING, 'partitionname', None, None, ),  # 3
     (4, TType.I32, 'type', None, None, ),  # 4
     (5, TType.STRING, 'runas', None, None, ),  # 5
     (6, TType.MAP, 'properties', (TType.STRING, None, TType.STRING, None, False), None, ),  # 6
     (7, TType.STRING, 'initiatorId', None, None, ),  # 7
     (8, TType.STRING, 'initiatorVersion', None, None, ),  # 8
+    (9, TType.STRING, 'poolName', None, None, ),  # 9
 )
 all_structs.append(CompactionInfoStruct)
 CompactionInfoStruct.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'id', None, None, ),  # 1
     (2, TType.STRING, 'dbname', None, None, ),  # 2
     (3, TType.STRING, 'tablename', None, None, ),  # 3
@@ -30370,14 +30579,15 @@
     (10, TType.STRING, 'workerId', None, None, ),  # 10
     (11, TType.I64, 'start', None, None, ),  # 11
     (12, TType.I64, 'highestWriteId', None, None, ),  # 12
     (13, TType.STRING, 'errorMessage', None, None, ),  # 13
     (14, TType.BOOL, 'hasoldabort', None, None, ),  # 14
     (15, TType.I64, 'enqueueTime', None, None, ),  # 15
     (16, TType.I64, 'retryRetention', None, None, ),  # 16
+    (17, TType.STRING, 'poolname', None, None, ),  # 17
 )
 all_structs.append(OptionalCompactionInfoStruct)
 OptionalCompactionInfoStruct.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'ci', [CompactionInfoStruct, None], None, ),  # 1
 )
 all_structs.append(CompactionMetricsDataStruct)
@@ -30410,14 +30620,16 @@
     (1, TType.I64, 'id', None, None, ),  # 1
     (2, TType.STRING, 'state', None, None, ),  # 2
     (3, TType.BOOL, 'accepted', None, None, ),  # 3
     (4, TType.STRING, 'errormessage', None, None, ),  # 4
 )
 all_structs.append(ShowCompactRequest)
 ShowCompactRequest.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'poolName', None, None, ),  # 1
 )
 all_structs.append(ShowCompactResponseElement)
 ShowCompactResponseElement.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'dbname', None, None, ),  # 1
     (2, TType.STRING, 'tablename', None, None, ),  # 2
     (3, TType.STRING, 'partitionname', None, None, ),  # 3
@@ -30433,14 +30645,15 @@
     (13, TType.I64, 'id', None, None, ),  # 13
     (14, TType.STRING, 'errorMessage', None, None, ),  # 14
     (15, TType.I64, 'enqueueTime', None, None, ),  # 15
     (16, TType.STRING, 'workerVersion', None, None, ),  # 16
     (17, TType.STRING, 'initiatorId', None, None, ),  # 17
     (18, TType.STRING, 'initiatorVersion', None, None, ),  # 18
     (19, TType.I64, 'cleanerStart', None, None, ),  # 19
+    (20, TType.STRING, 'poolName', None, None, ),  # 20
 )
 all_structs.append(ShowCompactResponse)
 ShowCompactResponse.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'compacts', (TType.STRUCT, [ShowCompactResponseElement, None], False), None, ),  # 1
 )
 all_structs.append(GetLatestCommittedCompactionInfoRequest)
@@ -30457,14 +30670,15 @@
     (1, TType.LIST, 'compactions', (TType.STRUCT, [CompactionInfoStruct, None], False), None, ),  # 1
 )
 all_structs.append(FindNextCompactRequest)
 FindNextCompactRequest.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'workerId', None, None, ),  # 1
     (2, TType.STRING, 'workerVersion', None, None, ),  # 2
+    (3, TType.STRING, 'poolName', None, None, ),  # 3
 )
 all_structs.append(AddDynamicPartitions)
 AddDynamicPartitions.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'txnid', None, None, ),  # 1
     (2, TType.I64, 'writeid', None, None, ),  # 2
     (3, TType.STRING, 'dbname', None, None, ),  # 3
@@ -30566,14 +30780,25 @@
     (4, TType.STRING, 'table', None, None, ),  # 4
     (5, TType.STRUCT, 'fileInfo', [InsertEventRequestData, None], None, ),  # 5
     (6, TType.LIST, 'partitionVals', (TType.STRING, None, False), None, ),  # 6
 )
 all_structs.append(WriteNotificationLogResponse)
 WriteNotificationLogResponse.thrift_spec = (
 )
+all_structs.append(WriteNotificationLogBatchRequest)
+WriteNotificationLogBatchRequest.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'catalog', None, None, ),  # 1
+    (2, TType.STRING, 'db', None, None, ),  # 2
+    (3, TType.STRING, 'table', None, None, ),  # 3
+    (4, TType.LIST, 'requestList', (TType.STRUCT, [WriteNotificationLogRequest, None], False), None, ),  # 4
+)
+all_structs.append(WriteNotificationLogBatchResponse)
+WriteNotificationLogBatchResponse.thrift_spec = (
+)
 all_structs.append(MetadataPpdResult)
 MetadataPpdResult.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'metadata', 'BINARY', None, ),  # 1
     (2, TType.STRING, 'includeBitset', 'BINARY', None, ),  # 2
 )
 all_structs.append(GetFileMetadataByExprResult)
```

### Comparing `impala_shell-4.3.0a2/impala_shell/hive_metastore/ThriftHiveMetastore.py` & `impala_shell-4.3.0a3/impala_shell/hive_metastore/ThriftHiveMetastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1814,14 +1814,22 @@
         """
         Parameters:
          - rqst
 
         """
         pass
 
+    def add_write_notification_log_in_batch(self, rqst):
+        """
+        Parameters:
+         - rqst
+
+        """
+        pass
+
     def cm_recycle(self, request):
         """
         Parameters:
          - request
 
         """
         pass
@@ -9942,14 +9950,46 @@
         result = add_write_notification_log_result()
         result.read(iprot)
         iprot.readMessageEnd()
         if result.success is not None:
             return result.success
         raise TApplicationException(TApplicationException.MISSING_RESULT, "add_write_notification_log failed: unknown result")
 
+    def add_write_notification_log_in_batch(self, rqst):
+        """
+        Parameters:
+         - rqst
+
+        """
+        self.send_add_write_notification_log_in_batch(rqst)
+        return self.recv_add_write_notification_log_in_batch()
+
+    def send_add_write_notification_log_in_batch(self, rqst):
+        self._oprot.writeMessageBegin('add_write_notification_log_in_batch', TMessageType.CALL, self._seqid)
+        args = add_write_notification_log_in_batch_args()
+        args.rqst = rqst
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_add_write_notification_log_in_batch(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = add_write_notification_log_in_batch_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "add_write_notification_log_in_batch failed: unknown result")
+
     def cm_recycle(self, request):
         """
         Parameters:
          - request
 
         """
         self.send_cm_recycle(request)
@@ -12230,14 +12270,15 @@
         self._processMap["get_latest_committed_compaction_info"] = Processor.process_get_latest_committed_compaction_info
         self._processMap["get_next_notification"] = Processor.process_get_next_notification
         self._processMap["get_current_notificationEventId"] = Processor.process_get_current_notificationEventId
         self._processMap["get_notification_events_count"] = Processor.process_get_notification_events_count
         self._processMap["fire_listener_event"] = Processor.process_fire_listener_event
         self._processMap["flushCache"] = Processor.process_flushCache
         self._processMap["add_write_notification_log"] = Processor.process_add_write_notification_log
+        self._processMap["add_write_notification_log_in_batch"] = Processor.process_add_write_notification_log_in_batch
         self._processMap["cm_recycle"] = Processor.process_cm_recycle
         self._processMap["get_file_metadata_by_expr"] = Processor.process_get_file_metadata_by_expr
         self._processMap["get_file_metadata"] = Processor.process_get_file_metadata
         self._processMap["put_file_metadata"] = Processor.process_put_file_metadata
         self._processMap["clear_file_metadata"] = Processor.process_clear_file_metadata
         self._processMap["cache_file_metadata"] = Processor.process_cache_file_metadata
         self._processMap["get_metastore_db_uuid"] = Processor.process_get_metastore_db_uuid
@@ -18287,14 +18328,37 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("add_write_notification_log", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_add_write_notification_log_in_batch(self, seqid, iprot, oprot):
+        args = add_write_notification_log_in_batch_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = add_write_notification_log_in_batch_result()
+        try:
+            result.success = self._handler.add_write_notification_log_in_batch(args.rqst)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("add_write_notification_log_in_batch", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_cm_recycle(self, seqid, iprot, oprot):
         args = cm_recycle_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = cm_recycle_result()
         try:
             result.success = self._handler.cm_recycle(args.request)
@@ -21925,18 +21989,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1247, _size1244) = iprot.readListBegin()
-                    for _i1248 in range(_size1244):
-                        _elem1249 = iprot.readString()
-                        self.success.append(_elem1249)
+                    (_etype1254, _size1251) = iprot.readListBegin()
+                    for _i1255 in range(_size1251):
+                        _elem1256 = iprot.readString()
+                        self.success.append(_elem1256)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -21950,16 +22014,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_databases_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1250 in self.success:
-                oprot.writeString(iter1250)
+            for iter1257 in self.success:
+                oprot.writeString(iter1257)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -22049,18 +22113,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1254, _size1251) = iprot.readListBegin()
-                    for _i1255 in range(_size1251):
-                        _elem1256 = iprot.readString()
-                        self.success.append(_elem1256)
+                    (_etype1261, _size1258) = iprot.readListBegin()
+                    for _i1262 in range(_size1258):
+                        _elem1263 = iprot.readString()
+                        self.success.append(_elem1263)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -22074,16 +22138,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_all_databases_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1257 in self.success:
-                oprot.writeString(iter1257)
+            for iter1264 in self.success:
+                oprot.writeString(iter1264)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -22787,18 +22851,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1261, _size1258) = iprot.readListBegin()
-                    for _i1262 in range(_size1258):
-                        _elem1263 = iprot.readString()
-                        self.success.append(_elem1263)
+                    (_etype1268, _size1265) = iprot.readListBegin()
+                    for _i1269 in range(_size1265):
+                        _elem1270 = iprot.readString()
+                        self.success.append(_elem1270)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -22812,16 +22876,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_dataconnectors_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1264 in self.success:
-                oprot.writeString(iter1264)
+            for iter1271 in self.success:
+                oprot.writeString(iter1271)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -23534,20 +23598,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype1266, _vtype1267, _size1265) = iprot.readMapBegin()
-                    for _i1269 in range(_size1265):
-                        _key1270 = iprot.readString()
-                        _val1271 = Type()
-                        _val1271.read(iprot)
-                        self.success[_key1270] = _val1271
+                    (_ktype1273, _vtype1274, _size1272) = iprot.readMapBegin()
+                    for _i1276 in range(_size1272):
+                        _key1277 = iprot.readString()
+                        _val1278 = Type()
+                        _val1278.read(iprot)
+                        self.success[_key1277] = _val1278
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o2 = MetaException.read(iprot)
                 else:
@@ -23561,17 +23625,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_type_all_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter1272, viter1273 in self.success.items():
-                oprot.writeString(kiter1272)
-                viter1273.write(oprot)
+            for kiter1279, viter1280 in self.success.items():
+                oprot.writeString(kiter1279)
+                viter1280.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.o2 is not None:
             oprot.writeFieldBegin('o2', TType.STRUCT, 1)
             self.o2.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -23696,19 +23760,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1277, _size1274) = iprot.readListBegin()
-                    for _i1278 in range(_size1274):
-                        _elem1279 = FieldSchema()
-                        _elem1279.read(iprot)
-                        self.success.append(_elem1279)
+                    (_etype1284, _size1281) = iprot.readListBegin()
+                    for _i1285 in range(_size1281):
+                        _elem1286 = FieldSchema()
+                        _elem1286.read(iprot)
+                        self.success.append(_elem1286)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -23732,16 +23796,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_fields_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1280 in self.success:
-                iter1280.write(oprot)
+            for iter1287 in self.success:
+                iter1287.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -23889,19 +23953,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1284, _size1281) = iprot.readListBegin()
-                    for _i1285 in range(_size1281):
-                        _elem1286 = FieldSchema()
-                        _elem1286.read(iprot)
-                        self.success.append(_elem1286)
+                    (_etype1291, _size1288) = iprot.readListBegin()
+                    for _i1292 in range(_size1288):
+                        _elem1293 = FieldSchema()
+                        _elem1293.read(iprot)
+                        self.success.append(_elem1293)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -23925,16 +23989,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_fields_with_environment_context_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1287 in self.success:
-                iter1287.write(oprot)
+            for iter1294 in self.success:
+                iter1294.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -24230,19 +24294,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1291, _size1288) = iprot.readListBegin()
-                    for _i1292 in range(_size1288):
-                        _elem1293 = FieldSchema()
-                        _elem1293.read(iprot)
-                        self.success.append(_elem1293)
+                    (_etype1298, _size1295) = iprot.readListBegin()
+                    for _i1299 in range(_size1295):
+                        _elem1300 = FieldSchema()
+                        _elem1300.read(iprot)
+                        self.success.append(_elem1300)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -24266,16 +24330,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_schema_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1294 in self.success:
-                iter1294.write(oprot)
+            for iter1301 in self.success:
+                iter1301.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -24423,19 +24487,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1298, _size1295) = iprot.readListBegin()
-                    for _i1299 in range(_size1295):
-                        _elem1300 = FieldSchema()
-                        _elem1300.read(iprot)
-                        self.success.append(_elem1300)
+                    (_etype1305, _size1302) = iprot.readListBegin()
+                    for _i1306 in range(_size1302):
+                        _elem1307 = FieldSchema()
+                        _elem1307.read(iprot)
+                        self.success.append(_elem1307)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -24459,16 +24523,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_schema_with_environment_context_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1301 in self.success:
-                iter1301.write(oprot)
+            for iter1308 in self.success:
+                iter1308.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -25037,74 +25101,74 @@
                     self.tbl = Table()
                     self.tbl.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.primaryKeys = []
-                    (_etype1305, _size1302) = iprot.readListBegin()
-                    for _i1306 in range(_size1302):
-                        _elem1307 = SQLPrimaryKey()
-                        _elem1307.read(iprot)
-                        self.primaryKeys.append(_elem1307)
+                    (_etype1312, _size1309) = iprot.readListBegin()
+                    for _i1313 in range(_size1309):
+                        _elem1314 = SQLPrimaryKey()
+                        _elem1314.read(iprot)
+                        self.primaryKeys.append(_elem1314)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.foreignKeys = []
-                    (_etype1311, _size1308) = iprot.readListBegin()
-                    for _i1312 in range(_size1308):
-                        _elem1313 = SQLForeignKey()
-                        _elem1313.read(iprot)
-                        self.foreignKeys.append(_elem1313)
+                    (_etype1318, _size1315) = iprot.readListBegin()
+                    for _i1319 in range(_size1315):
+                        _elem1320 = SQLForeignKey()
+                        _elem1320.read(iprot)
+                        self.foreignKeys.append(_elem1320)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.uniqueConstraints = []
-                    (_etype1317, _size1314) = iprot.readListBegin()
-                    for _i1318 in range(_size1314):
-                        _elem1319 = SQLUniqueConstraint()
-                        _elem1319.read(iprot)
-                        self.uniqueConstraints.append(_elem1319)
+                    (_etype1324, _size1321) = iprot.readListBegin()
+                    for _i1325 in range(_size1321):
+                        _elem1326 = SQLUniqueConstraint()
+                        _elem1326.read(iprot)
+                        self.uniqueConstraints.append(_elem1326)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.notNullConstraints = []
-                    (_etype1323, _size1320) = iprot.readListBegin()
-                    for _i1324 in range(_size1320):
-                        _elem1325 = SQLNotNullConstraint()
-                        _elem1325.read(iprot)
-                        self.notNullConstraints.append(_elem1325)
+                    (_etype1330, _size1327) = iprot.readListBegin()
+                    for _i1331 in range(_size1327):
+                        _elem1332 = SQLNotNullConstraint()
+                        _elem1332.read(iprot)
+                        self.notNullConstraints.append(_elem1332)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.defaultConstraints = []
-                    (_etype1329, _size1326) = iprot.readListBegin()
-                    for _i1330 in range(_size1326):
-                        _elem1331 = SQLDefaultConstraint()
-                        _elem1331.read(iprot)
-                        self.defaultConstraints.append(_elem1331)
+                    (_etype1336, _size1333) = iprot.readListBegin()
+                    for _i1337 in range(_size1333):
+                        _elem1338 = SQLDefaultConstraint()
+                        _elem1338.read(iprot)
+                        self.defaultConstraints.append(_elem1338)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.checkConstraints = []
-                    (_etype1335, _size1332) = iprot.readListBegin()
-                    for _i1336 in range(_size1332):
-                        _elem1337 = SQLCheckConstraint()
-                        _elem1337.read(iprot)
-                        self.checkConstraints.append(_elem1337)
+                    (_etype1342, _size1339) = iprot.readListBegin()
+                    for _i1343 in range(_size1339):
+                        _elem1344 = SQLCheckConstraint()
+                        _elem1344.read(iprot)
+                        self.checkConstraints.append(_elem1344)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -25117,51 +25181,51 @@
         if self.tbl is not None:
             oprot.writeFieldBegin('tbl', TType.STRUCT, 1)
             self.tbl.write(oprot)
             oprot.writeFieldEnd()
         if self.primaryKeys is not None:
             oprot.writeFieldBegin('primaryKeys', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.primaryKeys))
-            for iter1338 in self.primaryKeys:
-                iter1338.write(oprot)
+            for iter1345 in self.primaryKeys:
+                iter1345.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.foreignKeys is not None:
             oprot.writeFieldBegin('foreignKeys', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.foreignKeys))
-            for iter1339 in self.foreignKeys:
-                iter1339.write(oprot)
+            for iter1346 in self.foreignKeys:
+                iter1346.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.uniqueConstraints is not None:
             oprot.writeFieldBegin('uniqueConstraints', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.uniqueConstraints))
-            for iter1340 in self.uniqueConstraints:
-                iter1340.write(oprot)
+            for iter1347 in self.uniqueConstraints:
+                iter1347.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.notNullConstraints is not None:
             oprot.writeFieldBegin('notNullConstraints', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.notNullConstraints))
-            for iter1341 in self.notNullConstraints:
-                iter1341.write(oprot)
+            for iter1348 in self.notNullConstraints:
+                iter1348.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.defaultConstraints is not None:
             oprot.writeFieldBegin('defaultConstraints', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.defaultConstraints))
-            for iter1342 in self.defaultConstraints:
-                iter1342.write(oprot)
+            for iter1349 in self.defaultConstraints:
+                iter1349.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.checkConstraints is not None:
             oprot.writeFieldBegin('checkConstraints', TType.LIST, 7)
             oprot.writeListBegin(TType.STRUCT, len(self.checkConstraints))
-            for iter1343 in self.checkConstraints:
-                iter1343.write(oprot)
+            for iter1350 in self.checkConstraints:
+                iter1350.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -26946,18 +27010,18 @@
                 if ftype == TType.STRING:
                     self.tableName = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.partNames = []
-                    (_etype1347, _size1344) = iprot.readListBegin()
-                    for _i1348 in range(_size1344):
-                        _elem1349 = iprot.readString()
-                        self.partNames.append(_elem1349)
+                    (_etype1354, _size1351) = iprot.readListBegin()
+                    for _i1355 in range(_size1351):
+                        _elem1356 = iprot.readString()
+                        self.partNames.append(_elem1356)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -26974,16 +27038,16 @@
         if self.tableName is not None:
             oprot.writeFieldBegin('tableName', TType.STRING, 2)
             oprot.writeString(self.tableName)
             oprot.writeFieldEnd()
         if self.partNames is not None:
             oprot.writeFieldBegin('partNames', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.partNames))
-            for iter1350 in self.partNames:
-                oprot.writeString(iter1350)
+            for iter1357 in self.partNames:
+                oprot.writeString(iter1357)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -27301,18 +27365,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1354, _size1351) = iprot.readListBegin()
-                    for _i1355 in range(_size1351):
-                        _elem1356 = iprot.readString()
-                        self.success.append(_elem1356)
+                    (_etype1361, _size1358) = iprot.readListBegin()
+                    for _i1362 in range(_size1358):
+                        _elem1363 = iprot.readString()
+                        self.success.append(_elem1363)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -27326,16 +27390,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_tables_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1357 in self.success:
-                oprot.writeString(iter1357)
+            for iter1364 in self.success:
+                oprot.writeString(iter1364)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -27468,18 +27532,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1361, _size1358) = iprot.readListBegin()
-                    for _i1362 in range(_size1358):
-                        _elem1363 = iprot.readString()
-                        self.success.append(_elem1363)
+                    (_etype1368, _size1365) = iprot.readListBegin()
+                    for _i1369 in range(_size1365):
+                        _elem1370 = iprot.readString()
+                        self.success.append(_elem1370)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -27493,16 +27557,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_tables_by_type_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1364 in self.success:
-                oprot.writeString(iter1364)
+            for iter1371 in self.success:
+                oprot.writeString(iter1371)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -27592,19 +27656,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1368, _size1365) = iprot.readListBegin()
-                    for _i1369 in range(_size1365):
-                        _elem1370 = Table()
-                        _elem1370.read(iprot)
-                        self.success.append(_elem1370)
+                    (_etype1375, _size1372) = iprot.readListBegin()
+                    for _i1376 in range(_size1372):
+                        _elem1377 = Table()
+                        _elem1377.read(iprot)
+                        self.success.append(_elem1377)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -27618,16 +27682,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_all_materialized_view_objects_for_rewriting_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1371 in self.success:
-                iter1371.write(oprot)
+            for iter1378 in self.success:
+                iter1378.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -27736,18 +27800,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1375, _size1372) = iprot.readListBegin()
-                    for _i1376 in range(_size1372):
-                        _elem1377 = iprot.readString()
-                        self.success.append(_elem1377)
+                    (_etype1382, _size1379) = iprot.readListBegin()
+                    for _i1383 in range(_size1379):
+                        _elem1384 = iprot.readString()
+                        self.success.append(_elem1384)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -27761,16 +27825,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_materialized_views_for_rewriting_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1378 in self.success:
-                oprot.writeString(iter1378)
+            for iter1385 in self.success:
+                oprot.writeString(iter1385)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -27829,18 +27893,18 @@
                 if ftype == TType.STRING:
                     self.tbl_patterns = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.tbl_types = []
-                    (_etype1382, _size1379) = iprot.readListBegin()
-                    for _i1383 in range(_size1379):
-                        _elem1384 = iprot.readString()
-                        self.tbl_types.append(_elem1384)
+                    (_etype1389, _size1386) = iprot.readListBegin()
+                    for _i1390 in range(_size1386):
+                        _elem1391 = iprot.readString()
+                        self.tbl_types.append(_elem1391)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -27857,16 +27921,16 @@
         if self.tbl_patterns is not None:
             oprot.writeFieldBegin('tbl_patterns', TType.STRING, 2)
             oprot.writeString(self.tbl_patterns)
             oprot.writeFieldEnd()
         if self.tbl_types is not None:
             oprot.writeFieldBegin('tbl_types', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.tbl_types))
-            for iter1385 in self.tbl_types:
-                oprot.writeString(iter1385)
+            for iter1392 in self.tbl_types:
+                oprot.writeString(iter1392)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -27911,19 +27975,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1389, _size1386) = iprot.readListBegin()
-                    for _i1390 in range(_size1386):
-                        _elem1391 = TableMeta()
-                        _elem1391.read(iprot)
-                        self.success.append(_elem1391)
+                    (_etype1396, _size1393) = iprot.readListBegin()
+                    for _i1397 in range(_size1393):
+                        _elem1398 = TableMeta()
+                        _elem1398.read(iprot)
+                        self.success.append(_elem1398)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -27937,16 +28001,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_table_meta_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1392 in self.success:
-                iter1392.write(oprot)
+            for iter1399 in self.success:
+                iter1399.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -28055,18 +28119,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1396, _size1393) = iprot.readListBegin()
-                    for _i1397 in range(_size1393):
-                        _elem1398 = iprot.readString()
-                        self.success.append(_elem1398)
+                    (_etype1403, _size1400) = iprot.readListBegin()
+                    for _i1404 in range(_size1400):
+                        _elem1405 = iprot.readString()
+                        self.success.append(_elem1405)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -28080,16 +28144,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_all_tables_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1399 in self.success:
-                oprot.writeString(iter1399)
+            for iter1406 in self.success:
+                oprot.writeString(iter1406)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -28301,18 +28365,18 @@
                 if ftype == TType.STRING:
                     self.dbname = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.tbl_names = []
-                    (_etype1403, _size1400) = iprot.readListBegin()
-                    for _i1404 in range(_size1400):
-                        _elem1405 = iprot.readString()
-                        self.tbl_names.append(_elem1405)
+                    (_etype1410, _size1407) = iprot.readListBegin()
+                    for _i1411 in range(_size1407):
+                        _elem1412 = iprot.readString()
+                        self.tbl_names.append(_elem1412)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -28325,16 +28389,16 @@
         if self.dbname is not None:
             oprot.writeFieldBegin('dbname', TType.STRING, 1)
             oprot.writeString(self.dbname)
             oprot.writeFieldEnd()
         if self.tbl_names is not None:
             oprot.writeFieldBegin('tbl_names', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.tbl_names))
-            for iter1406 in self.tbl_names:
-                oprot.writeString(iter1406)
+            for iter1413 in self.tbl_names:
+                oprot.writeString(iter1413)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -28376,19 +28440,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1410, _size1407) = iprot.readListBegin()
-                    for _i1411 in range(_size1407):
-                        _elem1412 = Table()
-                        _elem1412.read(iprot)
-                        self.success.append(_elem1412)
+                    (_etype1417, _size1414) = iprot.readListBegin()
+                    for _i1418 in range(_size1414):
+                        _elem1419 = Table()
+                        _elem1419.read(iprot)
+                        self.success.append(_elem1419)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -28397,16 +28461,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_table_objects_by_name_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1413 in self.success:
-                iter1413.write(oprot)
+            for iter1420 in self.success:
+                iter1420.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -28511,19 +28575,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1417, _size1414) = iprot.readListBegin()
-                    for _i1418 in range(_size1414):
-                        _elem1419 = ExtendedTableInfo()
-                        _elem1419.read(iprot)
-                        self.success.append(_elem1419)
+                    (_etype1424, _size1421) = iprot.readListBegin()
+                    for _i1425 in range(_size1421):
+                        _elem1426 = ExtendedTableInfo()
+                        _elem1426.read(iprot)
+                        self.success.append(_elem1426)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -28537,16 +28601,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_tables_ext_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1420 in self.success:
-                iter1420.write(oprot)
+            for iter1427 in self.success:
+                iter1427.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -29351,18 +29415,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1424, _size1421) = iprot.readListBegin()
-                    for _i1425 in range(_size1421):
-                        _elem1426 = iprot.readString()
-                        self.success.append(_elem1426)
+                    (_etype1431, _size1428) = iprot.readListBegin()
+                    for _i1432 in range(_size1428):
+                        _elem1433 = iprot.readString()
+                        self.success.append(_elem1433)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -29386,16 +29450,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_table_names_by_filter_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1427 in self.success:
-                oprot.writeString(iter1427)
+            for iter1434 in self.success:
+                oprot.writeString(iter1434)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -30442,19 +30506,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.new_parts = []
-                    (_etype1431, _size1428) = iprot.readListBegin()
-                    for _i1432 in range(_size1428):
-                        _elem1433 = Partition()
-                        _elem1433.read(iprot)
-                        self.new_parts.append(_elem1433)
+                    (_etype1438, _size1435) = iprot.readListBegin()
+                    for _i1439 in range(_size1435):
+                        _elem1440 = Partition()
+                        _elem1440.read(iprot)
+                        self.new_parts.append(_elem1440)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -30463,16 +30527,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('add_partitions_args')
         if self.new_parts is not None:
             oprot.writeFieldBegin('new_parts', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.new_parts))
-            for iter1434 in self.new_parts:
-                iter1434.write(oprot)
+            for iter1441 in self.new_parts:
+                iter1441.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -30610,19 +30674,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.new_parts = []
-                    (_etype1438, _size1435) = iprot.readListBegin()
-                    for _i1439 in range(_size1435):
-                        _elem1440 = PartitionSpec()
-                        _elem1440.read(iprot)
-                        self.new_parts.append(_elem1440)
+                    (_etype1445, _size1442) = iprot.readListBegin()
+                    for _i1446 in range(_size1442):
+                        _elem1447 = PartitionSpec()
+                        _elem1447.read(iprot)
+                        self.new_parts.append(_elem1447)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -30631,16 +30695,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('add_partitions_pspec_args')
         if self.new_parts is not None:
             oprot.writeFieldBegin('new_parts', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.new_parts))
-            for iter1441 in self.new_parts:
-                iter1441.write(oprot)
+            for iter1448 in self.new_parts:
+                iter1448.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -30792,18 +30856,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1445, _size1442) = iprot.readListBegin()
-                    for _i1446 in range(_size1442):
-                        _elem1447 = iprot.readString()
-                        self.part_vals.append(_elem1447)
+                    (_etype1452, _size1449) = iprot.readListBegin()
+                    for _i1453 in range(_size1449):
+                        _elem1454 = iprot.readString()
+                        self.part_vals.append(_elem1454)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -30820,16 +30884,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1448 in self.part_vals:
-                oprot.writeString(iter1448)
+            for iter1455 in self.part_vals:
+                oprot.writeString(iter1455)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -31147,18 +31211,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1452, _size1449) = iprot.readListBegin()
-                    for _i1453 in range(_size1449):
-                        _elem1454 = iprot.readString()
-                        self.part_vals.append(_elem1454)
+                    (_etype1459, _size1456) = iprot.readListBegin()
+                    for _i1460 in range(_size1456):
+                        _elem1461 = iprot.readString()
+                        self.part_vals.append(_elem1461)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.environment_context = EnvironmentContext()
                     self.environment_context.read(iprot)
@@ -31181,16 +31245,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1455 in self.part_vals:
-                oprot.writeString(iter1455)
+            for iter1462 in self.part_vals:
+                oprot.writeString(iter1462)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.environment_context is not None:
             oprot.writeFieldBegin('environment_context', TType.STRUCT, 4)
             self.environment_context.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -31733,18 +31797,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1459, _size1456) = iprot.readListBegin()
-                    for _i1460 in range(_size1456):
-                        _elem1461 = iprot.readString()
-                        self.part_vals.append(_elem1461)
+                    (_etype1466, _size1463) = iprot.readListBegin()
+                    for _i1467 in range(_size1463):
+                        _elem1468 = iprot.readString()
+                        self.part_vals.append(_elem1468)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.BOOL:
                     self.deleteData = iprot.readBool()
                 else:
@@ -31766,16 +31830,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1462 in self.part_vals:
-                oprot.writeString(iter1462)
+            for iter1469 in self.part_vals:
+                oprot.writeString(iter1469)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.deleteData is not None:
             oprot.writeFieldBegin('deleteData', TType.BOOL, 4)
             oprot.writeBool(self.deleteData)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -31926,18 +31990,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1466, _size1463) = iprot.readListBegin()
-                    for _i1467 in range(_size1463):
-                        _elem1468 = iprot.readString()
-                        self.part_vals.append(_elem1468)
+                    (_etype1473, _size1470) = iprot.readListBegin()
+                    for _i1474 in range(_size1470):
+                        _elem1475 = iprot.readString()
+                        self.part_vals.append(_elem1475)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.BOOL:
                     self.deleteData = iprot.readBool()
                 else:
@@ -31965,16 +32029,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1469 in self.part_vals:
-                oprot.writeString(iter1469)
+            for iter1476 in self.part_vals:
+                oprot.writeString(iter1476)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.deleteData is not None:
             oprot.writeFieldBegin('deleteData', TType.BOOL, 4)
             oprot.writeBool(self.deleteData)
             oprot.writeFieldEnd()
         if self.environment_context is not None:
@@ -32654,18 +32718,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1473, _size1470) = iprot.readListBegin()
-                    for _i1474 in range(_size1470):
-                        _elem1475 = iprot.readString()
-                        self.part_vals.append(_elem1475)
+                    (_etype1480, _size1477) = iprot.readListBegin()
+                    for _i1481 in range(_size1477):
+                        _elem1482 = iprot.readString()
+                        self.part_vals.append(_elem1482)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -32682,16 +32746,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1476 in self.part_vals:
-                oprot.writeString(iter1476)
+            for iter1483 in self.part_vals:
+                oprot.writeString(iter1483)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -32977,19 +33041,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.partitionSpecs = {}
-                    (_ktype1478, _vtype1479, _size1477) = iprot.readMapBegin()
-                    for _i1481 in range(_size1477):
-                        _key1482 = iprot.readString()
-                        _val1483 = iprot.readString()
-                        self.partitionSpecs[_key1482] = _val1483
+                    (_ktype1485, _vtype1486, _size1484) = iprot.readMapBegin()
+                    for _i1488 in range(_size1484):
+                        _key1489 = iprot.readString()
+                        _val1490 = iprot.readString()
+                        self.partitionSpecs[_key1489] = _val1490
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.source_db = iprot.readString()
                 else:
@@ -33018,17 +33082,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('exchange_partition_args')
         if self.partitionSpecs is not None:
             oprot.writeFieldBegin('partitionSpecs', TType.MAP, 1)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.partitionSpecs))
-            for kiter1484, viter1485 in self.partitionSpecs.items():
-                oprot.writeString(kiter1484)
-                oprot.writeString(viter1485)
+            for kiter1491, viter1492 in self.partitionSpecs.items():
+                oprot.writeString(kiter1491)
+                oprot.writeString(viter1492)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.source_db is not None:
             oprot.writeFieldBegin('source_db', TType.STRING, 2)
             oprot.writeString(self.source_db)
             oprot.writeFieldEnd()
         if self.source_table_name is not None:
@@ -33207,19 +33271,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.partitionSpecs = {}
-                    (_ktype1487, _vtype1488, _size1486) = iprot.readMapBegin()
-                    for _i1490 in range(_size1486):
-                        _key1491 = iprot.readString()
-                        _val1492 = iprot.readString()
-                        self.partitionSpecs[_key1491] = _val1492
+                    (_ktype1494, _vtype1495, _size1493) = iprot.readMapBegin()
+                    for _i1497 in range(_size1493):
+                        _key1498 = iprot.readString()
+                        _val1499 = iprot.readString()
+                        self.partitionSpecs[_key1498] = _val1499
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
                     self.source_db = iprot.readString()
                 else:
@@ -33248,17 +33312,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('exchange_partitions_args')
         if self.partitionSpecs is not None:
             oprot.writeFieldBegin('partitionSpecs', TType.MAP, 1)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.partitionSpecs))
-            for kiter1493, viter1494 in self.partitionSpecs.items():
-                oprot.writeString(kiter1493)
-                oprot.writeString(viter1494)
+            for kiter1500, viter1501 in self.partitionSpecs.items():
+                oprot.writeString(kiter1500)
+                oprot.writeString(viter1501)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.source_db is not None:
             oprot.writeFieldBegin('source_db', TType.STRING, 2)
             oprot.writeString(self.source_db)
             oprot.writeFieldEnd()
         if self.source_table_name is not None:
@@ -33327,19 +33391,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1498, _size1495) = iprot.readListBegin()
-                    for _i1499 in range(_size1495):
-                        _elem1500 = Partition()
-                        _elem1500.read(iprot)
-                        self.success.append(_elem1500)
+                    (_etype1505, _size1502) = iprot.readListBegin()
+                    for _i1506 in range(_size1502):
+                        _elem1507 = Partition()
+                        _elem1507.read(iprot)
+                        self.success.append(_elem1507)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -33368,16 +33432,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('exchange_partitions_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1501 in self.success:
-                iter1501.write(oprot)
+            for iter1508 in self.success:
+                iter1508.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -33455,33 +33519,33 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1505, _size1502) = iprot.readListBegin()
-                    for _i1506 in range(_size1502):
-                        _elem1507 = iprot.readString()
-                        self.part_vals.append(_elem1507)
+                    (_etype1512, _size1509) = iprot.readListBegin()
+                    for _i1513 in range(_size1509):
+                        _elem1514 = iprot.readString()
+                        self.part_vals.append(_elem1514)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRING:
                     self.user_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.group_names = []
-                    (_etype1511, _size1508) = iprot.readListBegin()
-                    for _i1512 in range(_size1508):
-                        _elem1513 = iprot.readString()
-                        self.group_names.append(_elem1513)
+                    (_etype1518, _size1515) = iprot.readListBegin()
+                    for _i1519 in range(_size1515):
+                        _elem1520 = iprot.readString()
+                        self.group_names.append(_elem1520)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -33498,27 +33562,27 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1514 in self.part_vals:
-                oprot.writeString(iter1514)
+            for iter1521 in self.part_vals:
+                oprot.writeString(iter1521)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.user_name is not None:
             oprot.writeFieldBegin('user_name', TType.STRING, 4)
             oprot.writeString(self.user_name)
             oprot.writeFieldEnd()
         if self.group_names is not None:
             oprot.writeFieldBegin('group_names', TType.LIST, 5)
             oprot.writeListBegin(TType.STRING, len(self.group_names))
-            for iter1515 in self.group_names:
-                oprot.writeString(iter1515)
+            for iter1522 in self.group_names:
+                oprot.writeString(iter1522)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -33911,19 +33975,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1519, _size1516) = iprot.readListBegin()
-                    for _i1520 in range(_size1516):
-                        _elem1521 = Partition()
-                        _elem1521.read(iprot)
-                        self.success.append(_elem1521)
+                    (_etype1526, _size1523) = iprot.readListBegin()
+                    for _i1527 in range(_size1523):
+                        _elem1528 = Partition()
+                        _elem1528.read(iprot)
+                        self.success.append(_elem1528)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = NoSuchObjectException.read(iprot)
                 else:
@@ -33942,16 +34006,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partitions_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1522 in self.success:
-                iter1522.write(oprot)
+            for iter1529 in self.success:
+                iter1529.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -34178,18 +34242,18 @@
                 if ftype == TType.STRING:
                     self.user_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.group_names = []
-                    (_etype1526, _size1523) = iprot.readListBegin()
-                    for _i1527 in range(_size1523):
-                        _elem1528 = iprot.readString()
-                        self.group_names.append(_elem1528)
+                    (_etype1533, _size1530) = iprot.readListBegin()
+                    for _i1534 in range(_size1530):
+                        _elem1535 = iprot.readString()
+                        self.group_names.append(_elem1535)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -34214,16 +34278,16 @@
         if self.user_name is not None:
             oprot.writeFieldBegin('user_name', TType.STRING, 4)
             oprot.writeString(self.user_name)
             oprot.writeFieldEnd()
         if self.group_names is not None:
             oprot.writeFieldBegin('group_names', TType.LIST, 5)
             oprot.writeListBegin(TType.STRING, len(self.group_names))
-            for iter1529 in self.group_names:
-                oprot.writeString(iter1529)
+            for iter1536 in self.group_names:
+                oprot.writeString(iter1536)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -34272,19 +34336,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1533, _size1530) = iprot.readListBegin()
-                    for _i1534 in range(_size1530):
-                        _elem1535 = Partition()
-                        _elem1535.read(iprot)
-                        self.success.append(_elem1535)
+                    (_etype1540, _size1537) = iprot.readListBegin()
+                    for _i1541 in range(_size1537):
+                        _elem1542 = Partition()
+                        _elem1542.read(iprot)
+                        self.success.append(_elem1542)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = NoSuchObjectException.read(iprot)
                 else:
@@ -34303,16 +34367,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partitions_with_auth_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1536 in self.success:
-                iter1536.write(oprot)
+            for iter1543 in self.success:
+                iter1543.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -34452,19 +34516,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1540, _size1537) = iprot.readListBegin()
-                    for _i1541 in range(_size1537):
-                        _elem1542 = PartitionSpec()
-                        _elem1542.read(iprot)
-                        self.success.append(_elem1542)
+                    (_etype1547, _size1544) = iprot.readListBegin()
+                    for _i1548 in range(_size1544):
+                        _elem1549 = PartitionSpec()
+                        _elem1549.read(iprot)
+                        self.success.append(_elem1549)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = NoSuchObjectException.read(iprot)
                 else:
@@ -34483,16 +34547,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partitions_pspec_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1543 in self.success:
-                iter1543.write(oprot)
+            for iter1550 in self.success:
+                iter1550.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -34632,18 +34696,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1547, _size1544) = iprot.readListBegin()
-                    for _i1548 in range(_size1544):
-                        _elem1549 = iprot.readString()
-                        self.success.append(_elem1549)
+                    (_etype1554, _size1551) = iprot.readListBegin()
+                    for _i1555 in range(_size1551):
+                        _elem1556 = iprot.readString()
+                        self.success.append(_elem1556)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = NoSuchObjectException.read(iprot)
                 else:
@@ -34662,16 +34726,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partition_names_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1550 in self.success:
-                oprot.writeString(iter1550)
+            for iter1557 in self.success:
+                oprot.writeString(iter1557)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -34886,18 +34950,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1554, _size1551) = iprot.readListBegin()
-                    for _i1555 in range(_size1551):
-                        _elem1556 = iprot.readString()
-                        self.part_vals.append(_elem1556)
+                    (_etype1561, _size1558) = iprot.readListBegin()
+                    for _i1562 in range(_size1558):
+                        _elem1563 = iprot.readString()
+                        self.part_vals.append(_elem1563)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I16:
                     self.max_parts = iprot.readI16()
                 else:
@@ -34919,16 +34983,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1557 in self.part_vals:
-                oprot.writeString(iter1557)
+            for iter1564 in self.part_vals:
+                oprot.writeString(iter1564)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.max_parts is not None:
             oprot.writeFieldBegin('max_parts', TType.I16, 4)
             oprot.writeI16(self.max_parts)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -34980,19 +35044,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1561, _size1558) = iprot.readListBegin()
-                    for _i1562 in range(_size1558):
-                        _elem1563 = Partition()
-                        _elem1563.read(iprot)
-                        self.success.append(_elem1563)
+                    (_etype1568, _size1565) = iprot.readListBegin()
+                    for _i1569 in range(_size1565):
+                        _elem1570 = Partition()
+                        _elem1570.read(iprot)
+                        self.success.append(_elem1570)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -35011,16 +35075,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partitions_ps_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1564 in self.success:
-                iter1564.write(oprot)
+            for iter1571 in self.success:
+                iter1571.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -35090,18 +35154,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1568, _size1565) = iprot.readListBegin()
-                    for _i1569 in range(_size1565):
-                        _elem1570 = iprot.readString()
-                        self.part_vals.append(_elem1570)
+                    (_etype1575, _size1572) = iprot.readListBegin()
+                    for _i1576 in range(_size1572):
+                        _elem1577 = iprot.readString()
+                        self.part_vals.append(_elem1577)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I16:
                     self.max_parts = iprot.readI16()
                 else:
@@ -35110,18 +35174,18 @@
                 if ftype == TType.STRING:
                     self.user_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.group_names = []
-                    (_etype1574, _size1571) = iprot.readListBegin()
-                    for _i1575 in range(_size1571):
-                        _elem1576 = iprot.readString()
-                        self.group_names.append(_elem1576)
+                    (_etype1581, _size1578) = iprot.readListBegin()
+                    for _i1582 in range(_size1578):
+                        _elem1583 = iprot.readString()
+                        self.group_names.append(_elem1583)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -35138,31 +35202,31 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1577 in self.part_vals:
-                oprot.writeString(iter1577)
+            for iter1584 in self.part_vals:
+                oprot.writeString(iter1584)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.max_parts is not None:
             oprot.writeFieldBegin('max_parts', TType.I16, 4)
             oprot.writeI16(self.max_parts)
             oprot.writeFieldEnd()
         if self.user_name is not None:
             oprot.writeFieldBegin('user_name', TType.STRING, 5)
             oprot.writeString(self.user_name)
             oprot.writeFieldEnd()
         if self.group_names is not None:
             oprot.writeFieldBegin('group_names', TType.LIST, 6)
             oprot.writeListBegin(TType.STRING, len(self.group_names))
-            for iter1578 in self.group_names:
-                oprot.writeString(iter1578)
+            for iter1585 in self.group_names:
+                oprot.writeString(iter1585)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -35212,19 +35276,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1582, _size1579) = iprot.readListBegin()
-                    for _i1583 in range(_size1579):
-                        _elem1584 = Partition()
-                        _elem1584.read(iprot)
-                        self.success.append(_elem1584)
+                    (_etype1589, _size1586) = iprot.readListBegin()
+                    for _i1590 in range(_size1586):
+                        _elem1591 = Partition()
+                        _elem1591.read(iprot)
+                        self.success.append(_elem1591)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = NoSuchObjectException.read(iprot)
                 else:
@@ -35243,16 +35307,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partitions_ps_with_auth_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1585 in self.success:
-                iter1585.write(oprot)
+            for iter1592 in self.success:
+                iter1592.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -35467,18 +35531,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1589, _size1586) = iprot.readListBegin()
-                    for _i1590 in range(_size1586):
-                        _elem1591 = iprot.readString()
-                        self.part_vals.append(_elem1591)
+                    (_etype1596, _size1593) = iprot.readListBegin()
+                    for _i1597 in range(_size1593):
+                        _elem1598 = iprot.readString()
+                        self.part_vals.append(_elem1598)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I16:
                     self.max_parts = iprot.readI16()
                 else:
@@ -35500,16 +35564,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1592 in self.part_vals:
-                oprot.writeString(iter1592)
+            for iter1599 in self.part_vals:
+                oprot.writeString(iter1599)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.max_parts is not None:
             oprot.writeFieldBegin('max_parts', TType.I16, 4)
             oprot.writeI16(self.max_parts)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -35561,18 +35625,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1596, _size1593) = iprot.readListBegin()
-                    for _i1597 in range(_size1593):
-                        _elem1598 = iprot.readString()
-                        self.success.append(_elem1598)
+                    (_etype1603, _size1600) = iprot.readListBegin()
+                    for _i1604 in range(_size1600):
+                        _elem1605 = iprot.readString()
+                        self.success.append(_elem1605)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -35591,16 +35655,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partition_names_ps_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1599 in self.success:
-                oprot.writeString(iter1599)
+            for iter1606 in self.success:
+                oprot.writeString(iter1606)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -35901,19 +35965,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1603, _size1600) = iprot.readListBegin()
-                    for _i1604 in range(_size1600):
-                        _elem1605 = Partition()
-                        _elem1605.read(iprot)
-                        self.success.append(_elem1605)
+                    (_etype1610, _size1607) = iprot.readListBegin()
+                    for _i1611 in range(_size1607):
+                        _elem1612 = Partition()
+                        _elem1612.read(iprot)
+                        self.success.append(_elem1612)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -35932,16 +35996,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partitions_by_filter_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1606 in self.success:
-                iter1606.write(oprot)
+            for iter1613 in self.success:
+                iter1613.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -36093,19 +36157,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1610, _size1607) = iprot.readListBegin()
-                    for _i1611 in range(_size1607):
-                        _elem1612 = PartitionSpec()
-                        _elem1612.read(iprot)
-                        self.success.append(_elem1612)
+                    (_etype1617, _size1614) = iprot.readListBegin()
+                    for _i1618 in range(_size1614):
+                        _elem1619 = PartitionSpec()
+                        _elem1619.read(iprot)
+                        self.success.append(_elem1619)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -36124,16 +36188,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_part_specs_by_filter_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1613 in self.success:
-                iter1613.write(oprot)
+            for iter1620 in self.success:
+                iter1620.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -36517,18 +36581,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.names = []
-                    (_etype1617, _size1614) = iprot.readListBegin()
-                    for _i1618 in range(_size1614):
-                        _elem1619 = iprot.readString()
-                        self.names.append(_elem1619)
+                    (_etype1624, _size1621) = iprot.readListBegin()
+                    for _i1625 in range(_size1621):
+                        _elem1626 = iprot.readString()
+                        self.names.append(_elem1626)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -36545,16 +36609,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.names is not None:
             oprot.writeFieldBegin('names', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.names))
-            for iter1620 in self.names:
-                oprot.writeString(iter1620)
+            for iter1627 in self.names:
+                oprot.writeString(iter1627)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -36601,19 +36665,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1624, _size1621) = iprot.readListBegin()
-                    for _i1625 in range(_size1621):
-                        _elem1626 = Partition()
-                        _elem1626.read(iprot)
-                        self.success.append(_elem1626)
+                    (_etype1631, _size1628) = iprot.readListBegin()
+                    for _i1632 in range(_size1628):
+                        _elem1633 = Partition()
+                        _elem1633.read(iprot)
+                        self.success.append(_elem1633)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -36632,16 +36696,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_partitions_by_names_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1627 in self.success:
-                iter1627.write(oprot)
+            for iter1634 in self.success:
+                iter1634.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -37015,19 +37079,19 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.new_parts = []
-                    (_etype1631, _size1628) = iprot.readListBegin()
-                    for _i1632 in range(_size1628):
-                        _elem1633 = Partition()
-                        _elem1633.read(iprot)
-                        self.new_parts.append(_elem1633)
+                    (_etype1638, _size1635) = iprot.readListBegin()
+                    for _i1639 in range(_size1635):
+                        _elem1640 = Partition()
+                        _elem1640.read(iprot)
+                        self.new_parts.append(_elem1640)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -37044,16 +37108,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.new_parts is not None:
             oprot.writeFieldBegin('new_parts', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.new_parts))
-            for iter1634 in self.new_parts:
-                iter1634.write(oprot)
+            for iter1641 in self.new_parts:
+                iter1641.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -37186,19 +37250,19 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.new_parts = []
-                    (_etype1638, _size1635) = iprot.readListBegin()
-                    for _i1639 in range(_size1635):
-                        _elem1640 = Partition()
-                        _elem1640.read(iprot)
-                        self.new_parts.append(_elem1640)
+                    (_etype1645, _size1642) = iprot.readListBegin()
+                    for _i1646 in range(_size1642):
+                        _elem1647 = Partition()
+                        _elem1647.read(iprot)
+                        self.new_parts.append(_elem1647)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.environment_context = EnvironmentContext()
                     self.environment_context.read(iprot)
@@ -37221,16 +37285,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.new_parts is not None:
             oprot.writeFieldBegin('new_parts', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.new_parts))
-            for iter1641 in self.new_parts:
-                iter1641.write(oprot)
+            for iter1648 in self.new_parts:
+                iter1648.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.environment_context is not None:
             oprot.writeFieldBegin('environment_context', TType.STRUCT, 4)
             self.environment_context.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -37691,18 +37755,18 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1645, _size1642) = iprot.readListBegin()
-                    for _i1646 in range(_size1642):
-                        _elem1647 = iprot.readString()
-                        self.part_vals.append(_elem1647)
+                    (_etype1652, _size1649) = iprot.readListBegin()
+                    for _i1653 in range(_size1649):
+                        _elem1654 = iprot.readString()
+                        self.part_vals.append(_elem1654)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.new_part = Partition()
                     self.new_part.read(iprot)
@@ -37725,16 +37789,16 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1648 in self.part_vals:
-                oprot.writeString(iter1648)
+            for iter1655 in self.part_vals:
+                oprot.writeString(iter1655)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.new_part is not None:
             oprot.writeFieldBegin('new_part', TType.STRUCT, 4)
             self.new_part.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -38007,18 +38071,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.part_vals = []
-                    (_etype1652, _size1649) = iprot.readListBegin()
-                    for _i1653 in range(_size1649):
-                        _elem1654 = iprot.readString()
-                        self.part_vals.append(_elem1654)
+                    (_etype1659, _size1656) = iprot.readListBegin()
+                    for _i1660 in range(_size1656):
+                        _elem1661 = iprot.readString()
+                        self.part_vals.append(_elem1661)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.BOOL:
                     self.throw_exception = iprot.readBool()
                 else:
@@ -38032,16 +38096,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('partition_name_has_valid_characters_args')
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.part_vals))
-            for iter1655 in self.part_vals:
-                oprot.writeString(iter1655)
+            for iter1662 in self.part_vals:
+                oprot.writeString(iter1662)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.throw_exception is not None:
             oprot.writeFieldBegin('throw_exception', TType.BOOL, 2)
             oprot.writeBool(self.throw_exception)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -38371,18 +38435,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1659, _size1656) = iprot.readListBegin()
-                    for _i1660 in range(_size1656):
-                        _elem1661 = iprot.readString()
-                        self.success.append(_elem1661)
+                    (_etype1666, _size1663) = iprot.readListBegin()
+                    for _i1667 in range(_size1663):
+                        _elem1668 = iprot.readString()
+                        self.success.append(_elem1668)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -38396,16 +38460,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('partition_name_to_vals_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1662 in self.success:
-                oprot.writeString(iter1662)
+            for iter1669 in self.success:
+                oprot.writeString(iter1669)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -38514,19 +38578,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype1664, _vtype1665, _size1663) = iprot.readMapBegin()
-                    for _i1667 in range(_size1663):
-                        _key1668 = iprot.readString()
-                        _val1669 = iprot.readString()
-                        self.success[_key1668] = _val1669
+                    (_ktype1671, _vtype1672, _size1670) = iprot.readMapBegin()
+                    for _i1674 in range(_size1670):
+                        _key1675 = iprot.readString()
+                        _val1676 = iprot.readString()
+                        self.success[_key1675] = _val1676
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -38540,17 +38604,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('partition_name_to_spec_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.success))
-            for kiter1670, viter1671 in self.success.items():
-                oprot.writeString(kiter1670)
-                oprot.writeString(viter1671)
+            for kiter1677, viter1678 in self.success.items():
+                oprot.writeString(kiter1677)
+                oprot.writeString(viter1678)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -38611,19 +38675,19 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.MAP:
                     self.part_vals = {}
-                    (_ktype1673, _vtype1674, _size1672) = iprot.readMapBegin()
-                    for _i1676 in range(_size1672):
-                        _key1677 = iprot.readString()
-                        _val1678 = iprot.readString()
-                        self.part_vals[_key1677] = _val1678
+                    (_ktype1680, _vtype1681, _size1679) = iprot.readMapBegin()
+                    for _i1683 in range(_size1679):
+                        _key1684 = iprot.readString()
+                        _val1685 = iprot.readString()
+                        self.part_vals[_key1684] = _val1685
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I32:
                     self.eventType = iprot.readI32()
                 else:
@@ -38645,17 +38709,17 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.MAP, 3)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.part_vals))
-            for kiter1679, viter1680 in self.part_vals.items():
-                oprot.writeString(kiter1679)
-                oprot.writeString(viter1680)
+            for kiter1686, viter1687 in self.part_vals.items():
+                oprot.writeString(kiter1686)
+                oprot.writeString(viter1687)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.eventType is not None:
             oprot.writeFieldBegin('eventType', TType.I32, 4)
             oprot.writeI32(self.eventType)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -38841,19 +38905,19 @@
                 if ftype == TType.STRING:
                     self.tbl_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.MAP:
                     self.part_vals = {}
-                    (_ktype1682, _vtype1683, _size1681) = iprot.readMapBegin()
-                    for _i1685 in range(_size1681):
-                        _key1686 = iprot.readString()
-                        _val1687 = iprot.readString()
-                        self.part_vals[_key1686] = _val1687
+                    (_ktype1689, _vtype1690, _size1688) = iprot.readMapBegin()
+                    for _i1692 in range(_size1688):
+                        _key1693 = iprot.readString()
+                        _val1694 = iprot.readString()
+                        self.part_vals[_key1693] = _val1694
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I32:
                     self.eventType = iprot.readI32()
                 else:
@@ -38875,17 +38939,17 @@
         if self.tbl_name is not None:
             oprot.writeFieldBegin('tbl_name', TType.STRING, 2)
             oprot.writeString(self.tbl_name)
             oprot.writeFieldEnd()
         if self.part_vals is not None:
             oprot.writeFieldBegin('part_vals', TType.MAP, 3)
             oprot.writeMapBegin(TType.STRING, TType.STRING, len(self.part_vals))
-            for kiter1688, viter1689 in self.part_vals.items():
-                oprot.writeString(kiter1688)
-                oprot.writeString(viter1689)
+            for kiter1695, viter1696 in self.part_vals.items():
+                oprot.writeString(kiter1695)
+                oprot.writeString(viter1696)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.eventType is not None:
             oprot.writeFieldBegin('eventType', TType.I32, 4)
             oprot.writeI32(self.eventType)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -42919,18 +42983,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1693, _size1690) = iprot.readListBegin()
-                    for _i1694 in range(_size1690):
-                        _elem1695 = iprot.readString()
-                        self.success.append(_elem1695)
+                    (_etype1700, _size1697) = iprot.readListBegin()
+                    for _i1701 in range(_size1697):
+                        _elem1702 = iprot.readString()
+                        self.success.append(_elem1702)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -42944,16 +43008,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_functions_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1696 in self.success:
-                oprot.writeString(iter1696)
+            for iter1703 in self.success:
+                oprot.writeString(iter1703)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -43591,18 +43655,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1700, _size1697) = iprot.readListBegin()
-                    for _i1701 in range(_size1697):
-                        _elem1702 = iprot.readString()
-                        self.success.append(_elem1702)
+                    (_etype1707, _size1704) = iprot.readListBegin()
+                    for _i1708 in range(_size1704):
+                        _elem1709 = iprot.readString()
+                        self.success.append(_elem1709)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -43616,16 +43680,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_role_names_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1703 in self.success:
-                oprot.writeString(iter1703)
+            for iter1710 in self.success:
+                oprot.writeString(iter1710)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -44100,19 +44164,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1707, _size1704) = iprot.readListBegin()
-                    for _i1708 in range(_size1704):
-                        _elem1709 = Role()
-                        _elem1709.read(iprot)
-                        self.success.append(_elem1709)
+                    (_etype1714, _size1711) = iprot.readListBegin()
+                    for _i1715 in range(_size1711):
+                        _elem1716 = Role()
+                        _elem1716.read(iprot)
+                        self.success.append(_elem1716)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -44126,16 +44190,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('list_roles_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1710 in self.success:
-                iter1710.write(oprot)
+            for iter1717 in self.success:
+                iter1717.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -44606,18 +44670,18 @@
                 if ftype == TType.STRING:
                     self.user_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.group_names = []
-                    (_etype1714, _size1711) = iprot.readListBegin()
-                    for _i1715 in range(_size1711):
-                        _elem1716 = iprot.readString()
-                        self.group_names.append(_elem1716)
+                    (_etype1721, _size1718) = iprot.readListBegin()
+                    for _i1722 in range(_size1718):
+                        _elem1723 = iprot.readString()
+                        self.group_names.append(_elem1723)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -44634,16 +44698,16 @@
         if self.user_name is not None:
             oprot.writeFieldBegin('user_name', TType.STRING, 2)
             oprot.writeString(self.user_name)
             oprot.writeFieldEnd()
         if self.group_names is not None:
             oprot.writeFieldBegin('group_names', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.group_names))
-            for iter1717 in self.group_names:
-                oprot.writeString(iter1717)
+            for iter1724 in self.group_names:
+                oprot.writeString(iter1724)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -44849,19 +44913,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1721, _size1718) = iprot.readListBegin()
-                    for _i1722 in range(_size1718):
-                        _elem1723 = HiveObjectPrivilege()
-                        _elem1723.read(iprot)
-                        self.success.append(_elem1723)
+                    (_etype1728, _size1725) = iprot.readListBegin()
+                    for _i1729 in range(_size1725):
+                        _elem1730 = HiveObjectPrivilege()
+                        _elem1730.read(iprot)
+                        self.success.append(_elem1730)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -44875,16 +44939,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('list_privileges_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1724 in self.success:
-                iter1724.write(oprot)
+            for iter1731 in self.success:
+                iter1731.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -45507,18 +45571,18 @@
                 if ftype == TType.STRING:
                     self.user_name = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.group_names = []
-                    (_etype1728, _size1725) = iprot.readListBegin()
-                    for _i1729 in range(_size1725):
-                        _elem1730 = iprot.readString()
-                        self.group_names.append(_elem1730)
+                    (_etype1735, _size1732) = iprot.readListBegin()
+                    for _i1736 in range(_size1732):
+                        _elem1737 = iprot.readString()
+                        self.group_names.append(_elem1737)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -45531,16 +45595,16 @@
         if self.user_name is not None:
             oprot.writeFieldBegin('user_name', TType.STRING, 1)
             oprot.writeString(self.user_name)
             oprot.writeFieldEnd()
         if self.group_names is not None:
             oprot.writeFieldBegin('group_names', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.group_names))
-            for iter1731 in self.group_names:
-                oprot.writeString(iter1731)
+            for iter1738 in self.group_names:
+                oprot.writeString(iter1738)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -45584,18 +45648,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1735, _size1732) = iprot.readListBegin()
-                    for _i1736 in range(_size1732):
-                        _elem1737 = iprot.readString()
-                        self.success.append(_elem1737)
+                    (_etype1742, _size1739) = iprot.readListBegin()
+                    for _i1743 in range(_size1739):
+                        _elem1744 = iprot.readString()
+                        self.success.append(_elem1744)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -45609,16 +45673,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('set_ugi_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1738 in self.success:
-                oprot.writeString(iter1738)
+            for iter1745 in self.success:
+                oprot.writeString(iter1745)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -46493,18 +46557,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1742, _size1739) = iprot.readListBegin()
-                    for _i1743 in range(_size1739):
-                        _elem1744 = iprot.readString()
-                        self.success.append(_elem1744)
+                    (_etype1749, _size1746) = iprot.readListBegin()
+                    for _i1750 in range(_size1746):
+                        _elem1751 = iprot.readString()
+                        self.success.append(_elem1751)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -46513,16 +46577,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_all_token_identifiers_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1745 in self.success:
-                oprot.writeString(iter1745)
+            for iter1752 in self.success:
+                oprot.writeString(iter1752)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -47011,18 +47075,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1749, _size1746) = iprot.readListBegin()
-                    for _i1750 in range(_size1746):
-                        _elem1751 = iprot.readString()
-                        self.success.append(_elem1751)
+                    (_etype1756, _size1753) = iprot.readListBegin()
+                    for _i1757 in range(_size1753):
+                        _elem1758 = iprot.readString()
+                        self.success.append(_elem1758)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -47031,16 +47095,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_master_keys_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1752 in self.success:
-                oprot.writeString(iter1752)
+            for iter1759 in self.success:
+                oprot.writeString(iter1759)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -50693,18 +50757,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1756, _size1753) = iprot.readListBegin()
-                    for _i1757 in range(_size1753):
-                        _elem1758 = iprot.readString()
-                        self.success.append(_elem1758)
+                    (_etype1763, _size1760) = iprot.readListBegin()
+                    for _i1764 in range(_size1760):
+                        _elem1765 = iprot.readString()
+                        self.success.append(_elem1765)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -50713,16 +50777,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('find_columns_with_stats_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1759 in self.success:
-                oprot.writeString(iter1759)
+            for iter1766 in self.success:
+                oprot.writeString(iter1766)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -52433,14 +52497,139 @@
         return not (self == other)
 all_structs.append(add_write_notification_log_result)
 add_write_notification_log_result.thrift_spec = (
     (0, TType.STRUCT, 'success', [WriteNotificationLogResponse, None], None, ),  # 0
 )
 
 
+class add_write_notification_log_in_batch_args(object):
+    """
+    Attributes:
+     - rqst
+
+    """
+
+
+    def __init__(self, rqst=None,):
+        self.rqst = rqst
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRUCT:
+                    self.rqst = WriteNotificationLogBatchRequest()
+                    self.rqst.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('add_write_notification_log_in_batch_args')
+        if self.rqst is not None:
+            oprot.writeFieldBegin('rqst', TType.STRUCT, 1)
+            self.rqst.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(add_write_notification_log_in_batch_args)
+add_write_notification_log_in_batch_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRUCT, 'rqst', [WriteNotificationLogBatchRequest, None], None, ),  # 1
+)
+
+
+class add_write_notification_log_in_batch_result(object):
+    """
+    Attributes:
+     - success
+
+    """
+
+
+    def __init__(self, success=None,):
+        self.success = success
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.STRUCT:
+                    self.success = WriteNotificationLogBatchResponse()
+                    self.success.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('add_write_notification_log_in_batch_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.STRUCT, 0)
+            self.success.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(add_write_notification_log_in_batch_result)
+add_write_notification_log_in_batch_result.thrift_spec = (
+    (0, TType.STRUCT, 'success', [WriteNotificationLogBatchResponse, None], None, ),  # 0
+)
+
+
 class cm_recycle_args(object):
     """
     Attributes:
      - request
 
     """
 
@@ -57145,19 +57334,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1763, _size1760) = iprot.readListBegin()
-                    for _i1764 in range(_size1760):
-                        _elem1765 = SchemaVersion()
-                        _elem1765.read(iprot)
-                        self.success.append(_elem1765)
+                    (_etype1770, _size1767) = iprot.readListBegin()
+                    for _i1771 in range(_size1767):
+                        _elem1772 = SchemaVersion()
+                        _elem1772.read(iprot)
+                        self.success.append(_elem1772)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = NoSuchObjectException.read(iprot)
                 else:
@@ -57176,16 +57365,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_schema_all_versions_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1766 in self.success:
-                iter1766.write(oprot)
+            for iter1773 in self.success:
+                iter1773.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         if self.o2 is not None:
@@ -58566,19 +58755,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1770, _size1767) = iprot.readListBegin()
-                    for _i1771 in range(_size1767):
-                        _elem1772 = RuntimeStat()
-                        _elem1772.read(iprot)
-                        self.success.append(_elem1772)
+                    (_etype1777, _size1774) = iprot.readListBegin()
+                    for _i1778 in range(_size1774):
+                        _elem1779 = RuntimeStat()
+                        _elem1779.read(iprot)
+                        self.success.append(_elem1779)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -58592,16 +58781,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_runtime_stats_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1773 in self.success:
-                iter1773.write(oprot)
+            for iter1780 in self.success:
+                iter1780.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -60230,18 +60419,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1777, _size1774) = iprot.readListBegin()
-                    for _i1778 in range(_size1774):
-                        _elem1779 = iprot.readString()
-                        self.success.append(_elem1779)
+                    (_etype1784, _size1781) = iprot.readListBegin()
+                    for _i1785 in range(_size1781):
+                        _elem1786 = iprot.readString()
+                        self.success.append(_elem1786)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -60255,16 +60444,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_all_stored_procedures_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1780 in self.success:
-                oprot.writeString(iter1780)
+            for iter1787 in self.success:
+                oprot.writeString(iter1787)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -60648,18 +60837,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1784, _size1781) = iprot.readListBegin()
-                    for _i1785 in range(_size1781):
-                        _elem1786 = iprot.readString()
-                        self.success.append(_elem1786)
+                    (_etype1791, _size1788) = iprot.readListBegin()
+                    for _i1792 in range(_size1788):
+                        _elem1793 = iprot.readString()
+                        self.success.append(_elem1793)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -60673,16 +60862,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_all_packages_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter1787 in self.success:
-                oprot.writeString(iter1787)
+            for iter1794 in self.success:
+                oprot.writeString(iter1794)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -60917,19 +61106,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype1791, _size1788) = iprot.readListBegin()
-                    for _i1792 in range(_size1788):
-                        _elem1793 = WriteEventInfo()
-                        _elem1793.read(iprot)
-                        self.success.append(_elem1793)
+                    (_etype1798, _size1795) = iprot.readListBegin()
+                    for _i1799 in range(_size1795):
+                        _elem1800 = WriteEventInfo()
+                        _elem1800.read(iprot)
+                        self.success.append(_elem1800)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.o1 = MetaException.read(iprot)
                 else:
@@ -60943,16 +61132,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('get_all_write_event_info_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter1794 in self.success:
-                iter1794.write(oprot)
+            for iter1801 in self.success:
+                iter1801.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.o1 is not None:
             oprot.writeFieldBegin('o1', TType.STRUCT, 1)
             self.o1.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
```

### Comparing `impala_shell-4.3.0a2/impala_shell/impala_shell.py` & `impala_shell-4.3.0a3/impala_shell/impala_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 import traceback
 
 from impala_client import ImpalaHS2Client, StrictHS2Client, \
     ImpalaBeeswaxClient, QueryOptionLevels
 from impala_shell_config_defaults import impala_shell_defaults
 from option_parser import get_option_parser, get_config_from_file
 from shell_output import (DelimitedOutputFormatter, OutputStream, PrettyOutputFormatter,
-                          OverwritingStdErrOutputStream, VerticalOutputFormatter)
+                          OverwritingStdErrOutputStream, VerticalOutputFormatter,
+                          match_string_type)
 from subprocess import call
 from shell_exceptions import (RPCException, DisconnectedException, QueryStateException,
     QueryCancelledByShellException, MissingThriftMethodException)
 
 from value_converter import HS2ValueConverter
 
 
@@ -186,22 +187,25 @@
     self.kerberos_host_fqdn = options.kerberos_host_fqdn
     self.use_kerberos = options.use_kerberos
     self.kerberos_service_name = options.kerberos_service_name
     self.use_ssl = options.ssl
     self.ca_cert = options.ca_cert
     self.user = options.user
     self.ldap_password_cmd = options.ldap_password_cmd
+    self.jwt_cmd = options.jwt_cmd
     self.strict_hs2_protocol = options.strict_hs2_protocol
     self.ldap_password = options.ldap_password
+    self.use_jwt = options.use_jwt
+    self.jwt = options.jwt
     # When running tests in strict mode, the server uses the ldap
     # protocol but can allow any password.
     if options.use_ldap_test_password:
       self.ldap_password = 'password'
     self.use_ldap = options.use_ldap or \
-        (self.strict_hs2_protocol and not self.use_kerberos)
+        (self.strict_hs2_protocol and not self.use_kerberos and not self.use_jwt)
     self.client_connect_timeout_ms = options.client_connect_timeout_ms
     self.http_socket_timeout_s = None
     if (options.http_socket_timeout_s != 'None' and
           options.http_socket_timeout_s is not None):
         self.http_socket_timeout_s = float(options.http_socket_timeout_s)
     self.connect_max_tries = options.connect_max_tries
     self.verbose = options.verbose
@@ -618,15 +622,16 @@
         return StrictHS2Client(self.impalad, self.fetch_size, self.kerberos_host_fqdn,
                           self.use_kerberos, self.kerberos_service_name, self.use_ssl,
                           self.ca_cert, self.user, self.ldap_password, self.use_ldap,
                           self.client_connect_timeout_ms, self.verbose,
                           use_http_base_transport=True, http_path=self.http_path,
                           http_cookie_names=self.http_cookie_names,
                           value_converter=value_converter, rpc_stdout=self.rpc_stdout,
-                          rpc_file=self.rpc_file, http_tracing=self.http_tracing)
+                          rpc_file=self.rpc_file, http_tracing=self.http_tracing,
+                          jwt=self.jwt)
     if protocol == 'hs2':
       return ImpalaHS2Client(self.impalad, self.fetch_size, self.kerberos_host_fqdn,
                           self.use_kerberos, self.kerberos_service_name, self.use_ssl,
                           self.ca_cert, self.user, self.ldap_password, self.use_ldap,
                           self.client_connect_timeout_ms, self.verbose,
                           use_http_base_transport=False, http_path=self.http_path,
                           http_cookie_names=None, value_converter=value_converter,
@@ -639,15 +644,15 @@
                           self.client_connect_timeout_ms, self.verbose,
                           use_http_base_transport=True, http_path=self.http_path,
                           http_cookie_names=self.http_cookie_names,
                           http_socket_timeout_s=self.http_socket_timeout_s,
                           value_converter=value_converter,
                           connect_max_tries=self.connect_max_tries,
                           rpc_stdout=self.rpc_stdout, rpc_file=self.rpc_file,
-                          http_tracing=self.http_tracing)
+                          http_tracing=self.http_tracing, jwt=self.jwt)
     elif protocol == 'beeswax':
       return ImpalaBeeswaxClient(self.impalad, self.fetch_size, self.kerberos_host_fqdn,
                           self.use_kerberos, self.kerberos_service_name, self.use_ssl,
                           self.ca_cert, self.user, self.ldap_password, self.use_ldap,
                           self.client_connect_timeout_ms, self.verbose)
     else:
       err_msg = "Invalid --protocol value {0}, must be beeswax, hs2 or hs2-http."
@@ -785,15 +790,15 @@
       if display_mode is None:
         return CmdStatus.ERROR
 
     try:
       summary, failed_summary = self.imp_client.get_summary(self.last_query_handle)
     except RPCException as e:
       import re
-      error_pattern = re.compile("ERROR: Query id \d+:\d+ not found.")
+      error_pattern = re.compile("ERROR: Query id [a-f0-9]+:[a-f0-9]+ not found.")
       if error_pattern.match(e.value):
         print("Could not retrieve summary for query.", file=sys.stderr)
       else:
         print(e, file=sys.stderr)
       return CmdStatus.ERROR
     if summary.nodes is None:
       print("Summary not available", file=sys.stderr)
@@ -804,25 +809,29 @@
       self.print_exec_summary(summary)
       if failed_summary:
         print("Failed Query Summary:")
         self.print_exec_summary(failed_summary)
     elif display_mode == QueryAttemptDisplayModes.LATEST:
       self.print_exec_summary(summary)
     elif display_mode == QueryAttemptDisplayModes.ORIGINAL:
-      self.print_exec_summary(failed_summary)
+      if failed_summary:
+        self.print_exec_summary(failed_summary)
+      else:
+        print("No failed summary found")
     else:
       raise FatalShellException("Invalid value for query summary display mode")
 
   @staticmethod
   def get_query_attempt_display_mode(arg_mode):
     arg_mode = str(arg_mode).lower()
     if arg_mode not in [QueryAttemptDisplayModes.ALL,
         QueryAttemptDisplayModes.LATEST, QueryAttemptDisplayModes.ORIGINAL]:
       print("Invalid value for query attempt display mode: \'" +
           arg_mode + "\'. Valid values are [ALL | LATEST | ORIGINAL]")
+      return None
     return arg_mode
 
   def print_exec_summary(self, summary):
     output = []
     table = self._default_summary_table()
     self.imp_client.build_summary_table(summary, 0, False, 0, False, output)
     formatter = PrettyOutputFormatter(table)
@@ -943,14 +952,17 @@
 
     """
     # Assume the user wants to connect to the local impalad if no connection string is
     # specified. Connecting to a kerberized impalad requires an fqdn as the host name.
     if self.use_ldap and self.ldap_password is None:
       self.ldap_password = getpass.getpass("LDAP password for %s: " % self.user)
 
+    if self.use_jwt and self.jwt is None:
+      self.jwt = getpass.getpass("Enter JWT: ")
+
     if not args: args = socket.getfqdn()
     tokens = args.split(" ")
     # validate the connection string.
     host_port = [val for val in tokens[0].split(':') if val.strip()]
     protocol = options.protocol.lower()
     if (':' in tokens[0] and len(host_port) != 2):
       print("Connection string must either be empty, or of the form "
@@ -987,14 +999,16 @@
       try:
         if call(["klist", "-s"]) == 0:
           print("Kerberos ticket found in the credentials cache, retrying "
                 "the connection with a secure transport.", file=sys.stderr)
           self.use_kerberos = True
           self.use_ldap = False
           self.ldap_password = None
+          self.use_jwt = False
+          self.jwt = None
           self.imp_client = self._new_impala_client()
           self._connect()
       except OSError:
         pass
 
     if self.imp_client.connected:
       self._print_if_verbose('Connected to %s:%s' % self.impalad)
@@ -1121,19 +1135,21 @@
         profile_display_mode=QueryAttemptDisplayModes.LATEST, status=False):
     """Prints the given runtime profiles to the console. Optionally prints the failed
     profile if the query was retried. The format the profiles are printed is controlled
     by the option profile_display_mode, see QueryProfileDisplayModes docs above.
     """
     if self.show_profiles or status:
       if profile:
-        query_profile_prefix = "Query Runtime Profile:\n"
+        query_profile_prefix = match_string_type("Query Runtime Profile:\n", profile)
         if profile_display_mode == QueryAttemptDisplayModes.ALL:
           print(query_profile_prefix + profile)
           if failed_profile:
-            print("Failed Query Runtime Profile(s):\n" + failed_profile)
+            failed_profile_prefix = \
+                match_string_type("Failed Query Runtime Profile(s):\n", failed_profile)
+            print(failed_profile_prefix + failed_profile)
         elif profile_display_mode == QueryAttemptDisplayModes.LATEST:
           print(query_profile_prefix + profile)
         elif profile_display_mode == QueryAttemptDisplayModes.ORIGINAL:
           print(query_profile_prefix + failed_profile if failed_profile else profile)
         else:
           raise FatalShellException("Invalid value for query profile display mode")
 
@@ -1780,15 +1796,15 @@
 all the performance and diagnostic information that Impala gathered for that query. Be \
 warned, it can be very long!",
   "To see more tips, run the TIP command.",
   "Every command must be terminated by a ';'.",
   "Want to know what version of Impala you're connected to? Run the VERSION command to \
 find out!",
   "You can change the Impala daemon that you're connected to by using the CONNECT \
-command."
+command.",
   "To see how Impala will plan to run your query without actually executing it, use the \
 EXPLAIN command. You can change the level of detail in the EXPLAIN output by setting the \
 EXPLAIN_LEVEL query option.",
   "When you set a query option it lasts for the duration of the Impala shell session."
 ]
 
 HEADER_DIVIDER =\
@@ -1934,14 +1950,18 @@
 
   intro = WELCOME_STRING
 
   if not options.ssl and options.creds_ok_in_clear and options.use_ldap:
     intro += ("\n\nLDAP authentication is enabled, but the connection to Impala is "
               "not secured by TLS.\nALL PASSWORDS WILL BE SENT IN THE CLEAR TO IMPALA.")
 
+  if not options.ssl and options.creds_ok_in_clear and options.use_jwt:
+    intro += ("\n\nJWT authentication is enabled, but the connection to Impala is "
+              "not secured by TLS.\nALL JWTs WILL BE SENT IN THE CLEAR TO IMPALA.")
+
   if options.protocol == 'beeswax':
     intro += ("\n\nWARNING: The beeswax protocol is deprecated and will be removed in a "
               "future version of Impala.")
     if options.hs2_fp_format:
       intro += ("\n\nWARNING: Formatting floating-point values is "
                 "not supported with Beeswax protocol")
 
@@ -1954,14 +1974,39 @@
     format_str.format(float())
   except UnicodeDecodeError as e:
     raise e
   except (ValueError, TypeError) as e:
     raise FatalShellException(e)
 
 
+def read_password_cmd(password_cmd, auth_method_desc, strip_newline=False):
+  try:
+    p = subprocess.Popen(shlex.split(password_cmd), stdout=subprocess.PIPE,
+                         stderr=subprocess.PIPE)
+    password, stderr = p.communicate()
+
+    if p.returncode != 0:
+      print("Error retrieving %s (command was '%s', error was: "
+            "'%s')" % (auth_method_desc, password_cmd, stderr.strip()), file=sys.stderr)
+      raise FatalShellException()
+
+    if sys.version_info.major > 2:
+      # Ensure we can manipulate the password as a string later.
+      password = password.decode('utf-8')
+
+    if strip_newline:
+      password = password.rstrip('\r\n')
+
+    return password
+  except Exception as e:
+    print("Error retrieving %s (command was: '%s', exception "
+          "was: '%s')" % (auth_method_desc, password_cmd, e), file=sys.stderr)
+    raise FatalShellException()
+
+
 
 def impala_shell_main():
   """
   There are two types of options: shell options and query_options. Both can be set on the
   command line, which override default options. Specifically, if there exists a global
   config file (default path: /etc/impalarc) then options are loaded from that file. If
   there exists a user config file (~/.impalarc), then options are loaded in from that
@@ -2041,30 +2086,59 @@
       delim_sequence = options.output_delimiter
     delim = delim_sequence.decode('unicode_escape')
     if len(delim) != 1:
       print("Illegal delimiter %s, the delimiter "
             "must be a 1-character string." % delim, file=sys.stderr)
       raise FatalShellException()
 
-  if options.use_kerberos and options.use_ldap:
-    print("Please specify at most one authentication mechanism (-k or -l)",
+  auth_method_count = 0
+  if options.use_kerberos:
+    auth_method_count += 1
+
+  if options.use_ldap:
+    auth_method_count += 1
+
+  if options.use_jwt:
+    auth_method_count += 1
+
+  if auth_method_count > 1:
+    print("Please specify at most one authentication mechanism (-k, -l, or -j)",
           file=sys.stderr)
     raise FatalShellException()
 
   if not options.ssl and not options.creds_ok_in_clear and options.use_ldap:
     print("LDAP credentials may not be sent over insecure " +
           "connections. Enable SSL or set --auth_creds_ok_in_clear",
           file=sys.stderr)
     raise FatalShellException()
 
   if not options.use_ldap and options.ldap_password_cmd:
     print("Option --ldap_password_cmd requires using LDAP authentication " +
           "mechanism (-l)", file=sys.stderr)
     raise FatalShellException()
 
+  if options.use_jwt and options.protocol.lower() != 'hs2-http':
+    print("Invalid protocol '{0}'. JWT authentication requires using the 'hs2-http' "
+          "protocol".format(options.protocol), file=sys.stderr)
+    raise FatalShellException()
+
+  if options.use_jwt and options.strict_hs2_protocol:
+    print("JWT authentication is not supported when using strict hs2.", file=sys.stderr)
+    raise FatalShellException()
+
+  if options.use_jwt and not options.ssl and not options.creds_ok_in_clear:
+    print("JWTs may not be sent over insecure connections. Enable SSL or "
+          "set --auth_creds_ok_in_clear", file=sys.stderr)
+    raise FatalShellException()
+
+  if not options.use_jwt and options.jwt_cmd:
+    print("Option --jwt_cmd requires using JWT authentication mechanism (-j)",
+          file=sys.stderr)
+    raise FatalShellException()
+
   if options.hs2_fp_format:
     try:
       _validate_hs2_fp_format_specification(options.hs2_fp_format)
     except FatalShellException as e:
       print("Invalid floating point format specification: %s" %
             options.hs2_fp_format, file=sys.stderr)
       raise e
@@ -2092,46 +2166,48 @@
     except OSError as e:
       print('klist not found on the system, install kerberos clients', file=sys.stderr)
       raise FatalShellException()
   elif options.use_ldap:
     if options.verbose:
       ldap_msg = "with LDAP-based authentication"
       print("{0} {1} {2}".format(start_msg, ldap_msg, py_version_msg), file=sys.stderr)
+  elif options.use_jwt:
+    if options.verbose:
+      ldap_msg = "with JWT-based authentication"
+      print("{0} {1} {2}".format(start_msg, ldap_msg, py_version_msg), file=sys.stderr)
   else:
     if options.verbose:
       no_auth_msg = "with no authentication"
       print("{0} {1} {2}".format(start_msg, no_auth_msg, py_version_msg), file=sys.stderr)
 
   options.ldap_password = None
   if options.use_ldap and options.ldap_password_cmd:
-    try:
-      p = subprocess.Popen(shlex.split(options.ldap_password_cmd), stdout=subprocess.PIPE,
-                           stderr=subprocess.PIPE)
-      options.ldap_password, stderr = p.communicate()
-      if p.returncode != 0:
-        print("Error retrieving LDAP password (command was '%s', error was: "
-              "'%s')" % (options.ldap_password_cmd, stderr.strip()), file=sys.stderr)
-        raise FatalShellException()
-      if sys.version_info.major > 2:
-        # Ensure we can manipulate the password as a string later.
-        options.ldap_password = options.ldap_password.decode('utf-8')
-    except Exception as e:
-      print("Error retrieving LDAP password (command was: '%s', exception "
-            "was: '%s')" % (options.ldap_password_cmd, e), file=sys.stderr)
-      raise FatalShellException()
+    options.ldap_password = read_password_cmd(options.ldap_password_cmd, "LDAP password")
+
+  options.jwt = None
+  if options.use_jwt and options.jwt_cmd:
+    options.jwt = read_password_cmd(options.jwt_cmd, "JWT", True)
 
   if options.ssl:
     if options.ca_cert is None:
       if options.verbose:
         print("SSL is enabled. Impala server certificates will NOT be verified "
               "(set --ca_cert to change)", file=sys.stderr)
     else:
       if options.verbose:
         print("SSL is enabled", file=sys.stderr)
 
+  if options.verbose:
+    try:
+      import thrift.protocol.fastbinary
+    except Exception as e:
+      print("WARNING: Failed to load Thrift's fastbinary module. Thrift's "
+            "BinaryProtocol will not be accelerated, which can reduce performance. "
+            "Error was '{0}'".format(e), file=sys.stderr)
+
   if options.output_file:
     try:
       # Make sure the given file can be opened for writing. This will also clear the file
       # if successful.
       open(options.output_file, 'wb')
     except IOError as e:
       print('Error opening output file for writing: %s' % e, file=sys.stderr)
```

### Comparing `impala_shell-4.3.0a2/impala_shell/BackendGflags/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/BackendGflags/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Frontend/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Frontend/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3718,19 +3718,20 @@
      - timeline
      - user_has_profile_access
      - admin_request
      - profile
      - testcase_data_path
      - remote_submit_time
      - profile_children
+     - request_pool_set_by_frontend
 
     """
 
 
-    def __init__(self, stmt_type=None, query_options=None, query_exec_request=None, catalog_op_request=None, result_set_metadata=None, explain_result=None, load_data_request=None, access_events=None, analysis_warnings=None, set_query_option_request=None, timeline=None, user_has_profile_access=None, admin_request=None, profile=None, testcase_data_path=None, remote_submit_time=None, profile_children=None,):
+    def __init__(self, stmt_type=None, query_options=None, query_exec_request=None, catalog_op_request=None, result_set_metadata=None, explain_result=None, load_data_request=None, access_events=None, analysis_warnings=None, set_query_option_request=None, timeline=None, user_has_profile_access=None, admin_request=None, profile=None, testcase_data_path=None, remote_submit_time=None, profile_children=None, request_pool_set_by_frontend=False,):
         self.stmt_type = stmt_type
         self.query_options = query_options
         self.query_exec_request = query_exec_request
         self.catalog_op_request = catalog_op_request
         self.result_set_metadata = result_set_metadata
         self.explain_result = explain_result
         self.load_data_request = load_data_request
@@ -3740,14 +3741,15 @@
         self.timeline = timeline
         self.user_has_profile_access = user_has_profile_access
         self.admin_request = admin_request
         self.profile = profile
         self.testcase_data_path = testcase_data_path
         self.remote_submit_time = remote_submit_time
         self.profile_children = profile_children
+        self.request_pool_set_by_frontend = request_pool_set_by_frontend
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -3862,14 +3864,19 @@
                     for _i149 in range(_size145):
                         _elem150 = RuntimeProfile.ttypes.TRuntimeProfileNode()
                         _elem150.read(iprot)
                         self.profile_children.append(_elem150)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
+            elif fid == 18:
+                if ftype == TType.BOOL:
+                    self.request_pool_set_by_frontend = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -3949,14 +3956,18 @@
         if self.profile_children is not None:
             oprot.writeFieldBegin('profile_children', TType.LIST, 17)
             oprot.writeListBegin(TType.STRUCT, len(self.profile_children))
             for iter153 in self.profile_children:
                 iter153.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
+        if self.request_pool_set_by_frontend is not None:
+            oprot.writeFieldBegin('request_pool_set_by_frontend', TType.BOOL, 18)
+            oprot.writeBool(self.request_pool_set_by_frontend)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.stmt_type is None:
             raise TProtocolException(message='Required field stmt_type is unset!')
         if self.query_options is None:
@@ -6631,14 +6642,15 @@
     (11, TType.STRUCT, 'timeline', [RuntimeProfile.ttypes.TEventSequence, None], None, ),  # 11
     (12, TType.BOOL, 'user_has_profile_access', None, None, ),  # 12
     (13, TType.STRUCT, 'admin_request', [TAdminRequest, None], None, ),  # 13
     (14, TType.STRUCT, 'profile', [RuntimeProfile.ttypes.TRuntimeProfileNode, None], None, ),  # 14
     (15, TType.STRING, 'testcase_data_path', None, None, ),  # 15
     (16, TType.I64, 'remote_submit_time', None, None, ),  # 16
     (17, TType.LIST, 'profile_children', (TType.STRUCT, [RuntimeProfile.ttypes.TRuntimeProfileNode, None], False), None, ),  # 17
+    (18, TType.BOOL, 'request_pool_set_by_frontend', None, False, ),  # 18
 )
 all_structs.append(TCacheJarParams)
 TCacheJarParams.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'hdfs_location', None, None, ),  # 1
 )
 all_structs.append(TCacheJarResult)
```

### Comparing `impala_shell-4.3.0a2/impala_shell/Zip/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Zip/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/TCLIService/constants.py` & `impala_shell-4.3.0a3/impala_shell/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/TCLIService/TCLIService.py` & `impala_shell-4.3.0a3/impala_shell/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/TCLIService/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/PlanNodes/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/PlanNodes/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1249,33 +1249,33 @@
      - replica_preference
      - random_replica
      - skip_header_line_count
      - use_mt_scan_node
      - stats_conjuncts
      - stats_tuple_id
      - dictionary_filter_conjuncts
-     - count_star_slot_offset
+     - parquet_count_star_slot_offset
      - is_partition_key_scan
      - file_formats
      - overlap_predicate_descs
 
     """
 
 
-    def __init__(self, tuple_id=None, collection_conjuncts=None, replica_preference=None, random_replica=None, skip_header_line_count=None, use_mt_scan_node=None, stats_conjuncts=None, stats_tuple_id=None, dictionary_filter_conjuncts=None, count_star_slot_offset=None, is_partition_key_scan=None, file_formats=None, overlap_predicate_descs=None,):
+    def __init__(self, tuple_id=None, collection_conjuncts=None, replica_preference=None, random_replica=None, skip_header_line_count=None, use_mt_scan_node=None, stats_conjuncts=None, stats_tuple_id=None, dictionary_filter_conjuncts=None, parquet_count_star_slot_offset=None, is_partition_key_scan=None, file_formats=None, overlap_predicate_descs=None,):
         self.tuple_id = tuple_id
         self.collection_conjuncts = collection_conjuncts
         self.replica_preference = replica_preference
         self.random_replica = random_replica
         self.skip_header_line_count = skip_header_line_count
         self.use_mt_scan_node = use_mt_scan_node
         self.stats_conjuncts = stats_conjuncts
         self.stats_tuple_id = stats_tuple_id
         self.dictionary_filter_conjuncts = dictionary_filter_conjuncts
-        self.count_star_slot_offset = count_star_slot_offset
+        self.parquet_count_star_slot_offset = parquet_count_star_slot_offset
         self.is_partition_key_scan = is_partition_key_scan
         self.file_formats = file_formats
         self.overlap_predicate_descs = overlap_predicate_descs
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
@@ -1357,15 +1357,15 @@
                         iprot.readListEnd()
                         self.dictionary_filter_conjuncts[_key47] = _val48
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 10:
                 if ftype == TType.I32:
-                    self.count_star_slot_offset = iprot.readI32()
+                    self.parquet_count_star_slot_offset = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 11:
                 if ftype == TType.BOOL:
                     self.is_partition_key_scan = iprot.readBool()
                 else:
                     iprot.skip(ftype)
@@ -1449,17 +1449,17 @@
                 oprot.writeI32(kiter71)
                 oprot.writeListBegin(TType.I32, len(viter72))
                 for iter73 in viter72:
                     oprot.writeI32(iter73)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
-        if self.count_star_slot_offset is not None:
-            oprot.writeFieldBegin('count_star_slot_offset', TType.I32, 10)
-            oprot.writeI32(self.count_star_slot_offset)
+        if self.parquet_count_star_slot_offset is not None:
+            oprot.writeFieldBegin('parquet_count_star_slot_offset', TType.I32, 10)
+            oprot.writeI32(self.parquet_count_star_slot_offset)
             oprot.writeFieldEnd()
         if self.is_partition_key_scan is not None:
             oprot.writeFieldBegin('is_partition_key_scan', TType.BOOL, 11)
             oprot.writeBool(self.is_partition_key_scan)
             oprot.writeFieldEnd()
         if self.file_formats is not None:
             oprot.writeFieldBegin('file_formats', TType.SET, 12)
@@ -4182,15 +4182,15 @@
     (3, TType.I32, 'replica_preference', None, None, ),  # 3
     (4, TType.BOOL, 'random_replica', None, None, ),  # 4
     (5, TType.I32, 'skip_header_line_count', None, None, ),  # 5
     (6, TType.BOOL, 'use_mt_scan_node', None, None, ),  # 6
     (7, TType.LIST, 'stats_conjuncts', (TType.STRUCT, [Exprs.ttypes.TExpr, None], False), None, ),  # 7
     (8, TType.I32, 'stats_tuple_id', None, None, ),  # 8
     (9, TType.MAP, 'dictionary_filter_conjuncts', (TType.I32, None, TType.LIST, (TType.I32, None, False), False), None, ),  # 9
-    (10, TType.I32, 'count_star_slot_offset', None, None, ),  # 10
+    (10, TType.I32, 'parquet_count_star_slot_offset', None, None, ),  # 10
     (11, TType.BOOL, 'is_partition_key_scan', None, None, ),  # 11
     (12, TType.SET, 'file_formats', (TType.I32, None, False), None, ),  # 12
     (13, TType.LIST, 'overlap_predicate_descs', (TType.STRUCT, [TOverlapPredicateDesc, None], False), None, ),  # 13
 )
 all_structs.append(TDataSourceScanNode)
 TDataSourceScanNode.thrift_spec = (
     None,  # 0
```

### Comparing `impala_shell-4.3.0a2/impala_shell/JniCatalog/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/JniCatalog/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -5998,20 +5998,22 @@
         return not (self == other)
 
 
 class TEventProcessorMetricsSummaryResponse(object):
     """
     Attributes:
      - summary
+     - error_msg
 
     """
 
 
-    def __init__(self, summary=None,):
+    def __init__(self, summary=None, error_msg=None,):
         self.summary = summary
+        self.error_msg = error_msg
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -6019,28 +6021,37 @@
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.STRING:
                     self.summary = iprot.readString()
                 else:
                     iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.error_msg = iprot.readString()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('TEventProcessorMetricsSummaryResponse')
         if self.summary is not None:
             oprot.writeFieldBegin('summary', TType.STRING, 1)
             oprot.writeString(self.summary)
             oprot.writeFieldEnd()
+        if self.error_msg is not None:
+            oprot.writeFieldBegin('error_msg', TType.STRING, 2)
+            oprot.writeString(self.error_msg)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         if self.summary is None:
             raise TProtocolException(message='Required field summary is unset!')
         return
@@ -6507,10 +6518,11 @@
     None,  # 0
     (1, TType.STRING, 'input_path', None, None, ),  # 1
 )
 all_structs.append(TEventProcessorMetricsSummaryResponse)
 TEventProcessorMetricsSummaryResponse.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'summary', None, None, ),  # 1
+    (2, TType.STRING, 'error_msg', None, None, ),  # 2
 )
 fix_spec(all_structs)
 del all_structs
```

### Comparing `impala_shell-4.3.0a2/impala_shell/ImpalaService/ImpalaHiveServer2Service.py` & `impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaHiveServer2Service.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/ImpalaService/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/ImpalaService/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,15 @@
     DISABLE_CODEGEN_CACHE = 149
     CODEGEN_CACHE_MODE = 150
     STRINGIFY_MAP_KEYS = 151
     ENABLE_TRIVIAL_QUERY_FOR_ADMISSION = 152
     COMPUTE_PROCESSING_COST = 153
     PROCESSING_COST_MIN_THREADS = 154
     JOIN_SELECTIVITY_CORRELATION_FACTOR = 155
+    MAX_FRAGMENT_INSTANCES_PER_NODE = 156
 
     _VALUES_TO_NAMES = {
         0: "ABORT_ON_ERROR",
         1: "MAX_ERRORS",
         2: "DISABLE_CODEGEN",
         3: "BATCH_SIZE",
         4: "MEM_LIMIT",
@@ -335,14 +336,15 @@
         149: "DISABLE_CODEGEN_CACHE",
         150: "CODEGEN_CACHE_MODE",
         151: "STRINGIFY_MAP_KEYS",
         152: "ENABLE_TRIVIAL_QUERY_FOR_ADMISSION",
         153: "COMPUTE_PROCESSING_COST",
         154: "PROCESSING_COST_MIN_THREADS",
         155: "JOIN_SELECTIVITY_CORRELATION_FACTOR",
+        156: "MAX_FRAGMENT_INSTANCES_PER_NODE",
     }
 
     _NAMES_TO_VALUES = {
         "ABORT_ON_ERROR": 0,
         "MAX_ERRORS": 1,
         "DISABLE_CODEGEN": 2,
         "BATCH_SIZE": 3,
@@ -494,14 +496,15 @@
         "DISABLE_CODEGEN_CACHE": 149,
         "CODEGEN_CACHE_MODE": 150,
         "STRINGIFY_MAP_KEYS": 151,
         "ENABLE_TRIVIAL_QUERY_FOR_ADMISSION": 152,
         "COMPUTE_PROCESSING_COST": 153,
         "PROCESSING_COST_MIN_THREADS": 154,
         "JOIN_SELECTIVITY_CORRELATION_FACTOR": 155,
+        "MAX_FRAGMENT_INSTANCES_PER_NODE": 156,
     }
 
 
 class TDmlResult(object):
     """
     Attributes:
      - rows_modified
```

### Comparing `impala_shell-4.3.0a2/impala_shell/ImpalaService/ImpalaService.py` & `impala_shell-4.3.0a3/impala_shell/ImpalaService/ImpalaService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/option_parser.py` & `impala_shell-4.3.0a3/impala_shell/option_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,18 @@
                     action="store_true", help="Continue on query failure")
   parser.add_option("-d", "--database", dest="default_db",
                     help="Issues a use database command on startup \t")
   parser.add_option("-l", "--ldap", dest="use_ldap",
                     action="store_true",
                     help="Use LDAP to authenticate with Impala. Impala must be configured"
                     " to allow LDAP authentication. \t\t")
+  parser.add_option("-j", "--jwt", dest="use_jwt",
+                    action="store_true",
+                    help="Use JWT to authenticate with Impala. Impala must be configured"
+                    " to allow JWT authentication. \t\t")
   parser.add_option("-u", "--user", dest="user",
                     help="User to authenticate with.")
   parser.add_option("--ssl", dest="ssl",
                     action="store_true",
                     help="Connect to Impala via SSL-secured connection \t")
   parser.add_option("--ca_cert", dest="ca_cert",
                     help=("Full path to "
@@ -263,14 +267,16 @@
   parser.add_option("--auth_creds_ok_in_clear", dest="creds_ok_in_clear",
                     action="store_true", help="If set, LDAP authentication " +
                     "may be used with an insecure connection to Impala. " +
                     "WARNING: Authentication credentials will therefore be sent " +
                     "unencrypted, and may be vulnerable to attack.")
   parser.add_option("--ldap_password_cmd", dest="ldap_password_cmd",
                     help="Shell command to run to retrieve the LDAP password")
+  parser.add_option("--jwt_cmd", dest="jwt_cmd",
+                    help="Shell command to run to retrieve the JWT")
   parser.add_option("--var", dest="keyval", action="append",
                     help="Defines a variable to be used within the Impala session."
                          " Can be used multiple times to set different variables."
                          " It must follow the pattern \"KEY=VALUE\","
                          " KEY starts with an alphabetic character and"
                          " contains alphanumeric characters or underscores.")
   parser.add_option("-Q", "--query_option", dest="query_options", action="append",
```

### Comparing `impala_shell-4.3.0a2/impala_shell/Logging/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Logging/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/DataSinks/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/DataSinks/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/MetricDefs/constants.py` & `impala_shell-4.3.0a3/impala_shell/MetricDefs/constants.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/MetricDefs/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/MetricDefs/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/StatestoreService/StatestoreService.py` & `impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/StatestoreService/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/StatestoreService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/StatestoreService/StatestoreSubscriber.py` & `impala_shell-4.3.0a3/impala_shell/StatestoreService/StatestoreSubscriber.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/shell_output.py` & `impala_shell-4.3.0a3/impala_shell/shell_output.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,34 @@
 
 try:
   from cStringIO import StringIO  # python 2
 except ImportError:
   from io import StringIO  # python 3
 
 
+def match_string_type(str_to_convert, reference_str):
+  """ Returns 'str_to_convert' converted to the same type as 'reference_str'.
+      Can handle only str and unicode. NOOP in Python 3.
+  """
+  if sys.version_info.major >= 3:
+    assert isinstance(reference_str, str)
+    assert isinstance(str_to_convert, str)
+    return str_to_convert
+
+  if type(str_to_convert) == type(reference_str):
+    return str_to_convert
+
+  if isinstance(reference_str, str):
+    assert isinstance(str_to_convert, unicode)
+    return str_to_convert.encode('UTF-8')
+  else:
+    assert isinstance(reference_str, str)
+    return str_to_convert.decode('UTF-8')
+
+
 class PrettyOutputFormatter(object):
   def __init__(self, prettytable):
     self.prettytable = prettytable
 
   def format(self, rows):
     """Returns string containing representation of the table data."""
```

### Comparing `impala_shell-4.3.0a2/impala_shell/CatalogObjects/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/CatalogObjects/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/NetworkTest/NetworkTestService.py` & `impala_shell-4.3.0a3/impala_shell/NetworkTest/NetworkTestService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/NetworkTest/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/NetworkTest/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/CatalogService/CatalogService.py` & `impala_shell-4.3.0a3/impala_shell/CatalogService/CatalogService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/CatalogService/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/CatalogService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/parquet/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/parquet/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/__init__.py` & `impala_shell-4.3.0a3/impala_shell/__init__.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/ExecStats/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/ExecStats/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/LineageGraph/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/LineageGraph/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/thrift_printer.py` & `impala_shell-4.3.0a3/impala_shell/thrift_printer.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Planner/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Planner/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/ExternalDataSource/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/ExternalDataSource/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/CatalogInternalService/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/CatalogInternalService/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Types/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Types/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/beeswaxd/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/beeswaxd/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/beeswaxd/BeeswaxService.py` & `impala_shell-4.3.0a3/impala_shell/beeswaxd/BeeswaxService.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/RuntimeProfile/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/RuntimeProfile/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Query/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Query/ttypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,22 +362,23 @@
      - disable_codegen_cache
      - codegen_cache_mode
      - stringify_map_keys
      - enable_trivial_query_for_admission
      - compute_processing_cost
      - processing_cost_min_threads
      - join_selectivity_correlation_factor
+     - max_fragment_instances_per_node
 
     """
 
 
     def __init__(self, abort_on_error=False, max_errors=100, disable_codegen=False, batch_size=0, num_nodes=0, max_scan_range_length=0, num_scanner_threads=0, debug_action="", mem_limit=0, compression_codec=None, hbase_caching=0, hbase_cache_blocks=False, parquet_file_size=0, explain_level=1, sync_ddl=False, request_pool=None, disable_outermost_topn=False, query_timeout_s=0, buffer_pool_limit=None, appx_count_distinct=False, disable_unsafe_spills=False, exec_single_node_rows_threshold=100, optimize_partition_key_scans=False, replica_preference=0, schedule_random_replica=False, disable_streaming_preaggregations=False, runtime_filter_mode=2, runtime_bloom_filter_size=1048576, runtime_filter_wait_time_ms=0, disable_row_runtime_filtering=False, max_num_runtime_filters=10, parquet_annotate_strings_utf8=False, parquet_fallback_schema_resolution=0, mt_dop=None, s3_skip_insert_staging=True, runtime_filter_min_size=1048576, runtime_filter_max_size=16777216, prefetch_mode=1, strict_mode=False, scratch_limit=-1, enable_expr_rewrites=True, decimal_v2=True, parquet_dictionary_filtering=True, parquet_array_resolution=0, parquet_read_statistics=True, default_join_distribution_mode=0, disable_codegen_rows_threshold=50000, default_spillable_buffer_size=2097152, min_spillable_buffer_size=65536, max_row_size=524288, idle_session_timeout=None, compute_stats_min_sample_size=1073741824, exec_time_limit_s=0, shuffle_distinct_exprs=True, max_mem_estimate_for_admission=0, thread_reservation_limit=3000, thread_reservation_aggregate_limit=0, kudu_read_mode=0, allow_erasure_coded_files=True, timezone="", scan_bytes_limit=0, cpu_limit_s=0, topn_bytes_limit=536870912, client_identifier=None, resource_trace_ratio=float(0), num_remote_executor_candidates=3, num_rows_produced_limit=0, planner_testcase_mode=False, default_file_format=0, parquet_timestamp_type=0, parquet_read_page_index=True, parquet_write_page_index=True, parquet_page_row_count_limit=None, disable_hdfs_num_rows_estimate=False, default_hints_insert_statement=None, spool_query_results=True, default_transactional_type=0, statement_expression_limit=250000, max_statement_length_bytes=16777216, disable_data_cache=False, max_result_spooling_mem=104857600, max_spilled_result_spooling_mem=1073741824, disable_hbase_num_rows_estimate=False, fetch_rows_timeout_ms=10000, now_string="", parquet_object_store_split_size=268435456, mem_limit_executors=0, broadcast_bytes_limit=34359738368, preagg_bytes_limit=-1, enable_cnf_rewrites=True, max_cnf_exprs=200, kudu_snapshot_read_timestamp_micros=0, retry_failed_queries=False, enabled_runtime_filter_types=set((
         0,
         1,
-    )), async_codegen=False, enable_distinct_semi_join_optimization=True, sort_run_bytes_limit=-1, max_fs_writers=0, refresh_updated_hms_partitions=False, spool_all_results_for_retries=True, runtime_filter_error_rate=None, use_local_tz_for_unix_timestamp_conversions=False, convert_legacy_hive_parquet_utc_timestamps=False, enable_outer_join_to_inner_transformation=False, targeted_kudu_scan_range_length=-1, report_skew_limit=1.0000000000000000, optimize_simple_limit=False, use_dop_for_costing=True, broadcast_to_partition_factor=1.0000000000000000, join_rows_produced_limit=0, utf8_mode=False, analytic_rank_pushdown_threshold=1000, minmax_filter_threshold=0.0000000000000000, minmax_filtering_level=1, compute_column_minmax_stats=False, show_column_minmax_stats=False, default_ndv_scale=2, kudu_replica_selection=1, delete_stats_in_truncate=True, parquet_bloom_filtering=True, minmax_filter_sorted_columns=True, minmax_filter_fast_code_path=1, enable_kudu_transaction=False, minmax_filter_partition_columns=True, parquet_bloom_filter_write=1, orc_read_statistics=True, enable_async_ddl_execution=True, enable_async_load_data_execution=True, parquet_late_materialization_threshold=20, parquet_dictionary_runtime_filter_entry_limit=1024, abort_java_udf_on_exception=False, orc_async_read=True, runtime_in_list_filter_entry_limit=1024, enable_replan=True, test_replan=False, lock_max_wait_time_s=300, orc_schema_resolution=0, expand_complex_types=False, fallback_db_for_functions=None, disable_codegen_cache=False, codegen_cache_mode=0, stringify_map_keys=False, enable_trivial_query_for_admission=True, compute_processing_cost=False, processing_cost_min_threads=1, join_selectivity_correlation_factor=0.0000000000000000,):
+    )), async_codegen=False, enable_distinct_semi_join_optimization=True, sort_run_bytes_limit=-1, max_fs_writers=0, refresh_updated_hms_partitions=False, spool_all_results_for_retries=True, runtime_filter_error_rate=None, use_local_tz_for_unix_timestamp_conversions=False, convert_legacy_hive_parquet_utc_timestamps=False, enable_outer_join_to_inner_transformation=False, targeted_kudu_scan_range_length=-1, report_skew_limit=1.0000000000000000, optimize_simple_limit=False, use_dop_for_costing=True, broadcast_to_partition_factor=1.0000000000000000, join_rows_produced_limit=0, utf8_mode=False, analytic_rank_pushdown_threshold=1000, minmax_filter_threshold=0.0000000000000000, minmax_filtering_level=1, compute_column_minmax_stats=False, show_column_minmax_stats=False, default_ndv_scale=2, kudu_replica_selection=1, delete_stats_in_truncate=True, parquet_bloom_filtering=True, minmax_filter_sorted_columns=True, minmax_filter_fast_code_path=1, enable_kudu_transaction=False, minmax_filter_partition_columns=True, parquet_bloom_filter_write=1, orc_read_statistics=True, enable_async_ddl_execution=True, enable_async_load_data_execution=True, parquet_late_materialization_threshold=20, parquet_dictionary_runtime_filter_entry_limit=1024, abort_java_udf_on_exception=False, orc_async_read=True, runtime_in_list_filter_entry_limit=1024, enable_replan=True, test_replan=False, lock_max_wait_time_s=300, orc_schema_resolution=0, expand_complex_types=False, fallback_db_for_functions=None, disable_codegen_cache=False, codegen_cache_mode=0, stringify_map_keys=False, enable_trivial_query_for_admission=True, compute_processing_cost=False, processing_cost_min_threads=1, join_selectivity_correlation_factor=0.0000000000000000, max_fragment_instances_per_node=128,):
         self.abort_on_error = abort_on_error
         self.max_errors = max_errors
         self.disable_codegen = disable_codegen
         self.batch_size = batch_size
         self.num_nodes = num_nodes
         self.max_scan_range_length = max_scan_range_length
         self.num_scanner_threads = num_scanner_threads
@@ -521,14 +522,15 @@
         self.disable_codegen_cache = disable_codegen_cache
         self.codegen_cache_mode = codegen_cache_mode
         self.stringify_map_keys = stringify_map_keys
         self.enable_trivial_query_for_admission = enable_trivial_query_for_admission
         self.compute_processing_cost = compute_processing_cost
         self.processing_cost_min_threads = processing_cost_min_threads
         self.join_selectivity_correlation_factor = join_selectivity_correlation_factor
+        self.max_fragment_instances_per_node = max_fragment_instances_per_node
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1267,14 +1269,19 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 156:
                 if ftype == TType.DOUBLE:
                     self.join_selectivity_correlation_factor = iprot.readDouble()
                 else:
                     iprot.skip(ftype)
+            elif fid == 157:
+                if ftype == TType.I32:
+                    self.max_fragment_instances_per_node = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1864,14 +1871,18 @@
             oprot.writeFieldBegin('processing_cost_min_threads', TType.I32, 155)
             oprot.writeI32(self.processing_cost_min_threads)
             oprot.writeFieldEnd()
         if self.join_selectivity_correlation_factor is not None:
             oprot.writeFieldBegin('join_selectivity_correlation_factor', TType.DOUBLE, 156)
             oprot.writeDouble(self.join_selectivity_correlation_factor)
             oprot.writeFieldEnd()
+        if self.max_fragment_instances_per_node is not None:
+            oprot.writeFieldBegin('max_fragment_instances_per_node', TType.I32, 157)
+            oprot.writeI32(self.max_fragment_instances_per_node)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -3176,14 +3187,15 @@
     (150, TType.BOOL, 'disable_codegen_cache', None, False, ),  # 150
     (151, TType.I32, 'codegen_cache_mode', None, 0, ),  # 151
     (152, TType.BOOL, 'stringify_map_keys', None, False, ),  # 152
     (153, TType.BOOL, 'enable_trivial_query_for_admission', None, True, ),  # 153
     (154, TType.BOOL, 'compute_processing_cost', None, False, ),  # 154
     (155, TType.I32, 'processing_cost_min_threads', None, 1, ),  # 155
     (156, TType.DOUBLE, 'join_selectivity_correlation_factor', None, 0.0000000000000000, ),  # 156
+    (157, TType.I32, 'max_fragment_instances_per_node', None, 128, ),  # 157
 )
 all_structs.append(TClientRequest)
 TClientRequest.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'stmt', None, None, ),  # 1
     (2, TType.STRUCT, 'query_options', [TQueryOptions, None], None, ),  # 2
     (3, TType.STRING, 'redacted_stmt', None, None, ),  # 3
```

### Comparing `impala_shell-4.3.0a2/impala_shell/ErrorCodes/constants.py` & `impala_shell-4.3.0a3/impala_shell/ErrorCodes/constants.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/ErrorCodes/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/ErrorCodes/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Data/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Data/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/TSSLSocketWithWildcardSAN.py` & `impala_shell-4.3.0a3/impala_shell/TSSLSocketWithWildcardSAN.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell/Results/ttypes.py` & `impala_shell-4.3.0a3/impala_shell/Results/ttypes.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/impala_shell.egg-info/PKG-INFO` & `impala_shell-4.3.0a3/impala_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impala-shell
-Version: 4.3.0a2
+Version: 4.3.0a3
 Summary: Impala Shell
 Home-page: https://impala.apache.org/
 Author: Impala Dev
 Author-email: dev@impala.apache.org
 License: Apache Software License
 Description: # Impala Interactive Shell
```

### Comparing `impala_shell-4.3.0a2/impala_shell.egg-info/SOURCES.txt` & `impala_shell-4.3.0a3/impala_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/setup.py` & `impala_shell-4.3.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `impala_shell-4.3.0a2/README.md` & `impala_shell-4.3.0a3/README.md`

 * *Files identical despite different names*


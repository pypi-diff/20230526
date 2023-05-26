# Comparing `tmp/vcrpy-4.3.0.tar.gz` & `tmp/vcrpy-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcrpy-4.3.0.tar", last modified: Wed May 24 18:50:19 2023, max compression
+gzip compressed data, was "vcrpy-4.3.1.tar", last modified: Fri May 26 16:04:05 2023, max compression
```

## Comparing `vcrpy-4.3.0.tar` & `vcrpy-4.3.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.886911 vcrpy-4.3.0/
--rw-r--r--   0 kevin      (501) staff       (20)     1063 2022-08-31 19:12:36.000000 vcrpy-4.3.0/LICENSE.txt
--rw-r--r--   0 kevin      (501) staff       (20)      142 2022-08-31 19:12:36.000000 vcrpy-4.3.0/MANIFEST.in
--rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-24 18:50:19.886977 vcrpy-4.3.0/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     2767 2022-08-31 19:12:36.000000 vcrpy-4.3.0/README.rst
--rw-r--r--   0 kevin      (501) staff       (20)      164 2023-05-24 18:36:09.000000 vcrpy-4.3.0/pyproject.toml
--rw-r--r--   0 kevin      (501) staff       (20)       67 2023-05-24 18:50:19.887157 vcrpy-4.3.0/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)     2610 2023-05-24 18:36:09.000000 vcrpy-4.3.0/setup.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.876960 vcrpy-4.3.0/tests/
--rw-r--r--   0 kevin      (501) staff       (20)      354 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/assertions.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.875477 vcrpy-4.3.0/tests/fixtures/
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.877487 vcrpy-4.3.0/tests/fixtures/migration/
--rw-r--r--   0 kevin      (501) staff       (20)     1115 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/new_cassette.json
--rw-r--r--   0 kevin      (501) staff       (20)      599 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/new_cassette.yaml
--rw-r--r--   0 kevin      (501) staff       (20)       23 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/not_cassette.txt
--rw-r--r--   0 kevin      (501) staff       (20)     1031 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/old_cassette.json
--rw-r--r--   0 kevin      (501) staff       (20)      869 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/migration/old_cassette.yaml
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.877589 vcrpy-4.3.0/tests/fixtures/wild/
--rw-r--r--   0 kevin      (501) staff       (20)     9705 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/fixtures/wild/domain_redirect.yaml
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.881018 vcrpy-4.3.0/tests/integration/
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/aiohttp_utils.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.881157 vcrpy-4.3.0/tests/integration/cassettes/
--rw-r--r--   0 kevin      (501) staff       (20)     1017 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
--rw-r--r--   0 kevin      (501) staff       (20)      316 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/conftest.py
--rw-r--r--   0 kevin      (501) staff       (20)    16008 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_aiohttp.py
--rw-r--r--   0 kevin      (501) staff       (20)     2766 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_basic.py
--rw-r--r--   0 kevin      (501) staff       (20)     2951 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_boto.py
--rw-r--r--   0 kevin      (501) staff       (20)     3589 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_boto3.py
--rw-r--r--   0 kevin      (501) staff       (20)     2526 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_config.py
--rw-r--r--   0 kevin      (501) staff       (20)     1563 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_disksaver.py
--rw-r--r--   0 kevin      (501) staff       (20)     5714 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_filter.py
--rw-r--r--   0 kevin      (501) staff       (20)     1030 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_http
--rw-r--r--   0 kevin      (501) staff       (20)     4926 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_httplib2.py
--rw-r--r--   0 kevin      (501) staff       (20)    10415 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_httpx.py
--rw-r--r--   0 kevin      (501) staff       (20)     2621 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_ignore.py
--rw-r--r--   0 kevin      (501) staff       (20)     4000 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)      878 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_multiple.py
--rw-r--r--   0 kevin      (501) staff       (20)     1779 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_proxy.py
--rw-r--r--   0 kevin      (501) staff       (20)     5170 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_record_mode.py
--rw-r--r--   0 kevin      (501) staff       (20)     1167 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_register_matcher.py
--rw-r--r--   0 kevin      (501) staff       (20)     1852 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_register_persister.py
--rw-r--r--   0 kevin      (501) staff       (20)      962 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_register_serializer.py
--rw-r--r--   0 kevin      (501) staff       (20)      739 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_request.py
--rw-r--r--   0 kevin      (501) staff       (20)    11635 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_requests.py
--rw-r--r--   0 kevin      (501) staff       (20)     5040 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)    12599 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_tornado.py
--rw-r--r--   0 kevin      (501) staff       (20)     1387 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_tornado_exception_can_be_caught.yaml
--rw-r--r--   0 kevin      (501) staff       (20)     1566 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml
--rw-r--r--   0 kevin      (501) staff       (20)     5072 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_urllib2.py
--rw-r--r--   0 kevin      (501) staff       (20)     6264 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_urllib3.py
--rw-r--r--   0 kevin      (501) staff       (20)     3429 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/integration/test_wild.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.882800 vcrpy-4.3.0/tests/unit/
--rw-r--r--   0 kevin      (501) staff       (20)    13163 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_cassettes.py
--rw-r--r--   0 kevin      (501) staff       (20)     2669 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/unit/test_errors.py
--rw-r--r--   0 kevin      (501) staff       (20)    11738 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_filters.py
--rw-r--r--   0 kevin      (501) staff       (20)      611 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_json_serializer.py
--rw-r--r--   0 kevin      (501) staff       (20)     9990 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)     1588 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_migration.py
--rw-r--r--   0 kevin      (501) staff       (20)     1067 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/unit/test_persist.py
--rw-r--r--   0 kevin      (501) staff       (20)     2471 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_request.py
--rw-r--r--   0 kevin      (501) staff       (20)     3648 2022-08-31 19:12:36.000000 vcrpy-4.3.0/tests/unit/test_response.py
--rw-r--r--   0 kevin      (501) staff       (20)     4038 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_serialize.py
--rw-r--r--   0 kevin      (501) staff       (20)      798 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)    12080 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_vcr.py
--rw-r--r--   0 kevin      (501) staff       (20)      395 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tests/unit/test_vcr_import.py
--rw-r--r--   0 kevin      (501) staff       (20)     3111 2023-05-24 18:36:09.000000 vcrpy-4.3.0/tox.ini
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.884471 vcrpy-4.3.0/vcr/
--rw-r--r--   0 kevin      (501) staff       (20)      296 2023-05-24 18:48:06.000000 vcrpy-4.3.0/vcr/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      125 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/_handle_coroutine.py
--rw-r--r--   0 kevin      (501) staff       (20)    13892 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/cassette.py
--rw-r--r--   0 kevin      (501) staff       (20)    10830 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/config.py
--rw-r--r--   0 kevin      (501) staff       (20)     1976 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/errors.py
--rw-r--r--   0 kevin      (501) staff       (20)     6651 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/filters.py
--rw-r--r--   0 kevin      (501) staff       (20)     4105 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)     4660 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/migration.py
--rw-r--r--   0 kevin      (501) staff       (20)    17807 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/patch.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.884676 vcrpy-4.3.0/vcr/persisters/
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/persisters/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     1095 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/persisters/filesystem.py
--rw-r--r--   0 kevin      (501) staff       (20)      630 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/record_mode.py
--rw-r--r--   0 kevin      (501) staff       (20)     3782 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/request.py
--rw-r--r--   0 kevin      (501) staff       (20)     2124 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/serialize.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.885112 vcrpy-4.3.0/vcr/serializers/
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/serializers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     2513 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/serializers/compat.py
--rw-r--r--   0 kevin      (501) staff       (20)      778 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/serializers/jsonserializer.py
--rw-r--r--   0 kevin      (501) staff       (20)      363 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/serializers/yamlserializer.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.886204 vcrpy-4.3.0/vcr/stubs/
--rw-r--r--   0 kevin      (501) staff       (20)    12461 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     9954 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/aiohttp_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     1202 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/boto3_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      235 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/boto_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      578 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/compat.py
--rw-r--r--   0 kevin      (501) staff       (20)     2166 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/httplib2_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     5579 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/httpx_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      562 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/requests_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     3407 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/stubs/tornado_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      508 2023-05-24 18:36:09.000000 vcrpy-4.3.0/vcr/stubs/urllib3_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     3882 2022-08-31 19:12:36.000000 vcrpy-4.3.0/vcr/util.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-24 18:50:19.886795 vcrpy-4.3.0/vcrpy.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     2650 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)       27 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)        4 2023-05-24 18:50:19.000000 vcrpy-4.3.0/vcrpy.egg-info/top_level.txt
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.109307 vcrpy-4.3.1/
+-rw-r--r--   0 kevin      (501) staff       (20)     1063 2022-08-31 19:12:36.000000 vcrpy-4.3.1/LICENSE.txt
+-rw-r--r--   0 kevin      (501) staff       (20)      142 2022-08-31 19:12:36.000000 vcrpy-4.3.1/MANIFEST.in
+-rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-26 16:04:05.109377 vcrpy-4.3.1/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     2767 2022-08-31 19:12:36.000000 vcrpy-4.3.1/README.rst
+-rw-r--r--   0 kevin      (501) staff       (20)      164 2023-05-24 18:36:09.000000 vcrpy-4.3.1/pyproject.toml
+-rw-r--r--   0 kevin      (501) staff       (20)       67 2023-05-26 16:04:05.109567 vcrpy-4.3.1/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     3557 2023-05-26 15:56:05.000000 vcrpy-4.3.1/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.097563 vcrpy-4.3.1/tests/
+-rw-r--r--   0 kevin      (501) staff       (20)      354 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/assertions.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.096258 vcrpy-4.3.1/tests/fixtures/
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.098448 vcrpy-4.3.1/tests/fixtures/migration/
+-rw-r--r--   0 kevin      (501) staff       (20)     1115 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/new_cassette.json
+-rw-r--r--   0 kevin      (501) staff       (20)      599 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/new_cassette.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)       23 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/not_cassette.txt
+-rw-r--r--   0 kevin      (501) staff       (20)     1031 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/old_cassette.json
+-rw-r--r--   0 kevin      (501) staff       (20)      869 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/old_cassette.yaml
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.098579 vcrpy-4.3.1/tests/fixtures/wild/
+-rw-r--r--   0 kevin      (501) staff       (20)     9705 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/wild/domain_redirect.yaml
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.103320 vcrpy-4.3.1/tests/integration/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/aiohttp_utils.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.103432 vcrpy-4.3.1/tests/integration/cassettes/
+-rw-r--r--   0 kevin      (501) staff       (20)     1017 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
+-rw-r--r--   0 kevin      (501) staff       (20)      781 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/conftest.py
+-rw-r--r--   0 kevin      (501) staff       (20)    16516 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/test_aiohttp.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2766 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_basic.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2951 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_boto.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3589 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_boto3.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2526 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_config.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1563 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_disksaver.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5714 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_filter.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1030 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_http
+-rw-r--r--   0 kevin      (501) staff       (20)     4926 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_httplib2.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10415 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_httpx.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2621 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_ignore.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4000 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)      878 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_multiple.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1779 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_proxy.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5170 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_record_mode.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1167 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_register_matcher.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1852 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_register_persister.py
+-rw-r--r--   0 kevin      (501) staff       (20)      962 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_register_serializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      739 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_request.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11635 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_requests.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5040 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12599 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_tornado.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1387 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_tornado_exception_can_be_caught.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)     1566 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_tornado_with_decorator_use_cassette.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)     5072 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_urllib2.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6364 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/test_urllib3.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3498 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/test_wild.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.105452 vcrpy-4.3.1/tests/unit/
+-rw-r--r--   0 kevin      (501) staff       (20)    13163 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_cassettes.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2669 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/unit/test_errors.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11738 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_filters.py
+-rw-r--r--   0 kevin      (501) staff       (20)      611 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_json_serializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     9990 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1588 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_migration.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1067 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/unit/test_persist.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2471 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_request.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3648 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/unit/test_response.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4038 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_serialize.py
+-rw-r--r--   0 kevin      (501) staff       (20)      798 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12082 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/unit/test_vcr.py
+-rw-r--r--   0 kevin      (501) staff       (20)      395 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_vcr_import.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3281 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tox.ini
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.107080 vcrpy-4.3.1/vcr/
+-rw-r--r--   0 kevin      (501) staff       (20)      296 2023-05-26 15:56:45.000000 vcrpy-4.3.1/vcr/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      125 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/_handle_coroutine.py
+-rw-r--r--   0 kevin      (501) staff       (20)    13892 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/cassette.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10830 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/config.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1976 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/errors.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6651 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/filters.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4105 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4660 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/migration.py
+-rw-r--r--   0 kevin      (501) staff       (20)    17948 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/patch.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.107272 vcrpy-4.3.1/vcr/persisters/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/persisters/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1095 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/persisters/filesystem.py
+-rw-r--r--   0 kevin      (501) staff       (20)      630 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/record_mode.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3782 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/request.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2124 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/serialize.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.107670 vcrpy-4.3.1/vcr/serializers/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/serializers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2513 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/serializers/compat.py
+-rw-r--r--   0 kevin      (501) staff       (20)      778 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/serializers/jsonserializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      363 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/serializers/yamlserializer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.108691 vcrpy-4.3.1/vcr/stubs/
+-rw-r--r--   0 kevin      (501) staff       (20)    13412 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/stubs/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     9954 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/aiohttp_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1202 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/boto3_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      235 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/boto_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      578 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/compat.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2166 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/httplib2_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5579 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/httpx_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      558 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/stubs/requests_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3407 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/stubs/tornado_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      504 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/stubs/urllib3_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3882 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/util.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.109201 vcrpy-4.3.1/vcrpy.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     2650 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       65 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        4 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/top_level.txt
```

### Comparing `vcrpy-4.3.0/LICENSE.txt` & `vcrpy-4.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/PKG-INFO` & `vcrpy-4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.3.0
+Version: 4.3.1
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `vcrpy-4.3.0/README.rst` & `vcrpy-4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/fixtures/migration/new_cassette.json` & `vcrpy-4.3.1/tests/fixtures/migration/new_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/fixtures/migration/new_cassette.yaml` & `vcrpy-4.3.1/tests/fixtures/migration/new_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/fixtures/migration/old_cassette.json` & `vcrpy-4.3.1/tests/fixtures/migration/old_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/fixtures/migration/old_cassette.yaml` & `vcrpy-4.3.1/tests/fixtures/migration/old_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/fixtures/wild/domain_redirect.yaml` & `vcrpy-4.3.1/tests/fixtures/wild/domain_redirect.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/aiohttp_utils.py` & `vcrpy-4.3.1/tests/integration/aiohttp_utils.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml` & `vcrpy-4.3.1/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_aiohttp.py` & `vcrpy-4.3.1/tests/integration/test_aiohttp.py`

 * *Files 10% similar despite different names*

```diff
@@ -316,39 +316,43 @@
 
         assert cassette_response_text == response_text2
 
         # Now that we made both requests, we should have played both.
         assert cassette.play_count == 2
 
 
-def test_cookies(scheme, tmpdir):
+def test_cookies(httpbin_both, httpbin_ssl_context, tmpdir):
     async def run(loop):
-        cookies_url = scheme + (
-            "://httpbin.org/response-headers?"
+        cookies_url = httpbin_both.url + (
+            "/response-headers?"
             "set-cookie=" + urllib.parse.quote("cookie_1=val_1; Path=/") + "&"
             "Set-Cookie=" + urllib.parse.quote("Cookie_2=Val_2; Path=/")
         )
-        home_url = scheme + "://httpbin.org/"
+        home_url = httpbin_both.url + "/"
         tmp = str(tmpdir.join("cookies.yaml"))
         req_cookies = {"Cookie_3": "Val_3"}
         req_headers = {"Cookie": "Cookie_4=Val_4"}
 
         # ------------------------- Record -------------------------- #
         with vcr.use_cassette(tmp) as cassette:
-            async with aiohttp.ClientSession(loop=loop) as session:
-                cookies_resp = await session.get(cookies_url)
-                home_resp = await session.get(home_url, cookies=req_cookies, headers=req_headers)
+            async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
+                cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
+                home_resp = await session.get(
+                    home_url, cookies=req_cookies, headers=req_headers, ssl=httpbin_ssl_context
+                )
                 assert cassette.play_count == 0
         assert_responses(cookies_resp, home_resp)
 
         # -------------------------- Play --------------------------- #
         with vcr.use_cassette(tmp, record_mode=vcr.mode.NONE) as cassette:
-            async with aiohttp.ClientSession(loop=loop) as session:
-                cookies_resp = await session.get(cookies_url)
-                home_resp = await session.get(home_url, cookies=req_cookies, headers=req_headers)
+            async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
+                cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
+                home_resp = await session.get(
+                    home_url, cookies=req_cookies, headers=req_headers, ssl=httpbin_ssl_context
+                )
                 assert cassette.play_count == 2
         assert_responses(cookies_resp, home_resp)
 
     def assert_responses(cookies_resp, home_resp):
         assert cookies_resp.cookies.get("cookie_1").value == "val_1"
         assert cookies_resp.cookies.get("Cookie_2").value == "Val_2"
         request_cookies = home_resp.request_info.headers["cookie"]
@@ -356,47 +360,47 @@
         assert "Cookie_2=Val_2" in request_cookies
         assert "Cookie_3=Val_3" in request_cookies
         assert "Cookie_4=Val_4" in request_cookies
 
     run_in_loop(run)
 
 
-def test_cookies_redirect(scheme, tmpdir):
+def test_cookies_redirect(httpbin_both, httpbin_ssl_context, tmpdir):
     async def run(loop):
         # Sets cookie as provided by the query string and redirects
-        cookies_url = scheme + "://httpbin.org/cookies/set?Cookie_1=Val_1"
+        cookies_url = httpbin_both.url + "/cookies/set?Cookie_1=Val_1"
         tmp = str(tmpdir.join("cookies.yaml"))
 
         # ------------------------- Record -------------------------- #
         with vcr.use_cassette(tmp) as cassette:
-            async with aiohttp.ClientSession(loop=loop) as session:
-                cookies_resp = await session.get(cookies_url)
+            async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
+                cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
                 assert cassette.play_count == 0
             cassette.requests[1].headers["Cookie"] == "Cookie_1=Val_1"
 
         # -------------------------- Play --------------------------- #
         with vcr.use_cassette(tmp, record_mode=vcr.mode.NONE) as cassette:
-            async with aiohttp.ClientSession(loop=loop) as session:
-                cookies_resp = await session.get(cookies_url)
+            async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
+                cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
                 assert cassette.play_count == 2
             cassette.requests[1].headers["Cookie"] == "Cookie_1=Val_1"
 
         # Assert that it's ignoring expiration date
         with vcr.use_cassette(tmp, record_mode=vcr.mode.NONE) as cassette:
             cassette.responses[0]["headers"]["set-cookie"] = [
                 "Cookie_1=Val_1; Expires=Wed, 21 Oct 2015 07:28:00 GMT"
             ]
-            async with aiohttp.ClientSession(loop=loop) as session:
-                cookies_resp = await session.get(cookies_url)
+            async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
+                cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
 
     run_in_loop(run)
```

### Comparing `vcrpy-4.3.0/tests/integration/test_basic.py` & `vcrpy-4.3.1/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_boto.py` & `vcrpy-4.3.1/tests/integration/test_boto.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_boto3.py` & `vcrpy-4.3.1/tests/integration/test_boto3.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_config.py` & `vcrpy-4.3.1/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_disksaver.py` & `vcrpy-4.3.1/tests/integration/test_disksaver.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_filter.py` & `vcrpy-4.3.1/tests/integration/test_filter.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_http` & `vcrpy-4.3.1/tests/integration/test_http`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_httplib2.py` & `vcrpy-4.3.1/tests/integration/test_httplib2.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_httpx.py` & `vcrpy-4.3.1/tests/integration/test_httpx.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_ignore.py` & `vcrpy-4.3.1/tests/integration/test_ignore.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_matchers.py` & `vcrpy-4.3.1/tests/integration/test_matchers.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_multiple.py` & `vcrpy-4.3.1/tests/integration/test_multiple.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_proxy.py` & `vcrpy-4.3.1/tests/integration/test_proxy.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_record_mode.py` & `vcrpy-4.3.1/tests/integration/test_record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_register_matcher.py` & `vcrpy-4.3.1/tests/integration/test_register_matcher.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_register_persister.py` & `vcrpy-4.3.1/tests/integration/test_register_persister.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_register_serializer.py` & `vcrpy-4.3.1/tests/integration/test_register_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_request.py` & `vcrpy-4.3.1/tests/integration/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_requests.py` & `vcrpy-4.3.1/tests/integration/test_requests.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_stubs.py` & `vcrpy-4.3.1/tests/integration/test_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_tornado.py` & `vcrpy-4.3.1/tests/integration/test_tornado.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_tornado_exception_can_be_caught.yaml` & `vcrpy-4.3.1/tests/integration/test_tornado_exception_can_be_caught.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml` & `vcrpy-4.3.1/tests/integration/test_tornado_with_decorator_use_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_urllib2.py` & `vcrpy-4.3.1/tests/integration/test_urllib2.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/integration/test_urllib3.py` & `vcrpy-4.3.1/tests/integration/test_urllib3.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 import pytest_httpbin
 from assertions import assert_cassette_empty, assert_is_json
 
 import vcr
 from vcr.patch import force_reset
+from vcr.stubs.compat import get_headers
 
 urllib3 = pytest.importorskip("urllib3")
 
 
 @pytest.fixture(scope="module")
 def verify_pool_mgr():
     return urllib3.PoolManager(
@@ -37,15 +38,16 @@
 def test_headers(tmpdir, httpbin_both, verify_pool_mgr):
     """Ensure that we can read the headers back"""
     url = httpbin_both.url
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
         headers = verify_pool_mgr.request("GET", url).headers
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
-        assert headers == verify_pool_mgr.request("GET", url).headers
+        new_headers = verify_pool_mgr.request("GET", url).headers
+        assert sorted(get_headers(headers)) == sorted(get_headers(new_headers))
 
 
 def test_body(tmpdir, httpbin_both, verify_pool_mgr):
     """Ensure the responses are all identical enough"""
     url = httpbin_both.url + "/bytes/1024"
     with vcr.use_cassette(str(tmpdir.join("body.yaml"))):
         content = verify_pool_mgr.request("GET", url).data
@@ -141,22 +143,22 @@
 
 def test_https_with_cert_validation_disabled(tmpdir, httpbin_secure, pool_mgr):
     with vcr.use_cassette(str(tmpdir.join("cert_validation_disabled.yaml"))):
         pool_mgr.request("GET", httpbin_secure.url)
 
 
 def test_urllib3_force_reset():
-    cpool = urllib3.connectionpool
-    http_original = cpool.HTTPConnection
-    https_original = cpool.HTTPSConnection
-    verified_https_original = cpool.VerifiedHTTPSConnection
+    conn = urllib3.connection
+    http_original = conn.HTTPConnection
+    https_original = conn.HTTPSConnection
+    verified_https_original = conn.VerifiedHTTPSConnection
     with vcr.use_cassette(path="test"):
-        first_cassette_HTTPConnection = cpool.HTTPConnection
-        first_cassette_HTTPSConnection = cpool.HTTPSConnection
-        first_cassette_VerifiedHTTPSConnection = cpool.VerifiedHTTPSConnection
+        first_cassette_HTTPConnection = conn.HTTPConnection
+        first_cassette_HTTPSConnection = conn.HTTPSConnection
+        first_cassette_VerifiedHTTPSConnection = conn.VerifiedHTTPSConnection
         with force_reset():
-            assert cpool.HTTPConnection is http_original
-            assert cpool.HTTPSConnection is https_original
-            assert cpool.VerifiedHTTPSConnection is verified_https_original
-        assert cpool.HTTPConnection is first_cassette_HTTPConnection
-        assert cpool.HTTPSConnection is first_cassette_HTTPSConnection
-        assert cpool.VerifiedHTTPSConnection is first_cassette_VerifiedHTTPSConnection
+            assert conn.HTTPConnection is http_original
+            assert conn.HTTPSConnection is https_original
+            assert conn.VerifiedHTTPSConnection is verified_https_original
+        assert conn.HTTPConnection is first_cassette_HTTPConnection
+        assert conn.HTTPSConnection is first_cassette_HTTPSConnection
+        assert conn.VerifiedHTTPSConnection is first_cassette_VerifiedHTTPSConnection
```

### Comparing `vcrpy-4.3.0/tests/integration/test_wild.py` & `vcrpy-4.3.1/tests/integration/test_wild.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,17 +60,18 @@
 
 
 def test_cookies(tmpdir, httpbin):
     testfile = str(tmpdir.join("cookies.yml"))
     with vcr.use_cassette(testfile):
         s = requests.Session()
         s.get(httpbin.url + "/cookies/set?k1=v1&k2=v2")
+        assert s.cookies.keys() == ["k1", "k2"]
 
         r2 = s.get(httpbin.url + "/cookies")
-        assert len(r2.json()["cookies"]) == 2
+        assert sorted(r2.json()["cookies"].keys()) == ["k1", "k2"]
 
 
 def test_amazon_doctype(tmpdir):
     # amazon gzips its homepage.  For some reason, in requests 2.7, it's not
     # getting gunzipped.
     with vcr.use_cassette(str(tmpdir.join("amz.yml"))):
         r = requests.get("http://www.amazon.com", verify=False)
```

### Comparing `vcrpy-4.3.0/tests/unit/test_cassettes.py` & `vcrpy-4.3.1/tests/unit/test_cassettes.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_errors.py` & `vcrpy-4.3.1/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_filters.py` & `vcrpy-4.3.1/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_json_serializer.py` & `vcrpy-4.3.1/tests/unit/test_json_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_matchers.py` & `vcrpy-4.3.1/tests/unit/test_matchers.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_migration.py` & `vcrpy-4.3.1/tests/unit/test_migration.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_persist.py` & `vcrpy-4.3.1/tests/unit/test_persist.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_request.py` & `vcrpy-4.3.1/tests/unit/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_response.py` & `vcrpy-4.3.1/tests/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_serialize.py` & `vcrpy-4.3.1/tests/unit/test_serialize.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_stubs.py` & `vcrpy-4.3.1/tests/unit/test_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/tests/unit/test_vcr.py` & `vcrpy-4.3.1/tests/unit/test_vcr.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         new_record_mode = mock.Mock()
 
     with test_vcr.use_cassette("test", record_mode=new_record_mode) as cassette:
         assert cassette.record_mode == new_record_mode
 
 
 def test_vcr_before_record_request_params():
-    base_path = "http://httpbin.org/"
+    base_path = "http://whatever.test/"
 
     def before_record_cb(request):
         if request.path != "/get":
             return request
 
     test_vcr = VCR(
         filter_headers=("cookie", ("bert", "ernie")),
```

### Comparing `vcrpy-4.3.0/tox.ini` & `vcrpy-4.3.1/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tox]
 skip_missing_interpreters=true
 envlist =
   cov-clean,
   lint,
-  {py37,py38,py39,py310,py311}-{requests,httplib2,urllib3,tornado4,boto3,aiohttp,httpx},
-  {pypy3}-{requests,httplib2,urllib3,tornado4,boto3},
+  {py37,py38,py39,py310,py311}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3,aiohttp,httpx},
+  {py310,py311}-{requests-urllib3-2,urllib3-2},
+  {pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},
   {py310}-httpx019,
   cov-report
 
 
 [gh-actions]
 python =
     3.7: py37
@@ -81,32 +82,31 @@
     Werkzeug==2.0.3
     pytest
     pytest-httpbin>=1.0.1
     pytest-cov
     PyYAML
     ipaddress
     requests: requests>=2.22.0
-    requests: urllib3<2
     httplib2: httplib2
-    urllib3: urllib3<2
+    urllib3-1: urllib3<2
+    urllib3-2: urllib3<3
     boto3: boto3
-    boto3: urllib3
     aiohttp: aiohttp
     aiohttp: pytest-asyncio
     aiohttp: pytest-aiohttp
     httpx: httpx
     {py37,py38,py39,py310}-{httpx}: httpx
     {py37,py38,py39,py310}-{httpx}: pytest-asyncio
     httpx: httpx>0.19
     # httpx==0.19 is the latest version that supports allow_redirects, newer versions use follow_redirects
     httpx019: httpx==0.19
     {py37,py38,py39,py310}-{httpx}: pytest-asyncio
 depends =
-  lint,{py37,py38,py39,py310,py311,pypy3}-{requests,httplib2,urllib3,tornado4,boto3},{py37,py38,py39,py310,py311}-{aiohttp},{py37,py38,py39,py310,py311}-{httpx}: cov-clean
-  cov-report: lint,{py37,py38,py39,py310,py311,pypy3}-{requests,httplib2,urllib3,tornado4,boto3},{py37,py38,py39,py310,py311}-{aiohttp}
+  lint,{py37,py38,py39,py310,py311,pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},{py310,py311}-{requests-urllib3-2,urllib3-2},{py37,py38,py39,py310,py311}-{aiohttp},{py37,py38,py39,py310,py311}-{httpx}: cov-clean
+  cov-report: lint,{py37,py38,py39,py310,py311,pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},{py310,py311}-{requests-urllib3-2,urllib3-2},{py37,py38,py39,py310,py311}-{aiohttp}
 passenv =
     AWS_ACCESS_KEY_ID
     AWS_DEFAULT_REGION
     AWS_SECRET_ACCESS_KEY
 
 [flake8]
 max_line_length = 110
```

### Comparing `vcrpy-4.3.0/vcr/cassette.py` & `vcrpy-4.3.1/vcr/cassette.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/config.py` & `vcrpy-4.3.1/vcr/config.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/errors.py` & `vcrpy-4.3.1/vcr/errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/filters.py` & `vcrpy-4.3.1/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/matchers.py` & `vcrpy-4.3.1/vcr/matchers.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/migration.py` & `vcrpy-4.3.1/vcr/migration.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/patch.py` & `vcrpy-4.3.1/vcr/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,23 +28,25 @@
         ) from e
 else:
     _Boto3VerifiedHTTPSConnection = AWSHTTPSConnection
     _cpoolBoto3HTTPConnection = AWSHTTPConnection
     _cpoolBoto3HTTPSConnection = AWSHTTPSConnection
 
 cpool = None
+conn = None
 # Try to save the original types for urllib3
 try:
+    import urllib3.connection as conn
     import urllib3.connectionpool as cpool
 except ImportError:  # pragma: no cover
     pass
 else:
-    _VerifiedHTTPSConnection = cpool.VerifiedHTTPSConnection
-    _cpoolHTTPConnection = cpool.HTTPConnection
-    _cpoolHTTPSConnection = cpool.HTTPSConnection
+    _VerifiedHTTPSConnection = conn.VerifiedHTTPSConnection
+    _connHTTPConnection = conn.HTTPConnection
+    _connHTTPSConnection = conn.HTTPSConnection
 
 # Try to save the original types for requests
 try:
     import requests
 except ImportError:  # pragma: no cover
     pass
 else:
@@ -194,15 +196,15 @@
         yield httplib, "HTTPSConnection", VCRHTTPSConnection
 
     def _requests(self):
         try:
             from .stubs import requests_stubs
         except ImportError:  # pragma: no cover
             return ()
-        return self._urllib3_patchers(cpool, requests_stubs)
+        return self._urllib3_patchers(cpool, conn, requests_stubs)
 
     @_build_patchers_from_mock_triples_decorator
     def _boto3(self):
         try:
             # botocore using awsrequest
             import botocore.awsrequest as cpool
         except ImportError:  # pragma: no cover
@@ -244,20 +246,21 @@
             connection_remover.add_connection_to_pool_entry(pool, new_connection)
             return new_connection
 
         return patched_new_conn
 
     def _urllib3(self):
         try:
+            import urllib3.connection as conn
             import urllib3.connectionpool as cpool
         except ImportError:  # pragma: no cover
             return ()
         from .stubs import urllib3_stubs
 
-        return self._urllib3_patchers(cpool, urllib3_stubs)
+        return self._urllib3_patchers(cpool, conn, urllib3_stubs)
 
     @_build_patchers_from_mock_triples_decorator
     def _httplib2(self):
         try:
             import httplib2 as cpool
         except ImportError:  # pragma: no cover
             pass
@@ -326,25 +329,25 @@
 
             new_async_client_send = async_vcr_send(self._cassette, _HttpxAsyncClient_send)
             yield httpx.AsyncClient, "send", new_async_client_send
 
             new_sync_client_send = sync_vcr_send(self._cassette, _HttpxSyncClient_send)
             yield httpx.Client, "send", new_sync_client_send
 
-    def _urllib3_patchers(self, cpool, stubs):
+    def _urllib3_patchers(self, cpool, conn, stubs):
         http_connection_remover = ConnectionRemover(
             self._get_cassette_subclass(stubs.VCRRequestsHTTPConnection)
         )
         https_connection_remover = ConnectionRemover(
             self._get_cassette_subclass(stubs.VCRRequestsHTTPSConnection)
         )
         mock_triples = (
-            (cpool, "VerifiedHTTPSConnection", stubs.VCRRequestsHTTPSConnection),
-            (cpool, "HTTPConnection", stubs.VCRRequestsHTTPConnection),
-            (cpool, "HTTPSConnection", stubs.VCRRequestsHTTPSConnection),
+            (conn, "VerifiedHTTPSConnection", stubs.VCRRequestsHTTPSConnection),
+            (conn, "HTTPConnection", stubs.VCRRequestsHTTPConnection),
+            (conn, "HTTPSConnection", stubs.VCRRequestsHTTPSConnection),
             (cpool, "is_connection_dropped", mock.Mock(return_value=False)),  # Needed on Windows only
             (cpool.HTTPConnectionPool, "ConnectionCls", stubs.VCRRequestsHTTPConnection),
             (cpool.HTTPSConnectionPool, "ConnectionCls", stubs.VCRRequestsHTTPSConnection),
         )
         # These handle making sure that sessions only use the
         # connections of the appropriate type.
         mock_triples += (
@@ -406,24 +409,25 @@
 
 
 def reset_patchers():
     yield mock.patch.object(httplib, "HTTPConnection", _HTTPConnection)
     yield mock.patch.object(httplib, "HTTPSConnection", _HTTPSConnection)
 
     try:
+        import urllib3.connection as conn
         import urllib3.connectionpool as cpool
     except ImportError:  # pragma: no cover
         pass
     else:
-        yield mock.patch.object(cpool, "VerifiedHTTPSConnection", _VerifiedHTTPSConnection)
-        yield mock.patch.object(cpool, "HTTPConnection", _cpoolHTTPConnection)
-        yield mock.patch.object(cpool, "HTTPSConnection", _cpoolHTTPSConnection)
+        yield mock.patch.object(conn, "VerifiedHTTPSConnection", _VerifiedHTTPSConnection)
+        yield mock.patch.object(conn, "HTTPConnection", _connHTTPConnection)
+        yield mock.patch.object(conn, "HTTPSConnection", _connHTTPSConnection)
         if hasattr(cpool.HTTPConnectionPool, "ConnectionCls"):
-            yield mock.patch.object(cpool.HTTPConnectionPool, "ConnectionCls", _cpoolHTTPConnection)
-            yield mock.patch.object(cpool.HTTPSConnectionPool, "ConnectionCls", _cpoolHTTPSConnection)
+            yield mock.patch.object(cpool.HTTPConnectionPool, "ConnectionCls", _connHTTPConnection)
+            yield mock.patch.object(cpool.HTTPSConnectionPool, "ConnectionCls", _connHTTPSConnection)
 
     try:
         # unpatch botocore with awsrequest
         import botocore.awsrequest as cpool
     except ImportError:  # pragma: no cover
         pass
     else:
```

### Comparing `vcrpy-4.3.0/vcr/persisters/filesystem.py` & `vcrpy-4.3.1/vcr/persisters/filesystem.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/record_mode.py` & `vcrpy-4.3.1/vcr/record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/request.py` & `vcrpy-4.3.1/vcr/request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/serialize.py` & `vcrpy-4.3.1/vcr/serialize.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/serializers/compat.py` & `vcrpy-4.3.1/vcr/serializers/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/serializers/jsonserializer.py` & `vcrpy-4.3.1/vcr/serializers/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/stubs/__init__.py` & `vcrpy-4.3.1/vcr/stubs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,17 @@
     for key, values in header_list.items():
         for v in values:
             header_string += key.encode("utf-8") + b":" + v.encode("utf-8") + b"\r\n"
     return compat.get_httpmessage(header_string)
 
 
 def serialize_headers(response):
+    headers = response.headers if response.msg is None else response.msg
     out = {}
-    for key, values in compat.get_headers(response.msg):
+    for key, values in compat.get_headers(headers):
         out.setdefault(key, [])
         out[key].extend(values)
     return out
 
 
 class VCRHTTPResponse(HTTPResponse):
     """
@@ -63,14 +64,15 @@
         self.fp = None
         self.recorded_response = recorded_response
         self.reason = recorded_response["status"]["message"]
         self.status = self.code = recorded_response["status"]["code"]
         self.version = None
         self._content = BytesIO(self.recorded_response["body"]["string"])
         self._closed = False
+        self._original_response = self  # for requests.session.Session cookie extraction
 
         headers = self.recorded_response["headers"]
         # Since we are loading a response that has already been serialized, our
         # response is no longer chunked.  That means we don't want any
         # libraries trying to process a chunked response.  By removing the
         # transfer-encoding: chunked header, this should cause the downstream
         # libraries to process this as a non-chunked response.
@@ -139,14 +141,36 @@
             return ", ".join(values)
         else:
             return default
 
     def readable(self):
         return self._content.readable()
 
+    @property
+    def length_remaining(self):
+        return self._content.getbuffer().nbytes - self._content.tell()
+
+    def get_redirect_location(self):
+        """
+        Returns (a) redirect location string if we got a redirect
+        status code and valid location, (b) None if redirect status and
+        no location, (c) False if not a redirect status code.
+        See https://urllib3.readthedocs.io/en/stable/reference/urllib3.response.html .
+        """
+        if not (300 <= self.status <= 399):
+            return False
+        return self.getheader("Location")
+
+    @property
+    def data(self):
+        return self._content.getbuffer().tobytes()
+
+    def drain_conn(self):
+        pass
+
 
 class VCRConnection:
     # A reference to the cassette that's currently being patched in
     cassette = None
 
     def _port_postfix(self):
         """
@@ -244,20 +268,21 @@
                     url=self._url(self._vcr_request.uri),
                     body=self._vcr_request.body,
                     headers=self._vcr_request.headers,
                 )
 
             # get the response
             response = self.real_connection.getresponse()
+            response_data = response.data if hasattr(response, "data") else response.read()
 
             # put the response into the cassette
             response = {
                 "status": {"code": response.status, "message": response.reason},
                 "headers": serialize_headers(response),
-                "body": {"string": response.read()},
+                "body": {"string": response_data},
             }
             self.cassette.append(self._vcr_request, response)
         return VCRHTTPResponse(response)
 
     def set_debuglevel(self, *args, **kwargs):
         self.real_connection.set_debuglevel(*args, **kwargs)
```

### Comparing `vcrpy-4.3.0/vcr/stubs/aiohttp_stubs.py` & `vcrpy-4.3.1/vcr/stubs/aiohttp_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/stubs/boto3_stubs.py` & `vcrpy-4.3.1/vcr/stubs/boto3_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/stubs/compat.py` & `vcrpy-4.3.1/vcr/stubs/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/stubs/httplib2_stubs.py` & `vcrpy-4.3.1/vcr/stubs/httplib2_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/stubs/httpx_stubs.py` & `vcrpy-4.3.1/vcr/stubs/httpx_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/stubs/requests_stubs.py` & `vcrpy-4.3.1/vcr/stubs/requests_stubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Stubs for requests"""
 
-from urllib3.connectionpool import HTTPConnection, VerifiedHTTPSConnection
+from urllib3.connection import HTTPConnection, VerifiedHTTPSConnection
 
 from ..stubs import VCRHTTPConnection, VCRHTTPSConnection
 
 # urllib3 defines its own HTTPConnection classes, which requests goes ahead and assumes
 # you're using.  It includes some polyfills for newer features missing in older pythons.
```

### Comparing `vcrpy-4.3.0/vcr/stubs/tornado_stubs.py` & `vcrpy-4.3.1/vcr/stubs/tornado_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcr/util.py` & `vcrpy-4.3.1/vcr/util.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.0/vcrpy.egg-info/PKG-INFO` & `vcrpy-4.3.1/vcrpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.3.0
+Version: 4.3.1
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `vcrpy-4.3.0/vcrpy.egg-info/SOURCES.txt` & `vcrpy-4.3.1/vcrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


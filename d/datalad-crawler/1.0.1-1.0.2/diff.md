# Comparing `tmp/datalad_crawler-1.0.1.tar.gz` & `tmp/datalad_crawler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_crawler-1.0.1.tar", last modified: Thu May 25 17:49:44 2023, max compression
+gzip compressed data, was "datalad_crawler-1.0.2.tar", last modified: Fri May 26 12:26:27 2023, max compression
```

## Comparing `datalad_crawler-1.0.1.tar` & `datalad_crawler-1.0.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.576411 datalad_crawler-1.0.1/datalad_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/crawl_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/dbs/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/dbs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69530 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/annex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/crawl_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/matches.py
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_annex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_crawl_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/abstractsonline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/balsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/crcns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/fcptable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/nda.py
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_with_archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/stanford_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_balsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_crcns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_fcptable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_nda.py
--rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_with_archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_xnat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/xnat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/support/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/datalad_crawler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/setup_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.537045 datalad_crawler-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-26 12:26:27.533045 datalad_crawler-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.529045 datalad_crawler-1.0.2/datalad_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/crawl_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.529045 datalad_crawler-1.0.2/datalad_crawler/dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/dbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/dbs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/dbs/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.529045 datalad_crawler-1.0.2/datalad_crawler/dbs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/dbs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/dbs/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/dbs/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.529045 datalad_crawler-1.0.2/datalad_crawler/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69530 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/annex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/crawl_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.529045 datalad_crawler-1.0.2/datalad_crawler/nodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_annex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_crawl_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.533045 datalad_crawler-1.0.2/datalad_crawler/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/abstractsonline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/balsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/crcns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/fcptable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/nda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/openfmri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/openfmri_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/simple_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/simple_with_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/stanford_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.533045 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_balsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_crcns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_fcptable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_nda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_openfmri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_openfmri_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_simple_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_simple_with_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_xnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/pipelines/xnat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.533045 datalad_crawler-1.0.2/datalad_crawler/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.533045 datalad_crawler-1.0.2/datalad_crawler/support/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/support/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/support/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/support/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.533045 datalad_crawler-1.0.2/datalad_crawler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/tests/test_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/tests/test_crawl_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/datalad_crawler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:26:27.529045 datalad_crawler-1.0.2/datalad_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-26 12:26:27.000000 datalad_crawler-1.0.2/datalad_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-26 12:26:27.000000 datalad_crawler-1.0.2/datalad_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:26:27.000000 datalad_crawler-1.0.2/datalad_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 12:26:27.000000 datalad_crawler-1.0.2/datalad_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 12:26:27.000000 datalad_crawler-1.0.2/datalad_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 12:26:27.000000 datalad_crawler-1.0.2/datalad_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:26:27.537045 datalad_crawler-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-26 12:26:13.000000 datalad_crawler-1.0.2/setup_support.py
```

### Comparing `datalad_crawler-1.0.1/COPYING` & `datalad_crawler-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/PKG-INFO` & `datalad_crawler-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_crawler
-Version: 1.0.1
+Version: 1.0.2
 Summary: DataLad extension package for crawling external web resources into an automated data distribution
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Description-Content-Type: text/markdown
 Provides-Extra: core
 Provides-Extra: devel-docs
 Provides-Extra: tests
```

### Comparing `datalad_crawler-1.0.1/README.md` & `datalad_crawler-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/__init__.py` & `datalad_crawler-1.0.2/datalad_crawler/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/consts.py` & `datalad_crawler-1.0.2/datalad_crawler/consts.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/crawl.py` & `datalad_crawler-1.0.2/datalad_crawler/crawl.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/crawl_init.py` & `datalad_crawler-1.0.2/datalad_crawler/crawl_init.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/dbs/base.py` & `datalad_crawler-1.0.2/datalad_crawler/dbs/base.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/dbs/files.py` & `datalad_crawler-1.0.2/datalad_crawler/dbs/files.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/dbs/tests/test_files.py` & `datalad_crawler-1.0.2/datalad_crawler/dbs/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/dbs/versions.py` & `datalad_crawler-1.0.2/datalad_crawler/dbs/versions.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/__init__.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/annex.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/annex.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/crawl_url.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/crawl_url.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/matches.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/matches.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/misc.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/misc.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/s3.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_annex.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_annex.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_crawl_url.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_crawl_url.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_matches.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_matches.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_misc.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_s3.py` & `datalad_crawler-1.0.2/datalad_crawler/nodes/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipeline.py` & `datalad_crawler-1.0.2/datalad_crawler/pipeline.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/abstractsonline.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/abstractsonline.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/balsa.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/balsa.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/crcns.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/crcns.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/fcptable.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/fcptable.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/gh.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/gh.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 # I guess due to all the "import magic" we can't simply force load of
 # global  github module whenever there is a local one, so we will rename
 # local one
 
 import re
 
+from datalad import cfg
+
 from datalad.api import Dataset, install
+from datalad.downloaders.credentials import Token
 from datalad.support import path as op
 from datalad.support.gitrepo import GitRepo
 from datalad.utils import (
     assure_bool,
     assure_list_from_str,
     rmtree,
     updated
@@ -27,14 +30,27 @@
 
 # Possibly instantiate a logger if you would like to log
 # during pipeline creation
 from logging import getLogger
 lgr = getLogger("datalad.crawler.pipelines.github")
 
 
+def _get_github_token(obtain=False) -> str:
+    # Quick and dirty adapter which would use stored Token if was stored in credentials
+    # or just access in cfg if present
+    try:
+        token = Token('api.github.com')()['token']
+        if not token:
+            raise ValueError("Empty value for token is stored")
+        return token
+    except Exception as exc:
+        lgr.warning("Failed to get api.github.com credential: %s", exc)
+    return (cfg.obtain if obtain else cfg.get)('hub.oauthtoken')
+
+
 def pipeline(org=None,
              repo_type='sources', include='.*', exclude=None,
              metadata_nativetypes=None, aggregate=False,
              get_data=False, drop_data=False):
     """Crawl github organization and install all matching repos as subdatasets
 
     Parameters
@@ -67,27 +83,25 @@
     """
     assert org, "Organization must be provided"
     aggregate = assure_bool(aggregate)
     get_data = assure_bool(get_data)
     drop_data = assure_bool(drop_data)
 
     import github as gh
-    # TODO: consider elevating that function to a "public" helper
-    from datalad.support.github_ import _gen_github_entity
     superds = Dataset('.')
     if metadata_nativetypes:
         metadata_nativetypes = assure_list_from_str(metadata_nativetypes, sep=',')
 
     aggregate_later = []
     def crawl_github_org(data):
         assert list(data) == ['datalad_stats'], data
-        # TODO: actually populate the datalad_stats with # of datasets and
-        # possibly amount of data downloaded in get below
-        # Needs DataLad >= 0.13.6~7^2~3 where password was removed
-        entity, cred = next(_gen_github_entity(None, org))
+
+        # TODO: redo with proper integration
+        g = gh.Github(_get_github_token(obtain=True))
+        entity = g.get_organization(org)
         all_repos = list(entity.get_repos(repo_type))
 
         for repo in all_repos:
             name = repo.name
             if include and not re.search(include, name):
                 lgr.debug(
                     "Skipping %s since include regex search returns nothing", name
@@ -103,14 +117,22 @@
             if op.exists(dspath):
                 lgr.info("Skipping %s since already exists", name)
                 # although we could just do install, which would at least
                 # verify that url is the same... to not try to aggregate
                 # etc, we will just skip for now
                 continue
 
+            # See if it has anything committed - we will not clone empty ones
+            try:
+                if not any(repo.get_commits()):
+                    raise ValueError("no commits")
+            except Exception as exc:
+                lgr.info("Skipping %s since: %s", name, exc)
+                continue
+
             # TODO: all the recursive etc options
             try:
                 ds = superds.install(
                     dspath, source=repo.clone_url, get_data=get_data,
                     on_failure='continue'
                 )
             except Exception as exc:
```

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/nda.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/nda.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/openfmri.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri_s3.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/openfmri_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_s3.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/simple_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_with_archives.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/simple_with_archives.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/stanford_lib.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/stanford_lib.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/template.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_balsa.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_balsa.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_crcns.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_crcns.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_fcptable.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_fcptable.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_gh.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_gh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from datalad.utils import chpwd
 
+from datalad import cfg
 from datalad.api import (
     crawl,
     crawl_init,
     create,
 )
 try:
-    from datalad.support.github_ import _get_github_cred
+    import github
 except ImportError:
-    # might be dated which has not merged
-    # https://github.com/datalad/datalad/pull/4400 yet
-    from datalad.downloaders.credentials import UserPassword
-    def _get_github_cred():
-        """Trimmed down helper"""
-        return UserPassword("github", "does not matter")
+    github = None
 
 from datalad.tests.utils_pytest import (
     assert_false,
     assert_greater,
     skip_if_no_network,
     with_tempfile,
 )
 import pytest
 
+from ..gh import _get_github_token
 
 @skip_if_no_network
 @with_tempfile
 def test_crawl(tempd=None):
-    if not _get_github_cred().is_known:
-        pytest.skip("no github credential")
+    if not github:
+        pytest.skip("no github package")
+    # set DATALAD_TESTS_CREDENTIALS=system to use system credentials
+    if not _get_github_token(obtain=False):
+        pytest.skip("no github credentials")
     ds = create(tempd)
     with chpwd(tempd):
         crawl_init(
             template='gh', save=True,
             args={'org': 'datalad-collection-1', 'include': 'kaggle'}
         )
         crawl()
```

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_nda.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_nda.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_openfmri.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri_collection.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_openfmri_collection.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_s3.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_simple_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_with_archives.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_simple_with_archives.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_utils.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_xnat.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/tests/test_xnat.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/pipelines/xnat.py` & `datalad_crawler-1.0.2/datalad_crawler/pipelines/xnat.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/support/tests/test_versions.py` & `datalad_crawler-1.0.2/datalad_crawler/support/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/support/versions.py` & `datalad_crawler-1.0.2/datalad_crawler/support/versions.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/tests/__init__.py` & `datalad_crawler-1.0.2/datalad_crawler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl.py` & `datalad_crawler-1.0.2/datalad_crawler/tests/test_crawl.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl_init.py` & `datalad_crawler-1.0.2/datalad_crawler/tests/test_crawl_init.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/tests/test_pipeline.py` & `datalad_crawler-1.0.2/datalad_crawler/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/tests/test_utils.py` & `datalad_crawler-1.0.2/datalad_crawler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler/utils.py` & `datalad_crawler-1.0.2/datalad_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/datalad_crawler.egg-info/PKG-INFO` & `datalad_crawler-1.0.2/datalad_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-crawler
-Version: 1.0.1
+Version: 1.0.2
 Summary: DataLad extension package for crawling external web resources into an automated data distribution
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 Description-Content-Type: text/markdown
 Provides-Extra: core
 Provides-Extra: devel-docs
 Provides-Extra: tests
```

### Comparing `datalad_crawler-1.0.1/datalad_crawler.egg-info/SOURCES.txt` & `datalad_crawler-1.0.2/datalad_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/formatters.py` & `datalad_crawler-1.0.2/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/setup.py` & `datalad_crawler-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-1.0.1/setup_support.py` & `datalad_crawler-1.0.2/setup_support.py`

 * *Files identical despite different names*


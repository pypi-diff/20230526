# Comparing `tmp/aixplain-0.2.0.tar.gz` & `tmp/aixplain-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixplain-0.2.0.tar", last modified: Thu May 11 12:45:33 2023, max compression
+gzip compressed data, was "aixplain-0.2.1.tar", last modified: Fri May 26 21:35:14 2023, max compression
```

## Comparing `aixplain-0.2.0.tar` & `aixplain-0.2.1.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.458853 aixplain-0.2.0/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     3822 2023-05-11 12:45:33.458853 aixplain-0.2.0/PKG-INFO
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     2254 2023-05-11 12:32:02.000000 aixplain-0.2.0/README.md
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.446852 aixplain-0.2.0/aixplain/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      852 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      954 2023-05-11 12:32:53.000000 aixplain-0.2.0/aixplain/__version__.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.450853 aixplain-0.2.0/aixplain/enums/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      336 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      793 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/data_split.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      842 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/data_subtype.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      887 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/data_type.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1007 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/file_type.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1441 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/function.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1846 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/language.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1600 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/license.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      837 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/onboard_status.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      796 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/privacy.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      781 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/enums/storage_type.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.450853 aixplain-0.2.0/aixplain/factories/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1021 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1284 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/asset_factory.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)    12342 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/benchmark_factory.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)    14290 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/corpus_factory.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)    22632 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/dataset_factory.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     2720 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/file_factory.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     4549 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/metric_factory.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     7150 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/model_factory.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     5854 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/factories/pipeline_factory.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.454853 aixplain-0.2.0/aixplain/modules/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      995 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1933 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/asset.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     3142 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/benchmark.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     2004 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/benchmark_job.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     3076 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/corpus.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     3346 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/data.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     5598 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/dataset.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1918 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/file.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     3663 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/metadata.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     2247 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/metric.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     9690 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/model.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     8116 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/modules/pipeline.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.454853 aixplain-0.2.0/aixplain/processes/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/processes/__init__.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.454853 aixplain-0.2.0/aixplain/processes/data_onboarding/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/processes/data_onboarding/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)    13261 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/processes/data_onboarding/onboard_functions.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     9361 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/processes/data_onboarding/process_audio_files.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     5225 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/processes/data_onboarding/process_text_files.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.454853 aixplain-0.2.0/aixplain/utils/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      680 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/utils/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1477 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/utils/config.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     5402 2023-05-11 12:32:02.000000 aixplain-0.2.0/aixplain/utils/file_utils.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.446852 aixplain-0.2.0/aixplain.egg-info/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     3822 2023-05-11 12:45:33.000000 aixplain-0.2.0/aixplain.egg-info/PKG-INFO
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1794 2023-05-11 12:45:33.000000 aixplain-0.2.0/aixplain.egg-info/SOURCES.txt
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        1 2023-05-11 12:45:33.000000 aixplain-0.2.0/aixplain.egg-info/dependency_links.txt
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        1 2023-05-02 15:21:25.000000 aixplain-0.2.0/aixplain.egg-info/not-zip-safe
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)       82 2023-05-11 12:45:33.000000 aixplain-0.2.0/aixplain.egg-info/requires.txt
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)       15 2023-05-11 12:45:33.000000 aixplain-0.2.0/aixplain.egg-info/top_level.txt
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      107 2023-05-11 12:45:33.458853 aixplain-0.2.0/setup.cfg
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     3448 2023-05-11 12:32:02.000000 aixplain-0.2.0/setup.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.458853 aixplain-0.2.0/tests/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)      680 2023-02-28 21:38:19.000000 aixplain-0.2.0/tests/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     4999 2023-05-11 12:32:02.000000 aixplain-0.2.0/tests/asset_factory_test.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     5955 2023-05-11 12:32:02.000000 aixplain-0.2.0/tests/benchmark_test.py
-drwxr-xr-x   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:45:33.458853 aixplain-0.2.0/tests/data_onboarding/
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)        0 2023-05-11 12:32:02.000000 aixplain-0.2.0/tests/data_onboarding/__init__.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1806 2023-05-11 12:32:02.000000 aixplain-0.2.0/tests/data_onboarding/corpus_onboarding_test.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     1837 2023-05-11 12:32:02.000000 aixplain-0.2.0/tests/data_onboarding/dataset_onboarding_test.py
--rw-r--r--   0 thiagocastroferreira  (1006) thiagocastroferreira  (1007)     2402 2023-05-11 12:32:02.000000 aixplain-0.2.0/tests/pipeline_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.692867 aixplain-0.2.1/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4501 2023-05-26 21:35:14.693127 aixplain-0.2.1/PKG-INFO
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2406 2023-05-26 21:35:07.000000 aixplain-0.2.1/README.md
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.662031 aixplain-0.2.1/aixplain/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1237 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      954 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/__version__.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.670773 aixplain-0.2.1/aixplain/enums/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      376 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/enums/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      793 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/enums/data_split.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      842 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/enums/data_subtype.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      887 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/enums/data_type.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      944 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/enums/error_handler.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1007 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/enums/file_type.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1754 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/enums/function.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2159 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/enums/language.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1932 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/enums/license.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      837 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/enums/onboard_status.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      796 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/enums/privacy.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      781 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/enums/storage_type.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.676449 aixplain-0.2.1/aixplain/factories/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1059 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/factories/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1284 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/factories/asset_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    12342 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/factories/benchmark_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    15033 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/factories/corpus_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3673 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/factories/data_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    23619 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/factories/dataset_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2720 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/factories/file_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4549 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/factories/metric_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     7150 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/factories/model_factory.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5854 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/factories/pipeline_factory.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.682994 aixplain-0.2.1/aixplain/modules/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      995 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/modules/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1933 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/modules/asset.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3142 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/modules/benchmark.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2004 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/modules/benchmark_job.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3076 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/modules/corpus.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3505 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/modules/data.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5598 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/modules/dataset.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1918 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/modules/file.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3663 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/modules/metadata.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2247 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/modules/metric.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    10269 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/modules/model.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     8651 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/modules/pipeline.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.683709 aixplain-0.2.1/aixplain/processes/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/processes/__init__.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.685691 aixplain-0.2.1/aixplain/processes/data_onboarding/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/processes/data_onboarding/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)    13947 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/processes/data_onboarding/onboard_functions.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     9610 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/processes/data_onboarding/process_audio_files.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4626 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/processes/data_onboarding/process_text_files.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.687603 aixplain-0.2.1/aixplain/utils/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      680 2023-04-17 18:33:08.000000 aixplain-0.2.1/aixplain/utils/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1192 2023-05-26 21:35:07.000000 aixplain-0.2.1/aixplain/utils/config.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5402 2023-05-10 20:18:24.000000 aixplain-0.2.1/aixplain/utils/file_utils.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.664729 aixplain-0.2.1/aixplain.egg-info/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4501 2023-05-26 21:35:14.000000 aixplain-0.2.1/aixplain.egg-info/PKG-INFO
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1861 2023-05-26 21:35:14.000000 aixplain-0.2.1/aixplain.egg-info/SOURCES.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        1 2023-05-26 21:35:14.000000 aixplain-0.2.1/aixplain.egg-info/dependency_links.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        1 2023-04-17 18:37:22.000000 aixplain-0.2.1/aixplain.egg-info/not-zip-safe
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       82 2023-05-26 21:35:14.000000 aixplain-0.2.1/aixplain.egg-info/requires.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)       15 2023-05-26 21:35:14.000000 aixplain-0.2.1/aixplain.egg-info/top_level.txt
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      107 2023-05-26 21:35:14.693786 aixplain-0.2.1/setup.cfg
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     3448 2023-05-10 20:18:24.000000 aixplain-0.2.1/setup.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.690937 aixplain-0.2.1/tests/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)      680 2023-04-17 18:33:08.000000 aixplain-0.2.1/tests/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     4999 2023-05-10 20:18:24.000000 aixplain-0.2.1/tests/asset_factory_test.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     5955 2023-05-10 20:18:24.000000 aixplain-0.2.1/tests/benchmark_test.py
+drwxr-xr-x   0 thiagocastroferreira   (501) staff       (20)        0 2023-05-26 21:35:14.692459 aixplain-0.2.1/tests/data_onboarding/
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)        0 2023-04-17 18:33:08.000000 aixplain-0.2.1/tests/data_onboarding/__init__.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1806 2023-05-10 20:18:24.000000 aixplain-0.2.1/tests/data_onboarding/corpus_onboarding_test.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     1837 2023-05-10 20:18:24.000000 aixplain-0.2.1/tests/data_onboarding/dataset_onboarding_test.py
+-rw-r--r--   0 thiagocastroferreira   (501) staff       (20)     2402 2023-04-17 18:33:08.000000 aixplain-0.2.1/tests/pipeline_test.py
```

### Comparing `aixplain-0.2.0/PKG-INFO` & `aixplain-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,81 @@
 Metadata-Version: 2.1
 Name: aixplain
-Version: 0.2.0
+Version: 0.2.1
 Summary: aiXplain SDK adds AI functions to software.
 Home-page: https://github.com/aixplain/pipelines/tree/main/docs
 Author: aiXplain
 Author-email: thiago.ferreira@aixplain.com, krishna.durai@aixplain.com, lucas.pavanelli@aixplain.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/aixplain/pipelines/tree/main/docs
 Project-URL: Source, https://github.com/aixplain/aiXplain
+Description: <img src="docs/assets/aixplain-brandmark-common.png" alt="aiXplain logo" title="aiXplain" align="right" height="132" width="85"/>
+        
+        # aiXplain
+        
+        aixplain is a software development kit (SDK) for the [aiXplain](https://aixplain.com/) platform. With aixplain, developers can quickly and easily:
+        
+        - [Discover](https://aixplain.com/platform/discovery/) aiXplain’s ever-expanding catalog of 35,000+ ready-to-use AI models and utilize them.
+        - [Benchmark](https://aixplain.com/platform/benchmark/) AI systems by choosing models, datasets and metrics.
+        - [Design](https://aixplain.com/platform/studio/) their own custom pipelines and run them.
+        
+        [🎓 **Documentation**](docs/user/user_doc.md)
+        
+        🔎 **Find [models](https://platform.aixplain.com/discovery/models), [datasets](https://platform.aixplain.com/discovery/datasets), [metrics](https://platform.aixplain.com/discovery/metrics) on the platform.**
+        
+        :yellow_heart: Our repository is constantly evolving. With the help of the scientific community, we plan to add even more datasets, models, and metrics across domains and tasks.
+        
+        ## Getting Started
+        
+        ### Installation
+        To install simply,
+        ```bash
+        pip install aixplain
+        ```
+        
+        ###  API Key Setup
+        Before you can use the aixplain SDK, you'll need to obtain an API key from our platform. For details refer this [Team API Key Guide](docs/user/api_setup.md).
+        
+        Once you get the API key, you'll  need to add this API key as an environment variable on your system.
+        #### Linux or macOS
+        ```bash
+        export TEAM_API_KEY=YOUR_API_KEY
+        ```
+        #### Windows
+        ```bash
+        set TEAM_API_KEY=YOUR_API_KEY
+        ```
+        #### Jupyter Notebook
+        ```
+        %env TEAM_API_KEY=YOUR_API_KEY
+        ```
+        
+        ## Usage
+        
+        Let’s see how we can use aixplain to run a machine translation model.
+        
+        ```python
+        from aixplain.factories.model_factory  import ModelFactory
+        model = ModelFactory.get("61b27086c45ecd3c10d0608c") # Got the ID of an MT model from on our platform
+        translation = model.run("This is a sample text") # Alternatively, you can input a public URL or provide a file path on your local machine.
+        ```
+        *Check out the [explore section](docs/user/user_doc.md#explore) of our guide on Models to get the ID of your desired model*
+        
+        ## Developer Guide
+        
+        Follow the [Developer Guide](docs/development/developer_guide.md).
+        
+        ## Support
+        Raise issues for support in this repository.  
+        Pull requests are welcome!
+        
+        ## Note
+        The aixtend python package was renamed to aixplain from the release v0.1.1.
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -26,65 +90,7 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
-
-<img src="docs/assets/aixplain-brandmark-common.png" alt="aiXplain logo" title="aiXplain" align="right" height="132" width="85"/>
-
-# aiXplain
-
-aixplain is a software development kit (SDK) for the [aiXplain](https://aixplain.com/) platform. With aixplain, developers can quickly and easily:
-
-- [Discover](https://aixplain.com/platform/discovery/) aiXplain’s ever-expanding catalog of 35,000+ ready-to-use AI models and utilize them.
-- [Benchmark](https://aixplain.com/platform/benchmark/) AI systems by choosing models, datasets and metrics.
-- [Design](https://aixplain.com/platform/studio/) their own custom pipelines and run them.
-
-[🎓 **Documentation**](docs/user/user_doc.md)
-
-🔎 **Find [models](https://platform.aixplain.com/discovery/models), [datasets](https://platform.aixplain.com/discovery/datasets), [metrics](https://platform.aixplain.com/discovery/metrics) on the platform.**
-
-:yellow_heart: Our repository is constantly evolving. With the help of the scientific community, we plan to add even more datasets, models, and metrics across domains and tasks.
-
-## Getting Started
-
-### Installation
-To install simply,
-```bash
-pip install aixplain
-```
-
-###  API Key Setup
-Before you can use the aixplain SDK, you'll need to obtain an API key from our platform. For details refer this [Team API Key Guide](docs/user/api_setup.md).
-
-Once you get the API key, you'll  need to add this API key as an environment variable on your system.
-#### Linux or macOS
-```bash
-export TEAM_API_KEY=YOUR_API_KEY
-```
-#### Windows
-```bash
-set TEAM_API_KEY=YOUR_API_KEY
-```
-## Usage
-
-Let’s see how we can use aixplain to run a machine translation model.
-
-```python
-from aixplain.factories.model_factory  import ModelFactory
-model = ModelFactory.get("61b27086c45ecd3c10d0608c") # Got the ID of an MT model from on our platform
-translation = model.run("This is a sample text")
-```
-*Check out the [explore section](docs/user/user_doc.md#explore) of our guide on Models to get the ID of your desired model*
-
-## Developer Guide
-
-Follow the [Developer Guide](docs/development/developer_guide.md).
-
-## Support
-Raise issues for support in this repository.  
-Pull requests are welcome!
-
-## Note
-The aixtend python package was renamed to aixplain from the release v0.1.1.
```

### Comparing `aixplain-0.2.0/README.md` & `aixplain-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,22 +30,27 @@
 ```bash
 export TEAM_API_KEY=YOUR_API_KEY
 ```
 #### Windows
 ```bash
 set TEAM_API_KEY=YOUR_API_KEY
 ```
+#### Jupyter Notebook
+```
+%env TEAM_API_KEY=YOUR_API_KEY
+```
+
 ## Usage
 
 Let’s see how we can use aixplain to run a machine translation model.
 
 ```python
 from aixplain.factories.model_factory  import ModelFactory
 model = ModelFactory.get("61b27086c45ecd3c10d0608c") # Got the ID of an MT model from on our platform
-translation = model.run("This is a sample text")
+translation = model.run("This is a sample text") # Alternatively, you can input a public URL or provide a file path on your local machine.
 ```
 *Check out the [explore section](docs/user/user_doc.md#explore) of our guide on Models to get the ID of your desired model*
 
 ## Developer Guide
 
 Follow the [Developer Guide](docs/development/developer_guide.md).
```

### Comparing `aixplain-0.2.0/aixplain/__init__.py` & `aixplain-0.2.1/aixplain/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,8 @@
      http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-"""
-
-# Set default logging handler to avoid "No handler found" warnings.
-import logging
-from logging import NullHandler
-
-logging.getLogger(__name__).addHandler(NullHandler())
+"""
```

### Comparing `aixplain-0.2.0/aixplain/__version__.py` & `aixplain-0.2.1/aixplain/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __title__ = "aixplain"
 __description__ = "aiXplain SDK adds AI functions to software."
 __url__ = "https://github.com/aixplain/pipelines/tree/main/docs"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "aiXplain"
 __author_email__ = "thiago.ferreira@aixplain.com, krishna.durai@aixplain.com, lucas.pavanelli@aixplain.com"
 __license__ = "http://www.apache.org/licenses/LICENSE-2.0"
 __copyright__ = """
 Copyright 2023 The aiXplain SDK authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `aixplain-0.2.0/aixplain/enums/data_split.py` & `aixplain-0.2.1/aixplain/enums/data_split.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/enums/data_subtype.py` & `aixplain-0.2.1/aixplain/enums/data_subtype.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/enums/data_type.py` & `aixplain-0.2.1/aixplain/enums/data_type.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/enums/file_type.py` & `aixplain-0.2.1/aixplain/enums/file_type.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/enums/function.py` & `aixplain-0.2.1/aixplain/enums/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,21 @@
 def load_functions():
     api_key = config.TEAM_API_KEY
     aixplain_key = config.AIXPLAIN_API_KEY
     backend_url = config.BACKEND_URL
 
     url = urljoin(backend_url, "sdk/functions")
     if aixplain_key != "":
+        api_key = aixplain_key
         headers = {"x-aixplain-key": aixplain_key, "Content-Type": "application/json"}
     else:
         headers = {"x-api-key": api_key, "Content-Type": "application/json"}
     r = _request_with_retry("get", url, headers=headers)
+    if not 200 <= r.status_code < 300:
+        raise Exception(
+            f'Functions could not be loaded, probably due to the set API key (e.g. "{api_key}") is not valid. For help, please refer to the documentation (https://github.com/aixplain/aixplain#api-key-setup)'
+        )
     resp = r.json()
     return Enum("Function", {w["id"].upper().replace("-", "_"): w["id"] for w in resp["items"]}, type=str)
 
 
 Function = load_functions()
```

### Comparing `aixplain-0.2.0/aixplain/enums/language.py` & `aixplain-0.2.1/aixplain/factories/asset_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,45 @@
 __author__ = "aiXplain"
 
 """
-Copyright 2023 The aiXplain SDK authors
+Copyright 2022 The aiXplain SDK authors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
-Author: aiXplain team
-Date: March 22th 2023
+Author: Duraikrishna Selvaraju, Thiago Castro Ferreira, Shreyas Sharma and Lucas Pavanelli
+Date: December 27th 2022
 Description:
-    Language Enum
+    Asset Factory Class
 """
 
-import logging
-
+from abc import abstractmethod
+from typing import List, Text
+from aixplain.modules.asset import Asset
 from aixplain.utils import config
-from aixplain.utils.file_utils import _request_with_retry
-from enum import Enum
-from urllib.parse import urljoin
 
 
-def load_languages():
+class AssetFactory:
     api_key = config.TEAM_API_KEY
     aixplain_key = config.AIXPLAIN_API_KEY
     backend_url = config.BACKEND_URL
 
-    url = urljoin(backend_url, "sdk/languages")
-    if aixplain_key != "":
-        headers = {"x-aixplain-key": aixplain_key, "Content-Type": "application/json"}
-    else:
-        headers = {"x-api-key": api_key, "Content-Type": "application/json"}
-    r = _request_with_retry("get", url, headers=headers)
-    resp = r.json()
-    languages = {}
-    for w in resp:
-        language = w["value"]
-        language_label = "_".join(w["label"].split())
-        languages[language_label] = {"language": language, "dialect": ""}
-        for dialect in w["dialects"]:
-            dialect_label = "_".join(dialect["label"].split()).upper()
-            dialect_value = dialect["value"]
-
-            languages[language_label + "_" + dialect_label] = {"language": language, "dialect": dialect_value}
-    return Enum("Language", languages, type=dict)
-
-
-Language = load_languages()
+    @abstractmethod
+    def get(self, asset_id: Text) -> Asset:
+        """Create a 'Asset' object from id
+
+        Args:
+            asset_id (str): ID of required asset.
+
+        Returns:
+            Asset: Created 'Asset' object
+        """
+        pass
```

### Comparing `aixplain-0.2.0/aixplain/enums/license.py` & `aixplain-0.2.1/aixplain/enums/license.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,18 +33,23 @@
     try:
         api_key = config.TEAM_API_KEY
         aixplain_key = config.AIXPLAIN_API_KEY
         backend_url = config.BACKEND_URL
 
         url = urljoin(backend_url, "sdk/licenses")
         if aixplain_key != "":
+            api_key = aixplain_key
             headers = {"x-aixplain-key": aixplain_key, "Content-Type": "application/json"}
         else:
             headers = {"x-api-key": api_key, "Content-Type": "application/json"}
         r = _request_with_retry("get", url, headers=headers)
+        if not 200 <= r.status_code < 300:
+            raise Exception(
+                f'Licenses could not be loaded, probably due to the set API key (e.g. "{api_key}") is not valid. For help, please refer to the documentation (https://github.com/aixplain/aixplain#api-key-setup)'
+            )
         resp = r.json()
         return Enum("License", {"_".join(w["name"].split()): w["id"] for w in resp}, type=str)
     except Exception as e:
         logging.exception("License Loading Error")
         raise Exception("License Loading Error")
```

### Comparing `aixplain-0.2.0/aixplain/enums/onboard_status.py` & `aixplain-0.2.1/aixplain/enums/onboard_status.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/enums/privacy.py` & `aixplain-0.2.1/aixplain/enums/privacy.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/enums/storage_type.py` & `aixplain-0.2.1/aixplain/enums/storage_type.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/factories/__init__.py` & `aixplain-0.2.1/aixplain/factories/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from .asset_factory import AssetFactory
 from .benchmark_factory import BenchmarkFactory
 from .corpus_factory import CorpusFactory
+from .data_factory import DataFactory
 from .dataset_factory import DatasetFactory
 from .file_factory import FileFactory
 from .metric_factory import MetricFactory
 from .model_factory import ModelFactory
 from .pipeline_factory import PipelineFactory
```

### Comparing `aixplain-0.2.0/aixplain/factories/benchmark_factory.py` & `aixplain-0.2.1/aixplain/factories/benchmark_factory.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/factories/corpus_factory.py` & `aixplain-0.2.1/aixplain/factories/corpus_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 import aixplain.utils.config as config
 import aixplain.processes.data_onboarding.onboard_functions as onboard_functions
 import json
 import logging
 import shutil
 
 from aixplain.factories.asset_factory import AssetFactory
+from aixplain.factories.data_factory import DataFactory
 from aixplain.modules.corpus import Corpus
 from aixplain.modules.data import Data
 from aixplain.modules.metadata import MetaData
 from aixplain.enums.data_subtype import DataSubtype
 from aixplain.enums.data_type import DataType
+from aixplain.enums.error_handler import ErrorHandler
 from aixplain.enums.function import Function
 from aixplain.enums.language import Language
 from aixplain.enums.license import License
 from aixplain.enums.privacy import Privacy
 from aixplain.utils.file_utils import _request_with_retry
 from aixplain.utils import config
 from pathlib import Path
@@ -234,27 +236,29 @@
         license: License,
         content_path: Union[Union[Text, Path], List[Union[Text, Path]]],
         schema: List[Union[Dict, MetaData]],
         ref_data: List[Any] = [],
         tags: List[Text] = [],
         functions: List[Function] = [],
         privacy: Privacy = Privacy.PRIVATE,
+        error_handler: ErrorHandler = ErrorHandler.SKIP,
     ) -> Dict:
         """Asynchronous call to Upload a corpus to the user's dashboard.
 
         Args:
             name (Text): corpus name
             description (Text): corpus description
             license (License): corpus license
             content_path (Union[Union[Text, Path], List[Union[Text, Path]]]): path to .csv files containing the data
             schema (List[Union[Dict, MetaData]]): meta data
             ref_data (Optional[List[Union[Text, Data]]], optional): referencing data which already exists and should be part of the corpus. Defaults to [].
             tags (Optional[List[Text]], optional): tags that explain the corpus. Defaults to [].
             functions (Optional[List[Function]], optional): AI functions for which the corpus may be used. Defaults to [].
             privacy (Optional[Privacy], optional): visibility of the corpus. Defaults to Privacy.PRIVATE.
+            error_handler (ErrorHandler, optional): how to handle failed rows in the data asset. Defaults to ErrorHandler.SKIP.
 
         Returns:
             Dict: response dict
         """
         folder, return_dict = None, {}
         # check team key
         try:
@@ -275,19 +279,20 @@
                 if isinstance(metadata, dict):
                     schema[i] = MetaData(**metadata)
 
             if len(ref_data) > 0:
                 if isinstance(ref_data[0], Data):
                     ref_data = [w.id for w in ref_data]
                 # check whether the referred data exist. Otherwise, raise an exception
-                for data_id in ref_data:
+                for i, data_id in enumerate(ref_data):
                     if onboard_functions.is_data(data_id) is False:
                         message = f"Data Asset Onboarding Error: Referenced Data {data_id} does not exist."
                         logging.exception(message)
                         raise Exception(message)
+                    ref_data[i] = DataFactory.get(data_id=data_id)
 
             # check whether reserved names are used as data/column names
             for metadata in schema:
                 for forbidden_name in onboard_functions.FORBIDDEN_COLUMN_NAMES:
                     if forbidden_name in [metadata.name, metadata.data_column]:
                         message = f"Data Asset Onboarding Error: {forbidden_name} is reserved name and must not be used as the name of a data or a column."
                         logging.error(message)
@@ -302,15 +307,15 @@
 
             dataset = []
             for i in tqdm(range(len(schema)), desc=" Corpus onboarding progress", position=0):
                 metadata = schema[i]
                 if metadata.privacy is None:
                     metadata.privacy = privacy
 
-                files, data_column_idx, start_column_idx, end_column_idx = onboard_functions.process_data_files(
+                files, data_column_idx, start_column_idx, end_column_idx, nrows = onboard_functions.process_data_files(
                     data_asset_name=name, metadata=metadata, paths=paths, folder=name
                 )
 
                 dataset.append(
                     Data(
                         id="",
                         name=metadata.name,
@@ -319,29 +324,37 @@
                         privacy=metadata.privacy,
                         onboard_status="onboarding",
                         data_column=data_column_idx,
                         start_column=start_column_idx,
                         end_column=end_column_idx,
                         files=files,
                         languages=metadata.languages,
+                        length=nrows,
                     )
                 )
 
+            # check alignment
+            sizes = [d.length for d in dataset] + [d.length for d in ref_data]
+            assert (
+                len(set(sizes)) == 1
+            ), f"Data Asset Onboarding Error: All data must have the same number of rows. Lengths: {str(set(sizes))}"
+
             corpus = Corpus(
                 id="",
                 name=name,
                 description=description,
                 data=dataset,
                 functions=functions,
                 tags=tags,
                 license=license,
                 privacy=privacy,
                 onboard_status="onboarding",
             )
-            corpus_payload = onboard_functions.build_payload_corpus(corpus, ref_data)
+
+            corpus_payload = onboard_functions.build_payload_corpus(corpus, [ref.id for ref in ref_data], error_handler)
 
             response = onboard_functions.create_data_asset(corpus_payload)
             if response["success"] is True:
                 return_dict = {"status": response["status"], "asset_id": response["asset_id"]}
             else:
                 raise Exception(response["error"])
             shutil.rmtree(folder)
```

### Comparing `aixplain-0.2.0/aixplain/factories/dataset_factory.py` & `aixplain-0.2.1/aixplain/factories/dataset_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 import aixplain.utils.config as config
 import aixplain.processes.data_onboarding.onboard_functions as onboard_functions
 import json
 import logging
 import shutil
 
 from aixplain.factories.asset_factory import AssetFactory
+from aixplain.factories.data_factory import DataFactory
 from aixplain.modules.data import Data
 from aixplain.modules.dataset import Dataset
 from aixplain.modules.metadata import MetaData
 from aixplain.enums.data_subtype import DataSubtype
 from aixplain.enums.data_type import DataType
+from aixplain.enums.error_handler import ErrorHandler
 from aixplain.enums.function import Function
 from aixplain.enums.language import Language
 from aixplain.enums.license import License
 from aixplain.enums.privacy import Privacy
 from aixplain.utils.file_utils import _request_with_retry
 from aixplain.utils import config
 from pathlib import Path
@@ -307,14 +309,15 @@
         output_ref_data: Dict[Text, List[Any]] = {},
         hypotheses_ref_data: Dict[Text, Any] = {},
         meta_ref_data: Dict[Text, Any] = {},
         tags: List[Text] = [],
         privacy: Privacy = Privacy.PRIVATE,
         split_labels: Optional[List[Text]] = None,
         split_rate: Optional[List[float]] = None,
+        error_handler: ErrorHandler = ErrorHandler.SKIP,
     ) -> Dict:
         """Dataset Onboard
 
         Args:
             name (Text): dataset name
             description (Text): dataset description
             license (License): dataset license
@@ -326,22 +329,23 @@
             metadata_schema (List[Union[Dict, MetaData]], optional): metadata of metadata information of the dataset. Defaults to [].
             input_ref_data (Dict[Text, Any], optional): reference to input data which is already in the platform. Defaults to {}.
             output_ref_data (Dict[Text, List[Any]], optional): reference to output data which is already in the platform. Defaults to {}.
             hypotheses_ref_data (Dict[Text, Any], optional): hypotheses which are already in the platform. Defaults to {}.
             meta_ref_data (Dict[Text, Any], optional): metadata which is already in the platform. Defaults to {}.
             tags (List[Text], optional): datasets description tags. Defaults to [].
             privacy (Privacy, optional): dataset privacy. Defaults to Privacy.PRIVATE.
+            error_handler (ErrorHandler, optional): how to handle failed rows in the data asset. Defaults to ErrorHandler.SKIP.
 
         Returns:
             Dict: dataset onboard status
         """
         assert (split_labels is not None and split_rate is not None) or (
             split_labels is None and split_rate is None
         ), "Data Asset Onboarding Error: Make sure you set the split labels values as well as their rates."
-        folder, return_dict = None, {}
+        folder, return_dict, ref_data = None, {}, []
         # check team key
         try:
             if config.TEAM_API_KEY.strip() == "":
                 message = "Data Asset Onboarding Error: Update your team key on the environment variable TEAM_API_KEY before the corpus onboarding process."
                 logging.exception(message)
                 raise Exception(message)
 
@@ -376,45 +380,49 @@
                     input_ref_data[input_data] = input_ref_data[input_data].id
                 # check whether the referred data exist. Otherwise, raise an exception
                 data_id = input_ref_data[input_data]
                 if onboard_functions.is_data(data_id) is False:
                     message = f"Data Asset Onboarding Error: Referenced Input Data {data_id} does not exist."
                     logging.exception(message)
                     raise Exception(message)
+                ref_data.append(DataFactory.get(data_id=data_id))
 
             for output_data in output_ref_data:
                 if len(output_ref_data[output_data]) > 0:
                     if isinstance(output_ref_data[output_data][0], Data):
                         output_ref_data[output_data] = [w.id for w in output_ref_data[output_data]]
                     # check whether the referred data exist. Otherwise, raise an exception
                     for data_id in output_ref_data[output_data]:
                         if onboard_functions.is_data(data_id) is False:
                             message = f"Data Asset Onboarding Error: Referenced Output Data {data_id} does not exist."
                             logging.exception(message)
                             raise Exception(message)
+                        ref_data.append(DataFactory.get(data_id=data_id))
 
             for hypdata in hypotheses_ref_data:
                 if isinstance(hypotheses_ref_data[hypdata], Data):
                     hypotheses_ref_data[hypdata] = hypotheses_ref_data[hypdata].id
                 # check whether the referred data exist. Otherwise, raise an exception
                 data_id = hypotheses_ref_data[hypdata]
                 if onboard_functions.is_data(data_id) is False:
                     message = f"Data Asset Onboarding Error: Referenced Hypotheses Data {data_id} does not exist."
                     logging.exception(message)
                     raise Exception(message)
+                ref_data.append(DataFactory.get(data_id=data_id))
 
             for meta_data in meta_ref_data:
                 if isinstance(meta_ref_data[meta_data], Data):
                     meta_ref_data[meta_data] = meta_ref_data[meta_data].id
                 # check whether the referred data exist. Otherwise, raise an exception
                 data_id = meta_ref_data[meta_data]
                 if onboard_functions.is_data(data_id) is False:
                     message = f"Data Asset Onboarding Error: Referenced Meta Data {data_id} does not exist."
                     logging.exception(message)
                     raise Exception(message)
+                ref_data.append(DataFactory.get(data_id=data_id))
 
             # check whether reserved names are used as data/column names
             for schema in [input_schema, output_schema, metadata_schema, hypotheses_schema]:
                 for metadata in schema:
                     for forbidden_name in onboard_functions.FORBIDDEN_COLUMN_NAMES:
                         if forbidden_name in [metadata.name, metadata.data_column]:
                             message = f"Data Asset Onboarding Error: {forbidden_name} is reserved name and must not be used as the name of a data or a column."
@@ -432,31 +440,34 @@
                 split_metadata = onboard_functions.split_data(paths=paths, split_labels=split_labels, split_rate=split_rate)
                 metadata_schema.append(split_metadata)
 
             # process data and create files
             folder = Path(name)
             folder.mkdir(exist_ok=True)
 
-            datasets = {}
+            datasets, sizes = {}, []
             for (key, schema) in [
                 ("inputs", input_schema),
                 ("outputs", output_schema),
                 ("hypotheses", hypotheses_schema),
                 ("meta", metadata_schema),
             ]:
                 datasets[key] = {}
                 for i in tqdm(range(len(schema)), desc=f" Dataset's {key} onboard progress", position=0):
                     metadata = schema[i]
                     if metadata.privacy is None:
                         metadata.privacy = privacy
 
-                    files, data_column_idx, start_column_idx, end_column_idx = onboard_functions.process_data_files(
+                    files, data_column_idx, start_column_idx, end_column_idx, nrows = onboard_functions.process_data_files(
                         data_asset_name=name, metadata=metadata, paths=paths, folder=name
                     )
 
+                    # save size
+                    sizes.append(nrows)
+
                     if metadata.name not in datasets[key]:
                         datasets[key][metadata.name] = []
 
                     datasets[key][metadata.name].append(
                         Data(
                             id=str(uuid4()).replace("-", ""),
                             name=metadata.name,
@@ -465,14 +476,15 @@
                             privacy=metadata.privacy,
                             onboard_status="onboarding",
                             data_column=data_column_idx,
                             start_column=start_column_idx,
                             end_column=end_column_idx,
                             files=files,
                             languages=metadata.languages,
+                            length=nrows,
                         )
                     )
 
             # validate and flat inputs, hypotheses and metadata
             for key_schema in ["inputs", "hypotheses", "meta"]:
                 for input_data in datasets[key_schema]:
                     assert len(datasets[key_schema][input_data]) == 1
@@ -488,16 +500,23 @@
                 hypotheses=datasets["hypotheses"],
                 metadata=datasets["meta"],
                 tags=tags,
                 license=license,
                 privacy=privacy,
                 onboard_status="onboarding",
             )
+
+            # check alignment
+            sizes += [d.length for d in ref_data]
+            assert (
+                len(set(sizes)) == 1
+            ), f"Data Asset Onboarding Error: All data must have the same number of rows. Lengths: {str(set(sizes))}"
+
             dataset_payload = onboard_functions.build_payload_dataset(
-                dataset, input_ref_data, output_ref_data, hypotheses_ref_data, meta_ref_data, tags
+                dataset, input_ref_data, output_ref_data, hypotheses_ref_data, meta_ref_data, tags, error_handler
             )
             assert (
                 len(dataset_payload["input"]) > 0
             ), "Data Asset Onboarding Error: Please specify the input data of your dataset."
             # assert (
             #     len(dataset_payload["output"]) > 0
             # ), "Data Asset Onboarding Error: Please specify the output data of your dataset."
```

### Comparing `aixplain-0.2.0/aixplain/factories/file_factory.py` & `aixplain-0.2.1/aixplain/factories/file_factory.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/factories/metric_factory.py` & `aixplain-0.2.1/aixplain/factories/metric_factory.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/factories/model_factory.py` & `aixplain-0.2.1/aixplain/factories/model_factory.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/factories/pipeline_factory.py` & `aixplain-0.2.1/aixplain/factories/pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/__init__.py` & `aixplain-0.2.1/aixplain/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/asset.py` & `aixplain-0.2.1/aixplain/modules/asset.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/benchmark.py` & `aixplain-0.2.1/aixplain/modules/benchmark.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/benchmark_job.py` & `aixplain-0.2.1/aixplain/modules/benchmark_job.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/corpus.py` & `aixplain-0.2.1/aixplain/modules/corpus.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/data.py` & `aixplain-0.2.1/aixplain/modules/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         onboard_status: OnboardStatus,
         data_column: Optional[Any] = None,
         start_column: Optional[Any] = None,
         end_column: Optional[Any] = None,
         files: List[File] = [],
         languages: List[Language] = [],
         dsubtype: DataSubtype = DataSubtype.OTHER,
+        length: Optional[int] = None,
         **kwargs
     ) -> None:
         """Data Class.
 
         Description:
             Data consists of a list of samples of same type and genre.
 
@@ -59,14 +60,15 @@
             onboard_status (OnboardStatus): onboard status
             data_column (Optional[Any], optional): Column index/name where the data is on a structured file (e.g. CSV). Defaults to None.
             start_column (Optional[Any], optional): Column index/name where the start indexes is on a structured file (e.g. CSV). Defaults to None.
             end_column (Optional[Any], optional): Column index/name where the end indexes is on a structured file (e.g. CSV). Defaults to None.
             files (List[File], optional): List of files where the data instances are stored. Defaults to [].
             languages (List[Language], optional): List of languages which the data consists of. Defaults to [].
             dsubtype (DataSubtype, optional): Data subtype (e.g., age, topic, race, split, etc.), used in datasets metadata. Defaults to Other.
+            length (Optional[int], optional): Number of rows in the Data. Defaults to None.
         """
         self.id = id
         self.name = name
         self.dtype = dtype
         self.privacy = privacy
         if isinstance(onboard_status, str):
             onboard_status = OnboardStatus(onboard_status)
@@ -80,8 +82,9 @@
         self.end_column = end_column
         self.languages = []
         for language in languages:
             if isinstance(language, str):
                 language = Language(language)
             self.languages.append(language)
         self.dsubtype = dsubtype
+        self.length = length
         self.kwargs = kwargs
```

### Comparing `aixplain-0.2.0/aixplain/modules/dataset.py` & `aixplain-0.2.1/aixplain/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/file.py` & `aixplain-0.2.1/aixplain/modules/file.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/metadata.py` & `aixplain-0.2.1/aixplain/modules/metadata.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/metric.py` & `aixplain-0.2.1/aixplain/modules/metric.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/modules/model.py` & `aixplain-0.2.1/aixplain/modules/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,39 +88,42 @@
 
         Returns:
             Dict: Model Information
         """
         clean_additional_info = {k: v for k, v in self.additional_info.items() if v is not None}
         return {"id": self.id, "name": self.name, "supplier": self.supplier, "additional_info": clean_additional_info}
 
-    def __polling(self, poll_url: Text, name: Text = "model_process", wait_time: float = 1.0, timeout: float = 300) -> Dict:
+    def __polling(self, poll_url: Text, name: Text = "model_process", wait_time: float = 0.5, timeout: float = 300) -> Dict:
         """Keeps polling the platform to check whether an asynchronous call is done.
 
         Args:
             poll_url (Text): polling URL
             name (Text, optional): ID given to a call. Defaults to "model_process".
-            wait_time (float, optional): wait time in seconds between polling calls. Defaults to 1.0.
+            wait_time (float, optional): wait time in seconds between polling calls. Defaults to 0.5.
             timeout (float, optional): total polling time. Defaults to 300.
 
         Returns:
             Dict: response obtained by polling call
         """
         logging.info(f"Polling for Model: Start polling for {name}")
         start, end = time.time(), time.time()
+        # keep wait time as 0.2 seconds the minimum
+        wait_time = max(wait_time, 0.2)
         completed = False
         response_body = {"status": "FAILED", "completed": False}
         while not completed and (end - start) < timeout:
             try:
                 response_body = self.poll(poll_url, name=name)
                 completed = response_body["completed"]
 
                 end = time.time()
-                time.sleep(wait_time)
-                if wait_time < 60:
-                    wait_time *= 1.1
+                if completed is False:
+                    time.sleep(wait_time)
+                    if wait_time < 60:
+                        wait_time *= 1.1
             except Exception as e:
                 response_body = {"status": "ERROR", "completed": False, "error": "No response from the service."}
                 logging.error(f"Polling for Model: polling for {name}: {e}")
                 break
         if response_body["completed"] is True:
             try:
                 response_body["status"] = "SUCCESS"
@@ -155,36 +158,44 @@
                 resp["status"] = "IN_PROGRESS"
             logging.info(f"Single Poll for Model: Status of polling for {name}: {resp}")
         except Exception as e:
             resp = {"status": "FAILED"}
             logging.error(f"Single Poll for Model: Error of polling for {name}: {e}")
         return resp
 
-    def run(self, data: Union[Text, Dict], name: Text = "model_process", timeout: float = 300, parameters: Dict = {}) -> Dict:
+    def run(
+        self,
+        data: Union[Text, Dict],
+        name: Text = "model_process",
+        timeout: float = 300,
+        parameters: Dict = {},
+        wait_time: float = 0.5,
+    ) -> Dict:
         """Runs a model call.
 
         Args:
             data (Union[Text, Dict]): link to the input data
             name (Text, optional): ID given to a call. Defaults to "model_process".
             timeout (float, optional): total polling time. Defaults to 300.
             parameters (Dict, optional): optional parameters to the model. Defaults to "{}".
+            wait_time (float, optional): wait time in seconds between polling calls. Defaults to 0.5.
 
         Returns:
             Dict: parsed output from model
         """
         start = time.time()
         try:
             response = self.run_async(data, name=name, parameters=parameters)
             if response["status"] == "FAILED":
                 end = time.time()
                 response["elapsed_time"] = end - start
                 return response
             poll_url = response["url"]
             end = time.time()
-            response = self.__polling(poll_url, name=name, timeout=timeout)
+            response = self.__polling(poll_url, name=name, timeout=timeout, wait_time=wait_time)
             return response
         except Exception as e:
             msg = f"Error in request for {name} - {traceback.format_exc()}"
             logging.error(f"Model Run: Error in running for {name}: {e}")
             end = time.time()
             return {"status": "FAILED", "error": msg, "elapsed_time": end - start}
 
@@ -195,14 +206,18 @@
             data (Union[Text, Dict]): link to the input data
             name (Text, optional): ID given to a call. Defaults to "model_process".
             parameters (Dict, optional): optional parameters to the model. Defaults to "{}".
 
         Returns:
             dict: polling URL in response
         """
+        if self.api_key == "":
+            raise Exception(
+                "A 'TEAM_API_KEY' is required to run a model. For help, please refer to the documentation (https://github.com/aixplain/aixplain#api-key-setup)"
+            )
         headers = {"x-api-key": self.api_key, "Content-Type": "application/json"}
 
         data = FileFactory.to_link(data)
         if isinstance(data, dict):
             payload = data
         else:
             try:
```

### Comparing `aixplain-0.2.0/aixplain/modules/pipeline.py` & `aixplain-0.2.1/aixplain/modules/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,29 +80,30 @@
             name (str, optional): ID given to a call. Defaults to "pipeline_process".
             wait_time (float, optional): wait time in seconds between polling calls. Defaults to 1.0.
             timeout (float, optional): total polling time. Defaults to 20000.0.
 
         Returns:
             dict: response obtained by polling call
         """
-
+        # TO DO: wait_time = to the longest path of the pipeline * minimum waiting time
         logging.debug(f"Polling for Pipeline: Start polling for {name} ")
         start, end = time.time(), time.time()
         completed = False
         response_body = {"status": "FAILED"}
         while not completed and (end - start) < timeout:
             try:
                 response_body = self.poll(poll_url, name=name)
                 logging.debug(f"Polling for Pipeline: Status of polling for {name} : {response_body}")
                 completed = response_body["completed"]
 
                 end = time.time()
-                time.sleep(wait_time)
-                if wait_time < 60:
-                    wait_time *= 1.1
+                if completed is False:
+                    time.sleep(wait_time)
+                    if wait_time < 60:
+                        wait_time *= 1.1
             except Exception as e:
                 logging.error(f"Polling for Pipeline: polling for {name} : Continue")
         if response_body and response_body["status"] == "SUCCESS":
             try:
                 logging.debug(f"Polling for Pipeline: Final status of polling for {name} : SUCCESS - {response_body}")
             except Exception as e:
                 logging.error(f"Polling for Pipeline: Final status of polling for {name} : ERROR - {response_body}")
@@ -128,35 +129,38 @@
         try:
             resp = r.json()
             logging.info(f"Single Poll for Pipeline: Status of polling for {name} : {resp}")
         except Exception as e:
             resp = {"status": "FAILED"}
         return resp
 
-    def run(self, data: Union[Text, Dict], name: Text = "pipeline_process", timeout: float = 20000.0) -> Dict:
+    def run(
+        self, data: Union[Text, Dict], name: Text = "pipeline_process", timeout: float = 20000.0, wait_time: float = 1.0
+    ) -> Dict:
         """Runs a pipeline call.
 
         Args:
             data (Union[Text, Dict]): link to the input data
             name (str, optional): ID given to a call. Defaults to "pipeline_process".
             timeout (float, optional): total polling time. Defaults to 20000.0.
+            wait_time (float, optional): wait time in seconds between polling calls. Defaults to 1.0.
 
         Returns:
             Dict: parsed output from pipeline
         """
         start = time.time()
         try:
             response = self.run_async(data, name=name)
             if response["status"] == "FAILED":
                 end = time.time()
                 response["elapsed_time"] = end - start
                 return response
             poll_url = response["url"]
             end = time.time()
-            response = self.__polling(poll_url, name=name, timeout=timeout)
+            response = self.__polling(poll_url, name=name, timeout=timeout, wait_time=wait_time)
             return response
         except Exception as e:
             error_message = f"Error in request for {name} "
             logging.error(error_message)
             logging.exception(error_message)
             end = time.time()
             return {"status": "FAILED", "error": error_message, "elapsed_time": end - start}
@@ -167,15 +171,18 @@
         Args:
             data (Union[Text, Dict]): link to the input data
             name (Text, optional): ID given to a call. Defaults to "pipeline_process".
 
         Returns:
             Dict: polling URL in response
         """
-
+        if self.api_key == "":
+            raise Exception(
+                "A 'TEAM_API_KEY' is required to run a pipeline. For help, please refer to the documentation (https://github.com/aixplain/aixplain#api-key-setup)"
+            )
         headers = {"x-api-key": self.api_key, "Content-Type": "application/json"}
 
         data = FileFactory.to_link(data)
         if isinstance(data, dict):
             payload = data
         else:
             try:
```

### Comparing `aixplain-0.2.0/aixplain/processes/data_onboarding/onboard_functions.py` & `aixplain-0.2.1/aixplain/processes/data_onboarding/onboard_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 __author__ = "aiXplain"
 
 import aixplain.processes.data_onboarding.process_audio_files as process_audio_files
 import aixplain.processes.data_onboarding.process_text_files as process_text_files
 import aixplain.utils.config as config
 import logging
+import os
 import pandas as pd
 import random
 
 from aixplain.enums.data_subtype import DataSubtype
 from aixplain.enums.data_type import DataType
+from aixplain.enums.error_handler import ErrorHandler
 from aixplain.enums.file_type import FileType
 from aixplain.enums.storage_type import StorageType
 from aixplain.modules.corpus import Corpus
 from aixplain.modules.data import Data
 from aixplain.modules.dataset import Dataset
 from aixplain.modules.file import File
 from aixplain.modules.metadata import MetaData
 from aixplain.utils.file_utils import _request_with_retry
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Text, Union
 from urllib.parse import urljoin
 
-FORBIDDEN_COLUMN_NAMES = ["@VOLUME", "@START_TIME", "@END_TIME", "@ORIGINAL", "@SOURCE", "@INDEX", "@SPLIT"]
+FORBIDDEN_COLUMN_NAMES = ["@VOLUME", "@START_TIME", "@END_TIME", "@ORIGINAL", "@SOURCE", "@INDEX", "@SPLIT", "@STATUS"]
 
 
 def get_paths(input_paths: List[Union[str, Path]]) -> List[Path]:
     """Recursively access all local paths. Check if file extensions are supported.
 
     Args:
         input_paths (List[Union[str, Path]]): list of input pahts including folders and files
@@ -47,45 +49,56 @@
                     logging.warning(f"Data Asset Onboarding: File Extension not Supported ({str(path)})")
         else:
             extension = FileType(path.suffix)
             if extension == FileType.CSV:
                 paths.append(path)
             else:
                 logging.warning(f"Data Asset Onboarding: File Extension not Supported ({str(path)})")
+
+    # check CSV sizes
+    for path in paths:
+        assert (
+            os.path.getsize(path) <= 100000000
+        ), f'Data Asset Onboarding Error: CSV file "{path}" exceeds the size limit of 1 GB.'
     return paths
 
 
 def process_data_files(
     data_asset_name: str, metadata: MetaData, paths: List, folder: Optional[Union[str, Path]] = None
-) -> Tuple[List[File], int, int, int]:
+) -> Tuple[List[File], int, int, int, int]:
     """Process a list of local files, compress and upload them to pre-signed URLs in S3
 
     Args:
         data_asset_name (str): name of the data asset
         metadata (MetaData): meta data of the asset
         paths (List): list of paths to local files
         folder (Union[str, Path], optional): local folder to save compressed files before upload them to s3. Defaults to data_asset_name.
 
     Returns:
-        Tuple[List[File], int]: list of s3 links; data, start and end columns index
+        Tuple[List[File], int, int, int]: list of s3 links; data, start and end columns index; and number of rows
     """
     if folder is None:
         folder = Path(data_asset_name)
     elif isinstance(folder, str):
         folder = Path(folder)
 
     files = []
-    data_column_idx, start_column_idx, end_column_idx = -1, -1, -1
+    data_column_idx, start_column_idx, end_column_idx, nrows, = (
+        -1,
+        -1,
+        -1,
+        0,
+    )
     if metadata.dtype in [DataType.TEXT, DataType.LABEL]:
-        files, data_column_idx = process_text_files.run(metadata=metadata, paths=paths, folder=folder)
+        files, data_column_idx, nrows = process_text_files.run(metadata=metadata, paths=paths, folder=folder)
     elif metadata.dtype in [DataType.AUDIO]:
-        files, data_column_idx, start_column_idx, end_column_idx = process_audio_files.run(
+        files, data_column_idx, start_column_idx, end_column_idx, nrows = process_audio_files.run(
             metadata=metadata, paths=paths, folder=folder
         )
-    return files, data_column_idx, start_column_idx, end_column_idx
+    return files, data_column_idx, start_column_idx, end_column_idx, nrows
 
 
 def build_payload_data(data: Data) -> Dict:
     """Create data payload to call coreengine on Corpus/Dataset onboard
 
     Args:
         data (Data): data object
@@ -112,28 +125,30 @@
             data_json["endTimeColumn"] = data.end_column
         else:
             data_json["startColumn"] = data.start_column
             data_json["endColumn"] = data.end_column
     return data_json
 
 
-def build_payload_corpus(corpus: Corpus, ref_data: List[Text]) -> Dict:
+def build_payload_corpus(corpus: Corpus, ref_data: List[Text], error_handler: ErrorHandler) -> Dict:
     """Create corpus payload to call coreengine on the onboard process
 
     Args:
         corpus (Corpus): corpus object
         ref_data (List[Text]): list of referred data
+        error_handler (ErrorHandler): how to handle failed rows
 
     Returns:
         Dict: payload
     """
     payload = {
         "name": corpus.name,
         "description": corpus.description,
         "suggestedFunctions": [f.value for f in corpus.functions],
+        "onboardingErrorsPolicy": error_handler.value,
         "tags": corpus.tags,
         "pricing": {"type": "FREE", "cost": 0},
         "privacy": corpus.privacy.value,
         "license": {"typeId": corpus.license.value},
         "refData": ref_data,
         "data": [],
     }
@@ -147,24 +162,26 @@
 def build_payload_dataset(
     dataset: Dataset,
     input_ref_data: Dict[Text, Any],
     output_ref_data: Dict[Text, List[Any]],
     hypotheses_ref_data: Dict[Text, Any],
     meta_ref_data: Dict[Text, Any],
     tags: List[Text],
+    error_handler: ErrorHandler,
 ) -> Dict:
     """Generate onboard payload to coreengine
 
     Args:
         dataset (Dataset): dataset to be onboard
         input_ref_data (Dict[Text, Any]): reference to existent input data
         output_ref_data (Dict[Text, List[Any]]): reference to existent output data
         hypotheses_ref_data (Dict[Text, Any]): reference to existent hypotheses to the target data
         meta_ref_data (Dict[Text, Any]): reference to existent metadata
         tags (List[Text]): description tags
+        error_handler (ErrorHandler): how to handle failed rows
 
     Returns:
         Dict: onboard payload
     """
     # compute ref data
     flat_input_ref_data = list(input_ref_data.values())
     flat_output_ref_data = [item for sublist in list(output_ref_data.values()) for item in sublist]
@@ -172,14 +189,15 @@
     flat_hypotheses_ref_data = list(hypotheses_ref_data.values())
     ref_data = flat_input_ref_data + flat_output_ref_data + flat_meta_ref_data + flat_hypotheses_ref_data
 
     payload = {
         "name": dataset.name,
         "description": dataset.description,
         "function": dataset.function.value,
+        "onboardingErrorsPolicy": error_handler.value,
         "tags": dataset.tags,
         "privacy": dataset.privacy.value,
         "license": {"typeId": dataset.license.value},
         "refData": ref_data,
         "tags": tags,
         "data": [],
         "input": [],
```

### Comparing `aixplain-0.2.0/aixplain/processes/data_onboarding/process_audio_files.py` & `aixplain-0.2.1/aixplain/processes/data_onboarding/process_audio_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 def compress_folder(folder_path: str):
     with tarfile.open(folder_path + ".tgz", "w:gz") as tar:
         for name in os.listdir(folder_path):
             tar.add(os.path.join(folder_path, name))
     return folder_path + ".tgz"
 
 
-def run(metadata: MetaData, paths: List, folder: Path, batch_size: int = 100) -> Tuple[List[File], int, int, int]:
+def run(metadata: MetaData, paths: List, folder: Path, batch_size: int = 100) -> Tuple[List[File], int, int, int, int]:
     """Process a list of local audio files, compress and upload them to pre-signed URLs in S3
 
     Explanation:
         Each audio on "paths" is processed. If the audio is in a public link, this link is added into an index CSV file.
         If the audio is in a local path, it will be copied into a local folder and its path will be added to the index CSV file.
         The audios are processed in batches such that at each "batch_size" audios, the index CSV file is uploaded into a pre-signed URL in s3 and reset.
         If the audios are stored locally, the local folder is compressed into a .tgz file and also uploaded into S3.
 
     Args:
         metadata (MetaData): meta data of the asset
         paths (List): list of paths to local files
         folder (Path): local folder to save compressed files before upload them to s3.
 
     Returns:
-        Tuple[List[File], int, int, int]: list of s3 links; data, start and end columns index
+        Tuple[List[File], int, int, int]: list of s3 links; data, start and end columns index, and number of rows
     """
     # if files are stored locally, create a folder to store it
     audio_folder = Path(".")
     if metadata.storage_type == StorageType.FILE:
         audio_folder = Path(os.path.join(folder, "data"))
         audio_folder.mkdir(exist_ok=True)
 
@@ -66,14 +66,18 @@
             except Exception as e:
                 message = f'Data Asset Onboarding Error: Column "{metadata.name}" not found in the local file "{path}".'
                 logging.exception(message)
                 raise Exception(message)
 
             # adding audios
             if metadata.storage_type == StorageType.FILE:
+                #
+                assert (
+                    os.path.getsize(audio_path) <= 50000000
+                ), f'Data Asset Onboarding Error: Local audio file "{audio_path}" exceeds the size limit of 50 MB.'
                 fname = os.path.basename(audio_path)
                 new_path = os.path.join(audio_folder, fname)
                 if os.path.exists(new_path) is False:
                     shutil.copy2(audio_path, new_path)
                 batch.append(fname)
             else:
                 batch.append(audio_path)
@@ -193,8 +197,8 @@
         df.to_csv(index_file_name, compression="gzip", index=False)
         s3_link = upload_data(index_file_name, content_type="text/csv", content_encoding="gzip")
         files.append(File(path=s3_link, extension=FileType.CSV, compression="gzip"))
         # get data column index
         data_column_idx = df.columns.to_list().index(metadata.name)
         # restart batch variables
         batch, start_times, end_times = [], [], []
-    return files, data_column_idx, start_column_idx, end_column_idx
+    return files, data_column_idx, start_column_idx, end_column_idx, idx
```

### Comparing `aixplain-0.2.0/aixplain/processes/data_onboarding/process_text_files.py` & `aixplain-0.2.1/aixplain/processes/data_onboarding/process_text_files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __author__ = "thiagocastroferreira"
 
 import logging
+import os
 import pandas as pd
 
 from aixplain.enums.file_type import FileType
 from aixplain.enums.storage_type import StorageType
 from aixplain.modules.file import File
 from aixplain.modules.metadata import MetaData
 from aixplain.utils.file_utils import upload_data
@@ -20,35 +21,39 @@
         content (str): URL with text, local path with text or textual content
         storage_type (StorageType): type of storage: URL, local path or textual content
 
     Returns:
         Text: textual content
     """
     if storage_type == StorageType.FILE:
+        # Check the size of file and assert a limit of 50 MB
+        assert (
+            os.path.getsize(content) <= 25000000
+        ), f'Data Asset Onboarding Error: Local text file "{content}" exceeds the size limit of 25 MB.'
         with open(content) as f:
             text = f.read()
     else:
         text = content
     return text
 
 
-def run(metadata: MetaData, paths: List, folder: Path, batch_size: int = 1000) -> Tuple[List[File], int]:
+def run(metadata: MetaData, paths: List, folder: Path, batch_size: int = 1000) -> Tuple[List[File], int, int]:
     """Process a list of local textual files, compress and upload them to pre-signed URLs in S3
 
     Explanation:
         Each text on "paths" is processed. If the text is in a public link or local file, it will be downloaded and added to an index CSV file.
         The texts are processed in batches such that at each "batch_size" texts, the index CSV file is uploaded into a pre-signed URL in s3 and reset.
 
     Args:
         metadata (MetaData): meta data of the asset
         paths (List): list of paths to local files
         folder (Path): local folder to save compressed files before upload them to s3.
 
     Returns:
-        Tuple[List[File], int]: list of s3 links and data colum index
+        Tuple[List[File], int, int]: list of s3 links, data colum index and number of rows
     """
     logging.debug(f'Data Asset Onboarding: Processing "{metadata.name}".')
     idx = 0
     data_column_idx = -1
     files, batch = [], []
     for i in tqdm(range(len(paths)), desc=f' Data "{metadata.name}" onboarding progress', position=1, leave=False):
         path = paths[i]
@@ -69,38 +74,19 @@
                 logging.exception(message)
                 raise Exception(message)
 
             try:
                 text = process_text(text_path, metadata.storage_type)
                 batch.append(text)
             except Exception as e:
-                logging.warning(
-                    f'Data Asset Onboarding: The instance "{row}" of "{metadata.name}" could not be processed and will be skipped.'
-                )
-
-            # if split_data is not None:
-            #     try:
-            #         split_row = str(row[split_data.name]).upper()
-            #     except Exception as e:
-            #         message = (
-            #             f'Data Asset Onboarding Error: Split Column "{split_data.name}" not found in the local file {path}.'
-            #         )
-            #         logging.exception(message)
-            #         raise Exception(message)
-
-            #     assert split_row in [
-            #         "TRAIN",
-            #         "VALIDATION",
-            #         "TEST",
-            #     ], f'Data Asset Onboarding Error: Split Column must consist of "TRAIN", "VALIDATION", "TEST" labels.'
-
-            #     split.append(split_row)
+                logging.exception(e)
+                raise Exception(e)
 
             idx += 1
-            if ((idx + 1) % batch_size) == 0:
+            if ((idx) % batch_size) == 0:
                 batch_index = str(len(files) + 1).zfill(8)
                 file_name = f"{folder}/{metadata.name}-{batch_index}.csv.gz"
 
                 df = pd.DataFrame({metadata.name: batch})
                 start, end = idx - len(batch), idx
                 df["@INDEX"] = range(start, end)
                 df.to_csv(file_name, compression="gzip", index=False)
@@ -119,8 +105,8 @@
         df["@INDEX"] = range(start, end)
         df.to_csv(file_name, compression="gzip", index=False)
         s3_link = upload_data(file_name, content_type="text/csv", content_encoding="gzip")
         files.append(File(path=s3_link, extension=FileType.CSV, compression="gzip"))
         # get data column index
         data_column_idx = df.columns.to_list().index(metadata.name)
         batch = []
-    return files, data_column_idx
+    return files, data_column_idx, idx
```

### Comparing `aixplain-0.2.0/aixplain/utils/__init__.py` & `aixplain-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain/utils/config.py` & `aixplain-0.2.1/aixplain/utils/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,28 +9,21 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import warnings
 import os
 import logging
-from dotenv import load_dotenv
 
 logger = logging.getLogger(__name__)
 
-load_dotenv()
 BACKEND_URL = os.getenv("BACKEND_URL", "https://platform-api.aixplain.com/")
 PIPELINES_RUN_URL = os.getenv("PIPELINES_RUN_URL", "https://platform-api.aixplain.com/assets/pipeline/execution/run")
 MODELS_RUN_URL = os.getenv("MODELS_RUN_URL", "https://models.aixplain.com/api/v1/execute")
 # GET THE API KEY FROM CMD
 TEAM_API_KEY = os.getenv("TEAM_API_KEY", "")
 AIXPLAIN_API_KEY = os.getenv("AIXPLAIN_API_KEY", "")
-if TEAM_API_KEY == "" and AIXPLAIN_API_KEY == "":
-    logger.warning(
-        "'TEAM_API_KEY' has not been set properly. For help, please refer to the documentation(https://github.com/aixplain/aixplain#api-key-setup)"
-    )
 PIPELINE_API_KEY = os.getenv("PIPELINE_API_KEY", "")
 MODEL_API_KEY = os.getenv("MODEL_API_KEY", "")
 LOG_LEVEL = os.getenv("LOG_LEVEL", "INFO")
```

### Comparing `aixplain-0.2.0/aixplain/utils/file_utils.py` & `aixplain-0.2.1/aixplain/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/aixplain.egg-info/PKG-INFO` & `aixplain-0.2.1/aixplain.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,81 @@
 Metadata-Version: 2.1
 Name: aixplain
-Version: 0.2.0
+Version: 0.2.1
 Summary: aiXplain SDK adds AI functions to software.
 Home-page: https://github.com/aixplain/pipelines/tree/main/docs
 Author: aiXplain
 Author-email: thiago.ferreira@aixplain.com, krishna.durai@aixplain.com, lucas.pavanelli@aixplain.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/aixplain/pipelines/tree/main/docs
 Project-URL: Source, https://github.com/aixplain/aiXplain
+Description: <img src="docs/assets/aixplain-brandmark-common.png" alt="aiXplain logo" title="aiXplain" align="right" height="132" width="85"/>
+        
+        # aiXplain
+        
+        aixplain is a software development kit (SDK) for the [aiXplain](https://aixplain.com/) platform. With aixplain, developers can quickly and easily:
+        
+        - [Discover](https://aixplain.com/platform/discovery/) aiXplain’s ever-expanding catalog of 35,000+ ready-to-use AI models and utilize them.
+        - [Benchmark](https://aixplain.com/platform/benchmark/) AI systems by choosing models, datasets and metrics.
+        - [Design](https://aixplain.com/platform/studio/) their own custom pipelines and run them.
+        
+        [🎓 **Documentation**](docs/user/user_doc.md)
+        
+        🔎 **Find [models](https://platform.aixplain.com/discovery/models), [datasets](https://platform.aixplain.com/discovery/datasets), [metrics](https://platform.aixplain.com/discovery/metrics) on the platform.**
+        
+        :yellow_heart: Our repository is constantly evolving. With the help of the scientific community, we plan to add even more datasets, models, and metrics across domains and tasks.
+        
+        ## Getting Started
+        
+        ### Installation
+        To install simply,
+        ```bash
+        pip install aixplain
+        ```
+        
+        ###  API Key Setup
+        Before you can use the aixplain SDK, you'll need to obtain an API key from our platform. For details refer this [Team API Key Guide](docs/user/api_setup.md).
+        
+        Once you get the API key, you'll  need to add this API key as an environment variable on your system.
+        #### Linux or macOS
+        ```bash
+        export TEAM_API_KEY=YOUR_API_KEY
+        ```
+        #### Windows
+        ```bash
+        set TEAM_API_KEY=YOUR_API_KEY
+        ```
+        #### Jupyter Notebook
+        ```
+        %env TEAM_API_KEY=YOUR_API_KEY
+        ```
+        
+        ## Usage
+        
+        Let’s see how we can use aixplain to run a machine translation model.
+        
+        ```python
+        from aixplain.factories.model_factory  import ModelFactory
+        model = ModelFactory.get("61b27086c45ecd3c10d0608c") # Got the ID of an MT model from on our platform
+        translation = model.run("This is a sample text") # Alternatively, you can input a public URL or provide a file path on your local machine.
+        ```
+        *Check out the [explore section](docs/user/user_doc.md#explore) of our guide on Models to get the ID of your desired model*
+        
+        ## Developer Guide
+        
+        Follow the [Developer Guide](docs/development/developer_guide.md).
+        
+        ## Support
+        Raise issues for support in this repository.  
+        Pull requests are welcome!
+        
+        ## Note
+        The aixtend python package was renamed to aixplain from the release v0.1.1.
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -26,65 +90,7 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
-
-<img src="docs/assets/aixplain-brandmark-common.png" alt="aiXplain logo" title="aiXplain" align="right" height="132" width="85"/>
-
-# aiXplain
-
-aixplain is a software development kit (SDK) for the [aiXplain](https://aixplain.com/) platform. With aixplain, developers can quickly and easily:
-
-- [Discover](https://aixplain.com/platform/discovery/) aiXplain’s ever-expanding catalog of 35,000+ ready-to-use AI models and utilize them.
-- [Benchmark](https://aixplain.com/platform/benchmark/) AI systems by choosing models, datasets and metrics.
-- [Design](https://aixplain.com/platform/studio/) their own custom pipelines and run them.
-
-[🎓 **Documentation**](docs/user/user_doc.md)
-
-🔎 **Find [models](https://platform.aixplain.com/discovery/models), [datasets](https://platform.aixplain.com/discovery/datasets), [metrics](https://platform.aixplain.com/discovery/metrics) on the platform.**
-
-:yellow_heart: Our repository is constantly evolving. With the help of the scientific community, we plan to add even more datasets, models, and metrics across domains and tasks.
-
-## Getting Started
-
-### Installation
-To install simply,
-```bash
-pip install aixplain
-```
-
-###  API Key Setup
-Before you can use the aixplain SDK, you'll need to obtain an API key from our platform. For details refer this [Team API Key Guide](docs/user/api_setup.md).
-
-Once you get the API key, you'll  need to add this API key as an environment variable on your system.
-#### Linux or macOS
-```bash
-export TEAM_API_KEY=YOUR_API_KEY
-```
-#### Windows
-```bash
-set TEAM_API_KEY=YOUR_API_KEY
-```
-## Usage
-
-Let’s see how we can use aixplain to run a machine translation model.
-
-```python
-from aixplain.factories.model_factory  import ModelFactory
-model = ModelFactory.get("61b27086c45ecd3c10d0608c") # Got the ID of an MT model from on our platform
-translation = model.run("This is a sample text")
-```
-*Check out the [explore section](docs/user/user_doc.md#explore) of our guide on Models to get the ID of your desired model*
-
-## Developer Guide
-
-Follow the [Developer Guide](docs/development/developer_guide.md).
-
-## Support
-Raise issues for support in this repository.  
-Pull requests are welcome!
-
-## Note
-The aixtend python package was renamed to aixplain from the release v0.1.1.
```

### Comparing `aixplain-0.2.0/aixplain.egg-info/SOURCES.txt` & `aixplain-0.2.1/aixplain.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 aixplain.egg-info/not-zip-safe
 aixplain.egg-info/requires.txt
 aixplain.egg-info/top_level.txt
 aixplain/enums/__init__.py
 aixplain/enums/data_split.py
 aixplain/enums/data_subtype.py
 aixplain/enums/data_type.py
+aixplain/enums/error_handler.py
 aixplain/enums/file_type.py
 aixplain/enums/function.py
 aixplain/enums/language.py
 aixplain/enums/license.py
 aixplain/enums/onboard_status.py
 aixplain/enums/privacy.py
 aixplain/enums/storage_type.py
 aixplain/factories/__init__.py
 aixplain/factories/asset_factory.py
 aixplain/factories/benchmark_factory.py
 aixplain/factories/corpus_factory.py
+aixplain/factories/data_factory.py
 aixplain/factories/dataset_factory.py
 aixplain/factories/file_factory.py
 aixplain/factories/metric_factory.py
 aixplain/factories/model_factory.py
 aixplain/factories/pipeline_factory.py
 aixplain/modules/__init__.py
 aixplain/modules/asset.py
```

### Comparing `aixplain-0.2.0/setup.py` & `aixplain-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/tests/asset_factory_test.py` & `aixplain-0.2.1/tests/asset_factory_test.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/tests/benchmark_test.py` & `aixplain-0.2.1/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/tests/data_onboarding/corpus_onboarding_test.py` & `aixplain-0.2.1/tests/data_onboarding/corpus_onboarding_test.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/tests/data_onboarding/dataset_onboarding_test.py` & `aixplain-0.2.1/tests/data_onboarding/dataset_onboarding_test.py`

 * *Files identical despite different names*

### Comparing `aixplain-0.2.0/tests/pipeline_test.py` & `aixplain-0.2.1/tests/pipeline_test.py`

 * *Files identical despite different names*


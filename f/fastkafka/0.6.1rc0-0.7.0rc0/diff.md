# Comparing `tmp/fastkafka-0.6.1rc0.tar.gz` & `tmp/fastkafka-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.6.1rc0.tar", last modified: Fri May 19 12:58:29 2023, max compression
+gzip compressed data, was "fastkafka-0.7.0rc0.tar", last modified: Fri May 26 15:52:52 2023, max compression
```

## Comparing `fastkafka-0.6.1rc0.tar` & `fastkafka-0.7.0rc0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11864 2023-05-19 12:02:29.000000 fastkafka-0.6.1rc0/CONTRIBUTING.md
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.6.1rc0/LICENSE
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.6.1rc0/MANIFEST.in
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28431 2023-04-20 13:45:13.000000 fastkafka-0.6.1rc0/README.md
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.874296 fastkafka-0.6.1rc0/fastkafka/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/__init__.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.874296 fastkafka-0.6.1rc0/fastkafka/_application/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_application/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    31006 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_application/app.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7746 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_application/tester.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1631 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_cli.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3879 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_cli_docs.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      852 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_cli_testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/fastkafka/_components/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3705 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    10188 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    16654 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2940 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/benchmarking.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4706 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/fastkafka/_components/encoder/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1640 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2952 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4446 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/logger.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12567 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/meta.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5930 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     8081 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_components/task_streaming.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5090 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    17520 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_docusaurus_helper.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    50547 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    80310 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_modidx.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6095 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/_server.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/fastkafka/_testing/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:53:41.000000 fastkafka-0.6.1rc0/fastkafka/_testing/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    19995 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20456 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12364 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4671 2023-05-19 12:53:39.000000 fastkafka-0.6.1rc0/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-19 12:53:40.000000 fastkafka-0.6.1rc0/fastkafka/encoder.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-19 12:53:38.000000 fastkafka-0.6.1rc0/fastkafka/testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-19 12:58:29.874296 fastkafka-0.6.1rc0/fastkafka.egg-info/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1387 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-03-14 07:23:45.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      611 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-19 12:58:29.000000 fastkafka-0.6.1rc0/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-19 12:53:24.000000 fastkafka-0.6.1rc0/settings.ini
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-19 12:58:29.878296 fastkafka-0.6.1rc0/setup.cfg
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3682 2023-05-19 12:02:29.000000 fastkafka-0.6.1rc0/setup.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12621 2023-05-19 13:11:05.000000 fastkafka-0.7.0rc0/CONTRIBUTING.md
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc0/LICENSE
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc0/MANIFEST.in
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28431 2023-05-23 06:49:06.000000 fastkafka-0.7.0rc0/README.md
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.284406 fastkafka-0.7.0rc0/fastkafka/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/__init__.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.284406 fastkafka-0.7.0rc0/fastkafka/_application/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_application/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    32608 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_application/app.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7773 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_application/tester.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1592 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_cli.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3879 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_cli_docs.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      852 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_cli_testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/fastkafka/_components/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3705 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13315 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    16528 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4695 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/fastkafka/_components/encoder/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3450 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4432 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/logger.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12567 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/meta.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5432 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11253 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5090 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    19749 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_docusaurus_helper.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    50531 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    81099 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_modidx.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6049 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_server.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/fastkafka/_testing/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_testing/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    19995 2023-05-26 15:49:55.000000 fastkafka-0.7.0rc0/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20363 2023-05-26 15:49:55.000000 fastkafka-0.7.0rc0/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12344 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4592 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/encoder.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/executors.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-26 15:49:55.000000 fastkafka-0.7.0rc0/fastkafka/testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.284406 fastkafka-0.7.0rc0/fastkafka.egg-info/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1410 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-23 12:47:36.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      643 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-26 15:49:31.000000 fastkafka-0.7.0rc0/settings.ini
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/setup.cfg
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3729 2023-05-23 06:49:06.000000 fastkafka-0.7.0rc0/setup.py
```

### Comparing `fastkafka-0.6.1rc0/CONTRIBUTING.md` & `fastkafka-0.7.0rc0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,22 @@
 Enhancement suggestions are tracked as [GitHub issues](https://github.com/airtai/fastkafka/issues).
 
 - Use a **clear and descriptive title** for the issue to identify the suggestion.
 - Provide a **step-by-step description of the suggested enhancement** in as many details as possible.
 - **Describe the current behavior** and **explain which behavior you expected to see instead** and why. At this point you can also tell which alternatives do not work for you.
 - **Explain why this enhancement would be useful** to most fastkafka users. You may also want to point out the other projects that solved it better and which could serve as inspiration.
 
+### Your First Code Contribution
+
+A great way to start contributing to FastKafka would be by solving an issue tagged with "good first issue". To find a list of issues that are tagged as "good first issue" and are suitable for newcomers, please visit the following link: [Good first issues](https://github.com/airtai/fastkafka/labels/good%20first%20issue)
+
+These issues are beginner-friendly and provide a great opportunity to get started with contributing to FastKafka. Choose an issue that interests you, follow the contribution process mentioned in [Way of working](#way-of-working) and [Before a PR](#before-a-pr), and help us make FastKafka even better!
+
+If you have any questions or need further assistance, feel free to reach out to us. Happy coding!
+
 ## Development
 
 ### Prepare the dev environment
 
 To start contributing to fastkafka, you first have to prepare the development environment.
 
 #### Clone the fastkafka repository
@@ -172,20 +180,20 @@
 - Function should be an atomic functionality, short and concise
    - Good rule of thumb: your function should be 5-10 lines long usually
 - If there are more than 2 params, enforce keywording using *
    - E.g.: `def function(param1, *, param2, param3): ...`
 - Define typing of arguments and return value
    - If not, mypy tests will fail and a lot of easily avoidable bugs will go undetected
 - After the function cell, write test cells using the assert keyword
-   - Whenever you implement something you should test tat functionality immediateli in the cells below 
+   - Whenever you implement something you should test that functionality immediately in the cells below 
 - Add Google style python docstrings when function is implemented and tested
 
 ### Before a PR
 
-After you have implemented your changes you will want to open a pull request to merge those changes into our main branch. To make this as painless for you and us, please do the following before opening the request (all the commands are to be run in the root of fastkafka project):
+After you have implemented your changes you will want to open a pull request to merge those changes into our main branch. To make this as smooth for you and us, please do the following before opening the request (all the commands are to be run in the root of fastkafka project):
 
 1. Format your notebooks: `nbqa black nbs`
 2. Close, shutdown, and clean the metadata from your notebooks: `nbdev_clean`
 3. Export your code: `nbdev_export`
 4. Run the tests: `nbdev_test`
 5. Test code typing: `mypy fastkafka`
 6. Test code safety with bandit: `bandit -r fastkafka`
```

### Comparing `fastkafka-0.6.1rc0/LICENSE` & `fastkafka-0.7.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/PKG-INFO` & `fastkafka-0.7.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.6.1rc0
+Version: 0.7.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.6.1rc0/README.md` & `fastkafka-0.7.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/__init__.py` & `fastkafka-0.7.0rc0/fastkafka/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.1rc0"
+__version__ = "0.7.0rc0"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/010_Application_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/010_Application_export.ipynb 1
 from ._application.app import FastKafka
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_application/app.py` & `fastkafka-0.7.0rc0/fastkafka/_application/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,32 +7,27 @@
 import asyncio
 import functools
 import inspect
 import json
 import types
 from asyncio import iscoroutinefunction  # do not use the version from inspect
 from collections import namedtuple
-from contextlib import AbstractAsyncContextManager
+from contextlib import asynccontextmanager
 from datetime import datetime, timedelta
 from functools import wraps
 from inspect import signature
 from pathlib import Path
 from typing import *
 from unittest.mock import AsyncMock, MagicMock
 
 import anyio
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
-import fastkafka._components.logger
-
-fastkafka._components.logger.should_supress_timestamps = True
-
-import fastkafka
 from fastkafka._components.aiokafka_consumer_loop import (
     aiokafka_consumer_loop,
     sanitize_kafka_config,
 )
 from fastkafka._components.asyncapi import (
     ConsumeCallable,
     ContactInfo,
@@ -43,15 +38,19 @@
 )
 from .._components.benchmarking import _benchmark
 from .._components.logger import get_logger
 from .._components.meta import delegates, export, filter_using_signature, patch
 from .._components.producer_decorator import ProduceCallable, producer_decorator
 from .._components.task_streaming import StreamExecutor
 
-# %% ../../nbs/015_FastKafka.ipynb 3
+# %% ../../nbs/015_FastKafka.ipynb 2
+if TYPE_CHECKING:
+    from fastapi import FastAPI
+
+# %% ../../nbs/015_FastKafka.ipynb 4
 logger = get_logger(__name__)
 
 # %% ../../nbs/015_FastKafka.ipynb 9
 @delegates(AIOKafkaConsumer, but=["bootstrap_servers"])
 @delegates(AIOKafkaProducer, but=["bootstrap_servers"], keep=True)
 def _get_kafka_config(
     **kwargs: Any,
@@ -148,15 +147,15 @@
     def __init__(
         self,
         *,
         title: Optional[str] = None,
         description: Optional[str] = None,
         version: Optional[str] = None,
         contact: Optional[Dict[str, str]] = None,
-        kafka_brokers: Dict[str, Any],
+        kafka_brokers: Optional[Dict[str, Any]] = None,
         root_path: Optional[Union[Path, str]] = None,
         lifespan: Optional[Callable[["FastKafka"], AsyncContextManager[None]]] = None,
         **kwargs: Any,
     ):
         """Creates FastKafka application
 
         Args:
@@ -165,16 +164,24 @@
             description: optional description for the documentation. If
                 None, the description will be set to empty string
             version: optional version for the documentation. If None,
                 the version will be set to empty string
             contact: optional contact for the documentation. If None, the
                 contact will be set to placeholder values:
                 name='Author' url=HttpUrl(' https://www.google.com ', ) email='noreply@gmail.com'
-            kafka_brokers: dictionary describing kafka brokers used for
-                generating documentation
+            kafka_brokers: dictionary describing kafka brokers used for setting
+                the bootstrap server when running the applicationa and for
+                generating documentation. Defaults to
+                    {
+                        "localhost": {
+                            "url": "localhost",
+                            "description": "local kafka broker",
+                            "port": "9092",
+                        }
+                    }
             root_path: path to where documentation will be created
             lifespan: asynccontextmanager that is used for setting lifespan hooks.
                 __aenter__ is called before app start and __aexit__ after app stop.
                 The lifespan is called whe application is started as async context
                 manager, e.g.:`async with kafka_app...`
 
         """
@@ -190,14 +197,24 @@
 
         self._kafka_service_info = KafkaServiceInfo(
             title=self._title,
             version=self._version,
             description=self._description,
             contact=self._contact_info,
         )
+
+        if kafka_brokers is None:
+            kafka_brokers = {
+                "localhost": {
+                    "url": "localhost",
+                    "description": "local kafka broker",
+                    "port": "9092",
+                }
+            }
+
         self._kafka_brokers = _get_kafka_brokers(kafka_brokers)
 
         self._root_path = Path(".") if root_path is None else Path(root_path)
 
         self._asyncapi_path = self._root_path / "asyncapi"
         (self._asyncapi_path / "docs").mkdir(exist_ok=True, parents=True)
         (self._asyncapi_path / "spec").mkdir(exist_ok=True, parents=True)
@@ -251,14 +268,27 @@
     def is_started(self) -> bool:
         return self._is_started
 
     def _set_bootstrap_servers(self, bootstrap_servers: str) -> None:
         self._kafka_config["bootstrap_servers"] = bootstrap_servers
 
     def set_kafka_broker(self, kafka_broker_name: str) -> None:
+        """
+        Sets the Kafka broker to start FastKafka with
+
+        Args:
+            kafka_broker_name: The name of the Kafka broker to start FastKafka
+
+        Raises:
+            ValueError: If the provided kafka_broker_name is not found in dictionary of kafka_brokers
+
+        Returns:
+            None
+        """
+
         if kafka_broker_name not in self._kafka_brokers.brokers:
             raise ValueError(
                 f"Given kafka_broker_name '{kafka_broker_name}' is not found in kafka_brokers, available options are {self._kafka_brokers.brokers.keys()}"
             )
 
         broker_to_use = self._kafka_brokers.brokers[kafka_broker_name]
         bootstrap_servers = f"{broker_to_use.url}:{broker_to_use.port}"
@@ -350,15 +380,15 @@
 
     async def _shutdown_producers(self) -> None:
         raise NotImplementedError
 
     async def _shutdown_bg_tasks(self) -> None:
         raise NotImplementedError
 
-# %% ../../nbs/015_FastKafka.ipynb 25
+# %% ../../nbs/015_FastKafka.ipynb 26
 def _get_decoder_fn(decoder: str) -> Callable[[bytes, ModelMetaclass], Any]:
     """
     Imports and returns decoder function based on input
     """
     if decoder == "json":
         from fastkafka._components.encoder.json import json_decoder
 
@@ -370,15 +400,15 @@
             raise ModuleNotFoundError(
                 "Unable to import avro packages. Please install FastKafka using the command 'fastkafka[avro]'"
             )
         return avro_decoder
     else:
         raise ValueError(f"Unknown decoder - {decoder}")
 
-# %% ../../nbs/015_FastKafka.ipynb 27
+# %% ../../nbs/015_FastKafka.ipynb 28
 @patch
 @delegates(AIOKafkaConsumer)
 def consumes(
     self: FastKafka,
     topic: Optional[str] = None,
     decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = "json",
     *,
@@ -436,15 +466,15 @@
         decoder_fn = _get_decoder_fn(decoder) if isinstance(decoder, str) else decoder
         self._consumers_store[topic_resolved] = (on_topic, decoder_fn, executor, kwargs)
         setattr(self, on_topic.__name__, on_topic)
         return on_topic
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 29
+# %% ../../nbs/015_FastKafka.ipynb 30
 def _get_encoder_fn(encoder: str) -> Callable[[BaseModel], bytes]:
     """
     Imports and returns encoder function based on input
     """
     if encoder == "json":
         from fastkafka._components.encoder.json import json_encoder
 
@@ -456,15 +486,15 @@
             raise ModuleNotFoundError(
                 "Unable to import avro packages. Please install FastKafka using the command 'fastkafka[avro]'"
             )
         return avro_encoder
     else:
         raise ValueError(f"Unknown encoder - {encoder}")
 
-# %% ../../nbs/015_FastKafka.ipynb 31
+# %% ../../nbs/015_FastKafka.ipynb 32
 @patch
 @delegates(AIOKafkaProducer)
 def produces(
     self: FastKafka,
     topic: Optional[str] = None,
     encoder: Union[str, Callable[[BaseModel], bytes]] = "json",
     *,
@@ -513,22 +543,22 @@
             self._producers_store, to_topic, topic_resolved, encoder_fn=encoder_fn
         )
         setattr(self, to_topic.__name__, decorated)
         return decorated
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 33
+# %% ../../nbs/015_FastKafka.ipynb 34
 @patch
 def get_topics(self: FastKafka) -> Iterable[str]:
     produce_topics = set(self._producers_store.keys())
     consume_topics = set(self._consumers_store.keys())
     return consume_topics.union(produce_topics)
 
-# %% ../../nbs/015_FastKafka.ipynb 35
+# %% ../../nbs/015_FastKafka.ipynb 36
 @patch
 def run_in_background(
     self: FastKafka,
 ) -> Callable[
     [Callable[..., Coroutine[Any, Any, Any]]], Callable[..., Coroutine[Any, Any, Any]]
 ]:
     """
@@ -557,15 +587,15 @@
         )
         self._scheduled_bg_tasks.append(bg_task)
 
         return bg_task
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 39
+# %% ../../nbs/015_FastKafka.ipynb 40
 @patch
 def _populate_consumers(
     self: FastKafka,
     is_shutting_down_f: Callable[[], bool],
 ) -> None:
     default_config: Dict[str, Any] = filter_using_signature(
         AIOKafkaConsumer, **self._kafka_config
@@ -594,15 +624,15 @@
 @patch
 async def _shutdown_consumers(
     self: FastKafka,
 ) -> None:
     if self._kafka_consumer_tasks:
         await asyncio.wait(self._kafka_consumer_tasks)
 
-# %% ../../nbs/015_FastKafka.ipynb 41
+# %% ../../nbs/015_FastKafka.ipynb 42
 # TODO: Add passing of vars
 async def _create_producer(  # type: ignore
     *,
     callback: ProduceCallable,
     default_config: Dict[str, Any],
     override_config: Dict[str, Any],
     producers_list: List[AIOKafkaProducer],
@@ -688,15 +718,15 @@
                 callback,
                 _,
                 override_config,
             ) in self._producers_store.items()
         }
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 43
+# %% ../../nbs/015_FastKafka.ipynb 44
 @patch
 async def _populate_bg_tasks(
     self: FastKafka,
 ) -> None:
     def _start_bg_task(task: Callable[..., Coroutine[Any, Any, Any]]) -> asyncio.Task:
         logger.info(
             f"_populate_bg_tasks() : Starting background task '{task.__name__}'"
@@ -724,15 +754,15 @@
             await task
         except asyncio.CancelledError:
             pass
         logger.info(
             f"_shutdown_bg_tasks() : Execution finished for background task '{task.get_name()}'"
         )
 
-# %% ../../nbs/015_FastKafka.ipynb 45
+# %% ../../nbs/015_FastKafka.ipynb 46
 @patch
 async def _start(self: FastKafka) -> None:
     def is_shutting_down_f(self: FastKafka = self) -> bool:
         return self._is_shutting_down
 
     #     self.create_docs()
     await self._populate_producers()
@@ -749,15 +779,15 @@
     await self._shutdown_bg_tasks()
     await self._shutdown_consumers()
     await self._shutdown_producers()
 
     self._is_shutting_down = False
     self._is_started = False
 
-# %% ../../nbs/015_FastKafka.ipynb 51
+# %% ../../nbs/015_FastKafka.ipynb 52
 @patch
 def create_docs(self: FastKafka) -> None:
     export_async_spec(
         consumers={
             topic: callback
             for topic, (callback, _, _, _) in self._consumers_store.items()
         },
@@ -765,15 +795,15 @@
             topic: callback for topic, (callback, _, _) in self._producers_store.items()
         },
         kafka_brokers=self._kafka_brokers,
         kafka_service_info=self._kafka_service_info,
         asyncapi_path=self._asyncapi_path,
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 55
+# %% ../../nbs/015_FastKafka.ipynb 56
 class AwaitedMock:
     @staticmethod
     def _await_for(f: Callable[..., Any]) -> Callable[..., Any]:
         @delegates(f)
         async def inner(
             *args: Any, f: Callable[..., Any] = f, timeout: int = 60, **kwargs: Any
         ) -> Any:
@@ -801,15 +831,15 @@
 
         for name in o.__dir__():
             if not name.startswith("_"):
                 f = getattr(o, name)
                 if inspect.ismethod(f):
                     setattr(self, name, self._await_for(f))
 
-# %% ../../nbs/015_FastKafka.ipynb 56
+# %% ../../nbs/015_FastKafka.ipynb 57
 @patch
 def create_mocks(self: FastKafka) -> None:
     """Creates self.mocks as a named tuple mapping a new function obtained by calling the original functions and a mock"""
     app_methods = [f for f, _, _, _ in self._consumers_store.values()] + [
         f for f, _, _ in self._producers_store.values()
     ]
     self.AppMocks = namedtuple(  # type: ignore
@@ -870,15 +900,15 @@
                 producer,
                 kwargs,
             )
             for name, (f, producer, kwargs) in self._producers_store.items()
         }
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 61
+# %% ../../nbs/015_FastKafka.ipynb 62
 @patch
 def benchmark(
     self: FastKafka,
     interval: Union[int, timedelta] = 1,
     *,
     sliding_window_size: Optional[int] = None,
 ) -> Callable[[Callable[[I], Optional[O]]], Callable[[I], Optional[O]]]:
@@ -924,7 +954,30 @@
 
         if inspect.iscoroutinefunction(func):
             return async_wrapper  # type: ignore
         else:
             return wrapper
 
     return _decorator
+
+# %% ../../nbs/015_FastKafka.ipynb 64
+@patch
+def fastapi_lifespan(
+    self: FastKafka, kafka_broker_name: str
+) -> Callable[["FastAPI"], AsyncIterator[None]]:
+    """
+    Method for managing the lifespan of a FastAPI application with a specific Kafka broker.
+
+    Args:
+        kafka_broker_name: The name of the Kafka broker to start FastKafka
+
+    Returns:
+        Lifespan function to use for initializing FastAPI
+    """
+
+    @asynccontextmanager
+    async def lifespan(fastapi_app: "FastAPI") -> AsyncIterator[None]:
+        self.set_kafka_broker(kafka_broker_name=kafka_broker_name)
+        async with self:
+            yield
+
+    return lifespan  # type: ignore
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_application/tester.py` & `fastkafka-0.7.0rc0/fastkafka/_application/tester.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import asyncio
 import inspect
 from contextlib import asynccontextmanager
 from typing import *
 
 from pydantic import BaseModel
 
-from .. import KafkaEvent
 from .app import FastKafka
+from .._components.helpers import unwrap_list_type
 from .._components.meta import delegates, export, patch
+from .._components.producer_decorator import unwrap_from_kafka_event
 from .._testing.apache_kafka_broker import ApacheKafkaBroker
 from .._testing.in_memory_broker import InMemoryBroker
 from .._testing.local_redpanda_broker import LocalRedpandaBroker
 
 # %% ../../nbs/016_Tester.ipynb 8
 @export("fastkafka.testing")
 class Tester(FastKafka):
@@ -144,19 +145,15 @@
     async def __aexit__(self, *args: Any) -> None:
         await self._ctx.__aexit__(*args)
 
 # %% ../../nbs/016_Tester.ipynb 13
 def mirror_producer(topic: str, producer_f: Callable[..., Any]) -> Callable[..., Any]:
     msg_type = inspect.signature(producer_f).return_annotation
 
-    if hasattr(msg_type, "__origin__") and msg_type.__origin__ == KafkaEvent:
-        msg_type = msg_type.__args__[0]
-
-    if hasattr(msg_type, "__origin__") and msg_type.__origin__ == list:
-        msg_type = msg_type.__args__[0]
+    msg_type_unwrapped = unwrap_list_type(unwrap_from_kafka_event(msg_type))
 
     async def skeleton_func(msg: BaseModel) -> None:
         pass
 
     mirror_func = skeleton_func
     sig = inspect.signature(skeleton_func)
 
@@ -164,39 +161,43 @@
     mirror_func.__name__ = "on_" + topic.replace(".", "_")
 
     # adjust arg and return val
     sig = sig.replace(
         parameters=[
             inspect.Parameter(
                 name="msg",
-                annotation=msg_type,
+                annotation=msg_type_unwrapped,
                 kind=inspect.Parameter.POSITIONAL_OR_KEYWORD,
             )
         ]
     )
 
     mirror_func.__signature__ = sig  # type: ignore
 
     return mirror_func
 
 # %% ../../nbs/016_Tester.ipynb 16
 def mirror_consumer(topic: str, consumer_f: Callable[..., Any]) -> Callable[..., Any]:
     msg_type = inspect.signature(consumer_f).parameters["msg"]
 
+    msg_type_unwrapped = unwrap_list_type(msg_type)
+
     async def skeleton_func(msg: BaseModel) -> BaseModel:
         return msg
 
     mirror_func = skeleton_func
     sig = inspect.signature(skeleton_func)
 
     # adjust name
     mirror_func.__name__ = "to_" + topic.replace(".", "_")
 
     # adjust arg and return val
-    sig = sig.replace(parameters=[msg_type], return_annotation=msg_type.annotation)
+    sig = sig.replace(
+        parameters=[msg_type], return_annotation=msg_type_unwrapped.annotation
+    )
 
     mirror_func.__signature__ = sig  # type: ignore
     return mirror_func
 
 # %% ../../nbs/016_Tester.ipynb 18
 @patch
 def create_mirrors(self: Tester) -> None:
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_cli.py` & `fastkafka-0.7.0rc0/fastkafka/_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 # %% ../nbs/023_CLI.ipynb 1
 import asyncio
 import multiprocessing
 from typing import *
 
 import typer
 
-from ._components.logger import get_logger, supress_timestamps
-
 from . import _cli_docs, _cli_testing
+from ._components.logger import get_logger
 from ._server import run_fastkafka_server
 
 # %% ../nbs/023_CLI.ipynb 5
-supress_timestamps(False)
 logger = get_logger(__name__, level=20)
 
 # %% ../nbs/023_CLI.ipynb 8
 _app = typer.Typer(help="")
 
 # %% ../nbs/023_CLI.ipynb 9
 @_app.command(
@@ -32,15 +30,15 @@
         help="Number of FastKafka instances to run, defaults to number of CPU cores.",
     ),
     app: str = typer.Argument(
         ...,
         help="input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
     ),
     kafka_broker: str = typer.Option(
-        ...,
+        "localhost",
         help="kafka_broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastaKafka class.",
     ),
 ) -> None:
     try:
         asyncio.run(
             run_fastkafka_server(
                 num_workers=num_workers, app=app, kafka_broker=kafka_broker
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_cli_docs.py` & `fastkafka-0.7.0rc0/fastkafka/_cli_docs.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/_cli_testing.py` & `fastkafka-0.7.0rc0/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/_subprocess.py` & `fastkafka-0.7.0rc0/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.7.0rc0/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/011_ConsumerLoop.ipynb.
 
 # %% auto 0
 __all__ = ['logger', 'AsyncConsume', 'AsyncConsumeMeta', 'SyncConsume', 'SyncConsumeMeta', 'ConsumeCallable', 'EventMetadata',
            'sanitize_kafka_config', 'aiokafka_consumer_loop']
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 1
-import asyncio
 from asyncio import iscoroutinefunction, Task  # do not use the version from inspect
 from typing import *
-from functools import wraps, partial
 from dataclasses import dataclass
-from contextlib import asynccontextmanager
 
-import anyio
 import asyncer
 from aiokafka import AIOKafkaConsumer
-from aiokafka.structs import ConsumerRecord, TopicPartition
-from anyio.streams.memory import MemoryObjectReceiveStream
+from aiokafka.structs import ConsumerRecord
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
 from .logger import get_logger
 from .meta import delegates, export
 from .task_streaming import get_executor, StreamExecutor
 
@@ -56,14 +51,22 @@
     checksum: int
     serialized_key_size: int
     serialized_value_size: int
     headers: Sequence[Tuple[str, bytes]]
 
     @staticmethod
     def create_event_metadata(record: ConsumerRecord) -> "EventMetadata":  # type: ignore
+        """Creates an instance of EventMetadata from a ConsumerRecord.
+
+        Args:
+            record: The Kafka ConsumerRecord.
+
+        Returns:
+            The created EventMetadata instance.
+        """
         return EventMetadata(
             topic=record.topic,
             partition=record.partition,
             offset=record.offset,
             timestamp=record.timestamp,
             timestamp_type=record.timestamp_type,
             value=record.value,
@@ -71,18 +74,23 @@
             key=record.key,
             serialized_key_size=record.serialized_key_size,
             serialized_value_size=record.serialized_value_size,
             headers=record.headers,
         )
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 11
-AsyncConsume = Callable[[BaseModel], Awaitable[None]]
-AsyncConsumeMeta = Callable[[BaseModel, EventMetadata], Awaitable[None]]
-SyncConsume = Callable[[BaseModel], None]
-SyncConsumeMeta = Callable[[BaseModel, EventMetadata], None]
+AsyncConsume = Callable[[Union[List[BaseModel], BaseModel]], Awaitable[None]]
+AsyncConsumeMeta = Callable[
+    [Union[List[BaseModel], BaseModel], Union[List[EventMetadata], EventMetadata]],
+    Awaitable[None],
+]
+SyncConsume = Callable[[Union[List[BaseModel], BaseModel]], None]
+SyncConsumeMeta = Callable[
+    [Union[List[BaseModel], BaseModel], Union[List[EventMetadata], EventMetadata]], None
+]
 
 ConsumeCallable = Union[AsyncConsume, AsyncConsumeMeta, SyncConsume, SyncConsumeMeta]
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 12
 def _callback_parameters_wrapper(
     callback: Union[AsyncConsume, AsyncConsumeMeta]
 ) -> AsyncConsumeMeta:
@@ -92,135 +100,223 @@
         callback: async callable that will be wrapped
 
     Returns:
         Wrapped callback with filtered params
     """
 
     async def _params_wrap(
-        msg: BaseModel,
-        meta: EventMetadata,
+        msg: Union[BaseModel, List[BaseModel]],
+        meta: Union[EventMetadata, List[EventMetadata]],
         callback: Union[AsyncConsume, AsyncConsumeMeta] = callback,
     ) -> None:
         types = list(get_type_hints(callback).values())
-        args: List[Union[BaseModel, EventMetadata]] = [msg]
+        args: List[
+            Union[BaseModel, List[BaseModel], EventMetadata, List[EventMetadata]]
+        ] = [msg]
         if EventMetadata in types:
             args.insert(types.index(EventMetadata), meta)
+        if List[EventMetadata] in types:
+            args.insert(types.index(List[EventMetadata]), meta)
         await callback(*args)  # type: ignore
 
     return _params_wrap
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 16
+# %% ../../nbs/011_ConsumerLoop.ipynb 17
 def _prepare_callback(callback: ConsumeCallable) -> AsyncConsumeMeta:
     """
     Prepares a callback to be used in the consumer loop.
         1. If callback is sync, asyncify it
         2. Wrap the callback into a safe callback for exception handling
 
-    Params:
+    Args:
         callback: async callable that will be prepared for use in consumer
 
     Returns:
         Prepared callback
     """
     async_callback: Union[AsyncConsume, AsyncConsumeMeta] = (
         callback if iscoroutinefunction(callback) else asyncer.asyncify(callback)  # type: ignore
     )
     return _callback_parameters_wrapper(async_callback)
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 18
-async def _stream_msgs(  # type: ignore
-    msgs: Dict[TopicPartition, bytes],
-    send_stream: anyio.streams.memory.MemoryObjectSendStream[Any],
-) -> None:
+# %% ../../nbs/011_ConsumerLoop.ipynb 24
+def _get_single_msg_handlers(  # type: ignore
+    *,
+    consumer: AIOKafkaConsumer,
+    callback: AsyncConsumeMeta,
+    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
+    msg_type: Type[BaseModel],
+    **kwargs: Any,
+) -> Tuple[
+    Callable[
+        [
+            ConsumerRecord,
+            AsyncConsumeMeta,
+            Callable[[bytes, ModelMetaclass], Any],
+            Type[BaseModel],
+        ],
+        Awaitable[None],
+    ],
+    Callable[[AIOKafkaConsumer, Any], Awaitable[List[ConsumerRecord]]],
+]:
     """
-    Decodes and streams the message and topic to the send_stream.
+    Retrieves the message handlers for consuming single messages from a Kafka topic.
+
+    Args:
+        consumer: The Kafka consumer instance.
+        callback: The callback function to handle the consumed message.
+        decoder_fn: The function to decode the consumed message.
+        msg_type: The type of the consumed message.
+        **kwargs: Additional keyword arguments for the consumer.
+
+    Returns:
+        The handle_msg function and poll_consumer function.
+    """
+
+    async def handle_msg(  # type: ignore
+        record: ConsumerRecord,
+        callback: AsyncConsumeMeta = callback,
+        decoder_fn: Callable[[bytes, ModelMetaclass], Any] = decoder_fn,
+        msg_type: Type[BaseModel] = msg_type,
+    ) -> None:
+        await callback(
+            decoder_fn(record.value, msg_type),
+            EventMetadata.create_event_metadata(record),
+        )
 
-    Params:
-        msgs:
-        send_stream:
-    """
-    for topic_partition, topic_msgs in msgs.items():
-        topic = topic_partition.topic
-        try:
-            await send_stream.send(topic_msgs)
-        except Exception as e:
-            logger.warning(
-                f"_stream_msgs(): Unexpected exception '{e.__repr__()}' caught and ignored for topic='{topic_partition.topic}', partition='{topic_partition.partition}' and messages: {topic_msgs!r}"
-            )
-
-
-def _decode_streamed_msgs(  # type: ignore
-    msgs: List[ConsumerRecord], msg_type: BaseModel
-) -> List[BaseModel]:
-    decoded_msgs = [msg_type.parse_raw(msg.value.decode("utf-8")) for msg in msgs]
-    return decoded_msgs
+    async def poll_consumer(  # type: ignore
+        consumer: AIOKafkaConsumer = consumer, kwargs: Any = kwargs
+    ) -> List[ConsumerRecord]:
+        msgs = await consumer.getmany(**kwargs)
+        return [msg for msg_group in msgs.values() for msg in msg_group]
+
+    return handle_msg, poll_consumer
+
+# %% ../../nbs/011_ConsumerLoop.ipynb 26
+def _get_batch_msg_handlers(  # type: ignore
+    *,
+    consumer: AIOKafkaConsumer,
+    callback: AsyncConsumeMeta,
+    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
+    msg_type: Type[BaseModel],
+    **kwargs: Any,
+) -> Tuple[
+    Callable[
+        [
+            List[ConsumerRecord],
+            AsyncConsumeMeta,
+            Callable[[bytes, ModelMetaclass], Any],
+            Type[BaseModel],
+        ],
+        Awaitable[None],
+    ],
+    Callable[[AIOKafkaConsumer, Any], Awaitable[List[List[ConsumerRecord]]]],
+]:
+    """
+    Retrieves the message handlers for consuming messages in batches from a Kafka topic.
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 23
+    Args:
+        consumer: The Kafka consumer instance.
+        callback: The callback function to handle the consumed messages.
+        decoder_fn: The function to decode the consumed messages.
+        msg_type: The type of the consumed messages.
+        **kwargs: Additional keyword arguments for the consumer.
+
+    Returns:
+        The handle_msg function and poll_consumer function.
+    """
+
+    async def handle_msg(  # type: ignore
+        records: List[ConsumerRecord],
+        callback: AsyncConsumeMeta = callback,
+        decoder_fn: Callable[[bytes, ModelMetaclass], Any] = decoder_fn,
+        msg_type: Type[BaseModel] = msg_type,
+    ) -> None:
+        await callback(
+            [decoder_fn(record.value, msg_type) for record in records],
+            [EventMetadata.create_event_metadata(record) for record in records],
+        )
+
+    async def poll_consumer(  # type: ignore
+        consumer: AIOKafkaConsumer = consumer, kwargs: Any = kwargs
+    ) -> List[List[ConsumerRecord]]:
+        msgs = await consumer.getmany(**kwargs)
+        return [value for value in msgs.values() if len(value) > 0]
+
+    return handle_msg, poll_consumer
+
+# %% ../../nbs/011_ConsumerLoop.ipynb 28
 @delegates(AIOKafkaConsumer.getmany)
 async def _aiokafka_consumer_loop(  # type: ignore
     consumer: AIOKafkaConsumer,
     *,
     topic: str,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     callback: ConsumeCallable,
     max_buffer_size: int = 100_000,
-    msg_type: Type[BaseModel],
+    msg_type: Union[Type[List[BaseModel]], Type[BaseModel]],
     is_shutting_down_f: Callable[[], bool],
     executor: Union[str, StreamExecutor, None] = None,
     **kwargs: Any,
 ) -> None:
     """
     Consumer loop for infinite pooling of the AIOKafka consumer for new messages. Calls consumer.getmany()
     and after the consumer return messages or times out, messages are decoded and streamed to defined callback.
 
-    Params:
+    Args:
         topic: Topic to subscribe
         decoder_fn: Function to decode the messages consumed from the topic
         callbacks: Dict of callbacks mapped to their respective topics
         timeout_ms: Time to timeut the getmany request by the consumer
         max_buffer_size: Maximum number of unconsumed messages in the callback buffer
         msg_types: Dict of message types mapped to their respective topics
         is_shutting_down_f: Function for controlling the shutdown of consumer loop
     """
 
     prepared_callback = _prepare_callback(callback)
 
-    async def handle_msg(  # type: ignore
-        record: ConsumerRecord,
-        callback: AsyncConsumeMeta = prepared_callback,
-        decoder_fn: Callable[[bytes, ModelMetaclass], Any] = decoder_fn,
-        msg_type: Type[BaseModel] = msg_type,
-    ) -> None:
-        await callback(
-            decoder_fn(record.value, msg_type),
-            EventMetadata.create_event_metadata(record),
+    if hasattr(msg_type, "__origin__") and msg_type.__origin__ == list:
+        handle_msg, poll_consumer = _get_batch_msg_handlers(
+            consumer=consumer,
+            callback=prepared_callback,
+            decoder_fn=decoder_fn,
+            msg_type=msg_type.__args__[0],  # type: ignore
+            **kwargs,
+        )
+    else:
+        handle_msg, poll_consumer = _get_single_msg_handlers(
+            consumer=consumer,
+            callback=prepared_callback,
+            decoder_fn=decoder_fn,
+            msg_type=msg_type,  # type: ignore
+            **kwargs,
         )
 
-    async def poll_consumer(kwargs: Any = kwargs) -> List[ConsumerRecord]:  # type: ignore
-        msgs = await consumer.getmany(**kwargs)
-        return [msg for msg_group in msgs.values() for msg in msg_group]
-
-    await get_executor(executor).run(is_shutting_down_f, poll_consumer, handle_msg)
+    await get_executor(executor).run(
+        is_shutting_down_f=is_shutting_down_f,
+        generator=poll_consumer,  # type: ignore
+        processor=handle_msg,  # type: ignore
+    )
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 28
+# %% ../../nbs/011_ConsumerLoop.ipynb 35
 def sanitize_kafka_config(**kwargs: Any) -> Dict[str, Any]:
     """Sanitize Kafka config"""
     return {k: "*" * len(v) if "pass" in k.lower() else v for k, v in kwargs.items()}
 
-# %% ../../nbs/011_ConsumerLoop.ipynb 30
+# %% ../../nbs/011_ConsumerLoop.ipynb 37
 @delegates(AIOKafkaConsumer)
 @delegates(_aiokafka_consumer_loop, keep=True)
 async def aiokafka_consumer_loop(
     topic: str,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     *,
     timeout_ms: int = 100,
     max_buffer_size: int = 100_000,
     callback: ConsumeCallable,
-    msg_type: Type[BaseModel],
+    msg_type: Union[Type[List[BaseModel]], Type[BaseModel]],
     is_shutting_down_f: Callable[[], bool],
     executor: Union[str, StreamExecutor, None] = None,
     **kwargs: Any,
 ) -> None:
     """Consumer loop for infinite pooling of the AIOKafka consumer for new messages. Creates and starts AIOKafkaConsumer
     and runs _aio_kafka_consumer loop fo infinite poling of the consumer for new messages.
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/asyncapi.py` & `fastkafka-0.7.0rc0/fastkafka/_components/asyncapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 import json
 import shutil
 import subprocess  # nosec: B404: Consider possible security implications associated with the subprocess module.
 import tempfile
 from datetime import timedelta
 from enum import Enum
 from pathlib import Path
-from tempfile import TemporaryDirectory
 from typing import *
 
 from pydantic import BaseModel, Field, HttpUrl
 from pydantic.json import timedelta_isoformat
 from pydantic.schema import schema
 
-import fastkafka._components.logger
-
-fastkafka._components.logger.should_supress_timestamps = True
-
+from .aiokafka_consumer_loop import ConsumeCallable
 from .docs_dependencies import _check_npm_with_local
+from .helpers import unwrap_list_type
 from .logger import get_logger
-from .producer_decorator import KafkaEvent, ProduceCallable
-from .aiokafka_consumer_loop import ConsumeCallable
+from fastkafka._components.producer_decorator import (
+    ProduceCallable,
+    unwrap_from_kafka_event,
+)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 3
 logger = get_logger(__name__)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 5
 class KafkaMessage(BaseModel):
     class Config:
@@ -152,47 +151,50 @@
     return_type = types.pop("return", type(None))
     # @app.producer must define a return value
     if return_type == type(None):
         raise ValueError(
             f"Producer function must have a defined return value, got {return_type} as return value"
         )
 
-    if hasattr(return_type, "__origin__") and return_type.__origin__ == KafkaEvent:
-        return_type = return_type.__args__[0]
-
-    if hasattr(return_type, "__origin__") and return_type.__origin__ == list:
-        return_type = return_type.__args__[0]
+    return_type = unwrap_from_kafka_event(return_type)
+    return_type = unwrap_list_type(return_type)
 
     if not hasattr(return_type, "json"):
         raise ValueError(f"Producer function return value must have json method")
     return return_type  # type: ignore
 
 # %% ../../nbs/014_AsyncAPI.ipynb 22
 def _get_msg_cls_for_consumer(f: ConsumeCallable) -> Type[Any]:
     types = get_type_hints(f)
     return_type = types.pop("return", type(None))
     types_list = list(types.values())
+    # @app.consumer does not return a value
+    if return_type != type(None):
+        raise ValueError(
+            f"Consumer function cannot return any value, got {return_type}"
+        )
     # @app.consumer first consumer argument must be a msg which is a subclass of BaseModel
     try:
-        if issubclass(BaseModel, types_list[0]):
+        msg_type = types_list[0]
+
+        msg_type = unwrap_list_type(msg_type)
+
+        if not issubclass(msg_type, BaseModel):
             raise ValueError(
                 f"Consumer function first param must be a BaseModel subclass msg, got {types_list}"
             )
+
+        return msg_type  # type: ignore
+
     except IndexError:
         raise ValueError(
             f"Consumer function first param must be a BaseModel subclass msg, got {types_list}"
         )
-    # @app.consumer does not return a value
-    if return_type != type(None):
-        raise ValueError(
-            f"Consumer function cannot return any value, got {return_type}"
-        )
-    return types_list[0]  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 25
+# %% ../../nbs/014_AsyncAPI.ipynb 27
 def _get_topic_dict(
     f: Callable[[Any], Any], direction: str = "publish"
 ) -> Dict[str, Any]:
     if not direction in ["publish", "subscribe"]:
         raise ValueError(
             f"direction must be one of ['publish', 'subscribe'], but it is '{direction}'."
         )
@@ -205,26 +207,26 @@
         msg_cls = _get_msg_cls_for_consumer(f)
 
     msg_schema = {"message": {"$ref": f"#/components/messages/{msg_cls.__name__}"}}
     if f.__doc__ is not None:
         msg_schema["description"] = f.__doc__  # type: ignore
     return {direction: msg_schema}
 
-# %% ../../nbs/014_AsyncAPI.ipynb 28
+# %% ../../nbs/014_AsyncAPI.ipynb 30
 def _get_channels_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Dict[str, Dict[str, Dict[str, Any]]]:
     topics = {}
     for ms, d in zip([consumers, producers], ["subscribe", "publish"]):
         for topic, f in ms.items():  # type: ignore
             topics[topic] = _get_topic_dict(f, d)
     return topics
 
-# %% ../../nbs/014_AsyncAPI.ipynb 30
+# %% ../../nbs/014_AsyncAPI.ipynb 32
 def _get_kafka_msg_classes(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Set[Type[BaseModel]]:
     fc = [_get_msg_cls_for_consumer(consumer) for consumer in consumers.values()]
     fp = [_get_msg_cls_for_producer(producer) for producer in producers.values()]
     return set(fc + fp)
@@ -232,15 +234,15 @@
 
 def _get_kafka_msg_definitions(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Dict[str, Dict[str, Any]]:
     return schema(_get_kafka_msg_classes(consumers, producers))  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 32
+# %% ../../nbs/014_AsyncAPI.ipynb 34
 def _get_example(cls: Type[BaseModel]) -> BaseModel:
     kwargs: Dict[str, Any] = {}
     for k, v in cls.__fields__.items():
         #         try:
         if (
             hasattr(v, "field_info")
             and hasattr(v.field_info, "extra")
@@ -249,15 +251,15 @@
             example = v.field_info.extra["example"]
             kwargs[k] = example
     #         except:
     #             pass
 
     return json.loads(cls(**kwargs).json())  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 34
+# %% ../../nbs/014_AsyncAPI.ipynb 36
 def _add_example_to_msg_definitions(
     msg_cls: Type[BaseModel], msg_schema: Dict[str, Dict[str, Any]]
 ) -> None:
     try:
         example = _get_example(msg_cls)
     except Exception as e:
         example = None
@@ -278,25 +280,25 @@
         {k: {"payload": v} for k, v in msg_schema["definitions"].items()}
         if "definitions" in msg_schema
         else {}
     )
 
     return msg_schema
 
-# %% ../../nbs/014_AsyncAPI.ipynb 36
+# %% ../../nbs/014_AsyncAPI.ipynb 38
 def _get_security_schemes(kafka_brokers: KafkaBrokers) -> Dict[str, Any]:
     security_schemes = {}
     for key, kafka_broker in kafka_brokers.brokers.items():
         if kafka_broker.security is not None:
             security_schemes[f"{key}_default_security"] = json.loads(
                 kafka_broker.security.json()
             )
     return security_schemes
 
-# %% ../../nbs/014_AsyncAPI.ipynb 38
+# %% ../../nbs/014_AsyncAPI.ipynb 40
 def _get_components_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
 ) -> Dict[str, Any]:
     definitions = _get_msg_definitions_with_examples(consumers, producers)
     msg_classes = [cls.__name__ for cls in _get_kafka_msg_classes(consumers, producers)]
@@ -321,24 +323,24 @@
             for k, v in substitutions.items():
                 if d == k:
                     d = v
         return d
 
     return _sub_values(components)  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 40
+# %% ../../nbs/014_AsyncAPI.ipynb 42
 def _get_servers_schema(kafka_brokers: KafkaBrokers) -> Dict[str, Any]:
     servers = json.loads(kafka_brokers.json(sort_keys=False))["brokers"]
 
     for key, kafka_broker in servers.items():
         if "security" in kafka_broker:
             servers[key]["security"] = [{f"{key}_default_security": []}]
     return servers  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 42
+# %% ../../nbs/014_AsyncAPI.ipynb 44
 def _get_asyncapi_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
     kafka_service_info: KafkaServiceInfo,
 ) -> Dict[str, Any]:
     #     # we don't use dict because we need custom JSON encoders
@@ -351,15 +353,15 @@
         "asyncapi": "2.5.0",
         "info": info,
         "servers": servers,
         "channels": channels,
         "components": components,
     }
 
-# %% ../../nbs/014_AsyncAPI.ipynb 44
+# %% ../../nbs/014_AsyncAPI.ipynb 46
 def yaml_file_cmp(file_1: Union[Path, str], file_2: Union[Path, str]) -> bool:
     try:
         import yaml
     except Exception as e:
         msg = "Please install docs version of fastkafka using 'pip install fastkafka[docs]' command"
         logger.error(msg)
         raise RuntimeError(msg)
@@ -367,15 +369,15 @@
     def _read(f: Union[Path, str]) -> Dict[str, Any]:
         with open(f) as stream:
             return yaml.safe_load(stream)  # type: ignore
 
     d = [_read(f) for f in [file_1, file_2]]
     return d[0] == d[1]
 
-# %% ../../nbs/014_AsyncAPI.ipynb 45
+# %% ../../nbs/014_AsyncAPI.ipynb 47
 def _generate_async_spec(
     *,
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
     kafka_service_info: KafkaServiceInfo,
     spec_path: Path,
@@ -411,15 +413,15 @@
             return True
         else:
             logger.info(
                 f"Keeping the old async specifications at: '{spec_path.resolve()}'"
             )
             return False
 
-# %% ../../nbs/014_AsyncAPI.ipynb 47
+# %% ../../nbs/014_AsyncAPI.ipynb 49
 def _generate_async_docs(
     *,
     spec_path: Path,
     docs_path: Path,
 ) -> None:
     _check_npm_with_local()
     cmd = [
@@ -443,15 +445,15 @@
     else:
         logger.error(f"Generation of async docs failed!")
         logger.info(f"Output of '$ {' '.join(cmd)}'{p.stdout.decode()}")
         raise ValueError(
             f"Generation of async docs failed, used '$ {' '.join(cmd)}'{p.stdout.decode()}"
         )
 
-# %% ../../nbs/014_AsyncAPI.ipynb 49
+# %% ../../nbs/014_AsyncAPI.ipynb 51
 def export_async_spec(
     *,
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
     kafka_service_info: KafkaServiceInfo,
     asyncapi_path: Union[Path, str],
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/benchmarking.py` & `fastkafka-0.7.0rc0/fastkafka/_components/benchmarking.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 # %% auto 0
 __all__ = ['logger']
 
 # %% ../../nbs/017_Benchmarking.ipynb 1
 from collections import deque
 from datetime import datetime, timedelta
-from functools import wraps
-from statistics import mean, stdev
+from statistics import mean
 from typing import *
 
 from .logger import get_logger
 
 # %% ../../nbs/017_Benchmarking.ipynb 4
 logger = get_logger("fastkafka.benchmark")
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.7.0rc0/fastkafka/_components/docs_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
            'node_path']
 
 # %% ../../nbs/097_Docs_Dependencies.ipynb 2
 import asyncio
 import os
 import shutil
 import subprocess  # nosec Issue: [B404:blacklist]
-import sys
 import tarfile
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from .helpers import in_notebook
 from .logger import get_logger
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/encoder/avro.py` & `fastkafka-0.7.0rc0/fastkafka/_components/encoder/avro.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/encoder/json.py` & `fastkafka-0.7.0rc0/fastkafka/_components/encoder/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/019_Json_Encode_Decoder.ipynb.
 
 # %% auto 0
 __all__ = ['logger', 'json_encoder', 'json_decoder']
 
 # %% ../../../nbs/019_Json_Encode_Decoder.ipynb 1
-import io
 import json
 from typing import *
 
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
 from ..logger import get_logger
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/helpers.py` & `fastkafka-0.7.0rc0/fastkafka/_components/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/998_Internal_Helpers.ipynb.
 
 # %% auto 0
-__all__ = ['in_notebook', 'change_dir', 'ImportFromStringError', 'true_after']
+__all__ = ['in_notebook', 'change_dir', 'ImportFromStringError', 'true_after', 'unwrap_list_type']
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 2
 def in_notebook() -> bool:
     try:
         from IPython import get_ipython
 
         if "IPKernelApp" not in get_ipython().config:
@@ -18,24 +18,19 @@
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 4
 import contextlib
 import importlib
 import os
 import sys
 from datetime import datetime, timedelta
-from functools import wraps
-from inspect import signature
-from pathlib import Path
+from inspect import Parameter
 from typing import *
 
-import docstring_parser
 import typer
 
-from .meta import delegates
-
 # %% ../../nbs/998_Internal_Helpers.ipynb 6
 @contextlib.contextmanager
 def change_dir(d: str) -> Generator[None, None, None]:
     curdir = os.getcwd()
     os.chdir(d)
     try:
         yield
@@ -96,7 +91,29 @@
     """Function returning True after a given number of seconds"""
     t = datetime.now()
 
     def _true_after(seconds: Union[int, float] = seconds, t: datetime = t) -> bool:
         return (datetime.now() - t) > timedelta(seconds=seconds)
 
     return _true_after
+
+# %% ../../nbs/998_Internal_Helpers.ipynb 12
+def unwrap_list_type(var_type: Union[Type, Parameter]) -> Union[Type, Parameter]:
+    """
+    Unwraps the type of a list.
+
+    Vars:
+        var_type: Type to unwrap.
+
+    Returns:
+        Unwrapped type if the given type is a list, otherwise returns the same type.
+
+    Example:
+        - Input: List[str]
+          Output: str
+        - Input: int
+          Output: int
+    """
+    if hasattr(var_type, "__origin__") and var_type.__origin__ == list:
+        return var_type.__args__[0]  # type: ignore
+    else:
+        return var_type
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/logger.py` & `fastkafka-0.7.0rc0/fastkafka/_components/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/Logger.ipynb.
 
 # %% auto 0
-__all__ = ['should_supress_timestamps', 'logger_spaces_added', 'supress_timestamps', 'get_default_logger_configuration',
+__all__ = ['should_suppress_timestamps', 'logger_spaces_added', 'suppress_timestamps', 'get_default_logger_configuration',
            'get_logger', 'set_level', 'cached_log']
 
 # %% ../../nbs/Logger.ipynb 2
 import logging
 import logging.config
 from typing import *
 
 from .helpers import true_after
-from .meta import patch
 
 # %% ../../nbs/Logger.ipynb 4
 # Logger Levels
 # CRITICAL = 50
 # ERROR = 40
 # WARNING = 30
 # INFO = 20
 # DEBUG = 10
 # NOTSET = 0
 
-should_supress_timestamps: bool = False
+should_suppress_timestamps: bool = False
 
 
-def supress_timestamps(flag: bool = True) -> None:
-    """Supress logger timestamp
+def suppress_timestamps(flag: bool = True) -> None:
+    """Suppress logger timestamp
 
     Args:
-        flag: If not set, then the default value **True** will be used to supress the timestamp
+        flag: If not set, then the default value **True** will be used to suppress the timestamp
             from the logger messages
     """
-    global should_supress_timestamps
-    should_supress_timestamps = flag
+    global should_suppress_timestamps
+    should_suppress_timestamps = flag
 
 
 def get_default_logger_configuration(level: int = logging.INFO) -> Dict[str, Any]:
     """Return the common configurations for the logger
 
     Args:
         level: Logger level to set
 
     Returns:
         A dict with default logger configuration
 
     """
-    global should_supress_timestamps
+    global should_suppress_timestamps
 
-    if should_supress_timestamps:
+    if should_suppress_timestamps:
         FORMAT = "[%(levelname)s] %(name)s: %(message)s"
     else:
         FORMAT = "%(asctime)s.%(msecs)03d [%(levelname)s] %(name)s: %(message)s"
 
     DATE_FMT = "%y-%m-%d %H:%M:%S"
 
     LOGGING_CONFIG = {
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/meta.py` & `fastkafka-0.7.0rc0/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/producer_decorator.py` & `fastkafka-0.7.0rc0/fastkafka/_components/producer_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/013_ProducerDecorator.ipynb.
 
 # %% auto 0
-__all__ = ['BaseSubmodel', 'ProduceReturnTypes', 'ProduceCallable', 'KafkaEvent', 'get_loop', 'release_callback',
+__all__ = ['BaseSubmodel', 'ProduceReturnTypes', 'ProduceCallable', 'KafkaEvent', 'unwrap_from_kafka_event', 'release_callback',
            'produce_single', 'send_batch', 'produce_batch', 'producer_decorator']
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 1
-import random
 import asyncio
 import functools
-import json
+import random
 import time
 from asyncio import iscoroutinefunction  # do not use the version from inspect
-from collections import namedtuple
 from dataclasses import dataclass
+from inspect import Parameter
 from typing import *
 
-import nest_asyncio
 from aiokafka import AIOKafkaProducer
 from aiokafka.producer.message_accumulator import BatchBuilder
 from pydantic import BaseModel
 
 from .meta import export
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 3
@@ -38,40 +36,50 @@
         key (bytes, optional): The optional key used to identify the Kafka event.
     """
 
     message: BaseSubmodel
     key: Optional[bytes] = None
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 5
+def unwrap_from_kafka_event(var_type: Union[Type, Parameter]) -> Union[Type, Parameter]:
+    """
+    Unwraps the type from a KafkaEvent.
+
+    Vars:
+        var_type: Type to unwrap.
+
+    Returns:
+        Type: Unwrapped type if the given type is a KafkaEvent, otherwise returns the same type.
+
+    Example:
+        - Input: KafkaEvent[str]
+          Output: str
+        - Input: int
+          Output: int
+    """
+    if hasattr(var_type, "__origin__") and var_type.__origin__ == KafkaEvent:
+        return var_type.__args__[0]  # type: ignore
+    else:
+        return var_type
+
+# %% ../../nbs/013_ProducerDecorator.ipynb 7
 ProduceReturnTypes = Union[
     BaseModel, KafkaEvent[BaseModel], List[BaseModel], KafkaEvent[List[BaseModel]]
 ]
 
 ProduceCallable = Union[
     Callable[..., ProduceReturnTypes], Callable[..., Awaitable[ProduceReturnTypes]]
 ]
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 8
+# %% ../../nbs/013_ProducerDecorator.ipynb 10
 def _wrap_in_event(
     message: Union[BaseModel, List[BaseModel], KafkaEvent]
 ) -> KafkaEvent:
     return message if type(message) == KafkaEvent else KafkaEvent(message)
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 11
-def get_loop() -> asyncio.AbstractEventLoop:
-    try:
-        loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()
-    except RuntimeError as e:
-        loop = asyncio.new_event_loop()
-
-    if loop.is_running():
-        nest_asyncio.apply(loop)
-
-    return loop
-
 # %% ../../nbs/013_ProducerDecorator.ipynb 13
 def release_callback(fut: asyncio.Future) -> None:
     pass
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 14
 async def produce_single(  # type: ignore
     producer: AIOKafkaProducer,
@@ -126,52 +134,32 @@
     producer_store: Dict[str, Any],
     func: ProduceCallable,
     topic: str,
     encoder_fn: Callable[[BaseModel], bytes],
 ) -> ProduceCallable:
     """todo: write documentation"""
 
-    loop = get_loop()
-
     @functools.wraps(func)
     async def _produce_async(
         *args: List[Any],
         topic: str = topic,
         encoder_fn: Callable[[BaseModel], bytes] = encoder_fn,
         producer_store: Dict[str, Any] = producer_store,
         f: Callable[..., Awaitable[ProduceReturnTypes]] = func,  # type: ignore
-        **kwargs: Any
+        **kwargs: Any,
     ) -> ProduceReturnTypes:
         return_val = await f(*args, **kwargs)
         wrapped_val = _wrap_in_event(return_val)
         _, producer, _ = producer_store[topic]
 
         if isinstance(wrapped_val.message, list):
             await produce_batch(producer, topic, encoder_fn, wrapped_val)
         else:
             await produce_single(producer, topic, encoder_fn, wrapped_val)
         return return_val
 
-    @functools.wraps(func)
-    def _produce_sync(
-        *args: List[Any],
-        topic: str = topic,
-        encoder_fn: Callable[[BaseModel], bytes] = encoder_fn,
-        producer_store: Dict[str, Any] = producer_store,
-        f: Callable[..., ProduceReturnTypes] = func,  # type: ignore
-        loop: asyncio.AbstractEventLoop = loop,
-        **kwargs: Any
-    ) -> ProduceReturnTypes:
-        return_val = f(*args, **kwargs)
-        wrapped_val = _wrap_in_event(return_val)
-        _, producer, _ = producer_store[topic]
-        if isinstance(wrapped_val.message, list):
-            loop.run_until_complete(
-                produce_batch(producer, topic, encoder_fn, wrapped_val)
-            )
-        else:
-            loop.run_until_complete(
-                produce_single(producer, topic, encoder_fn, wrapped_val)
-            )
-        return return_val
+    if not iscoroutinefunction(func):
+        raise ValueError(
+            "Synchronous functions are not supported for produce operation"
+        )
 
-    return _produce_async if iscoroutinefunction(func) else _produce_sync
+    return _produce_async
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_components/test_dependencies.py` & `fastkafka-0.7.0rc0/fastkafka/_components/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/_docusaurus_helper.py` & `fastkafka-0.7.0rc0/fastkafka/_docusaurus_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/096_Docusaurus_Helper.ipynb.
 
 # %% auto 0
-__all__ = ['fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'generate_sidebar']
+__all__ = ['fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'generate_sidebar',
+           'delete_unused_markdown_files_from_sidebar']
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 2
 import itertools
 import re
+import ast
 import types
 from inspect import Signature, getmembers, isclass, isfunction, signature
 from pathlib import Path
 from typing import *
 from urllib.parse import urljoin
 
-import yaml
+import typer
 from docstring_parser import parse
 from docstring_parser.common import DocstringParam, DocstringRaises, DocstringReturns
 from nbdev.config import get_config
 from nbdev_mkdocs.mkdocs import (
     _add_all_submodules,
-    _get_api_summary,
     _import_all_members,
     _import_functions_and_classes,
     _import_submodules,
 )
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 4
 def _format_docstring_sections(
@@ -484,7 +485,70 @@
             + """
     "LICENSE",
     "CONTRIBUTING",
     "CHANGELOG",
 ],
 };"""
         )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 68
+def _get_markdown_filenames_from_sidebar(sidebar_file_path: str) -> List[str]:
+    """Get a list of Markdown filenames included in the sidebar.
+
+    Args:
+        sidebar_file_path: The path to the sidebar file.
+
+    Returns:
+        A list of Markdown filenames included in the sidebar.
+    """
+    with open(sidebar_file_path, "r") as file:
+        file_content = file.read()
+
+        pattern = r"tutorialSidebar:\s*(\[.*\])\s*,\s*\n?\s*};"
+        match = re.search(pattern, file_content, re.DOTALL)
+        all_sidebar_files = ast.literal_eval(match.group(1)) if match else []
+        markdown_filenames = [
+            f"{v}.md" for v in all_sidebar_files if isinstance(v, str)
+        ]
+        return markdown_filenames
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 70
+def _delete_files(files: List[Path]) -> None:
+    """Deletes a list of files.
+
+    Args:
+        files: A list of Path objects representing the files to be deleted.
+
+    Raises:
+        OSError: If an error occurs while deleting a file.
+
+    """
+    for file in files:
+        try:
+            file.unlink()
+        except OSError as e:
+            typer.echo(
+                f"Error deleting files from docusaurus/docs directory. Could not delete file: {file} - {e}"
+            )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 73
+def delete_unused_markdown_files_from_sidebar(
+    docs_path: str, sidebar_file_path: str
+) -> None:
+    """Delete the markdown files from the docs directory that are not present in the sidebar.
+
+    Args:
+        docs_path: Path to the directory containing the markdown files.
+        sidebar_file_path: Path to the sidebar file.
+    """
+    md_filenames_in_sidebar = _get_markdown_filenames_from_sidebar(
+        str(sidebar_file_path)
+    )
+    if len(md_filenames_in_sidebar) > 0:
+        all_md_files_in_docs_dir = [
+            file_path for file_path in Path(docs_path).glob("*.md")
+        ]
+        md_files_in_sidebar = [Path(docs_path) / f for f in md_filenames_in_sidebar]
+        md_files_to_delete = list(
+            set(all_md_files_in_docs_dir) - set(md_files_in_sidebar)
+        )
+        _delete_files(md_files_to_delete)
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_helpers.py` & `fastkafka-0.7.0rc0/fastkafka/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import inspect
 import json
 import textwrap
 from datetime import datetime, timedelta
 from typing import *
 
 import aiohttp
-import aiokafka
 import anyio
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.helpers import create_ssl_context
 from aiokafka.structs import RecordMetadata
 from IPython.display import Markdown
 
 from ._components.helpers import in_notebook
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_modidx.py` & `fastkafka-0.7.0rc0/fastkafka/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
                                                                                                 'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.consumes': ( 'fastkafka.html#fastkafka.consumes',
                                                                                                'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.create_docs': ( 'fastkafka.html#fastkafka.create_docs',
                                                                                                   'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.create_mocks': ( 'fastkafka.html#fastkafka.create_mocks',
                                                                                                    'fastkafka/_application/app.py'),
+                                            'fastkafka._application.app.FastKafka.fastapi_lifespan': ( 'fastkafka.html#fastkafka.fastapi_lifespan',
+                                                                                                       'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.get_topics': ( 'fastkafka.html#fastkafka.get_topics',
                                                                                                  'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.is_started': ( 'fastkafka.html#fastkafka.is_started',
                                                                                                  'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.produces': ( 'fastkafka.html#fastkafka.produces',
                                                                                                'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.run_in_background': ( 'fastkafka.html#fastkafka.run_in_background',
@@ -97,20 +99,20 @@
                                                                                                                               'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.EventMetadata.create_event_metadata': ( 'consumerloop.html#eventmetadata.create_event_metadata',
                                                                                                                                                     'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._aiokafka_consumer_loop': ( 'consumerloop.html#_aiokafka_consumer_loop',
                                                                                                                                         'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._callback_parameters_wrapper': ( 'consumerloop.html#_callback_parameters_wrapper',
                                                                                                                                              'fastkafka/_components/aiokafka_consumer_loop.py'),
-                                                              'fastkafka._components.aiokafka_consumer_loop._decode_streamed_msgs': ( 'consumerloop.html#_decode_streamed_msgs',
-                                                                                                                                      'fastkafka/_components/aiokafka_consumer_loop.py'),
+                                                              'fastkafka._components.aiokafka_consumer_loop._get_batch_msg_handlers': ( 'consumerloop.html#_get_batch_msg_handlers',
+                                                                                                                                        'fastkafka/_components/aiokafka_consumer_loop.py'),
+                                                              'fastkafka._components.aiokafka_consumer_loop._get_single_msg_handlers': ( 'consumerloop.html#_get_single_msg_handlers',
+                                                                                                                                         'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._prepare_callback': ( 'consumerloop.html#_prepare_callback',
                                                                                                                                   'fastkafka/_components/aiokafka_consumer_loop.py'),
-                                                              'fastkafka._components.aiokafka_consumer_loop._stream_msgs': ( 'consumerloop.html#_stream_msgs',
-                                                                                                                             'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.aiokafka_consumer_loop': ( 'consumerloop.html#aiokafka_consumer_loop',
                                                                                                                                        'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.sanitize_kafka_config': ( 'consumerloop.html#sanitize_kafka_config',
                                                                                                                                       'fastkafka/_components/aiokafka_consumer_loop.py')},
             'fastkafka._components.asyncapi': { 'fastkafka._components.asyncapi.APIKeyLocation': ( 'asyncapi.html#apikeylocation',
                                                                                                    'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.ContactInfo': ( 'asyncapi.html#contactinfo',
@@ -208,25 +210,27 @@
                                                'fastkafka._components.helpers._import_from_string': ( 'internal_helpers.html#_import_from_string',
                                                                                                       'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.change_dir': ( 'internal_helpers.html#change_dir',
                                                                                              'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.in_notebook': ( 'internal_helpers.html#in_notebook',
                                                                                               'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.true_after': ( 'internal_helpers.html#true_after',
-                                                                                             'fastkafka/_components/helpers.py')},
+                                                                                             'fastkafka/_components/helpers.py'),
+                                               'fastkafka._components.helpers.unwrap_list_type': ( 'internal_helpers.html#unwrap_list_type',
+                                                                                                   'fastkafka/_components/helpers.py')},
             'fastkafka._components.logger': { 'fastkafka._components.logger.cached_log': ( 'logger.html#cached_log',
                                                                                            'fastkafka/_components/logger.py'),
                                               'fastkafka._components.logger.get_default_logger_configuration': ( 'logger.html#get_default_logger_configuration',
                                                                                                                  'fastkafka/_components/logger.py'),
                                               'fastkafka._components.logger.get_logger': ( 'logger.html#get_logger',
                                                                                            'fastkafka/_components/logger.py'),
                                               'fastkafka._components.logger.set_level': ( 'logger.html#set_level',
                                                                                           'fastkafka/_components/logger.py'),
-                                              'fastkafka._components.logger.supress_timestamps': ( 'logger.html#supress_timestamps',
-                                                                                                   'fastkafka/_components/logger.py')},
+                                              'fastkafka._components.logger.suppress_timestamps': ( 'logger.html#suppress_timestamps',
+                                                                                                    'fastkafka/_components/logger.py')},
             'fastkafka._components.meta': { 'fastkafka._components.meta._delegates_without_docs': ( 'meta.html#_delegates_without_docs',
                                                                                                     'fastkafka/_components/meta.py'),
                                             'fastkafka._components.meta._format_args': ( 'meta.html#_format_args',
                                                                                          'fastkafka/_components/meta.py'),
                                             'fastkafka._components.meta._get_default_kwargs_from_sig': ( 'meta.html#_get_default_kwargs_from_sig',
                                                                                                          'fastkafka/_components/meta.py'),
                                             'fastkafka._components.meta.classcontextmanager': ( 'meta.html#classcontextmanager',
@@ -251,26 +255,26 @@
                                                                                         'fastkafka/_components/meta.py'),
                                             'fastkafka._components.meta.use_parameters_of': ( 'meta.html#use_parameters_of',
                                                                                               'fastkafka/_components/meta.py')},
             'fastkafka._components.producer_decorator': { 'fastkafka._components.producer_decorator.KafkaEvent': ( 'producerdecorator.html#kafkaevent',
                                                                                                                    'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator._wrap_in_event': ( 'producerdecorator.html#_wrap_in_event',
                                                                                                                        'fastkafka/_components/producer_decorator.py'),
-                                                          'fastkafka._components.producer_decorator.get_loop': ( 'producerdecorator.html#get_loop',
-                                                                                                                 'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.produce_batch': ( 'producerdecorator.html#produce_batch',
                                                                                                                       'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.produce_single': ( 'producerdecorator.html#produce_single',
                                                                                                                        'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.producer_decorator': ( 'producerdecorator.html#producer_decorator',
                                                                                                                            'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.release_callback': ( 'producerdecorator.html#release_callback',
                                                                                                                          'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.send_batch': ( 'producerdecorator.html#send_batch',
-                                                                                                                   'fastkafka/_components/producer_decorator.py')},
+                                                                                                                   'fastkafka/_components/producer_decorator.py'),
+                                                          'fastkafka._components.producer_decorator.unwrap_from_kafka_event': ( 'producerdecorator.html#unwrap_from_kafka_event',
+                                                                                                                                'fastkafka/_components/producer_decorator.py')},
             'fastkafka._components.task_streaming': { 'fastkafka._components.task_streaming.DynamicTaskExecutor': ( 'taskstreaming.html#dynamictaskexecutor',
                                                                                                                     'fastkafka/_components/task_streaming.py'),
                                                       'fastkafka._components.task_streaming.DynamicTaskExecutor.__init__': ( 'taskstreaming.html#dynamictaskexecutor.__init__',
                                                                                                                              'fastkafka/_components/task_streaming.py'),
                                                       'fastkafka._components.task_streaming.DynamicTaskExecutor.run': ( 'taskstreaming.html#dynamictaskexecutor.run',
                                                                                                                         'fastkafka/_components/task_streaming.py'),
                                                       'fastkafka._components.task_streaming.ExceptionMonitor': ( 'taskstreaming.html#exceptionmonitor',
@@ -520,8 +524,9 @@
                                                'fastkafka._testing.test_utils.mock_AIOKafkaProducer_send': ( 'test_utils.html#mock_aiokafkaproducer_send',
                                                                                                              'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.nb_safe_seed': ( 'test_utils.html#nb_safe_seed',
                                                                                                'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.run_script_and_cancel': ( 'test_utils.html#run_script_and_cancel',
                                                                                                         'fastkafka/_testing/test_utils.py')},
             'fastkafka.encoder': {'fastkafka.encoder.dummy': ('encoder_export.html#dummy', 'fastkafka/encoder.py')},
+            'fastkafka.executors': {'fastkafka.executors.dummy': ('application_executors_export.html#dummy', 'fastkafka/executors.py')},
             'fastkafka.testing': {'fastkafka.testing.dummy': ('testing_export.html#dummy', 'fastkafka/testing.py')}}}
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_server.py` & `fastkafka-0.7.0rc0/fastkafka/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 from contextlib import contextmanager
 from typing import *
 
 import asyncer
 import typer
 
 from ._components.helpers import _import_from_string
-from ._components.logger import get_logger, supress_timestamps
+from ._components.logger import get_logger
 
 # %% ../nbs/021_FastKafkaServer.ipynb 5
-supress_timestamps(False)
 logger = get_logger(__name__, level=20)
 
 # %% ../nbs/021_FastKafkaServer.ipynb 7
 class ServerProcess:
     def __init__(self, app: str, kafka_broker_name: str):
         self.app = app
         self.should_exit = False
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.7.0rc0/fastkafka/_testing/apache_kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.7.0rc0/fastkafka/_testing/in_memory_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,36 +2,31 @@
 
 # %% auto 0
 __all__ = ['logger', 'KafkaRecord', 'KafkaPartition', 'KafkaTopic', 'split_list', 'GroupMetadata', 'InMemoryBroker',
            'InMemoryConsumer', 'InMemoryProducer', 'MockBatch']
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 1
 import asyncio
-import copy
 import hashlib
-import inspect
 import random
 import string
 import uuid
-from collections import namedtuple
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from typing import *
 
-import aiokafka
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord, RecordMetadata, TopicPartition
 
 import fastkafka._application.app
 import fastkafka._components.aiokafka_consumer_loop
 from .._components.logger import get_logger
 from fastkafka._components.meta import (
     _get_default_kwargs_from_sig,
     classcontextmanager,
-    copy_func,
     delegates,
     patch,
 )
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 3
 logger = get_logger(__name__)
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.7.0rc0/fastkafka/_testing/local_redpanda_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import *
 
 import asyncer
 import nest_asyncio
 
 from .._components._subprocess import terminate_asyncio_process
 from .._components.helpers import in_notebook
-from .._components.logger import get_logger, supress_timestamps
+from .._components.logger import get_logger
 from .._components.meta import delegates, export, patch
 from .apache_kafka_broker import get_free_port, run_and_match
 
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 3
 if in_notebook():
     from tqdm.notebook import tqdm
 else:
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/_testing/test_utils.py` & `fastkafka-0.7.0rc0/fastkafka/_testing/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 import asyncio
 import hashlib
 import shlex
 import subprocess  # nosec
 import unittest
 import unittest.mock
 from contextlib import contextmanager
-from datetime import datetime, timedelta
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import *
 
 import asyncer
-from aiokafka import AIOKafkaProducer
 from IPython.display import IFrame
 
 from .._application.app import FastKafka
 from .._components._subprocess import terminate_asyncio_process
 from .._components.helpers import _import_from_string, change_dir
 from .._components.logger import get_logger
```

### Comparing `fastkafka-0.6.1rc0/fastkafka/encoder.py` & `fastkafka-0.7.0rc0/fastkafka/encoder.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka/testing.py` & `fastkafka-0.7.0rc0/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.6.1rc0/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.7.0rc0/fastkafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.6.1rc0
+Version: 0.7.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.6.1rc0/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.7.0rc0/fastkafka.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 fastkafka/_cli_docs.py
 fastkafka/_cli_testing.py
 fastkafka/_docusaurus_helper.py
 fastkafka/_helpers.py
 fastkafka/_modidx.py
 fastkafka/_server.py
 fastkafka/encoder.py
+fastkafka/executors.py
 fastkafka/testing.py
 fastkafka.egg-info/PKG-INFO
 fastkafka.egg-info/SOURCES.txt
 fastkafka.egg-info/dependency_links.txt
 fastkafka.egg-info/entry_points.txt
 fastkafka.egg-info/not-zip-safe
 fastkafka.egg-info/requires.txt
```

### Comparing `fastkafka-0.6.1rc0/settings.ini` & `fastkafka-0.7.0rc0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.6.1rc0
+version = 0.7.0rc0
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.6.1rc0/setup.py` & `fastkafka-0.7.0rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,28 +49,30 @@
 
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 
 dev_requirements = [
     "nbconvert>=7.2.9",
     "nbformat>=5.7.3",
-    "nbdev-mkdocs==0.4.0",
+    "nbdev-mkdocs==0.5.0",
     "mypy==1.3.0",
     "pre-commit==3.3.1",
     "nbqa==1.6.3",
     "black==23.3.0",
     "isort==5.12.0",
     "bandit==1.7.5",
     "semgrep==1.21.0",
     "pytest==7.3.1",
     "numpy>=1.21.0",
     "pandas>=1.2.0",
     "email-validator==1.3.1",
     "scikit-learn==1.2.1",
-    "ipython<8.13"
+    "ipython<8.13",
+    "fastapi>=0.95.1",
+    "uvicorn==0.22.0",
 ]
 
 project_urls = {
    'Bug Tracker': cfg['git_url'] + '/issues',
    'CI': cfg['git_url'] + '/actions',
    'Documentation': 'https://fastkafka.airt.ai/',
 #    'Source Code': cfg['git_url'],
```


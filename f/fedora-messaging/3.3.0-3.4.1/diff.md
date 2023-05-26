# Comparing `tmp/fedora_messaging-3.3.0.tar.gz` & `tmp/fedora_messaging-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedora_messaging-3.3.0.tar", last modified: Fri Mar 31 11:23:40 2023, max compression
+gzip compressed data, was "fedora_messaging-3.4.1.tar", last modified: Fri May 26 11:50:56 2023, max compression
```

## Comparing `fedora_messaging-3.3.0.tar` & `fedora_messaging-3.4.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.051151 fedora_messaging-3.3.0/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    18092 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/LICENSE
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      199 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/MANIFEST.in
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2519 2023-03-31 11:23:40.051151 fedora_messaging-3.3.0/PKG-INFO
--rw-r--r--   0 abompard  (1000) abompard  (1000)     1653 2022-09-13 09:47:35.000000 fedora_messaging-3.3.0/README.rst
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1842 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/config.toml.example
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.041151 fedora_messaging-3.3.0/configs/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1216 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/configs/cacert.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1233 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/configs/fedora-cert.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1708 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/configs/fedora-key.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1229 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/configs/fedora.stg-cert.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1704 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/configs/fedora.stg-key.pem
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2874 2022-09-13 09:47:35.000000 fedora_messaging-3.3.0/configs/fedora.stg.toml
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2846 2022-09-13 09:47:35.000000 fedora_messaging-3.3.0/configs/fedora.toml
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1204 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/configs/stg-cacert.pem
--rw-r--r--   0 abompard  (1000) abompard  (1000)      114 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/dev-requirements.txt
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.041151 fedora_messaging-3.3.0/docs/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      617 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/docs/Makefile
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.041151 fedora_messaging-3.3.0/docs/api/
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2744 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/api/api.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     4059 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/api/wire-format.rst
--rwxr-xr-x   0 abompard  (1000) abompard  (1000)     6259 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/build-schemas-list.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    27539 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/changelog.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     6164 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/conf.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)     6330 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/contributing.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     1209 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/index.rst
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.042151 fedora_messaging-3.3.0/docs/sample_schema_package/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    18092 2018-08-01 10:49:11.000000 fedora_messaging-3.3.0/docs/sample_schema_package/LICENSE
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       23 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/docs/sample_schema_package/MANIFEST.in
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      147 2018-08-01 10:49:11.000000 fedora_messaging-3.3.0/docs/sample_schema_package/README
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.042151 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      742 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__init__.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.044151 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      182 2018-08-20 13:14:36.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      192 2020-06-30 06:35:31.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     6228 2020-06-30 07:01:50.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/messages.cpython-38.pyc
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     5966 2018-08-20 13:14:36.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/schema.cpython-36.pyc
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1001 2018-08-20 13:14:36.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 abompard  (1000) abompard  (1000)     7674 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/messages.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.044151 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      742 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__init__.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.045151 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__pycache__/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      188 2018-08-20 13:14:36.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      198 2020-06-30 06:35:31.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     5471 2020-06-30 07:01:26.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_messages.cpython-38.pyc
--rw-------   0 abompard  (1000) abompard  (1000)     6306 2018-08-20 13:15:34.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_schema.cpython-36-PYTEST.pyc
--rw-r--r--   0 abompard  (1000) abompard  (1000)     7127 2022-12-21 14:07:36.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/test_messages.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.043151 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1022 2020-06-30 07:01:50.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/PKG-INFO
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      459 2020-06-30 07:01:50.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/SOURCES.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2020-06-30 07:01:50.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/dependency_links.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      131 2020-06-30 07:01:50.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/entry_points.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2020-06-30 06:35:31.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/not-zip-safe
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       17 2020-06-30 07:01:50.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/requires.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       17 2020-06-30 07:01:50.000000 fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/top_level.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       59 2018-08-21 12:58:53.000000 fedora_messaging-3.3.0/docs/sample_schema_package/setup.cfg
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2262 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/docs/sample_schema_package/setup.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)      368 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/schema-packages.txt
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.045151 fedora_messaging-3.3.0/docs/tutorial/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    15964 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/docs/tutorial/conversion.rst
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2120 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/docs/tutorial/exceptions.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2091 2022-12-19 10:46:57.000000 fedora_messaging-3.3.0/docs/tutorial/installation.rst
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     7939 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/docs/tutorial/schemas.rst
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     4337 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/docs/tutorial/usage.rst
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.046151 fedora_messaging-3.3.0/docs/user-guide/
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.046151 fedora_messaging-3.3.0/docs/user-guide/cli/
--rw-r--r--   0 abompard  (1000) abompard  (1000)     9278 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/cli/fedora-messaging.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)      117 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/cli.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)       97 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/configuration.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     8460 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/consuming.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)      477 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/installation.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     8242 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/messages.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     2764 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/publishing.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)     5634 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/quick-start.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)    32244 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/schemas.rst
--rw-r--r--   0 abompard  (1000) abompard  (1000)       94 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/docs/user-guide/testing.rst
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.047150 fedora_messaging-3.3.0/fedora_messaging/
--rw-r--r--   0 abompard  (1000) abompard  (1000)      923 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/fedora_messaging/__init__.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    12952 2022-09-13 09:47:35.000000 fedora_messaging-3.3.0/fedora_messaging/api.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    16594 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/fedora_messaging/cli.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    17857 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/fedora_messaging/config.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1174 2022-05-05 08:06:17.000000 fedora_messaging-3.3.0/fedora_messaging/example.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     5349 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/exceptions.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    28888 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/fedora_messaging/message.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2706 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/schema_utils.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2019 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/signals.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     3429 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/testing.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.048151 fedora_messaging-3.3.0/fedora_messaging/tests/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1051 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/__init__.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.049151 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       24 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/bad_cb
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       40 2018-08-21 12:54:37.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/bad_conf.toml
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1375 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/ca_bundle.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       32 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/callback.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     7476 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/cert.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/cli_integration.toml
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      117 2018-12-13 10:38:10.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/good_conf.toml
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      260 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/good_msg_dump.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/invalid_ca.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/invalid_key.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      234 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/invalid_msg_dump.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     3272 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/key.pem
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      214 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/msg_without_id_dump.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        2 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/wrong_json_msg_dump.txt
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.049151 fedora_messaging-3.3.0/fedora_messaging/tests/integration/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/fedora_messaging/tests/integration/__init__.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    30841 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/integration/test_api.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2830 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/integration/test_cli.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      204 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/integration/utils.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.050150 fedora_messaging-3.3.0/fedora_messaging/tests/unit/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/__init__.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    12558 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_api.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    30764 2022-12-21 14:07:36.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_cli.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    18746 2022-12-21 14:07:36.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_config.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     1868 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_example.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    25221 2023-03-31 11:20:13.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_message.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2510 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_schema_utils.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     4108 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_testing.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.050150 fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-08-01 10:49:11.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/__init__.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    18458 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_consumer.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    10658 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_factory.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    12064 2023-03-31 11:20:13.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_protocol.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     8160 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_service.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2685 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/utils.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.051151 fedora_messaging-3.3.0/fedora_messaging/twisted/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.3.0/fedora_messaging/twisted/__init__.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)    14738 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/fedora_messaging/twisted/consumer.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    13668 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/twisted/factory.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)    17448 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/twisted/protocol.py
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     7479 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/fedora_messaging/twisted/service.py
-drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-03-31 11:23:40.048151 fedora_messaging-3.3.0/fedora_messaging.egg-info/
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     2519 2023-03-31 11:23:39.000000 fedora_messaging-3.3.0/fedora_messaging.egg-info/PKG-INFO
--rw-rw-r--   0 abompard  (1000) abompard  (1000)     4878 2023-03-31 11:23:40.000000 fedora_messaging-3.3.0/fedora_messaging.egg-info/SOURCES.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2023-03-31 11:23:39.000000 fedora_messaging-3.3.0/fedora_messaging.egg-info/dependency_links.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      129 2023-03-31 11:23:39.000000 fedora_messaging-3.3.0/fedora_messaging.egg-info/entry_points.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2021-12-14 11:27:18.000000 fedora_messaging-3.3.0/fedora_messaging.egg-info/not-zip-safe
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      130 2023-03-31 11:23:39.000000 fedora_messaging-3.3.0/fedora_messaging.egg-info/requires.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)       17 2023-03-31 11:23:39.000000 fedora_messaging-3.3.0/fedora_messaging.egg-info/top_level.txt
--rw-rw-r--   0 abompard  (1000) abompard  (1000)      274 2021-11-22 15:44:30.000000 fedora_messaging-3.3.0/fm-consumer@.service
--rw-r--r--   0 abompard  (1000) abompard  (1000)     1120 2022-12-21 14:07:36.000000 fedora_messaging-3.3.0/pyproject.toml
--rw-r--r--   0 abompard  (1000) abompard  (1000)      124 2022-12-21 14:07:36.000000 fedora_messaging-3.3.0/requirements.txt
--rw-r--r--   0 abompard  (1000) abompard  (1000)       38 2023-03-31 11:23:40.051151 fedora_messaging-3.3.0/setup.cfg
--rwxrwxr-x   0 abompard  (1000) abompard  (1000)     3003 2021-12-10 15:40:42.000000 fedora_messaging-3.3.0/setup.py
--rw-r--r--   0 abompard  (1000) abompard  (1000)      972 2023-03-31 11:20:47.000000 fedora_messaging-3.3.0/tox.ini
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.250586 fedora_messaging-3.4.1/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    18092 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/LICENSE
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      199 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/MANIFEST.in
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2519 2023-05-26 11:50:56.249586 fedora_messaging-3.4.1/PKG-INFO
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1653 2022-09-13 09:47:35.000000 fedora_messaging-3.4.1/README.rst
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1842 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/config.toml.example
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.230586 fedora_messaging-3.4.1/configs/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1216 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/configs/cacert.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1233 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/configs/fedora-cert.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1708 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/configs/fedora-key.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1229 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/configs/fedora.stg-cert.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1704 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/configs/fedora.stg-key.pem
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2874 2022-09-13 09:47:35.000000 fedora_messaging-3.4.1/configs/fedora.stg.toml
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2846 2022-09-13 09:47:35.000000 fedora_messaging-3.4.1/configs/fedora.toml
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1204 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/configs/stg-cacert.pem
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      114 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/dev-requirements.txt
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.232586 fedora_messaging-3.4.1/docs/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      617 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/docs/Makefile
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.232586 fedora_messaging-3.4.1/docs/api/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2744 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/api/api.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     4059 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/api/wire-format.rst
+-rwxr-xr-x   0 abompard  (1000) abompard  (1000)     6259 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/build-schemas-list.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    27877 2023-05-26 11:50:05.000000 fedora_messaging-3.4.1/docs/changelog.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     6164 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/conf.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     6330 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/contributing.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1209 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/index.rst
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.233586 fedora_messaging-3.4.1/docs/sample_schema_package/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    18092 2018-08-01 10:49:11.000000 fedora_messaging-3.4.1/docs/sample_schema_package/LICENSE
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       23 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/docs/sample_schema_package/MANIFEST.in
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      147 2018-08-01 10:49:11.000000 fedora_messaging-3.4.1/docs/sample_schema_package/README
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.234586 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      742 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__init__.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.237586 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      182 2018-08-20 13:14:36.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      192 2020-06-30 06:35:31.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     6228 2020-06-30 07:01:50.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/messages.cpython-38.pyc
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     5966 2018-08-20 13:14:36.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/schema.cpython-36.pyc
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1001 2018-08-20 13:14:36.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     7674 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/messages.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.237586 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      742 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__init__.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.238586 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__pycache__/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      188 2018-08-20 13:14:36.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      198 2020-06-30 06:35:31.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     5471 2020-06-30 07:01:26.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_messages.cpython-38.pyc
+-rw-------   0 abompard  (1000) abompard  (1000)     6306 2018-08-20 13:15:34.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_schema.cpython-36-PYTEST.pyc
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     7127 2022-12-21 14:07:36.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/test_messages.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.236585 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1022 2020-06-30 07:01:50.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/PKG-INFO
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      459 2020-06-30 07:01:50.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/SOURCES.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2020-06-30 07:01:50.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/dependency_links.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      131 2020-06-30 07:01:50.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/entry_points.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2020-06-30 06:35:31.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/not-zip-safe
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       17 2020-06-30 07:01:50.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/requires.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       17 2020-06-30 07:01:50.000000 fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/top_level.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       59 2018-08-21 12:58:53.000000 fedora_messaging-3.4.1/docs/sample_schema_package/setup.cfg
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2262 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/docs/sample_schema_package/setup.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      368 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/schema-packages.txt
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.239585 fedora_messaging-3.4.1/docs/tutorial/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    15964 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/docs/tutorial/conversion.rst
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2120 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/docs/tutorial/exceptions.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2091 2022-12-19 10:46:57.000000 fedora_messaging-3.4.1/docs/tutorial/installation.rst
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     7939 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/docs/tutorial/schemas.rst
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     4337 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/docs/tutorial/usage.rst
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.241586 fedora_messaging-3.4.1/docs/user-guide/
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.242586 fedora_messaging-3.4.1/docs/user-guide/cli/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     9278 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/cli/fedora-messaging.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      117 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/cli.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       97 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/configuration.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     8460 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/consuming.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      477 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/installation.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     8242 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/messages.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2764 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/publishing.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     5634 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/quick-start.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    32244 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/schemas.rst
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       94 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/docs/user-guide/testing.rst
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.243586 fedora_messaging-3.4.1/fedora_messaging/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      923 2023-05-26 11:43:48.000000 fedora_messaging-3.4.1/fedora_messaging/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    12952 2022-09-13 09:47:35.000000 fedora_messaging-3.4.1/fedora_messaging/api.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    16594 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/fedora_messaging/cli.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    17857 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/fedora_messaging/config.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1174 2022-05-05 08:06:17.000000 fedora_messaging-3.4.1/fedora_messaging/example.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     5349 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/exceptions.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    29138 2023-05-26 11:07:51.000000 fedora_messaging-3.4.1/fedora_messaging/message.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2706 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/schema_utils.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2019 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/signals.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     3429 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/testing.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.244586 fedora_messaging-3.4.1/fedora_messaging/tests/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1051 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/__init__.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.246586 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       24 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/bad_cb
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       40 2018-08-21 12:54:37.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/bad_conf.toml
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1375 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/ca_bundle.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       32 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/callback.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     7476 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/cert.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/cli_integration.toml
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      117 2018-12-13 10:38:10.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/good_conf.toml
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      260 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/good_msg_dump.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/invalid_ca.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/invalid_key.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      234 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/invalid_msg_dump.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     3272 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/key.pem
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      214 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/msg_without_id_dump.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        2 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/wrong_json_msg_dump.txt
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.247586 fedora_messaging-3.4.1/fedora_messaging/tests/integration/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/fedora_messaging/tests/integration/__init__.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    30864 2023-05-26 11:14:32.000000 fedora_messaging-3.4.1/fedora_messaging/tests/integration/test_api.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2830 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/integration/test_cli.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      204 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/integration/utils.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.248586 fedora_messaging-3.4.1/fedora_messaging/tests/unit/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/__init__.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    12558 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_api.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    30809 2023-05-26 11:07:51.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_cli.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    18746 2022-12-21 14:07:36.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_config.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     1868 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_example.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    25384 2023-05-26 11:07:51.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_message.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2510 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_schema_utils.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     4108 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_testing.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.249586 fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-08-01 10:49:11.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    18458 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_consumer.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    10658 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_factory.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    12064 2023-03-31 11:20:13.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_protocol.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     8160 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_service.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2685 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/utils.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.249586 fedora_messaging-3.4.1/fedora_messaging/twisted/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        0 2018-07-16 15:17:59.000000 fedora_messaging-3.4.1/fedora_messaging/twisted/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    14738 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/fedora_messaging/twisted/consumer.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    13668 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/twisted/factory.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)    17448 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/twisted/protocol.py
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     7479 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/fedora_messaging/twisted/service.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-26 11:50:56.244586 fedora_messaging-3.4.1/fedora_messaging.egg-info/
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     2519 2023-05-26 11:50:55.000000 fedora_messaging-3.4.1/fedora_messaging.egg-info/PKG-INFO
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)     4878 2023-05-26 11:50:56.000000 fedora_messaging-3.4.1/fedora_messaging.egg-info/SOURCES.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2023-05-26 11:50:55.000000 fedora_messaging-3.4.1/fedora_messaging.egg-info/dependency_links.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      129 2023-05-26 11:50:55.000000 fedora_messaging-3.4.1/fedora_messaging.egg-info/entry_points.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)        1 2021-12-14 11:27:18.000000 fedora_messaging-3.4.1/fedora_messaging.egg-info/not-zip-safe
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      130 2023-05-26 11:50:55.000000 fedora_messaging-3.4.1/fedora_messaging.egg-info/requires.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)       17 2023-05-26 11:50:56.000000 fedora_messaging-3.4.1/fedora_messaging.egg-info/top_level.txt
+-rw-rw-r--   0 abompard  (1000) abompard  (1000)      274 2021-11-22 15:44:30.000000 fedora_messaging-3.4.1/fm-consumer@.service
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1120 2022-12-21 14:07:36.000000 fedora_messaging-3.4.1/pyproject.toml
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      124 2022-12-21 14:07:36.000000 fedora_messaging-3.4.1/requirements.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       38 2023-05-26 11:50:56.250586 fedora_messaging-3.4.1/setup.cfg
+-rwxrwxr-x   0 abompard  (1000) abompard  (1000)     3003 2021-12-10 15:40:42.000000 fedora_messaging-3.4.1/setup.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      972 2023-03-31 11:20:47.000000 fedora_messaging-3.4.1/tox.ini
```

### Comparing `fedora_messaging-3.3.0/LICENSE` & `fedora_messaging-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/PKG-INFO` & `fedora_messaging-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedora_messaging
-Version: 3.3.0
+Version: 3.4.1
 Summary: A set of tools for using Fedora's messaging infrastructure
 Home-page: https://github.com/fedora-infra/fedora-messaging
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
 License: GPLv2+
 Keywords: fedora
 Platform: Fedora
```

### Comparing `fedora_messaging-3.3.0/README.rst` & `fedora_messaging-3.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/config.toml.example` & `fedora_messaging-3.4.1/config.toml.example`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/cacert.pem` & `fedora_messaging-3.4.1/configs/cacert.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/fedora-cert.pem` & `fedora_messaging-3.4.1/configs/fedora-cert.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/fedora-key.pem` & `fedora_messaging-3.4.1/configs/fedora-key.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/fedora.stg-cert.pem` & `fedora_messaging-3.4.1/configs/fedora.stg-cert.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/fedora.stg-key.pem` & `fedora_messaging-3.4.1/configs/fedora.stg-key.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/fedora.stg.toml` & `fedora_messaging-3.4.1/configs/fedora.stg.toml`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/fedora.toml` & `fedora_messaging-3.4.1/configs/fedora.toml`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/configs/stg-cacert.pem` & `fedora_messaging-3.4.1/configs/stg-cacert.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/Makefile` & `fedora_messaging-3.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/api/api.rst` & `fedora_messaging-3.4.1/docs/api/api.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/api/wire-format.rst` & `fedora_messaging-3.4.1/docs/api/wire-format.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/build-schemas-list.py` & `fedora_messaging-3.4.1/docs/build-schemas-list.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/changelog.rst` & `fedora_messaging-3.4.1/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 =============
 Release Notes
 =============
 
 .. towncrier release notes start
 
+3.4.1 (2023-05-26)
+==================
+
+Bug Fixes
+---------
+
+* Fix CI
+  (`0f2e39c <https://github.com/fedora-infra/fedora-messaging/commit/0f2e39c>`_)
+
+
+3.4.0 (2023-05-26)
+==================
+
+Features
+--------
+
+* Mirror the message priority in the headers
+  (`eba336b <https://github.com/fedora-infra/fedora-messaging/commit/eba336b>`_)
+
+
 3.3.0 (2023-03-31)
 ==================
 
 Features
 --------
 
 * Add support for asyncio-based callbacks in the consumer. As a consequence,
```

### Comparing `fedora_messaging-3.3.0/docs/conf.py` & `fedora_messaging-3.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/contributing.rst` & `fedora_messaging-3.4.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/index.rst` & `fedora_messaging-3.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/LICENSE` & `fedora_messaging-3.4.1/docs/sample_schema_package/LICENSE`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__init__.py` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/messages.cpython-38.pyc` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/messages.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/schema.cpython-36.pyc` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/schema.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/__pycache__/utils.cpython-36.pyc` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/messages.py` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/messages.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__init__.py` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_messages.cpython-38.pyc` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_messages.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_schema.cpython-36-PYTEST.pyc` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/__pycache__/test_schema.cpython-36-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages/tests/test_messages.py` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/mailman_messages.egg-info/PKG-INFO` & `fedora_messaging-3.4.1/docs/sample_schema_package/mailman_messages.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/sample_schema_package/setup.py` & `fedora_messaging-3.4.1/docs/sample_schema_package/setup.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/tutorial/conversion.rst` & `fedora_messaging-3.4.1/docs/tutorial/conversion.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/tutorial/exceptions.rst` & `fedora_messaging-3.4.1/docs/tutorial/exceptions.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/tutorial/installation.rst` & `fedora_messaging-3.4.1/docs/tutorial/installation.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/tutorial/schemas.rst` & `fedora_messaging-3.4.1/docs/tutorial/schemas.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/tutorial/usage.rst` & `fedora_messaging-3.4.1/docs/tutorial/usage.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/user-guide/cli/fedora-messaging.rst` & `fedora_messaging-3.4.1/docs/user-guide/cli/fedora-messaging.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/user-guide/consuming.rst` & `fedora_messaging-3.4.1/docs/user-guide/consuming.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/user-guide/messages.rst` & `fedora_messaging-3.4.1/docs/user-guide/messages.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/user-guide/publishing.rst` & `fedora_messaging-3.4.1/docs/user-guide/publishing.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/user-guide/quick-start.rst` & `fedora_messaging-3.4.1/docs/user-guide/quick-start.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/docs/user-guide/schemas.rst` & `fedora_messaging-3.4.1/docs/user-guide/schemas.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/api.py` & `fedora_messaging-3.4.1/fedora_messaging/api.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/cli.py` & `fedora_messaging-3.4.1/fedora_messaging/cli.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/config.py` & `fedora_messaging-3.4.1/fedora_messaging/config.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/example.py` & `fedora_messaging-3.4.1/fedora_messaging/example.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/exceptions.py` & `fedora_messaging-3.4.1/fedora_messaging/exceptions.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/message.py` & `fedora_messaging-3.4.1/fedora_messaging/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,14 +348,16 @@
         # Consumers use this to determine what schema to use and if they're out
         # of date.
         headers = headers.copy()
         headers["fedora_messaging_schema"] = get_name(self.__class__)
         now = datetime.datetime.utcnow().replace(microsecond=0, tzinfo=pytz.utc)
         headers["sent-at"] = now.isoformat()
         headers["fedora_messaging_severity"] = self.severity
+        # Mirror the priority in the headers for debugging purposes
+        headers["priority"] = config.conf["publish_priority"] or 0
         headers.update(self._filter_headers())
         message_id = str(uuid.uuid4())
         return pika.BasicProperties(
             content_type="application/json",
             content_encoding="utf-8",
             delivery_mode=2,
             headers=headers,
@@ -410,14 +412,16 @@
     @property
     def priority(self):
         return self._properties.priority or 0
 
     @priority.setter
     def priority(self, value):
         self._properties.priority = value
+        # Mirror the priority in the headers for debugging purposes
+        self._headers["priority"] = value or 0
 
     @property
     def _encoded_routing_key(self):
         """The encoded routing key used to publish the message on the broker."""
         topic = self.topic
         if config.conf["topic_prefix"]:
             topic = ".".join((config.conf["topic_prefix"].rstrip("."), topic))
```

### Comparing `fedora_messaging-3.3.0/fedora_messaging/schema_utils.py` & `fedora_messaging-3.4.1/fedora_messaging/schema_utils.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/signals.py` & `fedora_messaging-3.4.1/fedora_messaging/signals.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/testing.py` & `fedora_messaging-3.4.1/fedora_messaging/testing.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/__init__.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/ca_bundle.pem` & `fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/ca_bundle.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/cert.pem` & `fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/cert.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/fixtures/key.pem` & `fedora_messaging-3.4.1/fedora_messaging/tests/fixtures/key.pem`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/integration/test_api.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/integration/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         topic="nice.message",
         headers={"niceness": "very"},
         body={"encouragement": "You're doing great!"},
     )
     expected_headers = {
         "fedora_messaging_severity": 20,
         "fedora_messaging_schema": "base.message",
+        "priority": 0,
         "niceness": "very",
     }
     messages_received = []
 
     def callback(message):
         """Count to 3 and quit."""
         messages_received.append(message)
```

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/integration/test_cli.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_api.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_cli.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,27 +731,28 @@
 
         mock_file = mock.MagicMock()
         test_recorder = cli.Recorder(2, mock_file)
         test_recorder.collect_message(msg1)
         mock_file.write.assert_called_with(
             '{"body": {"test_key1": "test_value1"}, "headers"'
             ': {"fedora_messaging_schema": "base.message", "fedora_messaging_severity": 20, '
-            '"sent-at": "2018-11-18T10:11:41+00:00"}, "id": "273ed91d-b8b5-487a-9576-95b9fbdf3eec"'
-            ', "priority": 0, "queue": null, "topic": "test_topic1"}\n'
+            '"priority": 0, "sent-at": "2018-11-18T10:11:41+00:00"}, '
+            '"id": "273ed91d-b8b5-487a-9576-95b9fbdf3eec", '
+            '"priority": 0, "queue": null, "topic": "test_topic1"}\n'
         )
 
         with self.assertRaises(exceptions.HaltConsumer) as cm:
             test_recorder.collect_message(msg2)
         the_exception = cm.exception
         self.assertEqual(the_exception.exit_code, 0)
         self.assertEqual(test_recorder.counter, 2)
         mock_file.write.assert_called_with(
             '{"body": {"test_key2": "test_value2"}, "headers": '
             '{"fedora_messaging_schema": "base.message", "fedora_messaging_severity": '
-            '20, "sent-at": "2018-11-18T10:11:41+00:00"}, "id": '
+            '20, "priority": 0, "sent-at": "2018-11-18T10:11:41+00:00"}, "id": '
             '"273ed91d-b8b5-487a-9576-95b9fbdf3eec", "priority": 0, "queue": null, '
             '"topic": "test_topic2"}\n'
         )
 
     def test_recorded_messages_dumps_failed(self):
         """Assert that attempt to save improper recorded message is reported."""
         mock_file = mock.MagicMock()
```

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_config.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_example.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_example.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_message.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,18 +420,21 @@
 
         self.assertEqual("1970-01-01T00:00:00+00:00", msg._headers["sent-at"])
 
     def test_priority(self):
         """Assert is set correctly."""
         msg = message.Message()
         self.assertEqual(0, msg.priority)
+        self.assertEqual(0, msg._headers["priority"])
         msg.priority = 42
         self.assertEqual(42, msg.priority)
+        self.assertEqual(42, msg._headers["priority"])
         msg.priority = None
         self.assertEqual(0, msg.priority)
+        self.assertEqual(0, msg._headers["priority"])
 
     def test_properties(self):
         properties = object()
         msg = message.Message(properties=properties)
         self.assertEqual(msg._properties, properties)
 
     def test_encoded_routing_key(self):
```

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_schema_utils.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_schema_utils.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/test_testing.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_consumer.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_consumer.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_factory.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_factory.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_protocol.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_protocol.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/test_service.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/test_service.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/tests/unit/twisted/utils.py` & `fedora_messaging-3.4.1/fedora_messaging/tests/unit/twisted/utils.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/twisted/consumer.py` & `fedora_messaging-3.4.1/fedora_messaging/twisted/consumer.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/twisted/factory.py` & `fedora_messaging-3.4.1/fedora_messaging/twisted/factory.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/twisted/protocol.py` & `fedora_messaging-3.4.1/fedora_messaging/twisted/protocol.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging/twisted/service.py` & `fedora_messaging-3.4.1/fedora_messaging/twisted/service.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/fedora_messaging.egg-info/PKG-INFO` & `fedora_messaging-3.4.1/fedora_messaging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedora-messaging
-Version: 3.3.0
+Version: 3.4.1
 Summary: A set of tools for using Fedora's messaging infrastructure
 Home-page: https://github.com/fedora-infra/fedora-messaging
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
 License: GPLv2+
 Keywords: fedora
 Platform: Fedora
```

### Comparing `fedora_messaging-3.3.0/fedora_messaging.egg-info/SOURCES.txt` & `fedora_messaging-3.4.1/fedora_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/pyproject.toml` & `fedora_messaging-3.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/setup.py` & `fedora_messaging-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `fedora_messaging-3.3.0/tox.ini` & `fedora_messaging-3.4.1/tox.ini`

 * *Files identical despite different names*


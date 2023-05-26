# Comparing `tmp/AkvoDjangoFormGateway-0.0.8.tar.gz` & `tmp/AkvoDjangoFormGateway-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoDjangoFormGateway-0.0.8.tar", last modified: Wed May 24 03:01:25 2023, max compression
+gzip compressed data, was "AkvoDjangoFormGateway-0.0.9.tar", last modified: Fri May 26 06:49:59 2023, max compression
```

## Comparing `AkvoDjangoFormGateway-0.0.8.tar` & `AkvoDjangoFormGateway-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-24 03:01:25.230201 AkvoDjangoFormGateway-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.222201 AkvoDjangoFormGateway-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.222201 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_twilio_instance_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-24 03:01:12.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:01:25.226201 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-24 03:01:25.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-24 03:01:25.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:01:25.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:01:25.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-24 03:01:25.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 03:01:25.000000 AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.241266 AkvoDjangoFormGateway-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-26 06:49:59.241266 AkvoDjangoFormGateway-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-26 06:49:59.241266 AkvoDjangoFormGateway-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.233265 AkvoDjangoFormGateway-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.237266 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.237266 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.237266 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/commands/gateway_geo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.237266 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/migrations/0002_alter_akvogatewaydata_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.237266 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_geo_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_geo_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_twilio_instance_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.241266 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/utils/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-26 06:49:44.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:59.237266 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-26 06:49:59.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-26 06:49:59.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:49:59.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:49:59.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 06:49:59.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 06:49:59.000000 AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/top_level.txt
```

### Comparing `AkvoDjangoFormGateway-0.0.8/LICENSE` & `AkvoDjangoFormGateway-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/PKG-INFO` & `AkvoDjangoFormGateway-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.8/README.md` & `AkvoDjangoFormGateway-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/setup.py` & `AkvoDjangoFormGateway-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,13 +59,14 @@
         "Topic :: Internet :: WWW/HTTP",
     ],
     python_requires=">=3.8.5",
     install_requires=[
         "setuptools>=36.2",
         "twilio>=8.2.0",
         "djangorestframework>=3.12.4",
+        "requests==2.26.0",
     ]
     + INSTALL_PYTHON_REQUIRES,
     extras_require={
         "dev": ["check-manifest"],
     },
 )
```

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/feed.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/feed.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,22 +111,29 @@
                 str(o.name).lower()
                 for o in question.ag_question_question_options.all()
             ]
             count = len(set(lto).intersection(set(opt)))
             is_valid = count > 0
         return is_valid
 
-    def insert_answer(self, text: str, question: Questions, data: FormData):
+    def insert_answer(
+        self,
+        text: str,
+        question: Questions,
+        data: FormData,
+        lat: str = None,
+        lng: str = None,
+    ):
         name = None
         value = None
         options = None
         if question.type == QuestionTypes.number:
             value = text
-        if question.type == QuestionTypes.geo:
-            options = text
+        if question.type == QuestionTypes.geo and lat and lng:
+            options = [lat, lng]
         if question.type == QuestionTypes.date:
             date_format = "%d-%m-%Y"
             dv = datetime.strptime(text, date_format)
             name = dv.strftime(date_format)
         if question.type in [
             QuestionTypes.option,
             QuestionTypes.multiple_option,
```

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/migrations/0001_initial.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/models.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/models.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/serializers.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/serializers.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_init.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_init.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,26 @@
 # consider that 8 digit phone number will
 # skip to send twillio message
 phone_number = "12345678"
 
 
 class TwilioEndpointTestCase(TestCase):
     def setUp(self):
+        super().setUp()
         call_command(
             "gateway_form_seeder",
             "-f",
             "./backend/source/forms/1.json",
             "-t",
             True,
         )
 
+    def tearDown(self):
+        super().tearDown()
+
     def test_request_type(self):
         # GET not allowed
         response = client.get("/api/gateway/twilio/")
         self.assertEqual(response.status_code, 405)
 
         # POST allowed
         response = client.post("/api/gateway/twilio/")
@@ -202,14 +206,17 @@
             feed.validate_answer(
                 text=text,
                 question=question,
                 data=datapoint,
             ),
             True,
         )
+        # check lat and lng options are not json dumped
+        geo_answer = datapoint.ag_data_answer.filter(question=question).first()
+        self.assertEqual(geo_answer.options, [lat, lng])
 
         # Phone question
         question = feed.get_question(form=survey, data=datapoint)
         # Answer Phone question
         reply_text = "0829111"
         json_form = {
             "Body": reply_text,
```

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_twilio_instance_endpoint.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_twilio_instance_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,7 +218,17 @@
             True,
         )
         answer = Answers.objects.filter(
             data=datapoint, question=question
         ).first()
         self.assertEqual(answer.name, reply_text)
         self.assertEqual(response.json(), "Thank you!")
+
+        # Test if second submission get first question
+        reply_text = "hi"
+        response = client.post(
+            f"/api/gateway/twilio/{form_id}?format=json",
+            {"From": f"whatsapp:+{phone_number}", "Body": reply_text},
+        )
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        # No welcome message and select forms
+        self.assertNotEqual(response.json(), feed.get_list_form())
```

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/tests/tests_validation.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/tests/tests_validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/urls.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/urls.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/utils/functions.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/utils/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,24 @@
 
 
 fake = Faker()
 
 
 def get_answer_value(answer: Answers):
     if answer.question.type in [
-        QuestionTypes.geo,
         QuestionTypes.option,
         QuestionTypes.multiple_option,
     ]:
         return answer.options
+    if answer.question.type == QuestionTypes.geo:
+        return {
+            "lat": answer.options[0],
+            "lng": answer.options[1],
+            "address": answer.name
+        }
     elif answer.question.type == QuestionTypes.number:
         return answer.value
     else:
         return answer.name
 
 
 def set_answer_option(data, question):
@@ -66,20 +71,23 @@
             date_end=timezone.datetime.now().date(),
         ).strftime("%d-%m-%Y")
     else:
         pass
     return name, value, option
 
 
-def add_fake_answers(data: FormData) -> None:
+def add_fake_answers(data: FormData, submitted: bool = False) -> None:
     form = data.form
-    number_of_answered = random.choice(
-        form.ag_form_questions.values_list("id", flat=True)
+    questions = form.ag_form_questions.all()
+    number_of_answered = (
+        questions.count()
+        if submitted
+        else random.choice(form.ag_form_questions.values_list("id", flat=True))
     )
-    for index, question in enumerate(form.ag_form_questions.all()):
+    for index, question in enumerate(questions):
         if index < number_of_answered:
             name, value, option = set_answer_data(data, question)
             Answers.objects.create(
                 data=data,
                 question=question,
                 name=name,
                 value=value,
@@ -94,24 +102,24 @@
         for i in range(repeat):
             now_date = datetime.now()
             start_date = now_date - timedelta(days=5 * 365)
             created = fake.date_between(start_date, now_date)
             created = datetime.combine(created, time.min)
             lat = fake.latitude()
             lng = fake.longitude()
-            geo_value = f"{lat},{lng}"
+            geo_value = [float(lat), float(lng)]
             data = FormData.objects.create(
                 form=form,
                 name=fake.pystr_format(),
                 phone=fake.phone_number(),
                 geo=geo_value,
             )
             data.created = make_aware(created)
             data.save()
-            add_fake_answers(data)
+            add_fake_answers(data=data, submitted=submitted)
             number_of_answered = Answers.objects.filter(data=data.id).count()
             if submitted:
                 data.status = StatusTypes.submitted
                 data.save()
             if len(form.ag_form_questions.all()) == number_of_answered:
                 data.status = StatusTypes.submitted
                 data.save()
```

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/utils/validation.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/utils/validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway/views.py` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,20 @@
     ListFormSerializer,
     TwilioSerializer,
     ListDataSerializer,
     DetailDataSerializer,
 )
 from .constants import StatusTypes
 from .feed import Feed
+from .utils.services import store_geo_service
 
 account_sid = settings.TWILIO_ACCOUNT_SID
 auth_token = settings.TWILIO_AUTH_TOKEN
 from_number = settings.TWILIO_PHONE_NUMBER
+google_api_key = settings.GOOGLE_MAPS_API_KEY
 
 
 @permission_classes([AllowAny])
 class CheckView(GenericViewSet):
     def check(self, request):
         return Response({"message": settings.TWILIO_ACCOUNT_SID})
 
@@ -61,14 +63,15 @@
         init, form_id = feed.get_init_survey_session(text=text)
         datapoint = feed.get_draft_datapoint(phone=phone)
         survey = (
             form_instance
             if form_instance
             else feed.get_form(form_id=form_id, data=datapoint)
         )
+        # get last question
         lq = feed.get_question(form=survey, data=datapoint)
         message = None
         if text in feed.welcome and not datapoint and not form_instance:
             message = feed.get_list_form()
 
         new_datapoint = not datapoint and phone and len(str(phone).strip())
         init_session = form_instance or init
@@ -82,15 +85,21 @@
             message = f"{lq.order}. {lq.text}"
 
         if datapoint and lq:
             valid_answer = feed.validate_answer(
                 text=text, question=lq, data=datapoint, image_type=image_type
             )
             if valid_answer:
-                feed.insert_answer(text=text, question=lq, data=datapoint)
+                aw = feed.insert_answer(
+                    text=text, question=lq, data=datapoint, lat=lat, lng=lng
+                )
+                store_geo_service(
+                    answer=aw,
+                    api_key=google_api_key,
+                )
                 nq = feed.get_last_question(data=datapoint)
                 if nq:
                     # show next question
                     message = f"{nq.order}. {nq.text}"
                     message += feed.show_options(question=nq)
                 else:
                     feed.set_as_completed(data=datapoint)
```

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/PKG-INFO` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.8/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt` & `AkvoDjangoFormGateway-0.0.9/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,23 +19,28 @@
 src/AkvoDjangoFormGateway.egg-info/not-zip-safe
 src/AkvoDjangoFormGateway.egg-info/requires.txt
 src/AkvoDjangoFormGateway.egg-info/top_level.txt
 src/AkvoDjangoFormGateway/management/__init__.py
 src/AkvoDjangoFormGateway/management/commands/__init__.py
 src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
 src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
+src/AkvoDjangoFormGateway/management/commands/gateway_geo_converter.py
 src/AkvoDjangoFormGateway/migrations/0001_initial.py
+src/AkvoDjangoFormGateway/migrations/0002_alter_akvogatewaydata_options.py
 src/AkvoDjangoFormGateway/migrations/__init__.py
 src/AkvoDjangoFormGateway/tests/__init__.py
 src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
 src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
 src/AkvoDjangoFormGateway/tests/tests_env.py
 src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
+src/AkvoDjangoFormGateway/tests/tests_geo_converter.py
+src/AkvoDjangoFormGateway/tests/tests_geo_question.py
 src/AkvoDjangoFormGateway/tests/tests_init.py
 src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
 src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
 src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
 src/AkvoDjangoFormGateway/tests/tests_twilio_instance_endpoint.py
 src/AkvoDjangoFormGateway/tests/tests_validation.py
 src/AkvoDjangoFormGateway/utils/__init__.py
 src/AkvoDjangoFormGateway/utils/functions.py
+src/AkvoDjangoFormGateway/utils/services.py
 src/AkvoDjangoFormGateway/utils/validation.py
```


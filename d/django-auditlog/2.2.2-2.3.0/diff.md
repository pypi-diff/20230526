# Comparing `tmp/django-auditlog-2.2.2.tar.gz` & `tmp/django-auditlog-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-auditlog-2.2.2.tar", last modified: Tue Jan 17 08:10:29 2023, max compression
+gzip compressed data, was "django-auditlog-2.3.0.tar", last modified: Fri May 26 13:20:06 2023, max compression
```

## Comparing `django-auditlog-2.2.2.tar` & `django-auditlog-2.3.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.041345 django-auditlog-2.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.029345 django-auditlog-2.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.033345 django-auditlog-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-17 08:10:29.041345 django-auditlog-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.033345 django-auditlog-2.2.2/auditlog/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.033345 django-auditlog-2.2.2/auditlog/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.033345 django-auditlog-2.2.2/auditlog/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/management/commands/auditlogflush.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.037345 django-auditlog-2.2.2/auditlog/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0002_auto_support_long_primary_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0003_logentry_remote_addr.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0004_logentry_detailed_object_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0005_logentry_additional_data_verbose_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0006_object_pk_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0007_object_pk_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0008_action_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0009_alter_logentry_additional_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0010_alter_logentry_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0011_logentry_serialized_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/0012_add_logentry_action_access.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    21179 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.037345 django-auditlog-2.2.2/auditlog_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.037345 django-auditlog-2.2.2/auditlog_tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/fixtures/m2m_test_fixture.json
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.037345 django-auditlog-2.2.2/auditlog_tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/templates/simplemodel_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    67124 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/auditlog_tests/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.037345 django-auditlog-2.2.2/django_auditlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-01-17 08:10:28.000000 django-auditlog-2.2.2/django_auditlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-01-17 08:10:28.000000 django-auditlog-2.2.2/django_auditlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 08:10:28.000000 django-auditlog-2.2.2/django_auditlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 08:10:28.000000 django-auditlog-2.2.2/django_auditlog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-17 08:10:28.000000 django-auditlog-2.2.2/django_auditlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-17 08:10:28.000000 django-auditlog-2.2.2/django_auditlog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.037345 django-auditlog-2.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:10:29.041345 django-auditlog-2.2.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/source/internals.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 08:10:29.041345 django-auditlog-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-17 08:10:11.000000 django-auditlog-2.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.251098 django-auditlog-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.243098 django-auditlog-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.243098 django-auditlog-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-26 13:20:06.251098 django-auditlog-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.247098 django-auditlog-2.3.0/auditlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.247098 django-auditlog-2.3.0/auditlog/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.247098 django-auditlog-2.3.0/auditlog/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/management/commands/auditlogflush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.247098 django-auditlog-2.3.0/auditlog/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0002_auto_support_long_primary_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0003_logentry_remote_addr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0004_logentry_detailed_object_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0005_logentry_additional_data_verbose_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0006_object_pk_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0007_object_pk_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0008_action_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0009_alter_logentry_additional_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0010_alter_logentry_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0011_logentry_serialized_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/0012_add_logentry_action_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21179 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.247098 django-auditlog-2.3.0/auditlog_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.247098 django-auditlog-2.3.0/auditlog_tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/fixtures/m2m_test_fixture.json
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.247098 django-auditlog-2.3.0/auditlog_tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/templates/simplemodel_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67571 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/auditlog_tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.251098 django-auditlog-2.3.0/django_auditlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-26 13:20:06.000000 django-auditlog-2.3.0/django_auditlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-26 13:20:06.000000 django-auditlog-2.3.0/django_auditlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:20:06.000000 django-auditlog-2.3.0/django_auditlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:20:06.000000 django-auditlog-2.3.0/django_auditlog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 13:20:06.000000 django-auditlog-2.3.0/django_auditlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 13:20:06.000000 django-auditlog-2.3.0/django_auditlog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.251098 django-auditlog-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:20:06.251098 django-auditlog-2.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/source/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:20:06.251098 django-auditlog-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 13:19:51.000000 django-auditlog-2.3.0/tox.ini
```

### Comparing `django-auditlog-2.2.2/.github/workflows/release.yml` & `django-auditlog-2.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/.github/workflows/test.yml` & `django-auditlog-2.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/.gitignore` & `django-auditlog-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/.pre-commit-config.yaml` & `django-auditlog-2.3.0/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ---
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.8
         args:
           - "--target-version"
           - "py37"
   - repo: https://github.com/PyCQA/flake8
-    rev: "5.0.4"
+    rev: "6.0.0"
     hooks:
       - id: flake8
         args: ["--max-line-length", "110"]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.2
+    rev: v3.4.0
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.12.0
+    rev: 1.13.0
     hooks:
     - id: django-upgrade
       args: [--target-version, "3.2"]
```

### Comparing `django-auditlog-2.2.2/CHANGELOG.md` & `django-auditlog-2.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changes
 
 ## Next Release
 
+## 2.3.0 (2023-05-26)
+
+#### Improvements
+
+- Django: Confirm Django 4.2 support ([#530](https://github.com/jazzband/django-auditlog/pull/530))
+
+#### Fixes
+fix: Fix a bug in audit log admin page when `USE_TZ=False`. ([#511](https://github.com/jazzband/django-auditlog/pull/511))
+
 ## 2.2.2 (2023-01-16)
 
 #### Fixes
 
 - fix: revert [#449](https://github.com/jazzband/django-auditlog/pull/449) "Make log entries read-only in the admin" as it breaks deletion of any auditlogged model through the admin when `AuditlogHistoryField` is used. ([#496](https://github.com/jazzband/django-auditlog/pull/496))
 
 ## 2.2.1 (2022-11-28)
```

### Comparing `django-auditlog-2.2.2/CODE_OF_CONDUCT.md` & `django-auditlog-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/LICENSE` & `django-auditlog-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/PKG-INFO` & `django-auditlog-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auditlog
-Version: 2.2.2
+Version: 2.3.0
 Summary: Audit log app for Django
 Home-page: https://github.com/jazzband/django-auditlog
 Author: Jan-Jelle Kester
 License: MIT
 Project-URL: Documentation, https://django-auditlog.readthedocs.io
 Project-URL: Source, https://github.com/jazzband/django-auditlog
 Project-URL: Tracker, https://github.com/jazzband/django-auditlog/issues
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 django-auditlog
 ===============
```

### Comparing `django-auditlog-2.2.2/README.md` & `django-auditlog-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/admin.py` & `django-auditlog-2.3.0/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/conf.py` & `django-auditlog-2.3.0/auditlog/conf.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/context.py` & `django-auditlog-2.3.0/auditlog/context.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/diff.py` & `django-auditlog-2.3.0/auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/filters.py` & `django-auditlog-2.3.0/auditlog/filters.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/management/commands/auditlogflush.py` & `django-auditlog-2.3.0/auditlog/management/commands/auditlogflush.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/middleware.py` & `django-auditlog-2.3.0/auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/migrations/0001_initial.py` & `django-auditlog-2.3.0/auditlog/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("contenttypes", "0001_initial"),
     ]
 
     operations = [
         migrations.CreateModel(
```

### Comparing `django-auditlog-2.2.2/auditlog/migrations/0012_add_logentry_action_access.py` & `django-auditlog-2.3.0/auditlog/migrations/0012_add_logentry_action_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.1 on 2022-10-13 07:56
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("auditlog", "0011_logentry_serialized_data"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="logentry",
```

### Comparing `django-auditlog-2.2.2/auditlog/mixins.py` & `django-auditlog-2.3.0/auditlog/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from django.conf import settings
 from django.contrib import admin
 from django.core.exceptions import FieldDoesNotExist
 from django.forms.utils import pretty_name
 from django.urls.exceptions import NoReverseMatch
 from django.utils.html import format_html, format_html_join
 from django.utils.safestring import mark_safe
-from django.utils.timezone import localtime
+from django.utils.timezone import is_aware, localtime
 
 from auditlog.models import LogEntry
 from auditlog.registry import auditlog
 from auditlog.signals import accessed
 
 MAX = 75
 
 
 class LogEntryAdminMixin:
     @admin.display(description="Created")
     def created(self, obj):
-        return localtime(obj.timestamp)
+        if is_aware(obj.timestamp):
+            return localtime(obj.timestamp)
+        return obj.timestamp
 
     @admin.display(description="User")
     def user_url(self, obj):
         if obj.actor:
             app_label, model = settings.AUTH_USER_MODEL.split(".")
             viewname = f"admin:{app_label}_{model.lower()}_change"
             try:
```

### Comparing `django-auditlog-2.2.2/auditlog/models.py` & `django-auditlog-2.3.0/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog/receivers.py` & `django-auditlog-2.3.0/auditlog/receivers.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 def log_access(sender, instance, **kwargs):
     """
     Signal receiver that creates a log entry when a model instance is accessed in a AccessLogDetailView.
 
     Direct use is discouraged, connect your model through :py:func:`auditlog.registry.register` instead.
     """
     if instance.pk is not None:
-
         LogEntry.objects.log_create(
             instance,
             action=LogEntry.Action.ACCESS,
             changes="null",
         )
```

### Comparing `django-auditlog-2.2.2/auditlog/registry.py` & `django-auditlog-2.3.0/auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog_tests/models.py` & `django-auditlog-2.3.0/auditlog_tests/models.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog_tests/test_commands.py` & `django-auditlog-2.3.0/auditlog_tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog_tests/test_settings.py` & `django-auditlog-2.3.0/auditlog_tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/auditlog_tests/tests.py` & `django-auditlog-2.3.0/auditlog_tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1310,14 +1310,25 @@
             ("America/Buenos_Aires", "2022-08-01 09:00:00"),
             ("Asia/Kathmandu", "2022-08-01 17:45:00"),
         ]:
             with self.settings(TIME_ZONE=tz):
                 created = self.admin.created(log_entry)
                 self.assertEqual(created.strftime("%Y-%m-%d %H:%M:%S"), timestamp)
 
+    @freezegun.freeze_time("2022-08-01 12:00:00Z")
+    def test_created_naive_datetime(self):
+        with self.settings(USE_TZ=False):
+            obj = SimpleModel.objects.create(text="For USE_TZ=False test")
+            log_entry = obj.history.latest()
+            created = self.admin.created(log_entry)
+            self.assertEqual(
+                created.strftime("%Y-%m-%d %H:%M:%S"),
+                "2022-08-01 12:00:00",
+            )
+
 
 class DiffMsgTest(TestCase):
     def setUp(self):
         super().setUp()
         self.site = AdminSite()
         self.admin = LogEntryAdmin(LogEntry, self.site)
```

### Comparing `django-auditlog-2.2.2/django_auditlog.egg-info/PKG-INFO` & `django-auditlog-2.3.0/django_auditlog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auditlog
-Version: 2.2.2
+Version: 2.3.0
 Summary: Audit log app for Django
 Home-page: https://github.com/jazzband/django-auditlog
 Author: Jan-Jelle Kester
 License: MIT
 Project-URL: Documentation, https://django-auditlog.readthedocs.io
 Project-URL: Source, https://github.com/jazzband/django-auditlog
 Project-URL: Tracker, https://github.com/jazzband/django-auditlog/issues
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 django-auditlog
 ===============
```

### Comparing `django-auditlog-2.2.2/django_auditlog.egg-info/SOURCES.txt` & `django-auditlog-2.3.0/django_auditlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/docs/Makefile` & `django-auditlog-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/docs/make.bat` & `django-auditlog-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/docs/source/conf.py` & `django-auditlog-2.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/docs/source/index.rst` & `django-auditlog-2.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/docs/source/installation.rst` & `django-auditlog-2.3.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/docs/source/internals.rst` & `django-auditlog-2.3.0/docs/source/internals.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/docs/source/usage.rst` & `django-auditlog-2.3.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-2.2.2/setup.py` & `django-auditlog-2.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,10 +37,11 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

### Comparing `django-auditlog-2.2.2/tox.ini` & `django-auditlog-2.3.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tox]
 envlist =
     {py37,py38,py39,py310}-django32
     {py38,py39,py310}-django40
-    {py38,py39,py310,py311}-django{41,main}
+    {py38,py39,py310,py311}-django{41,42}
+    {py310,py311}-djangomain
     py37-docs
     py38-lint
 
 [testenv]
 setenv =
   COVERAGE_FILE={toxworkdir}/.coverage.{envname}
 commands =
     coverage run --source auditlog runtests.py
     coverage xml
 deps =
     django32: Django>=3.2,<3.3
     django40: Django>=4.0,<4.1
     django41: Django>=4.1,<4.2
+    django42: Django>=4.2,<4.3
     djangomain: https://github.com/django/django/archive/main.tar.gz
     # Test requirements
     coverage
     codecov
     freezegun
     psycopg2-binary
 passenv=
```


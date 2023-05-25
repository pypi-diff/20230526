# Comparing `tmp/lndb-0.44.7.tar.gz` & `tmp/lndb-0.45a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.44.7.tar", last modified: Fri Apr 28 05:57:26 2023, max compression
+gzip compressed data, was "lndb-0.45a1.tar", last modified: Thu May 25 22:03:25 2023, max compression
```

## Comparing `lndb-0.44.7.tar` & `lndb-0.45a1.tar`

### file list

```diff
@@ -1,80 +1,79 @@
--rw-r--r--   0        0        0     3832 2023-04-10 14:26:28.783318 lndb-0.44.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-15 08:56:55.830020 lndb-0.44.7/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-15 08:56:55.830119 lndb-0.44.7/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-03-15 08:56:55.830224 lndb-0.44.7/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-24 09:27:00.933000 lndb-0.44.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-15 08:56:55.830520 lndb-0.44.7/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 05:09:16.038571 lndb-0.44.7/README.md
--rw-r--r--   0        0        0       52 2023-03-15 08:56:55.830736 lndb-0.44.7/docs/api.md
--rw-r--r--   0        0        0    48191 2023-04-28 05:56:59.401992 lndb-0.44.7/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-15 08:56:55.831086 lndb-0.44.7/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-15 08:56:55.831186 lndb-0.44.7/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-27 05:09:16.039131 lndb-0.44.7/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-27 05:09:16.039234 lndb-0.44.7/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-22 15:24:35.393597 lndb-0.44.7/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-15 08:56:55.831660 lndb-0.44.7/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-10 14:26:28.783932 lndb-0.44.7/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-10 14:26:28.784059 lndb-0.44.7/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-03-27 05:09:16.039598 lndb-0.44.7/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10238 2023-04-27 10:15:48.138286 lndb-0.44.7/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     6419 2023-04-27 10:15:48.138461 lndb-0.44.7/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6390 2023-04-24 09:27:00.941223 lndb-0.44.7/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3746 2023-04-26 05:23:05.373464 lndb-0.44.7/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-27 05:09:16.039994 lndb-0.44.7/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-21 03:09:31.419101 lndb-0.44.7/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-03-15 08:56:55.832700 lndb-0.44.7/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-22 15:24:35.394504 lndb-0.44.7/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-03-15 08:56:55.832922 lndb-0.44.7/docs/index.md
--rw-r--r--   0        0        0      118 2023-03-15 08:56:55.833018 lndb-0.44.7/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-28 05:56:52.880114 lndb-0.44.7/lndb/__init__.py
--rw-r--r--   0        0        0     4697 2023-04-27 17:03:55.795190 lndb-0.44.7/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-03-15 08:56:55.833550 lndb-0.44.7/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 14:26:28.784379 lndb-0.44.7/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-28 05:45:57.926671 lndb-0.44.7/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-10 14:26:28.784709 lndb-0.44.7/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-10 14:26:28.784835 lndb-0.44.7/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-26 05:23:05.375280 lndb-0.44.7/lndb/_info.py
--rw-r--r--   0        0        0     6035 2023-04-27 10:15:48.139549 lndb-0.44.7/lndb/_init_instance.py
--rw-r--r--   0        0        0     6729 2023-04-27 10:15:48.140360 lndb-0.44.7/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-10 14:26:28.785194 lndb-0.44.7/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-10 14:26:28.785299 lndb-0.44.7/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-26 05:23:05.375597 lndb-0.44.7/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-22 15:24:35.395863 lndb-0.44.7/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-03-15 08:56:55.834680 lndb-0.44.7/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-26 05:23:05.375756 lndb-0.44.7/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-10 14:26:28.785570 lndb-0.44.7/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      803 2023-04-27 10:15:48.140662 lndb-0.44.7/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-03-15 08:56:55.834857 lndb-0.44.7/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-24 09:27:00.946199 lndb-0.44.7/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-19 06:33:40.117765 lndb-0.44.7/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-03-15 08:56:55.835145 lndb-0.44.7/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-03-15 08:56:55.835215 lndb-0.44.7/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-21 03:09:31.420591 lndb-0.44.7/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-10 14:26:28.785901 lndb-0.44.7/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-28 04:03:47.769616 lndb-0.44.7/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-10 14:26:28.786021 lndb-0.44.7/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-03-15 08:56:55.835748 lndb-0.44.7/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-03-15 08:56:55.835829 lndb-0.44.7/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-10 14:26:28.786141 lndb-0.44.7/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-04-27 10:15:48.140982 lndb-0.44.7/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-27 05:09:16.041820 lndb-0.44.7/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-03-15 08:56:55.836258 lndb-0.44.7/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-10 14:26:28.786361 lndb-0.44.7/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-03-15 08:56:55.836438 lndb-0.44.7/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-20 10:25:09.955595 lndb-0.44.7/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-23 05:23:25.735656 lndb-0.44.7/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-24 09:27:00.951105 lndb-0.44.7/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-03-15 08:56:55.836803 lndb-0.44.7/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-10 14:26:28.786692 lndb-0.44.7/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-10 14:26:28.786816 lndb-0.44.7/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-03-15 08:56:55.837137 lndb-0.44.7/lndb/test/_env.py
--rw-r--r--   0        0        0     3911 2023-04-27 10:15:48.141161 lndb-0.44.7/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-10 14:26:28.787063 lndb-0.44.7/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-03-15 08:56:55.837581 lndb-0.44.7/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-03-15 08:56:55.837695 lndb-0.44.7/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 14:26:28.787186 lndb-0.44.7/noxfile.py
--rw-r--r--   0        0        0     1396 2023-04-28 05:45:57.926943 lndb-0.44.7/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 14:26:28.787386 lndb-0.44.7/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-15 08:56:55.838152 lndb-0.44.7/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:24:58.325988 lndb-0.44.7/tests/test_notebooks.py
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.7/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-05-24 18:13:34.371502 lndb-0.45a1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-24 18:13:34.371611 lndb-0.45a1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-24 18:13:34.371684 lndb-0.45a1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-24 18:13:34.371770 lndb-0.45a1/.gitignore
+-rw-r--r--   0        0        0     1777 2023-05-24 18:13:34.371851 lndb-0.45a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-24 18:13:34.371968 lndb-0.45a1/LICENSE
+-rw-r--r--   0        0        0      173 2023-05-24 18:13:34.372033 lndb-0.45a1/README.md
+-rw-r--r--   0        0        0       52 2023-05-24 18:13:34.372124 lndb-0.45a1/docs/api.md
+-rw-r--r--   0        0        0    48915 2023-05-25 22:02:57.989850 lndb-0.45a1/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-05-24 18:13:34.372476 lndb-0.45a1/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-05-24 18:13:34.372565 lndb-0.45a1/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-05-24 18:13:34.372660 lndb-0.45a1/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-05-24 18:13:34.372727 lndb-0.45a1/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-05-24 18:13:34.372809 lndb-0.45a1/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-05-24 18:13:34.372876 lndb-0.45a1/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2589 2023-05-25 22:02:47.332671 lndb-0.45a1/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-05-24 18:13:34.373075 lndb-0.45a1/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5025 2023-05-25 13:55:42.990512 lndb-0.45a1/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11082 2023-05-25 13:55:42.990674 lndb-0.45a1/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     6639 2023-05-25 13:55:42.990928 lndb-0.45a1/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     7616 2023-05-25 13:56:23.677378 lndb-0.45a1/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-05-25 15:46:50.017574 lndb-0.45a1/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-05-25 13:55:42.991225 lndb-0.45a1/docs/guide/index.md
+-rw-r--r--   0        0        0     3331 2023-05-24 18:13:34.373961 lndb-0.45a1/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-05-24 18:13:34.374075 lndb-0.45a1/docs/index.md
+-rw-r--r--   0        0        0      118 2023-05-24 18:13:34.374173 lndb-0.45a1/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-05-25 22:02:36.128361 lndb-0.45a1/lndb/__init__.py
+-rw-r--r--   0        0        0     5268 2023-05-24 18:13:34.374405 lndb-0.45a1/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-05-24 18:13:34.374517 lndb-0.45a1/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-24 18:13:34.374613 lndb-0.45a1/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-05-24 18:13:34.374688 lndb-0.45a1/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-05-24 18:13:34.374754 lndb-0.45a1/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-05-24 18:13:34.374825 lndb-0.45a1/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-05-24 18:13:34.374892 lndb-0.45a1/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-05-25 12:49:05.083933 lndb-0.45a1/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6729 2023-05-24 18:13:34.375083 lndb-0.45a1/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-05-24 18:13:34.375181 lndb-0.45a1/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-24 18:13:34.375248 lndb-0.45a1/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-05-24 18:13:34.375322 lndb-0.45a1/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-05-24 18:13:34.375413 lndb-0.45a1/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-05-24 18:13:34.375498 lndb-0.45a1/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-05-24 18:13:34.375575 lndb-0.45a1/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-05-24 18:13:34.375787 lndb-0.45a1/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      790 2023-05-24 18:13:34.375906 lndb-0.45a1/lndb/_notebook.py
+-rw-r--r--   0        0        0      803 2023-05-24 18:13:34.375990 lndb-0.45a1/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-05-24 18:13:34.376692 lndb-0.45a1/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-05-24 18:13:34.377124 lndb-0.45a1/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-05-24 18:13:34.377222 lndb-0.45a1/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-05-24 18:13:34.377292 lndb-0.45a1/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-05-24 18:13:34.377359 lndb-0.45a1/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3905 2023-05-24 18:13:34.377464 lndb-0.45a1/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-05-24 18:13:34.377571 lndb-0.45a1/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-05-24 18:13:34.377656 lndb-0.45a1/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     7299 2023-05-25 21:32:27.594442 lndb-0.45a1/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-05-24 18:13:34.397245 lndb-0.45a1/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-05-24 18:13:34.397345 lndb-0.45a1/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-05-24 18:13:34.397862 lndb-0.45a1/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-05-24 18:13:34.397995 lndb-0.45a1/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-05-24 18:13:34.398092 lndb-0.45a1/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-05-24 18:13:34.398168 lndb-0.45a1/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-05-24 18:13:34.398249 lndb-0.45a1/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-05-24 18:13:34.398328 lndb-0.45a1/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2710 2023-05-25 21:55:19.754812 lndb-0.45a1/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-05-24 18:13:34.398512 lndb-0.45a1/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-05-24 18:13:34.398603 lndb-0.45a1/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-05-24 18:13:34.398679 lndb-0.45a1/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-05-24 18:13:34.398758 lndb-0.45a1/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-05-24 18:13:34.398886 lndb-0.45a1/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-24 18:13:34.398951 lndb-0.45a1/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-05-24 18:13:34.399040 lndb-0.45a1/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-05-24 18:13:34.399143 lndb-0.45a1/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-05-24 18:13:34.399213 lndb-0.45a1/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-05-24 18:13:34.399292 lndb-0.45a1/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-05-24 18:13:34.399371 lndb-0.45a1/noxfile.py
+-rw-r--r--   0        0        0     1420 2023-05-24 18:13:34.399454 lndb-0.45a1/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-05-24 18:13:34.399557 lndb-0.45a1/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-05-24 18:13:34.399639 lndb-0.45a1/tests/test_init_instance.py
+-rw-r--r--   0        0        0      379 2023-05-24 18:13:34.399723 lndb-0.45a1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 lndb-0.45a1/PKG-INFO
```

### Comparing `lndb-0.44.7/.github/workflows/build.yml` & `lndb-0.45a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/.github/workflows/latest-changes.yml` & `lndb-0.45a1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/.gitignore` & `lndb-0.45a1/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/.pre-commit-config.yaml` & `lndb-0.45a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/LICENSE` & `lndb-0.45a1/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/docs/changelog.md` & `lndb-0.45a1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🏗️ Remove SQL-level schema modules | [380](https://github.com/laminlabs/lndb/pull/380) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.45a1
+✨ Add track command to CLI | [378](https://github.com/laminlabs/lndb/pull/378) | [Koncopd](https://github.com/Koncopd) | 2023-05-23 |
+📝 Improve migration docs | [379](https://github.com/laminlabs/lndb/pull/379) | [Zethson](https://github.com/Zethson) | 2023-05-22 |
+🔊 Use lamin_logger in test_notebooks.py | [376](https://github.com/laminlabs/lndb/pull/376) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
+Add universal_pathlib to dependencies | [375](https://github.com/laminlabs/lndb/pull/375) | [Zethson](https://github.com/Zethson) | 2023-05-02 |
 ⬆️ Upgrade lnhub-rest to 0.9.4 | [373](https://github.com/laminlabs/lndb/pull/373) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.44.7
 🚑 Fix load | [372](https://github.com/laminlabs/lndb/pull/372) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-27 | 0.44.6
 ✨ Add `--storage` arg to `lamin load` | [370](https://github.com/laminlabs/lndb/pull/370) | [falexwolf](https://github.com/falexwolf) | 2023-04-27 |
 ⬆️ Upgrade lnhub-rest | [369](https://github.com/laminlabs/lndb/pull/369) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.44.5
 ✨ Allow to set additional fsspec kwargs for cloud instances | [366](https://github.com/laminlabs/lndb/pull/366) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 | 0.44.4
 ⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
 🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
```

### Comparing `lndb-0.44.7/docs/faq/check-synchronization.ipynb` & `lndb-0.45a1/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/docs/faq/clone.ipynb` & `lndb-0.45a1/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.45a1/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/docs/faq/manage-migrations.ipynb` & `lndb-0.45a1/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/docs/faq/switch-environment.ipynb` & `lndb-0.45a1/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.45a1/docs/faq/test-migrations-e2e.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9764583333333333%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 3: "*

 * *            "{'attachments': OrderedDict()}, 7: {'attachments': OrderedDict()}, 8: {'source': "*

 * *            "['lndb.test.migrate_clone(\\n', '    "*

 * *            'db="postgresql://batman:robin@35.222.187.204:5432/lamindata", '*

 * *            'schema="bionty,lamin1"\\n\', \')\']}, delete: [9]}'}*

```diff
@@ -1,20 +1,22 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "# Test migrations e2e on clones of instances"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "78e419b6-cfe0-452f-ac8f-49adc91621df",
             "metadata": {},
             "source": [
                 "There are two ways of invoking this functionality: `migrate_clone` and `migrate_clones`. "
             ]
         },
@@ -25,14 +27,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lndb"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "119134fc-1362-4b6f-85e9-d65e5ab091cf",
             "metadata": {},
             "source": [
                 "## SQLite"
             ]
         },
@@ -67,42 +70,32 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "lndb.test.migrate_clones(\"lnschema_core\", n_instances=1, dialect_name=\"sqlite\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "e53c8996-73a1-4c5f-b54f-4ea9ea117702",
             "metadata": {},
             "source": [
                 "## Postgres"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cd10731f-5667-4550-99db-90fb47e92c32",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# replace with lamindata!\n",
-                "# lndb.test.migrate_clone(\n",
-                "#     db=\"postgresql://batman:robin@35.222.187.204:5432/retro\", schema=\"bionty,retro\"\n",
-                "# )"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "58c449e1-74e3-46b4-9361-343802fc1841",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "lndb.test.migrate_clones(\"lnschema_core\", n_instances=1, dialect_name=\"postgresql\")"
+                "lndb.test.migrate_clone(\n",
+                "    db=\"postgresql://batman:robin@35.222.187.204:5432/lamindata\", schema=\"bionty,lamin1\"\n",
+                ")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "py39",
             "language": "python",
```

### Comparing `lndb-0.44.7/docs/faq/test-migrations-unit.ipynb` & `lndb-0.45a1/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/docs/guide/01-setup-user.ipynb` & `lndb-0.45a1/docs/guide/01-setup-user.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9633556547619048%*

 * *Differences: {"'cells'": "{3: {'source': ['### Your user account does not yet exist'], 'attachments': "*

 * *            "OrderedDict()}, 4: {'attachments': OrderedDict()}, 5: {'source': ['### Your user "*

 * *            "account exists'], 'attachments': OrderedDict()}, 6: {'attachments': OrderedDict()}, "*

 * *            "8: {'source': ['### You did not confim the email and try to sign up again'], "*

 * *            "'attachments': OrderedDict()}, 9: {'attachments': OrderedDict()}, 11: {'attachments': "*

 * *            "OrderedDict()}, 12:  […]*

```diff
@@ -24,21 +24,23 @@
                 "tags": []
             },
             "source": [
                 "## Sign up"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### The user account does not yet exist"
+                "### Your user account does not yet exist"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You only need to sign up once. For a non-signed-up email, on the CLI, call\n",
                 "```\n",
                 "!lamin signup testuser1@lamin.ai\n",
                 "```\n",
@@ -54,21 +56,23 @@
                 "Generated login password: cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\n",
                 "Email & password are cached: /Users/testuser1/.lndb/user-testuser1@lamin.ai.env!\n",
                 "Going forward, credentials are auto-loaded. In case of loss, recover your password via email: https://lamin.ai\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### The user account exists"
+                "### Your user account exists"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If the user tries to sign up again, an error message is raised:\n",
                 "\n",
                 "```\n",
                 "!lamin signup testuser1@lamin.ai\n",
@@ -81,21 +85,23 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert ln.setup.signup(\"testuser1@lamin.ai\") == \"user-exists\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### The user did not confim the email and tries to sign up again"
+                "### You did not confim the email and try to sign up again"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This raises the following error.\n",
                 "```\n",
                 "RuntimeError: It seems you already signed up with this email. Please click on the link in the confirmation email that you should have received from lamin.ai.\n",
                 "```\n",
@@ -110,82 +116,58 @@
                 "tags": []
             },
             "source": [
                 "## Log in"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Log in with your email:"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "!lamin login \"testuser1@lamin.ai\" --password \"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\"\n",
-                "```"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.login(\n",
                 "    \"testuser1@lamin.ai\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\"\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Or with your handle:\n",
-                "```\n",
-                "!lamin login testuser1 --password \"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\"\n",
-                "```"
+                ")  # CLI: lamin login \"testuser1@lamin.ai\" --password \"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.login(\"testuser1\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\")"
+                "ln.setup.login(\n",
+                "    \"testuser1\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\"\n",
+                ")  # CLI: lamin login testuser1 --password \"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You don't have to provide your password the second time as it's cached:"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "!lamin login testuser1\n",
-                "```"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.login(\"testuser1\")"
+                "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -221,15 +203,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
             }
         }
     },
```

### Comparing `lndb-0.44.7/docs/guide/02-init-instance.ipynb` & `lndb-0.45a1/docs/guide/02-init-instance.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9826360544217687%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 2: {'attachments': OrderedDict()}, 4: "*

 * *            "{'attachments': OrderedDict()}, 5: {'attachments': OrderedDict()}, 8: {'attachments': "*

 * *            "OrderedDict()}, 10: {'source': {insert: [(5, 'assert ln.setup.settings.storage.id is "*

 * *            "not None\\n')]}}, 11: {'attachments': OrderedDict()}, 12: {'attachments': "*

 * *            "OrderedDict()}, 14: {'attachments': OrderedDict()}, 16: {'attachments': "*

 * *            "OrderedDict()}, 18: {'source': {i […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "# Init an instance"
             ]
@@ -17,14 +18,15 @@
             "source": [
                 "import lamindb as ln\n",
                 "from laminci.db import setup_local_test_postgres\n",
                 "from pathlib import Path"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We already set up a user account for \"testuser1@lamin.ai\" and chose handle `testuser1`."
             ]
         },
         {
@@ -33,37 +35,49 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Local database & storage"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### SQLite"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "!lamin delete mydata"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "ln.setup.init(storage=\"./mydata\")  # CLI: lamin init --storage ./mydata"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This automatically assigns an instance name that equals the name of the storage root along with a few other settings:"
             ]
         },
         {
@@ -86,31 +100,34 @@
             "outputs": [],
             "source": [
                 "assert ln.setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.name == \"mydata\"\n",
                 "assert ln.setup.settings.storage.root.as_posix() == Path(\"mydata\").resolve().as_posix()\n",
                 "assert ln.setup.settings.storage.cache_dir is None\n",
+                "assert ln.setup.settings.storage.id is not None\n",
                 "assert (\n",
                 "    ln.setup.settings.instance.db\n",
                 "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/mydata.lndb\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If you want to register it on the hub at lamin.ai, call:\n",
                 "```\n",
                 "ln.setup.register()\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Postgres"
             ]
         },
         {
@@ -123,14 +140,15 @@
             },
             "outputs": [],
             "source": [
                 "pgurl = setup_local_test_postgres()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "A connection string for postgres looks like this:"
             ]
         },
         {
@@ -139,14 +157,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "pgurl"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let us call init:"
             ]
         },
         {
@@ -169,25 +188,27 @@
             "outputs": [],
             "source": [
                 "assert ln.setup.settings.instance.name == \"pgtest\"\n",
                 "assert ln.setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.dialect == \"postgresql\"\n",
                 "assert ln.setup.settings.instance.db == pgurl\n",
+                "assert ln.setup.settings.storage.id is not None\n",
                 "assert (\n",
                 "    ln.setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"mydatapg\").absolute().as_posix()\n",
                 ")\n",
                 "assert ln.setup.settings.instance.storage.cache_dir is None\n",
                 "\n",
                 "!lamin delete pgtest\n",
                 "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Custom instance name"
             ]
         },
         {
@@ -200,29 +221,30 @@
             },
             "outputs": [],
             "source": [
                 "pgurl = setup_local_test_postgres()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Instead of having the instance name be auto-determined from `storage` or `db`, you can provide a custom name:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(\n",
                 "    storage=\"./mystorage\", name=\"mydata2\", db=pgurl\n",
-                ")  # CLI: lamin init --storage ./mystorage --name \"mydata\" --db {pgurl}"
+                ")  # CLI: lamin init --storage ./mystorage --name \"mydata\" --db ..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -232,46 +254,51 @@
             "outputs": [],
             "source": [
                 "assert ln.setup.settings.instance.name == \"mydata2\"\n",
                 "assert ln.setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.dialect == \"postgresql\"\n",
                 "assert ln.setup.settings.instance.db == pgurl\n",
+                "assert ln.setup.settings.storage.id is not None\n",
                 "assert (\n",
                 "    ln.setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"mystorage\").absolute().as_posix()\n",
                 ")\n",
                 "assert ln.setup.settings.instance.storage.cache_dir is None\n",
                 "\n",
                 "!lamin delete mydata2\n",
                 "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Configure with cloud storage"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### AWS"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You need to have access to AWS S3 via `awscli configure`."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let us look at the special case of an sqlite instance:"
             ]
         },
         {
@@ -326,34 +353,38 @@
                 "assert ln.setup.settings.storage.is_cloud == True\n",
                 "assert str(ln.setup.settings.storage.root) == \"s3://lndb-setup-ci/\"\n",
                 "assert ln.setup.settings.storage.region == \"us-east-1\"\n",
                 "assert (\n",
                 "    str(ln.setup.settings.instance._sqlite_file)\n",
                 "    == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
                 ")\n",
+                "assert ln.setup.settings.storage.id is not None\n",
                 "\n",
                 "# do the same for an S3 bucket in Europe\n",
                 "ln.setup.init(storage=\"s3://lndb-setup-ci-eu-central-1\", name=\"lndb-setup-ci-europe\")\n",
                 "assert ln.setup.settings.storage.region == \"eu-central-1\"\n",
                 "assert ln.setup.settings.instance.name == \"lndb-setup-ci-europe\"\n",
                 "assert (\n",
                 "    str(ln.setup.settings.instance._sqlite_file)\n",
                 "    == \"s3://lndb-setup-ci-eu-central-1/lndb-setup-ci-europe.lndb\"\n",
                 ")\n",
+                "assert ln.setup.settings.storage.id is not None\n",
                 "ln.setup.delete(\"lndb-setup-ci-europe\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### GCP"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You need to authenticate for Google Clod.\n",
                 "\n",
                 "* Either, set the environment variable `export GOOGLE_APPLICATION_CREDENTIALS=<HOME-DIR>/.lndb/<GOOGLE CLOUD PROJECT>.json`.\n",
                 "* Alternatively, if you set up the `gcloud` CLI, log in with `gcloud auth application-default login`.\n"
@@ -390,21 +421,23 @@
                 "# this should move up in this guide\n",
                 "pgurl = setup_local_test_postgres(name=\"pgtest-registered\")\n",
                 "ln.setup.init(storage=\"s3://lndb-setup-ci\", db=pgurl)\n",
                 "ln.setup.register()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Re-initialize an existing instance"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Assume we accidentally `init` an existing instance, it will be loaded:"
             ]
         },
         {
```

### Comparing `lndb-0.44.7/docs/guide/03-load-instance.ipynb` & `lndb-0.45a1/docs/guide/03-load-instance.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893849206349207%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 3: {'attachments': OrderedDict()}, 4: "*

 * *            "{'attachments': OrderedDict()}, 7: {'metadata': {replace: OrderedDict([('tags', "*

 * *            "['hide-cell'])])}}, 9: {'attachments': OrderedDict()}, 13: {'source': ['## Load an "*

 * *            "instance from another owner'], 'attachments': OrderedDict()}, 14: {'attachments': "*

 * *            "OrderedDict()}, 16: {'attachments': OrderedDict()}, 18: {'attachments': "*

 * *            'OrderedDict()}}'}*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "# Load & close an instance"
@@ -31,22 +32,24 @@
                 "import pytest\n",
                 "import lamindb as ln\n",
                 "from lamindb.setup import settings\n",
                 "from lndb.dev._settings_store import instance_settings_file"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "1be836bb",
             "metadata": {},
             "source": [
                 "## Load your own instance by name"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a5c94e19",
             "metadata": {},
             "source": [
                 "If the user is the instance owner, just load the instance by name:"
             ]
         },
@@ -83,15 +86,19 @@
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ac0d2b30",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
                 "# assume we move the storage location\n",
                 "!mv mydata mydata_new_loc\n",
                 "with pytest.raises(\n",
                 "    RuntimeError\n",
                 "):  # triggers because it does not find the SQLite file anymore\n",
@@ -124,14 +131,15 @@
                 "ln.setup.load(\"pgtest-registered\")\n",
                 "assert settings.instance.storage.is_cloud == True\n",
                 "assert settings.instance.name == \"pgtest-registered\"\n",
                 "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "3f47a1d4",
             "metadata": {},
             "source": [
                 "This also works for remote instances:"
             ]
         },
@@ -175,22 +183,24 @@
                 "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
                 "assert (\n",
                 "    settings.instance._sqlite_file.as_posix() == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "914af9a6",
             "metadata": {},
             "source": [
-                "## Load instance from another owner"
+                "## Load an instance from another owner"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "65ab467e",
             "metadata": {},
             "source": [
                 "If you have the permission, you can load an instance from another owner. "
             ]
         },
@@ -201,14 +211,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.load(\"testuser1/mydata\")  # lamin load \"testuser1/mydata\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "0986a5f3",
             "metadata": {},
             "source": [
                 "Load an instance from wrong owner."
             ]
         },
@@ -219,14 +230,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert ln.setup.load(\"testuser2/mydata\") == \"instance-not-reachable\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "e3701120",
             "metadata": {},
             "source": [
                 "## Close an instance"
             ]
         },
```

### Comparing `lndb-0.44.7/docs/guide/04-set-storage.ipynb` & `lndb-0.45a1/docs/guide/04-set-storage.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9526545698924731%*

 * *Differences: {"'cells'": "{0: {'source': ['# Get info, set storage & delete an instance'], 'attachments': "*

 * *            "OrderedDict()}, 1: {'source': ['import lamindb as ln']}, 2: {'id': 'fe33eb9b', "*

 * *            "'source': ['## Get info'], 'attachments': OrderedDict()}, 3: {'id': '00a97004', "*

 * *            '\'metadata\': {replace: OrderedDict()}, \'source\': [\'ln.setup.load("mydata")\']}, '*

 * *            "4: {'id': 'd6f127d1', 'source': ['ln.setup.info()  # CLI: lamin info']}, 5: {'id': "*

 * *            "'a7cf42fb', 'sourc […]*

```diff
@@ -1,154 +1,193 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Set storage"
+                "# Get info, set storage & delete an instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb as ln\n",
-                "from pathlib import Path\n",
-                "import laminci"
+                "import lamindb as ln"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "fe33eb9b",
+            "metadata": {},
+            "source": [
+                "## Get info"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "00a97004",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.load(\"mydata\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d6f127d1",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.info()  # CLI: lamin info"
+            ]
+        },
+        {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a7cf42fb",
             "metadata": {},
             "source": [
-                "## Set storage for PostgreSQL instance"
+                "## Set storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8fd59ad3-04b9-42fb-83cc-ab7beedbec72",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
+                "import laminci\n",
+                "\n",
                 "pgurl = laminci.db.setup_local_test_postgres()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d6b0bd5e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(storage=\"./storage_1\", db=pgurl)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "ceb57cc9",
+            "id": "e6638f44",
             "metadata": {},
             "source": [
-                "Running \n",
-                "```\n",
-                "!lamin set --storage ./storage_2\n",
-                "```\n",
-                "on the command line runs the following Python function:"
+                "Local storage:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "49b9ef11",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.set.storage(\"./storage_2\")"
+                "ln.setup.set.storage(\"./storage_2\")  # CLI: lamin set --storage ./storage_2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8e481aa0",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-cell"
+                ]
             },
             "outputs": [],
             "source": [
+                "from pathlib import Path\n",
+                "\n",
                 "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "25a13298",
+            "id": "de1c12b8",
             "metadata": {},
             "source": [
-                "Running \n",
-                "```\n",
-                "lamin set --storage s3://lndb-setup-ci\n",
-                "```\n",
-                "\n",
-                "on the command line runs the following:"
+                "Cloud storage:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8436575d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.set.storage(\"s3://lndb-setup-ci\")"
+                "ln.setup.set.storage(\"s3://lndb-setup-ci\")  # lamin set --storage s3://lndb-setup-ci"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "859a972e",
+            "metadata": {},
+            "source": [
+                "See an overview:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d2934990",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "146192a7",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln.setup.settings.storage.is_cloud\n",
-                "assert ln.setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\""
+                "ln.select(ln.Storage).df()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7bd9997b",
-            "metadata": {},
+            "id": "d2934990",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
+                "assert ln.setup.settings.storage.is_cloud\n",
+                "assert ln.setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
                 "# root.fs contains the underlying fsspec filesystem\n",
                 "assert (\n",
                 "    ln.setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "ae953b6a",
             "metadata": {},
             "source": [
-                "It is possible to set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
+                "You can set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f9294082",
             "metadata": {},
@@ -156,143 +195,158 @@
             "source": [
                 "ln.setup.set.storage(\"s3://lndb-setup-ci\", cache_regions=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5f320819",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "assert not ln.setup.settings.storage.root.fs.cache_regions"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "529e68e5-9b10-4fdb-9d4c-ac8206bbbb68",
-            "metadata": {},
-            "source": [
-                "### Set storage not by owner"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "d6915638-db49-4d3d-bd91-819bb4719ef7",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
+                "# test cache_regions\n",
+                "assert not ln.setup.settings.storage.root.fs.cache_regions\n",
+                "# test setting storage not by owner\n",
                 "ln.setup.login(\n",
                 "    \"testuser2@lamin.ai\", password=\"goeoNJKE61ygbz1vhaCVynGERaRrlviPBVQsjkhz\"\n",
-                ")"
+                ")\n",
+                "ln.setup.set.storage(\"./storage_3\")\n",
+                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\"\n",
+                "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "2ed8716f-852f-4ce9-8eef-5b824d6e92b3",
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "3fb6a223",
             "metadata": {
                 "tags": []
             },
-            "outputs": [],
             "source": [
-                "ln.setup.set.storage(\"./storage_3\")"
+                "### Currently not possible: setting storage for SQLite instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cad87623",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "49309f3a-199f-40bc-b318-a396ebcaafec",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\""
+                "ln.setup.login(\"testuser1\")\n",
+                "ln.setup.load(\"mydata\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "6ccb6573",
+            "metadata": {},
+            "source": [
+                "If you try to set the storage for an sqlite instance, an error message is returned:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "78a819fa-48d6-4c6f-95d4-7dc7e94283bb",
+            "id": "e4f2545f",
             "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
+                "tags": []
             },
             "outputs": [],
             "source": [
-                "!docker stop pgtest && docker rm pgtest"
+                "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "3fb6a223",
-            "metadata": {
-                "tags": []
-            },
+            "id": "675739c6",
+            "metadata": {},
             "source": [
-                "## Set storage for SQLite instance"
+                "## Delete an instance"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "6ccb6573",
+            "id": "cceb345b",
             "metadata": {},
             "source": [
-                "If the user tries to set the storage for an sqlite instance, an error message is raised:"
+                "### With local default storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "49309f3a-199f-40bc-b318-a396ebcaafec",
+            "id": "562024da",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.login(\"testuser1\")"
+                "ln.setup.init(storage=\"mydata-delete\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f988a386",
+            "id": "e7d4860a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.load(\"mydata\")"
+                "ln.setup.delete(\"mydata-delete\")  # CLI: lamin delete mydata"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e4f2545f",
+            "id": "5d558511",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-cell"
+                ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\""
+                "from lndb.dev._settings_store import instance_settings_file\n",
+                "\n",
+                "settings_file = instance_settings_file(\"mydata-delete\", \"testuser1\")\n",
+                "assert settings_file.exists() == False"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "83d675b0",
+            "metadata": {},
+            "source": [
+                "### With remote default storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4fa82d8b",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "dccb27bf",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.init(storage=\"s3://lndb-setup-delete-ci\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "fde88024",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.set_storage(\"mydata_storage_2\")"
+                "ln.setup.delete(\"lndb-setup-delete-ci\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lndb-0.44.7/docs/guide/05-schema-modules.ipynb` & `lndb-0.45a1/docs/guide/05-schema-modules.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9438657407407407%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 2: {'source': ['## Core schema module'], "*

 * *            "'attachments': OrderedDict()}, 3: {'source': ['The core schema module is part of any "*

 * *            "LaminDB instance and tracks data lineage.'], 'attachments': OrderedDict()}, 4: "*

 * *            "{'metadata': {replace: OrderedDict([('tags', ['hide-cell'])])}, 'source': "*

 * *            '[\'ln.setup.load("mydata")\']}, 5: {\'source\': [\'You can find the code here: '*

 * *            "https://github.com/laminlabs/l […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Configure schema modules"
             ]
         },
         {
@@ -13,170 +14,145 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lamindb as ln"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## The core schema module"
+                "## Core schema module"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The core schema module is part of LaminDB instance and tracks data lineage."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.init(storage=\"mydata\")"
+                "The core schema module is part of any LaminDB instance and tracks data lineage."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ln.setup.schema.draw()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Mount schema modules bionty and wetlab"
+                "ln.setup.load(\"mydata\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "```\n",
-                "!lamin init --storage mydata2 --schema bionty,lamin1\n",
-                "```"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\")"
+                "You can find the code here: https://github.com/laminlabs/lnschema-core"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.schema.draw()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In the case of Bionty, ontology versions are automatically tracked:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from lndb.dev._setup_knowledge import load_bionty_versions"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "load_bionty_versions(ln.setup.settings.instance, display=True)"
+                "## Schema modules `bionty` & `lamin1`"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Clean up"
+                "The `bionty` schema module maps fundamental biological entities: https://github.com/laminlabs/lnschema-bionty\n",
+                "\n",
+                "The `lamin1` module is an example for a configurable in-house schema that tracks lab operations: https://github.com/laminlabs/lnschema-lamin1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.delete(\"mydata2\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Postgres"
+                "ln.setup.init(\n",
+                "    storage=\"mydata2\", schema=\"bionty,lamin1\"\n",
+                ")  # CLI: lamin init --storage mydata2 --schema bionty,lamin1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from laminci.db import setup_local_test_postgres"
+                "ln.setup.schema.draw()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "pgurl = setup_local_test_postgres()"
+                "For `bionty`, supporting public ontology versions are automatically tracked:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\", db=pgurl)"
+                "from lndb.dev._setup_knowledge import load_bionty_versions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!docker stop pgtest && docker rm pgtest"
+                "load_bionty_versions(ln.setup.settings.instance, display=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
+                "# clean up\n",
+                "ln.setup.delete(\"mydata2\")\n",
+                "# test with postgres\n",
+                "from laminci.db import setup_local_test_postgres\n",
+                "\n",
+                "pgurl = setup_local_test_postgres()\n",
+                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\", db=pgurl)\n",
+                "!docker stop pgtest && docker rm pgtest\n",
                 "ln.setup.delete(\"pgtest\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
```

### Comparing `lndb-0.44.7/docs/guide/migrate.md` & `lndb-0.45a1/docs/guide/migrate.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 Currently only recommended on the enterprise plan. [Reach out](https://lamin.ai/contact) if you are interested!
 
 `lamin`'s migrations are a convenient wrapper around [alembic](https://alembic.sqlalchemy.org/en/latest/). All scripts generated by `lamin` are fully compatible with `alembic`. The main value added by `lamin` is a CI-tested process for a migration.
 ```
 
 This page documents how to create a tested migration using the CI-guided workflow for postgres-based instances.
 
+Ensure that you have installed the schema module in editable mode for example through
+
+```bash
+pip install -e .
+```
+
+Further, ensure that you have loaded a Lamin instance.
+
 1. Create a new branch (e.g. `migr`) in your repository: Update an ORM, e.g., by renaming a column.
 
    :::{dropdown} Example: Rename a column.
    Let's try to rename the `version` column to `v` in the `Transform` ORM of `lnschema_core`.
 
    In the `lnschema_core/_core.py` `Transform` ORM, modify line:
```

### Comparing `lndb-0.44.7/lndb/__init__.py` & `lndb-0.45a1/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.44.7"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.45a1"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.44.7/lndb/__main__.py` & `lndb-0.45a1/lndb/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 
 from lamin_logger import logger
 
 from . import _init_instance, _setup_user, delete, info, register, set
 from ._close import close as close_instance
 from ._init_instance import description as instance
+from ._notebook import track
 from .dev._settings_user import user_description as user
 
 signup_help = "First time sign up."
 login_help = "Log in an already-signed-up user."
 init_help = "Init & config instance with db & storage."
 load_help = "Load instance by name."
 set_storage_help = "Set storage used by an instance."
@@ -18,15 +19,15 @@
 info_help = "Show current instance information."
 close_help = "Close instance."
 migr_help = "Manage migrations."
 delete_help = "Delete an instance."
 register_help = (
     "Register instance on hub (local instances are not automatically registered)."
 )
-
+track_help = "Track a notebook (init metadata)."
 
 description_cli = "Configure LaminDB and perform simple actions."
 parser = argparse.ArgumentParser(
     description=description_cli, formatter_class=argparse.RawTextHelpFormatter
 )
 subparsers = parser.add_subparsers(dest="command")
 
@@ -70,27 +71,35 @@
 
 # show instance info
 info_parser = subparsers.add_parser("info", help=info_help)
 
 # set storage
 set_storage_parser = subparsers.add_parser("set", help=set_storage_help)
 aa = set_storage_parser.add_argument
-aa("--storage", type=str, metavar="s", help=instance.storage_root)
+aa("--storage", type=str, metavar="f", help=instance.storage_root)
 
 # close instance
 subparsers.add_parser("close", help=close_help)
 
 # register instance
 subparsers.add_parser("register", help=register_help)
 
 # migrate
 migr = subparsers.add_parser("migrate", help=migr_help)
 aa = migr.add_argument
 aa("action", choices=["generate"], help="Generate migration.")
 
+# track anotebook (init nbproject metadata)
+track_parser = subparsers.add_parser("track", help=track_help)
+aa = track_parser.add_argument
+filepath_help = "A path to the notebook to track."
+aa("filepath", type=str, metavar="filepath", help=filepath_help)
+pypackage_help = "One or more (delimited by ',') python packages to track."
+aa("--pypackage", type=str, metavar="pypackage", default=None, help=pypackage_help)
+
 # parse args
 args = parser.parse_args()
 
 
 def process_result(result):
     if result in ["migrate-unnecessary", "migrate-success", "migrate-skipped", None]:
         return None  # is interpreted as success (exit code 0) by shell
@@ -135,10 +144,12 @@
     elif args.command == "set":
         return set.storage(args.storage)
     elif args.command == "migrate":
         from . import migrate
 
         if args.action == "generate":
             return migrate.generate()
+    elif args.command == "track":
+        track(args.filepath, args.pypackage)
     else:
         logger.error("Invalid command. Try `lamin -h`.")
         return 1
```

### Comparing `lndb-0.44.7/lndb/_check_instance_setup.py` & `lndb-0.45a1/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_close.py` & `lndb-0.45a1/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_delete.py` & `lndb-0.45a1/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_init_instance.py` & `lndb-0.45a1/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_load_instance.py` & `lndb-0.45a1/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_migrate/alembic.ini` & `lndb-0.45a1/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_migrate/core.py` & `lndb-0.45a1/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_migrate/deploy.py` & `lndb-0.45a1/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_migrate/env.py` & `lndb-0.45a1/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_migrate/utils.py` & `lndb-0.45a1/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_register_instance.py` & `lndb-0.45a1/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_schema.py` & `lndb-0.45a1/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_set.py` & `lndb-0.45a1/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_settings.py` & `lndb-0.45a1/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/_setup_user.py` & `lndb-0.45a1/lndb/_setup_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def signup(email: str) -> Union[str, None]:
     """Sign up user."""
     response = sign_up_hub(email)
     if response == "handle-exists":  # handle already exists
         logger.error("The handle already exists. Please choose a different one.")
         return "handle-exists"
     if response == "user-exists":  # user already exists
-        logger.error("User already exists! Please login instead: `lndb login`.")
+        logger.error("User already exists! Please login instead: `lamin login`.")
         return "user-exists"
     user_settings = load_or_create_user_settings()
     user_settings.email = email
     save_user_settings(user_settings)
     user_settings.password = response
     save_user_settings(user_settings)
     return None  # user needs to confirm email now
@@ -68,19 +68,19 @@
 
     user_settings = load_or_create_user_settings()
 
     if password:
         user_settings.password = password
 
     if user_settings.email is None:
-        raise RuntimeError("No stored user email, please call: lndb login {user}")
+        raise RuntimeError("No stored user email, please call: lamin login {user}")
 
     if user_settings.password is None:
         raise RuntimeError(
-            "No stored user password, please call: lndb login <your-email>"
+            "No stored user password, please call: lamin login <your-email>"
             " --password <your-password>"
         )
 
     response = sign_in_hub(
         user_settings.email, user_settings.password, user_settings.handle
     )
     if response == "could-not-login":
```

### Comparing `lndb-0.44.7/lndb/dev/__init__.py` & `lndb-0.45a1/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_clone.py` & `lndb-0.45a1/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_db.py` & `lndb-0.45a1/lndb/dev/_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # We see a lot of import statements for lnschema_core below
 # This is currently needed as we can only import the schema module
 # once isettings have been adjusted
 from typing import Any, List
 
+import sqlalchemy as sa
 import sqlmodel as sqm
 from lamin_logger import logger
-from sqlalchemy.exc import ProgrammingError
 
 from .._settings import settings
 from ._storage import StorageSettings
 
 
 class upsert:
     @classmethod
     def user(cls, email: str, user_id: str, handle: str, name: str = None):
-        import lnschema_core as schema_core
-
-        with sqm.Session(settings.instance.engine) as session:
-            user_table = (
-                schema_core.User if hasattr(schema_core, "User") else schema_core.user
-            )  # noqa
-            try:
-                user = session.get(user_table, user_id)
-            except ProgrammingError as e:
-                logger.error(
-                    "Cannot find user table.\nLikely, you try to run SQLite and"
-                    " Postgres from the same process.\n\n->Abort and restart with only"
-                    " one SQL dialect in one process.\n\n"
+        try:
+            with settings.instance.engine.connect() as conn:
+                table = (
+                    "core.user"
+                    if settings.instance.dialect == "postgresql"
+                    else '"core.user"'
                 )
-                raise e
+                user = conn.execute(
+                    sa.text(f"select * from {table} where id = '{user_id}'")
+                ).first()
+        except Exception:
+            with settings.instance.engine.connect() as conn:
+                user = conn.execute(
+                    sa.text(f"select * from lnschema_core_user where id = '{user_id}'")
+                ).first()
         if user is None:
             user_id = insert.user(email, user_id, handle, name)  # type: ignore
             # do not update sqlite on the cloud as this happens within
             # insert.user
         else:
             # update the user record
             update_email = email != user.email
@@ -64,25 +64,35 @@
 class insert_if_not_exists:
     """Insert data if it does not yet exist.
 
     A wrapper around the `insert` class below.
     """
 
     @classmethod
-    def storage(cls, storage_settings: StorageSettings):
-        from lnschema_core import Storage as StorageORM
-
+    def storage(cls, storage_settings: StorageSettings) -> None:
         root_str = storage_settings.root_as_str
-        with sqm.Session(settings.instance.engine) as session:
-            storage = session.exec(
-                sqm.select(StorageORM).where(StorageORM.root == root_str)
-            ).first()
+        try:
+            with settings.instance.engine.connect() as conn:
+                table = (
+                    "core.storage"
+                    if settings.instance.dialect == "postgresql"
+                    else '"core.storage"'
+                )
+                storage = conn.execute(
+                    sa.text(f"select * from {table} where root = '{root_str}'")
+                ).first()
+        except Exception:
+            with settings.instance.engine.connect() as conn:
+                storage = conn.execute(
+                    sa.text(
+                        f"select * from lnschema_core_storage where root = '{root_str}'"
+                    )
+                ).first()
         if storage is None:
             storage = insert.storage(root_str, storage_settings.region)
-        return storage
 
 
 class insert:
     """Insert data."""
 
     # this here actually first checks for existence
     @classmethod
@@ -127,48 +137,64 @@
 
     @classmethod
     def user(cls, email, user_id, handle, name):
         """User."""
         import lnschema_core as schema_core
 
         with sqm.Session(settings.instance.engine) as session:
-            user_table = (
-                schema_core.User if hasattr(schema_core, "User") else schema_core.user
-            )  # noqa
+            user_table = schema_core.User
             user = user_table(id=user_id, email=email, handle=handle, name=name)
             session.add(user)
             session.commit()
             session.refresh(user)
 
         settings.instance._update_cloud_sqlite_file()
 
         return user.id
 
     @classmethod
-    def storage(cls, root, region):
+    def storage(cls, root, region) -> None:
         """Storage."""
-        import lnschema_core as schema_core
+        from lnschema_core.dev.id import storage as storage_id
 
-        with sqm.Session(settings.instance.engine) as session:
-            storage_table = (
-                schema_core.Storage
-                if hasattr(schema_core, "Storage")
-                else schema_core.storage
-            )  # noqa
-            storage = storage_table(
-                root=root, region=region, type=settings.instance.storage.type
-            )
-            session.add(storage)
-            session.commit()
-            session.refresh(storage)
+        id = storage_id()
 
+        try:
+            with settings.instance.engine.begin() as conn:
+                table = (
+                    "core.storage"
+                    if settings.instance.dialect == "postgresql"
+                    else '"core.storage"'
+                )
+                conn.execute(
+                    sa.text(
+                        f"insert into {table} (id, root, region, type) values"
+                        " (:id, :root, :region, :type)"
+                    ).bindparams(
+                        id=id,
+                        root=root,
+                        region=region,
+                        type=settings.instance.storage.type,
+                    )
+                )
+        except Exception:
+            with settings.instance.engine.begin() as conn:
+                conn.execute(
+                    sa.text(
+                        "insert into lnschema_core_storage (id, root, region, type)"
+                        " values (:id, :root, :region, :type)"
+                    ).bindparams(
+                        id=id,
+                        root=root,
+                        region=region,
+                        type=settings.instance.storage.type,
+                    )
+                )
         settings.instance._update_cloud_sqlite_file()
 
-        return storage
-
     @classmethod
     def bionty_versions(cls, records: List[sqm.SQLModel]):
         """Bionty versions."""
         from lnschema_bionty import dev
 
         with sqm.Session(settings.instance.engine) as session:
             for record in records:
```

### Comparing `lndb-0.44.7/lndb/dev/_deprecated.py` & `lndb-0.45a1/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_exclusion.py` & `lndb-0.45a1/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_settings_instance.py` & `lndb-0.45a1/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_settings_load.py` & `lndb-0.45a1/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_settings_save.py` & `lndb-0.45a1/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_settings_store.py` & `lndb-0.45a1/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_settings_user.py` & `lndb-0.45a1/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_setup_knowledge.py` & `lndb-0.45a1/lndb/dev/_setup_knowledge.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,20 @@
     if "bionty" in isettings.schema:
         import bionty as bt
         from bionty.dev._io import write_yaml
         from lnschema_bionty import dev
 
         basedir = Path(bt.__file__).parent / "versions"
 
+        # these two lines help over the incomplete migration
+        # of the core schema module v0.34.0 and related in lnschema_bionty
+        # v0.18.0
+        dev.BiontyVersions.__table__.schema = None
+        dev.CurrentBiontyVersions.__table__.schema = None
+
         stmt = sqm.select(dev.BiontyVersions).join(dev.CurrentBiontyVersions)
         with isettings.session() as ss:
             results = ss.exec(stmt).all()
         # avoid breaking change
         # if no versions were written in the db, write versions from bionty
         if len(results) == 0:
             write_bionty_versions(isettings)
```

### Comparing `lndb-0.44.7/lndb/dev/_setup_schema.py` & `lndb-0.45a1/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/_storage.py` & `lndb-0.45a1/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/dev/upath.py` & `lndb-0.45a1/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/test/_migrations_e2e.py` & `lndb-0.45a1/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/lndb/test/_migrations_unit.py` & `lndb-0.45a1/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/noxfile.py` & `lndb-0.45a1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/pyproject.toml` & `lndb-0.45a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "appdirs",
     "python-dotenv",
     "erdiagram",
     "alembic",
     "natsort",
     "pandas",
     "python-dateutil",
+    "universal_pathlib"
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lndb"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `lndb-0.44.7/tests/test_bionty.py` & `lndb-0.45a1/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/tests/test_init_instance.py` & `lndb-0.45a1/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.7/PKG-INFO` & `lndb-0.45a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.44.7
+Version: 0.45a1
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.4
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
@@ -15,14 +15,15 @@
 Requires-Dist: appdirs
 Requires-Dist: python-dotenv
 Requires-Dist: erdiagram
 Requires-Dist: alembic
 Requires-Dist: natsort
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
+Requires-Dist: universal_pathlib
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: lamindb[bionty,lamin1]>=0.39rc1 ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
```


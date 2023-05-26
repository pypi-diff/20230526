# Comparing `tmp/lndb-0.45a1.tar.gz` & `tmp/lndb-0.45a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.45a1.tar", last modified: Thu May 25 22:03:25 2023, max compression
+gzip compressed data, was "lndb-0.45a2.tar", last modified: Fri May 26 09:56:30 2023, max compression
```

## Comparing `lndb-0.45a1.tar` & `lndb-0.45a2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     3832 2023-05-24 18:13:34.371502 lndb-0.45a1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-24 18:13:34.371611 lndb-0.45a1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-24 18:13:34.371684 lndb-0.45a1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-24 18:13:34.371770 lndb-0.45a1/.gitignore
--rw-r--r--   0        0        0     1777 2023-05-24 18:13:34.371851 lndb-0.45a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-24 18:13:34.371968 lndb-0.45a1/LICENSE
--rw-r--r--   0        0        0      173 2023-05-24 18:13:34.372033 lndb-0.45a1/README.md
--rw-r--r--   0        0        0       52 2023-05-24 18:13:34.372124 lndb-0.45a1/docs/api.md
--rw-r--r--   0        0        0    48915 2023-05-25 22:02:57.989850 lndb-0.45a1/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-05-24 18:13:34.372476 lndb-0.45a1/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-05-24 18:13:34.372565 lndb-0.45a1/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-05-24 18:13:34.372660 lndb-0.45a1/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-05-24 18:13:34.372727 lndb-0.45a1/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-05-24 18:13:34.372809 lndb-0.45a1/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-05-24 18:13:34.372876 lndb-0.45a1/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2589 2023-05-25 22:02:47.332671 lndb-0.45a1/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-05-24 18:13:34.373075 lndb-0.45a1/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5025 2023-05-25 13:55:42.990512 lndb-0.45a1/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11082 2023-05-25 13:55:42.990674 lndb-0.45a1/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     6639 2023-05-25 13:55:42.990928 lndb-0.45a1/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     7616 2023-05-25 13:56:23.677378 lndb-0.45a1/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-05-25 15:46:50.017574 lndb-0.45a1/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-05-25 13:55:42.991225 lndb-0.45a1/docs/guide/index.md
--rw-r--r--   0        0        0     3331 2023-05-24 18:13:34.373961 lndb-0.45a1/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-05-24 18:13:34.374075 lndb-0.45a1/docs/index.md
--rw-r--r--   0        0        0      118 2023-05-24 18:13:34.374173 lndb-0.45a1/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-05-25 22:02:36.128361 lndb-0.45a1/lndb/__init__.py
--rw-r--r--   0        0        0     5268 2023-05-24 18:13:34.374405 lndb-0.45a1/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-05-24 18:13:34.374517 lndb-0.45a1/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-24 18:13:34.374613 lndb-0.45a1/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-05-24 18:13:34.374688 lndb-0.45a1/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-05-24 18:13:34.374754 lndb-0.45a1/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-05-24 18:13:34.374825 lndb-0.45a1/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-05-24 18:13:34.374892 lndb-0.45a1/lndb/_info.py
--rw-r--r--   0        0        0     6035 2023-05-25 12:49:05.083933 lndb-0.45a1/lndb/_init_instance.py
--rw-r--r--   0        0        0     6729 2023-05-24 18:13:34.375083 lndb-0.45a1/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-05-24 18:13:34.375181 lndb-0.45a1/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-05-24 18:13:34.375248 lndb-0.45a1/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-05-24 18:13:34.375322 lndb-0.45a1/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-05-24 18:13:34.375413 lndb-0.45a1/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-05-24 18:13:34.375498 lndb-0.45a1/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-05-24 18:13:34.375575 lndb-0.45a1/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-05-24 18:13:34.375787 lndb-0.45a1/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      790 2023-05-24 18:13:34.375906 lndb-0.45a1/lndb/_notebook.py
--rw-r--r--   0        0        0      803 2023-05-24 18:13:34.375990 lndb-0.45a1/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-05-24 18:13:34.376692 lndb-0.45a1/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-05-24 18:13:34.377124 lndb-0.45a1/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-05-24 18:13:34.377222 lndb-0.45a1/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-05-24 18:13:34.377292 lndb-0.45a1/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-05-24 18:13:34.377359 lndb-0.45a1/lndb/_settings_store.py
--rw-r--r--   0        0        0     3905 2023-05-24 18:13:34.377464 lndb-0.45a1/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-05-24 18:13:34.377571 lndb-0.45a1/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-05-24 18:13:34.377656 lndb-0.45a1/lndb/dev/_clone.py
--rw-r--r--   0        0        0     7299 2023-05-25 21:32:27.594442 lndb-0.45a1/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-05-24 18:13:34.397245 lndb-0.45a1/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-05-24 18:13:34.397345 lndb-0.45a1/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-05-24 18:13:34.397862 lndb-0.45a1/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-05-24 18:13:34.397995 lndb-0.45a1/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-05-24 18:13:34.398092 lndb-0.45a1/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-05-24 18:13:34.398168 lndb-0.45a1/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-05-24 18:13:34.398249 lndb-0.45a1/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-05-24 18:13:34.398328 lndb-0.45a1/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2710 2023-05-25 21:55:19.754812 lndb-0.45a1/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-05-24 18:13:34.398512 lndb-0.45a1/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-05-24 18:13:34.398603 lndb-0.45a1/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-05-24 18:13:34.398679 lndb-0.45a1/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-05-24 18:13:34.398758 lndb-0.45a1/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-05-24 18:13:34.398886 lndb-0.45a1/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-05-24 18:13:34.398951 lndb-0.45a1/lndb/test/_env.py
--rw-r--r--   0        0        0     3911 2023-05-24 18:13:34.399040 lndb-0.45a1/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-05-24 18:13:34.399143 lndb-0.45a1/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-05-24 18:13:34.399213 lndb-0.45a1/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-05-24 18:13:34.399292 lndb-0.45a1/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-05-24 18:13:34.399371 lndb-0.45a1/noxfile.py
--rw-r--r--   0        0        0     1420 2023-05-24 18:13:34.399454 lndb-0.45a1/pyproject.toml
--rw-r--r--   0        0        0      513 2023-05-24 18:13:34.399557 lndb-0.45a1/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-05-24 18:13:34.399639 lndb-0.45a1/tests/test_init_instance.py
--rw-r--r--   0        0        0      379 2023-05-24 18:13:34.399723 lndb-0.45a1/tests/test_notebooks.py
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 lndb-0.45a1/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-05-24 18:13:34.371502 lndb-0.45a2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-24 18:13:34.371611 lndb-0.45a2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-24 18:13:34.371684 lndb-0.45a2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-24 18:13:34.371770 lndb-0.45a2/.gitignore
+-rw-r--r--   0        0        0     1777 2023-05-24 18:13:34.371851 lndb-0.45a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-24 18:13:34.371968 lndb-0.45a2/LICENSE
+-rw-r--r--   0        0        0      173 2023-05-24 18:13:34.372033 lndb-0.45a2/README.md
+-rw-r--r--   0        0        0       52 2023-05-24 18:13:34.372124 lndb-0.45a2/docs/api.md
+-rw-r--r--   0        0        0    49086 2023-05-26 09:55:24.478970 lndb-0.45a2/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-05-24 18:13:34.372476 lndb-0.45a2/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-05-24 18:13:34.372565 lndb-0.45a2/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-05-24 18:13:34.372660 lndb-0.45a2/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-05-24 18:13:34.372727 lndb-0.45a2/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-05-24 18:13:34.372809 lndb-0.45a2/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-05-24 18:13:34.372876 lndb-0.45a2/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2589 2023-05-25 22:02:47.332671 lndb-0.45a2/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-05-24 18:13:34.373075 lndb-0.45a2/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5025 2023-05-25 13:55:42.990512 lndb-0.45a2/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11082 2023-05-26 09:53:42.760584 lndb-0.45a2/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     6639 2023-05-25 13:55:42.990928 lndb-0.45a2/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     7616 2023-05-25 13:56:23.677378 lndb-0.45a2/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-05-25 15:46:50.017574 lndb-0.45a2/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-05-25 13:55:42.991225 lndb-0.45a2/docs/guide/index.md
+-rw-r--r--   0        0        0     3331 2023-05-24 18:13:34.373961 lndb-0.45a2/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-05-24 18:13:34.374075 lndb-0.45a2/docs/index.md
+-rw-r--r--   0        0        0      118 2023-05-24 18:13:34.374173 lndb-0.45a2/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-05-26 09:54:53.204802 lndb-0.45a2/lndb/__init__.py
+-rw-r--r--   0        0        0     5268 2023-05-24 18:13:34.374405 lndb-0.45a2/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-05-24 18:13:34.374517 lndb-0.45a2/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-24 18:13:34.374613 lndb-0.45a2/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-05-26 09:08:58.517667 lndb-0.45a2/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-05-24 18:13:34.374754 lndb-0.45a2/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-05-24 18:13:34.374825 lndb-0.45a2/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-05-24 18:13:34.374892 lndb-0.45a2/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-05-25 12:49:05.083933 lndb-0.45a2/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6729 2023-05-24 18:13:34.375083 lndb-0.45a2/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-05-24 18:13:34.375181 lndb-0.45a2/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-24 18:13:34.375248 lndb-0.45a2/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-05-24 18:13:34.375322 lndb-0.45a2/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7555 2023-05-26 09:53:47.457599 lndb-0.45a2/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-05-24 18:13:34.375498 lndb-0.45a2/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-05-24 18:13:34.375575 lndb-0.45a2/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-05-24 18:13:34.375787 lndb-0.45a2/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      790 2023-05-24 18:13:34.375906 lndb-0.45a2/lndb/_notebook.py
+-rw-r--r--   0        0        0      803 2023-05-24 18:13:34.375990 lndb-0.45a2/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-05-24 18:13:34.376692 lndb-0.45a2/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-05-24 18:13:34.377124 lndb-0.45a2/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-05-24 18:13:34.377222 lndb-0.45a2/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-05-24 18:13:34.377292 lndb-0.45a2/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-05-24 18:13:34.377359 lndb-0.45a2/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3905 2023-05-24 18:13:34.377464 lndb-0.45a2/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-05-24 18:13:34.377571 lndb-0.45a2/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-05-24 18:13:34.377656 lndb-0.45a2/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     7299 2023-05-26 07:50:36.465517 lndb-0.45a2/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-05-24 18:13:34.397245 lndb-0.45a2/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-05-24 18:13:34.397345 lndb-0.45a2/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-05-24 18:13:34.397862 lndb-0.45a2/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-05-24 18:13:34.397995 lndb-0.45a2/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-05-24 18:13:34.398092 lndb-0.45a2/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-05-24 18:13:34.398168 lndb-0.45a2/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-05-24 18:13:34.398249 lndb-0.45a2/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-05-24 18:13:34.398328 lndb-0.45a2/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2710 2023-05-25 21:55:19.754812 lndb-0.45a2/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     4466 2023-05-26 09:53:47.457948 lndb-0.45a2/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-05-24 18:13:34.398603 lndb-0.45a2/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-05-24 18:13:34.398679 lndb-0.45a2/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-05-24 18:13:34.398758 lndb-0.45a2/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-05-24 18:13:34.398886 lndb-0.45a2/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-24 18:13:34.398951 lndb-0.45a2/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-05-24 18:13:34.399040 lndb-0.45a2/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-05-24 18:13:34.399143 lndb-0.45a2/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-05-24 18:13:34.399213 lndb-0.45a2/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-05-24 18:13:34.399292 lndb-0.45a2/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-05-24 18:13:34.399371 lndb-0.45a2/noxfile.py
+-rw-r--r--   0        0        0     1419 2023-05-26 09:53:47.458248 lndb-0.45a2/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-05-24 18:13:34.399557 lndb-0.45a2/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-05-24 18:13:34.399639 lndb-0.45a2/tests/test_init_instance.py
+-rw-r--r--   0        0        0      379 2023-05-24 18:13:34.399723 lndb-0.45a2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 lndb-0.45a2/PKG-INFO
```

### Comparing `lndb-0.45a1/.github/workflows/build.yml` & `lndb-0.45a2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/.github/workflows/latest-changes.yml` & `lndb-0.45a2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/.gitignore` & `lndb-0.45a2/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/.pre-commit-config.yaml` & `lndb-0.45a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/LICENSE` & `lndb-0.45a2/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/changelog.md` & `lndb-0.45a2/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🔥 Remove schema modules logic from `setup_schema` | [381](https://github.com/laminlabs/lndb/pull/381) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.45a2
 🏗️ Remove SQL-level schema modules | [380](https://github.com/laminlabs/lndb/pull/380) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.45a1
 ✨ Add track command to CLI | [378](https://github.com/laminlabs/lndb/pull/378) | [Koncopd](https://github.com/Koncopd) | 2023-05-23 |
 📝 Improve migration docs | [379](https://github.com/laminlabs/lndb/pull/379) | [Zethson](https://github.com/Zethson) | 2023-05-22 |
 🔊 Use lamin_logger in test_notebooks.py | [376](https://github.com/laminlabs/lndb/pull/376) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 Add universal_pathlib to dependencies | [375](https://github.com/laminlabs/lndb/pull/375) | [Zethson](https://github.com/Zethson) | 2023-05-02 |
 ⬆️ Upgrade lnhub-rest to 0.9.4 | [373](https://github.com/laminlabs/lndb/pull/373) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.44.7
 🚑 Fix load | [372](https://github.com/laminlabs/lndb/pull/372) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-27 | 0.44.6
```

### Comparing `lndb-0.45a1/docs/faq/check-synchronization.ipynb` & `lndb-0.45a2/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/faq/clone.ipynb` & `lndb-0.45a2/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.45a2/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/faq/manage-migrations.ipynb` & `lndb-0.45a2/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/faq/switch-environment.ipynb` & `lndb-0.45a2/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.45a2/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/faq/test-migrations-unit.ipynb` & `lndb-0.45a2/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/guide/01-setup-user.ipynb` & `lndb-0.45a2/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/guide/02-init-instance.ipynb` & `lndb-0.45a2/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/guide/03-load-instance.ipynb` & `lndb-0.45a2/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/guide/04-set-storage.ipynb` & `lndb-0.45a2/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/guide/05-schema-modules.ipynb` & `lndb-0.45a2/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/docs/guide/migrate.md` & `lndb-0.45a2/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/__init__.py` & `lndb-0.45a2/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.45a1"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.45a2"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.45a1/lndb/__main__.py` & `lndb-0.45a2/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_check_instance_setup.py` & `lndb-0.45a2/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_close.py` & `lndb-0.45a2/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_delete.py` & `lndb-0.45a2/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_init_instance.py` & `lndb-0.45a2/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_load_instance.py` & `lndb-0.45a2/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_migrate/alembic.ini` & `lndb-0.45a2/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_migrate/core.py` & `lndb-0.45a2/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_migrate/deploy.py` & `lndb-0.45a2/lndb/_migrate/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from lamin_logger import logger
 from packaging.version import parse as vparse
 
 from lndb._migrate.utils import generate_module_files, modify_alembic_ini
 from lndb.dev._db import insert
 from lndb.dev._settings_instance import InstanceSettings
 from lndb.dev._settings_user import UserSettings
-from lndb.dev._setup_schema import create_schema_if_not_exists, get_schema_module_name
+from lndb.dev._setup_schema import get_schema_module_name
 
 
 def decide_deploy_migration(
     schema_name: str, isettings: InstanceSettings, schema_module: ModuleType
 ) -> bool:
     schema_id = schema_module._schema_id
     schema_module_name = schema_module.__name__
@@ -114,15 +114,14 @@
     schema_names = ["core"] + list(isettings.schema)
     # enforce order (if bionty is part of schema_names, it needs to come 2nd)
     if "bionty" in schema_names:
         schema_names.remove("bionty")
         schema_names.insert(1, "bionty")
 
     for schema_name in schema_names:
-        create_schema_if_not_exists(schema_name, isettings)
         schema_module_name = get_schema_module_name(schema_name)
         schema_module = importlib.import_module(schema_module_name)
         schema_id = schema_module._schema_id
         current_version = schema_module.__version__
 
         if attempt_deploy:  # attempt deploy as we want to test migrating the database
             deploy_migration = True
```

### Comparing `lndb-0.45a1/lndb/_migrate/env.py` & `lndb-0.45a2/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_migrate/utils.py` & `lndb-0.45a2/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_notebook.py` & `lndb-0.45a2/lndb/_notebook.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_register_instance.py` & `lndb-0.45a2/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_schema.py` & `lndb-0.45a2/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_set.py` & `lndb-0.45a2/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_settings.py` & `lndb-0.45a2/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/_setup_user.py` & `lndb-0.45a2/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/__init__.py` & `lndb-0.45a2/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_clone.py` & `lndb-0.45a2/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_db.py` & `lndb-0.45a2/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_deprecated.py` & `lndb-0.45a2/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_exclusion.py` & `lndb-0.45a2/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_settings_instance.py` & `lndb-0.45a2/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_settings_load.py` & `lndb-0.45a2/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_settings_save.py` & `lndb-0.45a2/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_settings_store.py` & `lndb-0.45a2/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_settings_user.py` & `lndb-0.45a2/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_setup_knowledge.py` & `lndb-0.45a2/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/_storage.py` & `lndb-0.45a2/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/dev/upath.py` & `lndb-0.45a2/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/test/_migrations_e2e.py` & `lndb-0.45a2/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/lndb/test/_migrations_unit.py` & `lndb-0.45a2/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/noxfile.py` & `lndb-0.45a2/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/pyproject.toml` & `lndb-0.45a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
     "lnhub_rest==0.9.4",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
-    "lnschema_core>=0.28.0",
+    "lnschema_core>=0.34a2",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
     "sqlmodel>=0.0.8",
     "psycopg2-binary",
     "appdirs",
@@ -36,15 +36,15 @@
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
-    "lamindb[bionty,lamin1]>=0.39rc1",
+    "lamindb[bionty,lamin1]>=0.41a1",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test>=0.4.3",
     "nbproject",
 ]
 
 [project.scripts]
```

### Comparing `lndb-0.45a1/tests/test_bionty.py` & `lndb-0.45a2/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/tests/test_init_instance.py` & `lndb-0.45a2/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a1/PKG-INFO` & `lndb-0.45a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.45a1
+Version: 0.45a2
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.4
 Requires-Dist: laminci>=0.3.0
-Requires-Dist: lnschema_core>=0.28.0
+Requires-Dist: lnschema_core>=0.34a2
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
 Requires-Dist: cloudpathlib
 Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
 Requires-Dist: appdirs
 Requires-Dist: python-dotenv
@@ -18,15 +18,15 @@
 Requires-Dist: alembic
 Requires-Dist: natsort
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: universal_pathlib
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
-Requires-Dist: lamindb[bionty,lamin1]>=0.39rc1 ; extra == "test"
+Requires-Dist: lamindb[bionty,lamin1]>=0.41a1 ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb
 Provides-Extra: dev
 Provides-Extra: test
```


# Comparing `tmp/irails-1.3.27.tar.gz` & `tmp/irails-1.3.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.27.tar", last modified: Thu May 25 10:09:19 2023, max compression
+gzip compressed data, was "irails-1.3.30.tar", last modified: Fri May 26 14:46:17 2023, max compression
```

## Comparing `irails-1.3.27.tar` & `irails-1.3.30.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.895746 irails-1.3.27/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.27/MANIFEST.in
--rw-rw-rw-   0        0        0     4878 2023-05-25 10:09:19.894748 irails-1.3.27/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.27/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.814961 irails-1.3.27/irails/
--rw-rw-rw-   0        0        0      307 2023-05-25 10:09:11.000000 irails-1.3.27/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.27/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.27/irails/_loader.py
--rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.27/irails/_utils.py
--rw-rw-rw-   0        0        0    14109 2023-05-25 09:35:24.000000 irails-1.3.27/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.27/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.822939 irails-1.3.27/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.824934 irails-1.3.27/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.27/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.27/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.27/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.27/irails/cbv.py
--rw-rw-rw-   0        0        0     6246 2023-05-25 04:55:46.000000 irails-1.3.27/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.27/irails/controller_utils.py
--rw-rw-rw-   0        0        0    25573 2023-05-25 10:05:10.000000 irails-1.3.27/irails/core.py
--rw-rw-rw-   0        0        0    20203 2023-05-25 05:00:17.000000 irails-1.3.27/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.27/irails/log.py
--rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.27/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.27/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.27/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.27/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.836901 irails-1.3.27/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.27/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.27/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.27/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.27/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.27/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.27/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.27/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.27/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.27/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.27/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.27/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.784043 irails-1.3.27/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.847871 irails-1.3.27/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.27/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.27/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.27/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.27/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.27/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.27/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.27/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.27/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.27/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.849867 irails-1.3.27/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.27/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.850865 irails-1.3.27/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.27/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.860841 irails-1.3.27/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.27/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.27/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.27/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.873802 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.27/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.27/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.27/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.27/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.27/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.787034 irails-1.3.27/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.877793 irails-1.3.27/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.27/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.27/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.27/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.27/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.881781 irails-1.3.27/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.27/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.27/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.883778 irails-1.3.27/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.790027 irails-1.3.27/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.886769 irails-1.3.27/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.27/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.890758 irails-1.3.27/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.27/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.27/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.27/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.791025 irails-1.3.27/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.891755 irails-1.3.27/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.27/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1585 2023-05-24 07:01:16.000000 irails-1.3.27/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.27/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:09:19.820944 irails-1.3.27/irails.egg-info/
--rw-rw-rw-   0        0        0     4878 2023-05-25 10:09:19.000000 irails-1.3.27/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3185 2023-05-25 10:09:19.000000 irails-1.3.27/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:09:19.000000 irails-1.3.27/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-25 10:09:19.000000 irails-1.3.27/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-05-25 10:09:19.000000 irails-1.3.27/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 10:09:19.000000 irails-1.3.27/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 10:09:19.895746 irails-1.3.27/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.421299 irails-1.3.30/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.30/MANIFEST.in
+-rw-rw-rw-   0        0        0     4878 2023-05-26 14:46:17.420311 irails-1.3.30/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.30/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.324638 irails-1.3.30/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-26 14:46:02.000000 irails-1.3.30/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.30/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.30/irails/_loader.py
+-rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.30/irails/_utils.py
+-rw-rw-rw-   0        0        0    14179 2023-05-26 14:38:40.000000 irails-1.3.30/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.30/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.336615 irails-1.3.30/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.339599 irails-1.3.30/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.30/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.30/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.30/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.30/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24995 2023-05-26 14:01:10.000000 irails-1.3.30/irails/core.py
+-rw-rw-rw-   0        0        0    20250 2023-05-25 14:04:48.000000 irails-1.3.30/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.30/irails/log.py
+-rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.30/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.30/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.30/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.30/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.353682 irails-1.3.30/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.30/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.30/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.30/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.30/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.30/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.30/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.30/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.30/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.30/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.30/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.30/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.278801 irails-1.3.30/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.363883 irails-1.3.30/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.30/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.30/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.30/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.30/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.30/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.30/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.30/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.30/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.30/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.365878 irails-1.3.30/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.30/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.367873 irails-1.3.30/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.30/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.378843 irails-1.3.30/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.30/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.30/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.30/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.392806 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.30/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.30/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.30/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.30/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.30/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.282790 irails-1.3.30/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.395798 irails-1.3.30/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.30/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.30/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.30/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.30/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.397792 irails-1.3.30/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.30/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.30/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.401783 irails-1.3.30/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.287776 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.407413 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.413493 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.289772 irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.415787 irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1662 2023-05-25 10:31:13.000000 irails-1.3.30/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.30/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:46:17.332618 irails-1.3.30/irails.egg-info/
+-rw-rw-rw-   0        0        0     4878 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3185 2023-05-26 14:46:17.000000 irails-1.3.30/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 14:46:16.000000 irails-1.3.30/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:46:17.421299 irails-1.3.30/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.30/setup.py
```

### Comparing `irails-1.3.27/PKG-INFO` & `irails-1.3.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.27
+Version: 1.3.30
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.27/README.md` & `irails-1.3.30/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/_i18n.py` & `irails-1.3.30/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/_loader.py` & `irails-1.3.30/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/_utils.py` & `irails-1.3.30/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/auth.py` & `irails-1.3.30/irails/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 _session_name:str = ""
 
 class DomainUser(BaseUser):
     def __init__(self,username: str='anonymous',group:str="",domain:str="") -> None:
         self.username = username
         self._group = group
         self._domain = domain
+        self._lang = "zh"
+        self._timezone =  'Asia/Shanghai'
         super().__init__()
     @property
     def group(self):
         return self._group 
     @group.setter
     def group(self,value):
         self._group = value
```

### Comparing `irails-1.3.27/irails/base_controller.py` & `irails-1.3.30/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.30/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.30/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/cbv.py` & `irails-1.3.30/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/config.py` & `irails-1.3.30/irails/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,16 +158,17 @@
             if "." in name:
                 segment_name, sub_key = name.split(".", 1)
                 if segment_name == "ROOT":
                     # value = value.replace("{" + name + "}", self.config.get(sub_key, ""))
                     value = value.replace(
                         "{" + name + "}", YamlConfig(config=self._raw_config).get(sub_key, ""))
                 else:
-                    segment_config = self.config.get(segment_name, {})
-                    if isinstance(segment_config, dict):
+                    # segment_config = self.config.get(segment_name, {})
+                    segment_config =  config.get(segment_name, {})
+                    if isinstance(segment_config, dict) or isinstance(segment_config,YamlConfig):
                         sub_keys = sub_key.split(".")
                         sub_value = segment_config
                         for sub_key in sub_keys:
                             sub_value = sub_value.get(sub_key, {})
                         value = value.replace("{" + name + "}", str(sub_value))
             else:
                 value = value.replace(
```

### Comparing `irails-1.3.27/irails/controller_utils.py` & `irails-1.3.30/irails/controller_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 VER_KEY = "__custom_version__"
 PATH_KEY = "__custom_path__"
 METHOD_KEY = "__custom_method__"
 KWARGS_KEY = "__custom_kwargs__"
 SIGNATURE_KEY = "__saved_signature__"
 ARGS_KEY = "__custom_args__"
 AUTH_KEY="__auth__"
+DEFAULT_KEY="__default_index__"
 
 
 class ControllerBase:
     """ """
     
     pass
 
@@ -251,62 +252,77 @@
     """
     path_template = getattr(controller, TEMPLATE_PATH_KEY)
     version = getattr(controller, VER_KEY)
 
     # Get all the routes information
     routes_dict = _get_routes_in_controller(controller)
     generic_dict = _get_generic_type_var_dict(controller)
+    default_method = getattr(controller,DEFAULT_KEY)
 
     for name, value in routes_dict.items():
         member = getattr(controller, name)
         new_member = _copy_func(member)
         # setattr(new_member,'__doc__',getattr(member,'__doc__'))
         _update_generic_parameters_signature(generic_dict, new_member)
         
         path = _compute_path(value[PATH_KEY], controller.__name__, path_template, version)
         kwargs = _update_generic_args(generic_dict, value[KWARGS_KEY])
-         
+        #check defalut method
+        if name==default_method:
+            #check is exists `_index_default_` func
+            if not hasattr(controller,f"_{name}_default_"):
+                p = path.split("/")
+                controller_path ='/'.join(p[:-1]) + '/'
+                _new_member = _copy_func(member)
+                _update_generic_parameters_signature(generic_dict, _new_member)
+                summa = router.get(controller_path,  **kwargs)(_new_member)
+                setattr(controller,f'_{name}_default_',summa)
+        
         if isinstance(value[METHOD_KEY],list):
             route_method = getattr(router, 'api_route') 
             # 添加到 fastapi apiroute
             new_route_method = route_method(path,methods=value[METHOD_KEY], **kwargs)(new_member)
             
     
         else:
             if 'websocket' == value[METHOD_KEY]:
                 route_method = getattr(router, 'websocket' )
                 new_route_method = route_method(path)(new_member)
             else:
                 route_method = getattr(router, value[METHOD_KEY]) 
                 # 添加到 fastapi apiroute
                 new_route_method = route_method(path, **kwargs)(new_member)
+
+        
         setattr(controller, name, new_route_method)
     
     cbv(router)(controller)
 
  
 
  
 
 def _route_method(path: str, method, *args, **mwargs): 
     if not path.startswith("/"):
         raise RuntimeError("path must start with '/'")
     def wrapper(func ): 
         @wraps(func)
         async def actions_decorator(  *args, **kwargs):
-            auth_type:str = getattr(func,AUTH_KEY) 
+            
             has_request = kwargs.get("__has_request__")
             has_response = kwargs.get("__has_response__")
             cls:BaseController = None
             if 'self' in kwargs:
                 cls = kwargs['self']
             else:
                 module = inspect.getmodule(func)
                 cls = getattr(module, func.__qualname__.split('.<locals>', 1)[0].rsplit('.', 1)[0]) 
-             
+            auth_type:str = getattr(func,AUTH_KEY) 
+            if auth_type is None:
+                auth_type = getattr(cls,AUTH_KEY)
             response:Response = None
             result:Response = None
             
             if 'request' in kwargs and 'response' in kwargs:
                 response  = kwargs["response"]
                 rqst:Request = kwargs['request']  
                 #auth first then call constructor
@@ -346,15 +362,15 @@
         setattr(actions_decorator, METHOD_KEY, method)
         setattr(actions_decorator, ARGS_KEY, args)
         if '__auth_url__' in mwargs: 
             setattr(func,'__auth_url__',mwargs['__auth_url__'])
             del mwargs['__auth_url__']
 
         if not 'auth' in mwargs:
-            mwargs["auth"] = 'none'
+            mwargs["auth"] = None
         setattr(func,AUTH_KEY,mwargs['auth'])
         del mwargs['auth']
         setattr(actions_decorator, KWARGS_KEY, mwargs)
         # setattr(decorator,'__doc__',getattr(func,'__doc__'))
         setattr(actions_decorator, "__signature__", inspect.signature(func))
         return actions_decorator
     return wrapper
```

### Comparing `irails-1.3.27/irails/core.py` & `irails-1.3.30/irails/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi.encoders import DictIntStrAny, SetIntStr
 from fastapi.params import Depends
 from fastapi.utils import generate_unique_id
 from starlette.responses import JSONResponse, Response
 from starlette.routing import BaseRoute
 from fastapi.types import DecoratedCallable
 from .mvc_router import create_controller,MvcRouter as api,   register_controllers_to_app 
-from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
+from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY,DEFAULT_KEY, VER_KEY,get_docs  
 from .config import config,ROOT_PATH,_project_name
 from .log import _log,set_logger
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
@@ -181,15 +181,15 @@
     :param path :special path format ,ex. '/{controller}/{version}'
            if given any value,it's will be ensure {controller} flag in here auto
     :param version :str like 'v1.0' ,'2.0'..
            if given any value,the :path will have {controller} flag auto
     '''
     if not 'auth' in allargs:
         allargs['auth'] = 'none'
-
+    
     caller_frame = inspect.currentframe().f_back
     caller_file = caller_frame.f_code.co_filename
     relative_path = caller_file.replace(ROOT_PATH,"")
     if relative_path.count(os.sep)>2:
         app_dir = os.sep.join(relative_path.split(os.sep)[:-2]) # os.path.dirname(os.path.dirname(relative_path)).replace(os.sep,"")
     else:
         raise RuntimeError(_("app dir must in apps dir"))
@@ -325,15 +325,20 @@
         controller_path_name = get_snaked_name(get_controller_name(targetController.__name__))
         _view_url_path:str = url_path.replace("{controller}",controller_path_name).replace("{version}",version)  
         
         controller_current_view_path = abs_path + '/views/' + controller_path_name
         if version:
             controller_current_view_path += '/' + version
         setattr(puppetController,"__view_url__",_view_url_path) 
-
+        if 'default' in allargs:
+            default_method=allargs['default'] 
+            setattr(targetController,DEFAULT_KEY,default_method)
+            del allargs['default']
+        else:
+            setattr(targetController,DEFAULT_KEY,'')
         #add app dir sub views to StaticFiles
         if not controller_current_view_path in application.app_views_dirs: #ensure  load it once
             application.app_views_dirs[controller_current_view_path.lower()] = _view_url_path.lower() 
             #path match static files
             
             
  
@@ -403,16 +408,15 @@
     _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %(loaded,unloaded))  
     if not len(__all_controller__)>0:
         raise RuntimeError(_("not found any controller class"))
     
     _register_controllers()
 
     
-    if __is_debug:
-        _log.info(_("checking database configure..."))
+    _log.info(_("checking database configure..."))
     db_cfg = check_init_database()
 
     # Initializing the authentication system
     auth_type = config.get("auth", None)
     _casbin_adapter_class = None
     _adapter_uri: str = None
     if auth_type:
@@ -423,48 +427,18 @@
             _casbin_adapter_class = auth.get_adapter_module(__type_casbin_adapter)
             _adapter_uri = config.get("auth").get("adapter_uri")
             if not _adapter_uri:
                 _adapter_uri = db_cfg.get('uri')
             # Raise an error if the adapter is not supported
             if not _casbin_adapter_class:
                 raise RuntimeError(_("Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
-    # Check for database migrations
-    check_db_migrate()
+    if __is_debug:
+        # Check for database migrations
+        check_db_migrate()
     # Initialize the authentication system if the adapter class and URI are present
-    
+    from .log import set_logger
+    set_logger(_log,check_level=True)
     _log.info(_("init casbin auth system..."))
     application.casbin_auth = __init_auth(application, auth_type, _casbin_adapter_class, _adapter_uri)
     _log.info(_("load irails apps finished."))
     return application
-# import subprocess
-# import time
-# # 定义启动和停止进程的方法
-# def start_uvicon():
-#     cmd = 'uvicorn main:app --host 0.0.0.0 --port 8000'
-#     uvicorn_process = subprocess.Popen(cmd.split(), stdout=subprocess.PIPE)
-#     return uvicorn_process
-
-# def restart_uvicon(uvicorn_process):
-#     uvicorn_process.terminate()
-#     # 等待 10 秒后重启进程
-#     time.sleep(10)
-#     # 启动进程
-#     uvicorn_process = start_uvicon()
-
-    
- 
-
-
-# def run(app,*args,**kwargs): 
-#     import uvicorn
-#     global __is_debug 
-#     if  "debug" in kwargs:
-#         __is_debug = kwargs["debug"] 
-#         del kwargs['debug'] 
-#     if __is_debug:
-#         kwargs['reload'] = __is_debug
-#         kwargs['log_level'] = _log.level
-#         kwargs['reload_dirs'] = application.apps_dirs 
-#         uvicorn.run('irails.core:application', **kwargs)
-   
-         
-        
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `irails-1.3.27/irails/database.py` & `irails-1.3.30/irails/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,16 @@
     # 匹配非法字符
     illegal_chars = r'[\\/:\*\?"<>\|]'
     # 将非法字符替换为下划线
     sanitized_path = re.sub(illegal_chars, '_', path)
     return sanitized_path
 
 def check_migration(engine:Engine,uri,alembic_ini,upgrade=None): 
-    alembic_ini = os.path.abspath(os.path.join(ROOT_PATH,alembic_ini))
+    if os.path.isabs(alembic_ini)==False:
+        alembic_ini = os.path.abspath(os.path.join(ROOT_PATH,alembic_ini))
     def _update_uri_to_ini(): 
         #auto update alembic.ini sqlalchemy.url section 
         
         config = configparser.ConfigParser() 
         # read ini config
         config.read(alembic_ini)
         config.set('alembic','sqlalchemy.url',uri)
```

### Comparing `irails-1.3.27/irails/log.py` & `irails-1.3.30/irails/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging,os,sys
 from .config import config
-def set_logger(logger: logging.Logger):
+def set_logger(logger: logging.Logger,check_level=False):
     log_config = config.get("log")
     if not log_config:
         return logger
-    __log_level = log_config.get('level', 'DEBUG')
+    __log_level = logging._nameToLevel[log_config.get('level', 'DEBUG')] 
+    if check_level:
+        return logger.setLevel(__log_level)
     __log_file = log_config.get('file', None)
 
     debug = config.get("debug", False)
     logger.name = logger.name or log_config.get("name", 'iRails')
     if __log_file:
         __log_file = os.path.abspath(__log_file)
 
@@ -20,24 +22,24 @@
         if debug:
             try:
                 os.remove(__log_file)
             except:
                 pass
 
         file_handler = logging.FileHandler(__log_file, mode='a')
-        file_handler.setLevel(logging.DEBUG)
+        file_handler.setLevel(__log_level)
         file_handler.setFormatter(logging.Formatter(
             fmt=log_format, datefmt=datefmt))
         if not file_handler in logger.handlers:
             logger.addHandler(file_handler)
 
     handler = logging.StreamHandler(sys.stdout)
-    handler.setLevel(logging.DEBUG)
+    handler.setLevel(__log_level)
     handler.setFormatter(logging.Formatter(fmt=log_format, datefmt=datefmt))
     if not handler in logger.handlers:
         logger.addHandler(handler) 
-
+    _log.setLevel(__log_level)
 _log =   logging.getLogger()
 _log.setLevel(logging._nameToLevel['DEBUG'])
 
 set_logger(_log)
 _log.info("initing log.")
```

### Comparing `irails-1.3.27/irails/midware.py` & `irails-1.3.30/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/midware_casbin.py` & `irails-1.3.30/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/midware_session.py` & `irails-1.3.30/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/mvc_router.py` & `irails-1.3.30/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_app.py` & `irails-1.3.30/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_controller.py` & `irails-1.3.30/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_i18n.py` & `irails-1.3.30/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_migrate.py` & `irails-1.3.30/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_model.py` & `irails-1.3.30/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_project.py` & `irails-1.3.30/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_shell.py` & `irails-1.3.30/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/_test.py` & `irails-1.3.30/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/main.py` & `irails-1.3.30/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.30/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/app/home.tpl` & `irails-1.3.30/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/app/model.jinja` & `irails-1.3.30/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.30/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.30/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.30/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.30/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.30/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.30/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.30/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.30/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.30/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.30/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails/unit_test.py` & `irails-1.3.30/irails/unit_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from ._i18n import set_module_i18n
 
 class _BaseUnitTest(unittest.TestCase):
     
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
     def __init_subclass__(cls,*args,**kwargs) -> None:  
-        set_module_i18n(cls,cls.__module__)
         super().__init_subclass__(*args,**kwargs)    
+        if not cls.__name__ in ['ControllerTest','ServiceTest']:
+            set_module_i18n(cls,cls.__module__)
+        
 class ControllerTest(_BaseUnitTest):
     
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
         if not hasattr(_BaseUnitTest,'application'):
             _BaseUnitTest.application = generate_mvc_app()
         from fastapi.testclient import TestClient 
@@ -36,8 +38,8 @@
             db_cfg = config.get("database")
             db_uri = db_cfg.get("uri")
             alembic_ini = db_cfg.get("alembic_ini")
             ServiceTest.engine = init_database(db_uri,debug=True,cfg = db_cfg)
             if ServiceTest.engine:
                 check_migration(engine=ServiceTest.engine,uri= db_uri,alembic_ini= alembic_ini )
             ServiceTest.service = Service 
-    pass
+
```

### Comparing `irails-1.3.27/irails/view.py` & `irails-1.3.30/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/irails.egg-info/PKG-INFO` & `irails-1.3.30/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.27
+Version: 1.3.30
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.27/irails.egg-info/SOURCES.txt` & `irails-1.3.30/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.27/setup.py` & `irails-1.3.30/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/starrail-toolkit-0.6.2.tar.gz` & `tmp/starrail-toolkit-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.6.2.tar", last modified: Thu May 25 03:33:54 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.6.5.tar", last modified: Fri May 26 18:16:20 2023, max compression
```

## Comparing `starrail-toolkit-0.6.2.tar` & `starrail-toolkit-0.6.5.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.218711 starrail-toolkit-0.6.2/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.2/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     5866 2023-05-25 03:33:54.218558 starrail-toolkit-0.6.2/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     5359 2023-05-25 03:32:23.000000 starrail-toolkit-0.6.2/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-25 03:33:54.218752 starrail-toolkit-0.6.2/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.2/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.210619 starrail-toolkit-0.6.2/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.211212 starrail-toolkit-0.6.2/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3650 2023-05-25 03:25:18.000000 starrail-toolkit-0.6.2/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.212605 starrail-toolkit-0.6.2/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6513 2023-05-25 03:24:42.000000 starrail-toolkit-0.6.2/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5097 2023-05-25 03:08:53.000000 starrail-toolkit-0.6.2/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4577 2023-05-25 03:29:28.000000 starrail-toolkit-0.6.2/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.212948 starrail-toolkit-0.6.2/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6480 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.213885 starrail-toolkit-0.6.2/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1802 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/config.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      282 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.215121 starrail-toolkit-0.6.2/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    13725 2023-05-25 03:30:12.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/unlock_fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.215708 starrail-toolkit-0.6.2/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.216102 starrail-toolkit-0.6.2/starrail/unlock/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/unlock/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/unlock/fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/unlock/service.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.216763 starrail-toolkit-0.6.2/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1804 2023-05-25 03:28:51.000000 starrail-toolkit-0.6.2/starrail/utils/accounts.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.217596 starrail-toolkit-0.6.2/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     4292 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     9255 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/misc.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-25 03:31:36.000000 starrail-toolkit-0.6.2/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.218376 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     5866 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1669 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.762319 starrail-toolkit-0.6.5/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.5/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6145 2023-05-26 18:16:20.762148 starrail-toolkit-0.6.5/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5638 2023-05-26 18:14:07.000000 starrail-toolkit-0.6.5/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-26 18:16:20.762368 starrail-toolkit-0.6.5/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.5/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.754496 starrail-toolkit-0.6.5/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.755015 starrail-toolkit-0.6.5/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3650 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.756449 starrail-toolkit-0.6.5/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-26 04:24:47.000000 starrail-toolkit-0.6.5/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6284 2023-05-26 04:23:47.000000 starrail-toolkit-0.6.5/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1318 2023-05-26 04:23:17.000000 starrail-toolkit-0.6.5/starrail/gacha/factory.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6566 2023-05-26 04:12:49.000000 starrail-toolkit-0.6.5/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1080 2023-05-26 04:23:17.000000 starrail-toolkit-0.6.5/starrail/gacha/migrate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     7702 2023-05-26 09:09:00.000000 starrail-toolkit-0.6.5/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4854 2023-05-26 18:02:21.000000 starrail-toolkit-0.6.5/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.756699 starrail-toolkit-0.6.5/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6509 2023-05-26 09:49:54.000000 starrail-toolkit-0.6.5/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.757333 starrail-toolkit-0.6.5/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1916 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      282 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      645 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.758335 starrail-toolkit-0.6.5/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    21352 2023-05-26 18:02:38.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/unlock_fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.758983 starrail-toolkit-0.6.5/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2830 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/pie_chart.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.759364 starrail-toolkit-0.6.5/starrail/unlock/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/unlock/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/unlock/fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/unlock/service.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.760113 starrail-toolkit-0.6.5/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1804 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.760988 starrail-toolkit-0.6.5/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4783 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    10001 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/misc.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-26 18:04:11.000000 starrail-toolkit-0.6.5/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.761878 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6145 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1755 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.6.2/LICENSE` & `starrail-toolkit-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/PKG-INFO` & `starrail-toolkit-0.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.6.2
+Version: 0.6.5
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,15 +21,15 @@
 
 <b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.0    |    0.6.2     |   0.6.2   |   0.6.0    |
+|   0.6.5    |    0.6.5     |   0.6.5   |   0.6.5    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
 - [ ] 支持国际服
 - [x] 支持解锁120帧
 - [x] 支持以 SRGF 标准导出
@@ -43,19 +43,19 @@
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/iwDYF0x00q0f)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/ig3lR0xdvwwh)，两种途径的内容相同，可以自行选择下载方式。
 
-***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
+***BREAKING：目前用户界面正在优化中，预览如下图所示。***（注意：该版本尚未发布，所以 release 中仍然是旧版界面，且该界面正在调试过程中，可能会有一些问题，如果出现问题，请先下载旧版 release 使用。）
 
-![gui preview gacha](https://s1.ax1x.com/2023/05/23/p9o7y3d.png)
+![gui preview gacha](https://s1.ax1x.com/2023/05/25/p9HOzLQ.png)
 
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
@@ -120,8 +120,8 @@
 
 ## 安全提醒
 
 本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
 
 ## Credits
 
-本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)。
+本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)，用户界面设计参考了 [**BoxCatTeam/SRCat**](https://github.com/BoxCatTeam/SRCat)。
```

### Comparing `starrail-toolkit-0.6.2/README.md` & `starrail-toolkit-0.6.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 <b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.0    |    0.6.2     |   0.6.2   |   0.6.0    |
+|   0.6.5    |    0.6.5     |   0.6.5   |   0.6.5    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
 - [ ] 支持国际服
 - [x] 支持解锁120帧
 - [x] 支持以 SRGF 标准导出
@@ -28,19 +28,19 @@
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/iwDYF0x00q0f)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/ig3lR0xdvwwh)，两种途径的内容相同，可以自行选择下载方式。
 
-***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
+***BREAKING：目前用户界面正在优化中，预览如下图所示。***（注意：该版本尚未发布，所以 release 中仍然是旧版界面，且该界面正在调试过程中，可能会有一些问题，如果出现问题，请先下载旧版 release 使用。）
 
-![gui preview gacha](https://s1.ax1x.com/2023/05/23/p9o7y3d.png)
+![gui preview gacha](https://s1.ax1x.com/2023/05/25/p9HOzLQ.png)
 
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
@@ -105,8 +105,8 @@
 
 ## 安全提醒
 
 本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
 
 ## Credits
 
-本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)。
+本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)，用户界面设计参考了 [**BoxCatTeam/SRCat**](https://github.com/BoxCatTeam/SRCat)。
```

### Comparing `starrail-toolkit-0.6.2/setup.py` & `starrail-toolkit-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/__init__.py` & `starrail-toolkit-0.6.5/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/config.py` & `starrail-toolkit-0.6.5/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/entry/cli.py` & `starrail-toolkit-0.6.5/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/entry/gui.py` & `starrail-toolkit-0.6.5/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/entry/setup.py` & `starrail-toolkit-0.6.5/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gacha/autodet.py` & `starrail-toolkit-0.6.5/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gacha/database.py` & `starrail-toolkit-0.6.5/starrail/gacha/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,74 +17,88 @@
                 to use.
         """
 
         self.conn = sqlite3.connect(db_name)
         self.cursor = self.conn.cursor()
         for gacha_type in GachaType:
             self.create_table(gacha_type.name)
+        self.columns = ', '.join([
+            'uid', 'gacha_id', 'gacha_type', 'item_id', 'count', 'time',
+            'name', 'lang', 'item_type', 'rank_type', 'region',
+            'region_time_zone', 'id',
+        ])
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
+    def __exec_update(self, sql, parameters=()):
+        self.cursor.execute(sql, parameters)
+        self.conn.commit()
+
+    def exec_update(self, sql, parameters=()):
+        logger.info(f'Call update from external package: {sql}; {parameters}')
+        self.__exec_update(sql, parameters)
+
     def create_table(self, table_name: str) -> None:
         """
         Creates a new table in the database with the specified name.
 
         Args:
             table_name: A string representing the name of the table to create.
         """
 
-        self.cursor.execute(f'''CREATE TABLE IF NOT EXISTS {table_name} (
+        self.__exec_update(f'''CREATE TABLE IF NOT EXISTS {table_name} (
             uid TEXT,
             gacha_id TEXT,
             gacha_type TEXT,
             item_id TEXT,
             count TEXT,
             time TEXT,
             name TEXT,
             lang TEXT,
             item_type TEXT,
             rank_type TEXT,
+            region TEXT,
+            region_time_zone TEXT,
             id TEXT PRIMARY KEY
         );''')
-        self.conn.commit()
 
     def add_entry(self, table: str, entry: Dict[str, str]) -> None:
         """
         Adds a new entry to the specified table in the database.
 
         Args:
             table: A string representing the name of the table to add the
                 entry to.
             entry: A dictionary representing the entry to add to the table.
         """
 
-        self.cursor.execute(
-            f'INSERT INTO {table} VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);',
+        self.__exec_update(
+            f'''INSERT INTO {table} ({self.columns})
+                VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);''',
             self.parse_entry(entry),
         )
-        self.conn.commit()
 
     def get_entries(self, table: str) -> List[Dict[str, str]]:
         """
         Retrieves all entries from the specified table in the database.
 
         Args:
             table: A string representing the name of the table to retrieve
                 entries from.
 
         Returns:
             A list of dictionaries representing the entries retrieved from the
                 table.
         """
 
-        self.cursor.execute(f'SELECT * FROM {table};')
+        self.cursor.execute(f'SELECT {self.columns} FROM {table};')
         entries = self.cursor.fetchall()
         return [self.unparse_entry(*entry) for entry in entries]
 
     def close(self) -> None:
         """
         Closes the connection to the database.
         """
@@ -110,16 +124,15 @@
         """
         Sets the version of the database.
 
         Args:
             value: An integer representing the new version of the database.
         """
 
-        self.cursor.execute(f'PRAGMA user_version={value};')
-        self.conn.commit()
+        self.__exec_update(f'PRAGMA user_version={value};')
 
     @staticmethod
     def parse_entry(entry: Dict[str, str]) -> Tuple:
         """
         Parses an entry dictionary into a tuple for insertion into the
         database.
 
@@ -136,25 +149,27 @@
         item_id = entry['item_id']
         count = entry['count']
         time_ = entry['time']
         name = entry['name']
         lang = entry['lang']
         item_type = entry['item_type']
         rank_type = entry['rank_type']
+        region = entry['region']
+        region_time_zone = entry['region_time_zone']
         id_ = entry['id']
         return (
             uid, gacha_id, gacha_type, item_id, count, time_, name, lang,
-            item_type, rank_type, id_,
+            item_type, rank_type, region, region_time_zone, id_,
         )
 
     @staticmethod
     def unparse_entry(
         uid: str, gacha_id: str, gacha_type: str, item_id: str, count: str,
         time_: str, name: str, lang: str, item_type: str, rank_type: str,
-        id_: str,
+        region: str, region_time_zone: str, id_: str,
     ) -> Dict[str, str]:
         """
         Unparses a tuple from the database into an entry dictionary.
 
         Args:
             uid: A string representing the UID of the entry.
             gacha_id: A string representing the Gacha ID of the entry.
@@ -172,43 +187,9 @@
             A dictionary representing the unparsed entry.
         """
 
         return dict(
             uid=uid, gacha_id=gacha_id, gacha_type=gacha_type,
             item_id=item_id, count=count, time=time_, name=name,
             lang=lang, item_type=item_type, rank_type=rank_type,
-            id=id_,
+            region=region, region_time_zone=region_time_zone, id=id_,
         )
-
-
-class DatabaseFactory:
-
-    API_VERSION = 1
-
-    @staticmethod
-    def get_database(db_name: str) -> GachaDatabase:
-        """
-        Retrieves a new instance of a GachaDatabase with the specified name.
-
-        Args:
-            db_name: A string representing the name of the database to
-                connect to.
-
-        Returns:
-            A new instance of a GachaDatabase.
-        """
-        db = GachaDatabase(db_name)
-        if db.version == 0:
-            db.version = DatabaseFactory.API_VERSION
-        elif db.version < DatabaseFactory.API_VERSION:
-            logger.warn(
-                'Version of your database is lower than api version. '
-                'Migration is required or potential data loss will '
-                'occur.',
-            )
-        elif db.version > DatabaseFactory.API_VERSION:
-            logger.warn(
-                'Version of the program is lower than database '
-                'version. Please update your program or unexpected '
-                'errors will occur.',
-            )
-        return db
```

### Comparing `starrail-toolkit-0.6.2/starrail/gacha/fetch.py` & `starrail-toolkit-0.6.5/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gacha/fileio.py` & `starrail-toolkit-0.6.5/starrail/gacha/fileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import time
 
 import pandas as pd
 
 import starrail
 import starrail.utils.babelfish as babelfish
-from starrail.gacha.database import DatabaseFactory
+from starrail.gacha.factory import DatabaseFactory
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
 from starrail.utils import loggings
 
 logger = loggings.get_logger(__file__)
 
 
@@ -128,17 +128,18 @@
 
 
 def export_as_srgf(manager: GachaDataManager, output_path: str) -> None:
     gacha_list = []
     for gacha_type in GachaType:
         gacha_list.extend(manager.gacha[gacha_type.value].tolist())
     gacha_list.sort(key=lambda x: x['id'])
-    uid = gacha_list[0]['uid'] if gacha_list else manager.uid
-    lang = gacha_list[0]['lang'] if gacha_list else 'zh-cn'
-    timezone = time.localtime().tm_gmtoff // 3600
+    uid = gacha_list[-1]['uid'] if gacha_list else manager.uid
+    lang = gacha_list[-1]['lang'] if gacha_list else 'zh-cn'
+    timezone = gacha_list[-1]['region_time_zone'] if gacha_list else '8'
+    timezone = int(timezone)
     timestamp = int(time.time())
     data = dict(
         info=dict(
             uid=uid,
             lang=lang,
             region_time_zone=timezone,
             export_timestamp=timestamp,
```

### Comparing `starrail-toolkit-0.6.2/starrail/gacha/parse.py` & `starrail-toolkit-0.6.5/starrail/gacha/parse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import copy
 import os
+import time
 from typing import Dict
 
 from prettytable import PrettyTable
 
 from starrail.config import configuration as cfg
-from starrail.gacha.database import DatabaseFactory
+from starrail.gacha.factory import DatabaseFactory
 from starrail.gacha.type import GachaType
 from starrail.utils import loggings
+from starrail.utils.babelfish.dictionary import record_type_mapping
 
 logger = loggings.get_logger(__file__)
 
 
 class GachaDataList:
     def __init__(self, name, iterable=[], hash_key='id'):
         self.name = name
@@ -39,14 +41,82 @@
     def sort(self):
         self.data.sort(key=lambda x: -int(x[self.hash_key]))
 
     def tolist(self):
         return copy.deepcopy(self.data)
 
     @property
+    def stats_v2(self):
+        today = time.strftime('%y.%m.%d')
+        if not self.data:
+            return dict(
+                character5=0,
+                character4=0,
+                lightcone5=0,
+                lightcone4=0,
+                lightcone3=0,
+                total=0,
+                since_last=0,
+                average_up=0,
+                average_5=0,
+                start_time=today,
+                end_time=today,
+                five_stars=[],
+            )
+        self.sort()
+        character5 = character4 = lightcone5 = lightcone4 = lightcone3 = 0
+        for item in self.data:
+            item_type = item['item_type']
+            item_type = record_type_mapping.get(item_type, item_type)
+            rank_type = item['rank_type']
+            if item_type == 'character':
+                if rank_type == '5':
+                    character5 += 1
+                elif rank_type == '4':
+                    character4 += 1
+            elif item_type == 'lightcone':
+                if rank_type == '5':
+                    lightcone5 += 1
+                elif rank_type == '4':
+                    lightcone4 += 1
+                elif rank_type == '3':
+                    lightcone3 += 1
+        five_stars = [['', 0, False]]
+        for item in reversed(self.data):
+            five_stars[-1][1] += 1
+            rank_type = item['rank_type']
+            name = item['name']
+            if rank_type == '5':
+                five_stars[-1] = (name, five_stars[-1][1], False)
+                five_stars.append(['', 0, False])
+        since_last = 0 if five_stars[-1][0] else five_stars[-1][1]
+        if not five_stars[-1][0]:
+            five_stars.pop(-1)
+        if not five_stars:
+            average_up = average_5 = 0
+        else:
+            average_5 = sum([it[1] for it in five_stars]) / len(five_stars)
+            ups = list(filter(lambda it: it[-1], five_stars))
+            average_up = sum([it[1] for it in ups]) / len(ups) if ups else 0
+        return dict(
+            character5=character5,
+            character4=character4,
+            lightcone5=lightcone5,
+            lightcone4=lightcone4,
+            lightcone3=lightcone3,
+            total=len(self.data),
+            since_last=since_last,
+            average_up=average_up,
+            average_5=average_5,
+            start_time=self.data[-1]['time'].split()[0].replace('-', '.'),
+            end_time=self.data[0]['time'].split()[0].replace('-', '.'),
+            five_stars=five_stars,
+        )
+
+    @property
     def stats(self):
         data = []
         for rank_type in ['5', '4', '3']:
             data.append(self.substats(rank_type))
         return data
 
     def substats(self, rank_type):
@@ -94,15 +164,15 @@
             average=f'{(total_items - since_last) / count:.2f}',
         )
 
 
 class GachaDataManager:
 
     def __init__(self, uid):
-        self.uid: str = uid
+        self.uid = uid
         self.gacha = self.load_cache(uid)
 
     def load_cache(self, uid: str):
         db_dir = cfg.db_dir
         self.cache_path = os.path.join(db_dir, f'{uid}.sqlite3')
         if os.path.isfile(self.cache_path):
             return parse_cache_from_sql(self.cache_path)
```

### Comparing `starrail-toolkit-0.6.2/starrail/gacha/service.py` & `starrail-toolkit-0.6.5/starrail/gacha/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,24 +46,29 @@
 ):
     r = []
     end_id = '0'
     for page in integers():
         logger.info(f'Downloading page {page} of type {gacha_type.name}')
         api_url = get_api_url(
             api_template, end_id, str(gacha_type.value),
-            str(page), '5',
+            str(page), '20',
         )
         logger.debug(f'Requesting {api_url}')
         response, code = fetch_json(api_url)
         time.sleep(request_interval)
         _, should_stop, msg = check_response(response, code)
         logger.info(f'check_response: {msg}')
         if should_stop:
             break
         data_list = response['data']['list']
+        region = response['data']['region']
+        timezone = response['data']['region_time_zone']
+        metainfo = dict(region=region, region_time_zone=timezone)
+        for data_item in data_list:
+            data_item.update(metainfo)
         r.extend(data_list)
         end_id = data_list[-1]['id']
     return r
 
 
 def deduce_uid(record_cache):
     for gacha_type in GachaType:
@@ -116,23 +121,24 @@
     manager.log_stats()
 
     export_hooks = dict(
         csv=fileio.export_as_csv,
         html=fileio.export_as_html,
         json=fileio.export_as_json,
         md=fileio.export_as_md,
+        srgf=fileio.export_as_srgf,
         xlsx=fileio.export_as_xlsx,
     )
     if 'all' in export:
         export = ['csv', 'html', 'json', 'md', 'srgf', 'xlsx']
 
     timestamp = time.strftime('%Y%m%d%H%M%S')
 
     for format in export:
-        if format == 'srgf':
-            format = 'srgf.json'
         logger.info(f'Exporting gacha data as {format} format')
         output_dir = os.getcwd()
         filename = f'HKSR-export-{uid}-{timestamp}.{format}'
+        if format == 'srgf':
+            filename += '.json'
         path = os.path.join(output_dir, filename)
         export_hooks[format](manager, path)
         logger.info(f'Gacha data in {format} format is saved to {path}')
```

### Comparing `starrail-toolkit-0.6.2/starrail/gacha/url.py` & `starrail-toolkit-0.6.5/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/application.py` & `starrail-toolkit-0.6.5/starrail/gui/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             NavigationItemPosition.TOP,
         )
 
         self.addSubInterface(
             self.unlockFpsInterface,
             'unlockFpsInterface',
             Icon.UNLOCK,
-            'unlock fps',
+            babelfish.ui_unlock_fps(),
             NavigationItemPosition.TOP,
         )
 
         self.addSubInterface(
             self.usersInterface,
             'usersInterface',
             Icon.USER,
@@ -138,16 +138,16 @@
             self.settingInterface,
             'settingInterface',
             qfluentwidgets.FluentIcon.SETTING,
             babelfish.ui_settings(),
             NavigationItemPosition.BOTTOM,
         )
 
-        self.navigationInterface.setDefaultRouteKey(
-            self.homeInterface.objectName(),
+        qfluentwidgets.qrouter.setDefaultRouteKey(
+            self.stackWidget, self.homeInterface.objectName(),
         )
         self.stackWidget.currentWidgetChanged.connect(
             lambda w: self.navigationInterface.setCurrentItem(w.objectName()),
         )
         self.navigationInterface.setCurrentItem(
             self.homeInterface.objectName(),
         )
```

### Comparing `starrail-toolkit-0.6.2/starrail/gui/common/config.py` & `starrail-toolkit-0.6.5/starrail/gui/common/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     cache_dir = os.path.join(userroot, '.starrail')
     db_dir = os.path.join(userroot, '.starrail', 'database')
     config_path = os.path.join(userroot, '.starrail', 'qconfig.json')
 
     locale = qfw.OptionsConfigItem(
         group='StarRailToolkit',
         name='Locale',
-        default=Language.AUTO,
+        default=Language.CHINESE_SIMPLIFIED,
         validator=qfw.OptionsValidator(Language),
         serializer=LanguageSerializer(),
         restart=True,
     )
 
     check_update = qfw.ConfigItem(
         group='StarRailToolkit',
@@ -58,12 +58,14 @@
         validator=qfw.BoolValidator(),
         restart=False,
     )
 
     def __init__(self, path):
         super().__init__()
         self.file = Path(path)
+        if not self.file.exists():
+            self.set(self.themeColor, '#ff0077dd')
+            self.set(self.themeMode, qfw.Theme.DARK)
 
 
 qcfg = StarRailConfig(path=StarRailConfig.config_path)
 qfw.qconfig.load(StarRailConfig.config_path, qcfg)
-qcfg.set(qcfg.themeColor, '#ff0077dd')
```

### Comparing `starrail-toolkit-0.6.2/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.6.5/starrail/gui/common/stylesheet.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class StyleSheet(StyleSheetBase, Enum):
     """ Style sheet  """
 
     BASE_INTERFACE = 'base_interface'
     CHECK_UPDATE_DIALOG = 'check_update_dialog'
+    GACHA_RECORD = 'gacha_record'
     HOME_INTERFACE = 'home_interface'
     LINK_CARD = 'link_card'
     RESULT_TABLE_WIDGET = 'result_table_widget'
     SETTING_INTERFACE = 'setting_interface'
     STAR_RAIL_TOOLKIT = 'star_rail_toolkit'
 
     def path(self, theme=Theme.AUTO):
```

### Comparing `starrail-toolkit-0.6.2/starrail/gui/common/utils.py` & `starrail-toolkit-0.6.5/starrail/gui/common/utils.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.6.5/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.6.5/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.6.5/starrail/gui/interfaces/setting.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/interfaces/unlock_fps.py` & `starrail-toolkit-0.6.5/starrail/gui/interfaces/unlock_fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.6.5/starrail/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.6.5/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.6.5/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/unlock/fps.py` & `starrail-toolkit-0.6.5/starrail/unlock/fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/utils/accounts.py` & `starrail-toolkit-0.6.5/starrail/utils/accounts.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/utils/auto_update.py` & `starrail-toolkit-0.6.5/starrail/utils/auto_update.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.6.5/starrail/utils/babelfish/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,24 @@
 
 average_gacha_per_5_star = dictionary.average_gacha_per_5_star
 gacha_report = dictionary.gacha_report
 gacha_title = dictionary.gacha_title
 history_of_5_stars = dictionary.history_of_5_stars
 html_thead = dictionary.html_thead
 markdown_thead = dictionary.markdown_thead
+ui_3star_light_cone = dictionary.ui_3star_light_cone
+ui_4star_character = dictionary.ui_4star_character
+ui_4star_light_cone = dictionary.ui_4star_light_cone
+ui_5star_character = dictionary.ui_5star_character
+ui_5star_light_cone = dictionary.ui_5star_light_cone
 ui_about = dictionary.ui_about
 ui_about_this = dictionary.ui_about_this
+ui_arerage_warps_per_5star = dictionary.ui_arerage_warps_per_5star
 ui_auto = dictionary.ui_auto
+ui_average_warps_per_up = dictionary.ui_average_warps_per_up
 ui_cancel_update = dictionary.ui_cancel_update
 ui_check_update = dictionary.ui_check_update
 ui_check_update_at_start = dictionary.ui_check_update_at_start
 ui_check_update_at_start_desc = dictionary.ui_check_update_at_start_desc
 ui_check_update_fail = dictionary.ui_check_update_fail
 ui_check_update_success = dictionary.ui_check_update_success
 ui_copyright = dictionary.ui_copyright
@@ -65,25 +72,27 @@
 ui_set_fps_fail_with_msg = dictionary.ui_set_fps_fail_with_msg
 ui_setting_failure = dictionary.ui_setting_failure
 ui_setting_panel = dictionary.ui_setting_panel
 ui_setting_restart_content = dictionary.ui_setting_restart_content
 ui_setting_restart_title = dictionary.ui_setting_restart_title
 ui_setting_success = dictionary.ui_setting_success
 ui_settings = dictionary.ui_settings
+ui_since_last_guarantee = dictionary.ui_since_last_guarantee
 ui_status_panel = dictionary.ui_status_panel
 ui_sync = dictionary.ui_sync
 ui_sync_gacha_fail = dictionary.ui_sync_gacha_fail
 ui_sync_gacha_initial = dictionary.ui_sync_gacha_initial
 ui_sync_gacha_success = dictionary.ui_sync_gacha_success
 ui_synchronizing_gacha = dictionary.ui_synchronizing_gacha
 ui_theme_mode = dictionary.ui_theme_mode
 ui_theme_mode_dark = dictionary.ui_theme_mode_dark
 ui_theme_mode_light = dictionary.ui_theme_mode_light
 ui_theme_mode_settings_desc = dictionary.ui_theme_mode_settings_desc
 ui_title = dictionary.ui_title
+ui_total_warp = dictionary.ui_total_warp
 ui_traceback = dictionary.ui_traceback
 ui_troubleshooting = dictionary.ui_troubleshooting
 ui_troubleshooting_desc = dictionary.ui_troubleshooting_desc
 ui_unlock_fps = dictionary.ui_unlock_fps
 ui_unlock_fps_desc = dictionary.ui_unlock_fps_desc
 ui_update_available = dictionary.ui_update_available
 ui_update_desc = dictionary.ui_update_desc
```

### Comparing `starrail-toolkit-0.6.2/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.6.5/starrail/utils/babelfish/dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,19 @@
     DEPARTURE=_MS(en='Departure Warp', zhs='始发跃迁'),
     CHARACTER=_MS(en='Character Event Warp', zhs='角色跃迁'),
     LIGHT_CONE=_MS(en='Light Cone Event Warp', zhs='光锥跃迁'),
     GitHub_dist=_MS(en='GitHub Distribution', zhs='GitHub下载'),
     netdisk_dist=_MS(en='Net Disk Distribution', zhs='网盘下载'),
 )
 
+record_type_mapping = {
+    '角色': 'character',
+    '光锥': 'lightcone',
+}
+
 # === BEGIN OF PRE-DEFINED VOCABULARIES ===
 
 average_gacha_per_5_star = _MS(
     en='Average gacha per 5-star',
     zhs='五星平均抽数',
 )
 gacha_report = _MS(en='Gacha Report', zhs='抽卡分析')
@@ -39,17 +44,30 @@
         '| ---- | ----- | ----------- | ---------- | ---------- |\n'
     ),
     zhs=(
         '| 星级 | 数量 | 基础概率 | 综合概率 | 距上次 |\n'
         '| ---- | ---- | ------ | ------- | ---- |\n'
     ),
 )
+ui_3star_light_cone = _MS(en='Light Cone (3)', zhs='三星光锥')
+ui_4star_character = _MS(en='Character (4)', zhs='四星角色')
+ui_4star_light_cone = _MS(en='Light Cone (4)', zhs='四星光锥')
+ui_5star_character = _MS(en='Character (5)', zhs='五星角色')
+ui_5star_light_cone = _MS(en='Light Cone (5)', zhs='五星光锥')
 ui_about = _MS(en='About', zhs='关于')
 ui_about_this = _MS(en='About This Application', zhs='关于本软件')
+ui_arerage_warps_per_5star = _MS(
+    en='Average warps per 5 star',
+    zhs='五星平均抽数',
+)
 ui_auto = _MS(en='Auto', zhs='跟随系统设置')
+ui_average_warps_per_up = _MS(
+    en='Average warps per up',
+    zhs='UP 平均抽数',
+)
 ui_cancel_update = _MS(en='Cancel Update', zhs='暂不更新')
 ui_check_update = _MS(en='Check Update', zhs='检查更新')
 ui_check_update_at_start = _MS(
     en='Check Update at Application Start',
     zhs='启动时自动检查更新',
 )
 ui_check_update_at_start_desc = _MS(
@@ -174,14 +192,18 @@
 ui_setting_restart_content = _MS(
     en='Please restart to apply changes.',
     zhs='请重启以应用新设置。',
 )
 ui_setting_restart_title = _MS(en='Success', zhs='设置成功')
 ui_setting_success = _MS(en='Success', zhs='设置成功')
 ui_settings = _MS(en='Settings', zhs='设置')
+ui_since_last_guarantee = _MS(
+    en='Since Last Guarantee',
+    zhs='保底已垫',
+)
 ui_status_panel = _MS(en='Status Panel', zhs='状态面板')
 ui_sync = _MS(en='Sync Data', zhs='同步数据')
 ui_sync_gacha_fail = _MS(
     en='Synchronization Failed',
     zhs='同步失败',
 )
 ui_sync_gacha_initial = _MS(
@@ -200,14 +222,15 @@
 ui_theme_mode_dark = _MS(en='Dark', zhs='深色')
 ui_theme_mode_light = _MS(en='Light', zhs='浅色')
 ui_theme_mode_settings_desc = _MS(
     en='Changing the appearance of application',
     zhs='改变应用外观',
 )
 ui_title = _MS(en='Honkai: Star Rail Toolkit', zhs='崩坏：星穹铁道工具箱')
+ui_total_warp = _MS(en='Total Warp', zhs='总抽数')
 ui_traceback = _MS(en='Traceback', zhs='报错信息')
 ui_troubleshooting = _MS(en='TroubleShooting', zhs='常见问题')
 ui_troubleshooting_desc = _MS(
     en='Click here to view FAQ.',
     zhs='点此查看常见问题解答。',
 )
 ui_unlock_fps = _MS(
```

### Comparing `starrail-toolkit-0.6.2/starrail/utils/babelfish/locale.py` & `starrail-toolkit-0.6.5/starrail/utils/babelfish/locale.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.6.5/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail/utils/loggings.py` & `starrail-toolkit-0.6.5/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.2/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.6.5/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.6.2
+Version: 0.6.5
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,15 +21,15 @@
 
 <b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.0    |    0.6.2     |   0.6.2   |   0.6.0    |
+|   0.6.5    |    0.6.5     |   0.6.5   |   0.6.5    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
 - [ ] 支持国际服
 - [x] 支持解锁120帧
 - [x] 支持以 SRGF 标准导出
@@ -43,19 +43,19 @@
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouy.com/iwDYF0x00q0f)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/ig3lR0xdvwwh)，两种途径的内容相同，可以自行选择下载方式。
 
-***BREAKING：目前用户界面的第一个版本已经实现完成，界面预览：***
+***BREAKING：目前用户界面正在优化中，预览如下图所示。***（注意：该版本尚未发布，所以 release 中仍然是旧版界面，且该界面正在调试过程中，可能会有一些问题，如果出现问题，请先下载旧版 release 使用。）
 
-![gui preview gacha](https://s1.ax1x.com/2023/05/23/p9o7y3d.png)
+![gui preview gacha](https://s1.ax1x.com/2023/05/25/p9HOzLQ.png)
 
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
@@ -120,8 +120,8 @@
 
 ## 安全提醒
 
 本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
 
 ## Credits
 
-本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)。
+本仓库用户界面部分基于 [**zhiyiYo/PyQt-Fluent-Widgets**](https://github.com/zhiyiYo/PyQt-Fluent-Widgets) 实现，缓存解析部分参考了 [**sunfkny/genshin-gacha-export**](https://github.com/sunfkny/genshin-gacha-export)，用户界面设计参考了 [**BoxCatTeam/SRCat**](https://github.com/BoxCatTeam/SRCat)。
```

### Comparing `starrail-toolkit-0.6.2/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.6.5/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 starrail/entry/__init__.py
 starrail/entry/cli.py
 starrail/entry/gui.py
 starrail/entry/setup.py
 starrail/gacha/__init__.py
 starrail/gacha/autodet.py
 starrail/gacha/database.py
+starrail/gacha/factory.py
 starrail/gacha/fetch.py
 starrail/gacha/fileio.py
+starrail/gacha/migrate.py
 starrail/gacha/parse.py
 starrail/gacha/service.py
 starrail/gacha/type.py
 starrail/gacha/url.py
 starrail/gui/__init__.py
 starrail/gui/application.py
 starrail/gui/common/__init__.py
@@ -30,14 +32,15 @@
 starrail/gui/interfaces/home.py
 starrail/gui/interfaces/setting.py
 starrail/gui/interfaces/unlock_fps.py
 starrail/gui/interfaces/users.py
 starrail/gui/widgets/__init__.py
 starrail/gui/widgets/dialog.py
 starrail/gui/widgets/link_card.py
+starrail/gui/widgets/pie_chart.py
 starrail/gui/widgets/title_bar.py
 starrail/unlock/__init__.py
 starrail/unlock/fps.py
 starrail/unlock/service.py
 starrail/utils/__init__.py
 starrail/utils/accounts.py
 starrail/utils/auto_update.py
```


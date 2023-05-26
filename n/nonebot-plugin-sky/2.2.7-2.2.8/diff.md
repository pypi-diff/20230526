# Comparing `tmp/nonebot-plugin-sky-2.2.7.tar.gz` & `tmp/nonebot-plugin-sky-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sky-2.2.7.tar", last modified: Sun Apr 30 05:21:33 2023, max compression
+gzip compressed data, was "nonebot-plugin-sky-2.2.8.tar", last modified: Fri May 26 14:24:34 2023, max compression
```

## Comparing `nonebot-plugin-sky-2.2.7.tar` & `nonebot-plugin-sky-2.2.8.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.583501 nonebot-plugin-sky-2.2.7/
--rw-rw-rw-   0        0        0    35823 2022-11-03 06:35:38.000000 nonebot-plugin-sky-2.2.7/LICENSE
--rw-rw-rw-   0        0        0    16034 2023-04-30 05:21:33.558566 nonebot-plugin-sky-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    15510 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.373413 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/
--rw-rw-rw-   0        0        0     6169 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.498080 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:49:56.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/__init__.py
--rw-rw-rw-   0        0        0     5707 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/command.py
--rw-rw-rw-   0        0        0     1810 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/helper_at_all.py
--rw-rw-rw-   0        0        0     1261 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/load_config.py
--rw-rw-rw-   0        0        0     1747 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/msg_forward.py
--rw-rw-rw-   0        0        0     1560 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/travelling_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.612774 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/
--rw-rw-rw-   0        0        0     1160 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/light_beauty.py
--rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/light_cute.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.684580 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.744420 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/__init__.py
--rw-rw-rw-   0        0        0     2547 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/international.py
--rw-rw-rw-   0        0        0     3077 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/national.py
--rw-rw-rw-   0        0        0   459817 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/get_id.png
--rw-rw-rw-   0        0        0      637 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/public_notice.py
--rw-rw-rw-   0        0        0    13461 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/query_tools.py
--rw-rw-rw-   0        0        0     1080 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/queue.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.796281 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/
--rw-rw-rw-   0        0        0        0 2023-03-01 12:32:18.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/international.py
--rw-rw-rw-   0        0        0     2996 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/national.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:32.592151 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:50:17.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.396004 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/
--rw-rw-rw-   0        0        0    16051 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/eating.jpg
--rw-rw-rw-   0        0        0    89789 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_braid.gif
--rw-rw-rw-   0        0        0    79644 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_bun.gif
--rw-rw-rw-   0        0        0    72146 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_cat.gif
--rw-rw-rw-   0        0        0    87935 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_fox.gif
--rw-rw-rw-   0        0        0    80542 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
--rw-rw-rw-   0        0        0    95522 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/go.jpg
--rw-rw-rw-   0        0        0      274 2023-01-02 06:48:03.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.414951 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu_image/
--rw-rw-rw-   0        0        0   824527 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu_image/menu.png
--rw-rw-rw-   0        0        0       95 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/pusher.py
--rw-rw-rw-   0        0        0     3791 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:33.545601 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/
--rw-rw-rw-   0        0        0     2280 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/__init__.py
--rw-rw-rw-   0        0        0      405 2022-12-22 07:28:55.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/bot_loader.py
--rw-rw-rw-   0        0        0      607 2023-03-01 12:37:46.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/chain_reply.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/check_update.py
--rw-rw-rw-   0        0        0     6369 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/data_pack.py
--rw-rw-rw-   0        0        0      391 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/date_util.py
--rw-rw-rw-   0        0        0      746 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/json_cards.py
--rw-rw-rw-   0        0        0     1264 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/notice_board.py
-drwxrwxrwx   0        0        0        0 2023-04-30 05:21:31.382390 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/
--rw-rw-rw-   0        0        0    16034 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1984 2023-04-30 05:21:31.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-30 05:21:30.000000 nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 05:21:33.583501 nonebot-plugin-sky-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1450 2023-04-30 05:20:01.000000 nonebot-plugin-sky-2.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.601519 nonebot-plugin-sky-2.2.8/
+-rw-rw-rw-   0        0        0    35823 2022-11-03 06:35:38.000000 nonebot-plugin-sky-2.2.8/LICENSE
+-rw-rw-rw-   0        0        0    15639 2023-05-26 14:24:34.600521 nonebot-plugin-sky-2.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    15115 2023-05-26 14:21:53.000000 nonebot-plugin-sky-2.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.402052 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/
+-rw-rw-rw-   0        0        0     7665 2023-05-26 14:18:37.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.420006 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:49:56.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/__init__.py
+-rw-rw-rw-   0        0        0     5707 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/command.py
+-rw-rw-rw-   0        0        0     1810 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/helper_at_all.py
+-rw-rw-rw-   0        0        0     1258 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/load_config.py
+-rw-rw-rw-   0        0        0     1748 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/msg_forward.py
+-rw-rw-rw-   0        0        0     1628 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/travelling_cache.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.436959 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/
+-rw-rw-rw-   0        0        0     1160 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/light_beauty.py
+-rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/light_cute.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.460895 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.476852 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2547 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/international.py
+-rw-rw-rw-   0        0        0     3077 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/national.py
+-rw-rw-rw-   0        0        0   459817 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/get_id.png
+-rw-rw-rw-   0        0        0      637 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/public_notice.py
+-rw-rw-rw-   0        0        0    14200 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/query_tools.py
+-rw-rw-rw-   0        0        0     1083 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/queue.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.484831 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/
+-rw-rw-rw-   0        0        0        0 2023-03-01 12:32:18.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
+-rw-rw-rw-   0        0        0     3225 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/international.py
+-rw-rw-rw-   0        0        0     3207 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/national.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.493807 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/
+-rw-rw-rw-   0        0        0        0 2023-03-01 11:50:17.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.553647 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/
+-rw-rw-rw-   0        0        0    16051 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/eating.jpg
+-rw-rw-rw-   0        0        0    89789 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_braid.gif
+-rw-rw-rw-   0        0        0    79644 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_bun.gif
+-rw-rw-rw-   0        0        0    72146 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_cat.gif
+-rw-rw-rw-   0        0        0    87935 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_fox.gif
+-rw-rw-rw-   0        0        0    80542 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
+-rw-rw-rw-   0        0        0    95522 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/go.jpg
+-rw-rw-rw-   0        0        0      274 2023-01-02 06:48:03.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.562624 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu_image/
+-rw-rw-rw-   0        0        0   824527 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu_image/menu.png
+-rw-rw-rw-   0        0        0       97 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/pusher.py
+-rw-rw-rw-   0        0        0     3907 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.598527 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/
+-rw-rw-rw-   0        0        0     2280 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/__init__.py
+-rw-rw-rw-   0        0        0      405 2022-12-22 07:28:55.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/bot_loader.py
+-rw-rw-rw-   0        0        0      607 2023-03-01 12:37:46.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/chain_reply.py
+-rw-rw-rw-   0        0        0     5064 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/check_update.py
+-rw-rw-rw-   0        0        0     6447 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/data_pack.py
+-rw-rw-rw-   0        0        0      391 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/date_util.py
+-rw-rw-rw-   0        0        0      746 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/json_cards.py
+-rw-rw-rw-   0        0        0     1264 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/notice_board.py
+-rw-rw-rw-   0        0        0     6565 2023-05-26 14:17:51.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/travel_cycle.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.410031 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/
+-rw-rw-rw-   0        0        0    15639 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2026 2023-05-26 14:24:34.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:24:34.601519 nonebot-plugin-sky-2.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1450 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/setup.py
```

### Comparing `nonebot-plugin-sky-2.2.7/LICENSE` & `nonebot-plugin-sky-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/PKG-INFO` & `nonebot-plugin-sky-2.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.7
+Version: 2.2.8
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -180,21 +180,15 @@
 | `remain -in`/`国际服季节剩余` | 查询国际服最新季节的剩余时间                 |
 | `开启/关闭转发模式`           | 开启和关闭全局消息转发形式                 |
 | `开启/关闭艾特全体`           | 开启和关闭雨林干饭小助手的艾特全体消息           |
 | `安装数据包`               | 安装光遇相关攻略的静态资源数据包              |
 | `菜单v2`                | 查看数据包的文件名注入命令，这些命令都需要遵循命令前缀规则 |
 | `插件公告`               | 获取插件官方公告                         |
 | `check`/`检查更新`       | 检查插件、数据包版本是否有更新             |
-| `光遇绑定+[原id]`        | 仅私聊模式有效，绑定光遇原id用于蜡烛查询    |
-| `查询白蜡`               | 查询普通蜡烛的变化记录                    |
-| `查询季蜡`               | 查询季节蜡烛的变化记录                    |
-| `蜡烛`                  | 查询蜡烛总览                             |
 | `更新插件`               | 检查插件更新进行升级操作                 |
-| `光遇天气预报`/`sky天气`/`光遇天气` | 查询今日天气预报               |
-| `活动日历`               | 查询活动日历                           |
 
 </details>
 
 ### **任何情况下攻略最后的版权信息请勿私自移除**
 
 **【攻略数据来自微博@今天游离翻车了吗 @旧日与春 @光遇陈陈和包包 @张张幼稚园】**
 
@@ -286,14 +280,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.5.22 v2.2.8
+
+新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
+
 2023.4.30 v2.2.7
 
 1.在这个版本之后所有querytools命令均废弃不再生效。
 
 2.更新季节时间（暂时不是很准确
 
 2023.4.25 v2.2.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.7 Summary: nonebot2
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.8 Summary: nonebot2
 plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
 pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -71,21 +71,16 @@
 `å½éæå­£èå©ä½` | æ¥è¯¢å½éæææ°å­£èçå©ä½æ¶é´ | |
 `å¼å¯/å³é­è½¬åæ¨¡å¼` | å¼å¯åå³é­å¨å±æ¶æ¯è½¬åå½¢å¼ | |
 `å¼å¯/å³é­è¾ç¹å¨ä½` |
 å¼å¯åå³é­é¨æå¹²é¥­å°å©æçè¾ç¹å¨ä½æ¶æ¯ | | `å®è£æ°æ®å`
 | å®è£åéç¸å³æ»ç¥çéæèµæºæ°æ®å | | `èåv2` |
 æ¥çæ°æ®åçæä»¶åæ³¨å¥å½ä»¤ï¼è¿äºå½ä»¤é½éè¦éµå¾ªå½ä»¤åç¼è§å
 | | `æä»¶å¬å` | è·åæä»¶å®æ¹å¬å | | `check`/`æ£æ¥æ´æ°` |
-æ£æ¥æä»¶ãæ°æ®åçæ¬æ¯å¦ææ´æ° | | `åéç»å®+[åid]` |
-ä»ç§èæ¨¡å¼ææï¼ç»å®åéåidç¨äºè¡çæ¥è¯¢ | | `æ¥è¯¢ç½è¡`
-| æ¥è¯¢æ®éè¡ççååè®°å½ | | `æ¥è¯¢å­£è¡` |
-æ¥è¯¢å­£èè¡ççååè®°å½ | | `è¡ç` | æ¥è¯¢è¡çæ»è§ | |
-`æ´æ°æä»¶` | æ£æ¥æä»¶æ´æ°è¿è¡åçº§æä½ | | `åéå¤©æ°é¢æ¥`/
-`skyå¤©æ°`/`åéå¤©æ°` | æ¥è¯¢ä»æ¥å¤©æ°é¢æ¥ | | `æ´»å¨æ¥å` |
-æ¥è¯¢æ´»å¨æ¥å |  ###
+æ£æ¥æä»¶ãæ°æ®åçæ¬æ¯å¦ææ´æ° | | `æ´æ°æä»¶` |
+æ£æ¥æä»¶æ´æ°è¿è¡åçº§æä½ |  ###
 **ä»»ä½æåµä¸æ»ç¥æåççæä¿¡æ¯è¯·å¿ç§èªç§»é¤**
 **ãæ»ç¥æ°æ®æ¥èªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå @æ§æ¥ä¸æ¥
 @åéééååå @å¼ å¼ å¹¼ç¨å­ã** ## å¨å±ç¼å­ç®å½ï¼
 Noneboté¡¹ç®æä»¶å¤¹ä¸ç`sky/`ç®å½ ## --å¨å±å½ä»¤ç®¡ç-
 - å¨2.2çæ¬ä¸­å¼å¥äºãå¨å±å½ä»¤ç®¡çãåè½
 ä»¥ä¸æ¯ãå¨å±å½ä»¤æ¨¡æ¿ãçè·¯å¾ï¼ `Sky/cmd_template.txt`
 ä½ å¯ä»¥å¨ãå¨å±å½ä»¤æ¨¡æ¿ãä¸­èªå®ä¹èªå·±çå½ä»¤ï¼æ¯æ¬¡éå¯åé½ä¼èªå¨å¯¼å¥çæï¼ç¤ºä¾ï¼
@@ -111,15 +106,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.30 v2.2.7
+â¨æ´æ°æ¥å¿â¨ 2023.5.22 v2.2.8
+æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
+2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
```

### Comparing `nonebot-plugin-sky-2.2.7/README.md` & `nonebot-plugin-sky-2.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -165,21 +165,15 @@
 | `remain -in`/`国际服季节剩余` | 查询国际服最新季节的剩余时间                 |
 | `开启/关闭转发模式`           | 开启和关闭全局消息转发形式                 |
 | `开启/关闭艾特全体`           | 开启和关闭雨林干饭小助手的艾特全体消息           |
 | `安装数据包`               | 安装光遇相关攻略的静态资源数据包              |
 | `菜单v2`                | 查看数据包的文件名注入命令，这些命令都需要遵循命令前缀规则 |
 | `插件公告`               | 获取插件官方公告                         |
 | `check`/`检查更新`       | 检查插件、数据包版本是否有更新             |
-| `光遇绑定+[原id]`        | 仅私聊模式有效，绑定光遇原id用于蜡烛查询    |
-| `查询白蜡`               | 查询普通蜡烛的变化记录                    |
-| `查询季蜡`               | 查询季节蜡烛的变化记录                    |
-| `蜡烛`                  | 查询蜡烛总览                             |
 | `更新插件`               | 检查插件更新进行升级操作                 |
-| `光遇天气预报`/`sky天气`/`光遇天气` | 查询今日天气预报               |
-| `活动日历`               | 查询活动日历                           |
 
 </details>
 
 ### **任何情况下攻略最后的版权信息请勿私自移除**
 
 **【攻略数据来自微博@今天游离翻车了吗 @旧日与春 @光遇陈陈和包包 @张张幼稚园】**
 
@@ -271,14 +265,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.5.22 v2.2.8
+
+新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
+
 2023.4.30 v2.2.7
 
 1.在这个版本之后所有querytools命令均废弃不再生效。
 
 2.更新季节时间（暂时不是很准确
 
 2023.4.25 v2.2.6
```

#### html2text {}

```diff
@@ -64,21 +64,16 @@
 `å½éæå­£èå©ä½` | æ¥è¯¢å½éæææ°å­£èçå©ä½æ¶é´ | |
 `å¼å¯/å³é­è½¬åæ¨¡å¼` | å¼å¯åå³é­å¨å±æ¶æ¯è½¬åå½¢å¼ | |
 `å¼å¯/å³é­è¾ç¹å¨ä½` |
 å¼å¯åå³é­é¨æå¹²é¥­å°å©æçè¾ç¹å¨ä½æ¶æ¯ | | `å®è£æ°æ®å`
 | å®è£åéç¸å³æ»ç¥çéæèµæºæ°æ®å | | `èåv2` |
 æ¥çæ°æ®åçæä»¶åæ³¨å¥å½ä»¤ï¼è¿äºå½ä»¤é½éè¦éµå¾ªå½ä»¤åç¼è§å
 | | `æä»¶å¬å` | è·åæä»¶å®æ¹å¬å | | `check`/`æ£æ¥æ´æ°` |
-æ£æ¥æä»¶ãæ°æ®åçæ¬æ¯å¦ææ´æ° | | `åéç»å®+[åid]` |
-ä»ç§èæ¨¡å¼ææï¼ç»å®åéåidç¨äºè¡çæ¥è¯¢ | | `æ¥è¯¢ç½è¡`
-| æ¥è¯¢æ®éè¡ççååè®°å½ | | `æ¥è¯¢å­£è¡` |
-æ¥è¯¢å­£èè¡ççååè®°å½ | | `è¡ç` | æ¥è¯¢è¡çæ»è§ | |
-`æ´æ°æä»¶` | æ£æ¥æä»¶æ´æ°è¿è¡åçº§æä½ | | `åéå¤©æ°é¢æ¥`/
-`skyå¤©æ°`/`åéå¤©æ°` | æ¥è¯¢ä»æ¥å¤©æ°é¢æ¥ | | `æ´»å¨æ¥å` |
-æ¥è¯¢æ´»å¨æ¥å |  ###
+æ£æ¥æä»¶ãæ°æ®åçæ¬æ¯å¦ææ´æ° | | `æ´æ°æä»¶` |
+æ£æ¥æä»¶æ´æ°è¿è¡åçº§æä½ |  ###
 **ä»»ä½æåµä¸æ»ç¥æåççæä¿¡æ¯è¯·å¿ç§èªç§»é¤**
 **ãæ»ç¥æ°æ®æ¥èªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå @æ§æ¥ä¸æ¥
 @åéééååå @å¼ å¼ å¹¼ç¨å­ã** ## å¨å±ç¼å­ç®å½ï¼
 Noneboté¡¹ç®æä»¶å¤¹ä¸ç`sky/`ç®å½ ## --å¨å±å½ä»¤ç®¡ç-
 - å¨2.2çæ¬ä¸­å¼å¥äºãå¨å±å½ä»¤ç®¡çãåè½
 ä»¥ä¸æ¯ãå¨å±å½ä»¤æ¨¡æ¿ãçè·¯å¾ï¼ `Sky/cmd_template.txt`
 ä½ å¯ä»¥å¨ãå¨å±å½ä»¤æ¨¡æ¿ãä¸­èªå®ä¹èªå·±çå½ä»¤ï¼æ¯æ¬¡éå¯åé½ä¼èªå¨å¯¼å¥çæï¼ç¤ºä¾ï¼
@@ -104,15 +99,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.30 v2.2.7
+â¨æ´æ°æ¥å¿â¨ 2023.5.22 v2.2.8
+æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
+2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/__init__.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 # @Author  : 子龙君
 # @Email   :  1435608435@qq.com
 # @Github  : neet姬辉夜大人
 # @Software: PyCharm
+import asyncio
+import datetime
+
 from nonebot.adapters.onebot.v11 import NetworkError, ActionFailed, Bot, MessageEvent
 
+from .config.command import *
+from .config.msg_forward import *
 from .sky.daily_tasks.international import SkyDaily as Task_in
 from .sky.daily_tasks.national import SkyDaily as Task_cn
-from .sky.travelling_spirit.international import get_data
-from .tools.menu import get_menu
 from .sky.public_notice import get_sky_notice
+from .sky.query_tools import *
 from .sky.queue import get_state
+from .sky.travelling_spirit.international import get_data
 from .sky.travelling_spirit.national import Travelling as Travelling_cn
+from .tools.menu import get_menu
+from .tools.scheduler import *
+from .utils_ import send_forward_msg
 from .utils_.chain_reply import chain_reply
+from .utils_.check_update import *
 from .utils_.data_pack import *
-from .config.msg_forward import *
-from .tools.scheduler import *
 from .utils_.notice_board import *
-from .utils_.check_update import *
-from .sky.query_tools import *
-from .config.command import *
-from .utils_ import send_forward_msg
-import datetime
+from .config.travelling_cache import *
+from .utils_.travel_cycle import download_img, is_exist, NormalTravel,bot_tips
 
 Menu = on_command("Sky", aliases=get_cmd_alias("sky_menu"))
 DailyCN = on_command("sky -cn", aliases=get_cmd_alias("sky_cn"))
 DailyIN = on_command("sky -in", aliases=get_cmd_alias("sky_in"))
 TravellingCN = on_command("travel -cn", aliases=get_cmd_alias("travel_cn"))
 TravellingIN = on_command("travel -in", aliases=get_cmd_alias("travel_in"))
 RemainCN = on_command("remain -cn", aliases=get_cmd_alias("remain_cn"))
@@ -112,30 +116,60 @@
         await Notice.send(
             message='网络环境较差，调用发送信息接口超时'
         )
 
 
 @TravellingCN.handle()
 async def travel_cn():
+    travel = NormalTravel()
     try:
-        travelling = Travelling_cn()
-        results = await travelling.get_data()
-        await TravellingCN.send(results)
+
+        status = travel.national()
+        tips = bot_tips(status)
+        if status.get('status') is True:
+            # 如果在复刻期间内就判断有无缓存
+            release_time = status.get('current_release').strip(' 12:00:00')
+            cache = is_exist(release_time)
+            if cache:
+                # 如果有复刻缓存则发送缓存
+                await TravellingCN.send(MessageSegment.image(cache))
+            else:
+                # 没有就执行实时调用
+                travelling = Travelling_cn()
+                img_url = await travelling.get_data()
+                if img_url:
+                    # 将收到的url下载下来并发送
+                    await download_img(img_url, release_time)
+                    cache = is_exist(release_time)
+                    await TravellingCN.send(cache)
+                else:
+                    await TravellingCN.send('没有找到国服复刻先祖的数据')
+        else:
+            # 如果不在复刻期间，则发送提示信息
+            await TravellingCN.send(
+                f'当前无复刻先祖信息，下次复刻公布时间：\n{status.get("next_release")}'
+            )
+            await asyncio.sleep(2)
+            await TravellingCN.send(tips)
     except (NetworkError, ActionFailed):
         logger.error('网络环境较差，调用发送信息接口超时')
         await TravellingCN.send(
             message='网络环境较差，调用发送信息接口超时'
         )
 
 
 @TravellingIN.handle()
 async def travel_in():
     try:
+        # 实时调用
         results = await get_data()
-        await TravellingIN.send(results)
+        if results:
+            await TravellingIN.send(results)
+        else:
+            await TravellingIN.send('未获取到国际服复刻先祖信息（维护中）')
     except (NetworkError, ActionFailed):
         logger.error('网络环境较差，调用发送信息接口超时')
         await TravellingIN.send(
             message='网络环境较差，调用发送信息接口超时'
         )
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/command.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/command.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/helper_at_all.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/helper_at_all.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/load_config.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/load_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,22 +25,21 @@
     载入配置项及初始化
     """
     if not Path('Sky').is_dir():
         os.mkdir('Sky')
     cfg_path_ = cfg_path()
     conf = configparser.ConfigParser()
     if not Path(cfg_path_).is_file():
-
         # 这里编写需要初始化的配置项
         conf.add_section('Message')
         conf.add_section('Helper')
         conf.add_section('Travelling')
         conf.set('Message', 'forward', 'True')
         conf.set('Helper', 'at_all', 'False')
-        conf.set('Travelling', 'cache', 'False')
+        conf.set('Travelling', 'cache', 'True')
 
         setting = open(cfg_path_, 'a')
         conf.write(setting)
         setting.close()
         logger.success('配置文件初始化成功')
 
     conf.read(cfg_path_, encoding="utf-8")
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/msg_forward.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/msg_forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     config().write(open(cfg_path_, 'w+'))
     logger.success('消息转发：关闭')
 
 
 Forward = get_is_forward()
 
 On = on_command("forward -on", aliases=get_cmd_alias('forward_on'))
-Off = on_command("forward -off",aliases=get_cmd_alias('forward_off'))
+Off = on_command("forward -off", aliases=get_cmd_alias('forward_off'))
 
 
 @On.handle()
 async def on_handle(matcher: Matcher):
     try:
         global Forward
         on()
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/config/travelling_cache.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/travelling_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,7 +60,13 @@
     except Exception as e:
         logger.error('复刻缓存关闭失败')
         await CacheOff.send('开启失败！原因：%s' % str(e))
 
 
 def is_cache():
     return Cache
+
+
+__all__ = (
+    "cache_on_handle",
+    "cache_off_handle"
+)
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/guild/__init__.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/international.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/daily_tasks/national.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/get_id.png` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/get_id.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/public_notice.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/public_notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/queue.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,10 +21,10 @@
         state = content['text']
         if 'enter' in state:
             return '当前服务器畅通，无需排队'
         elif 'queue' in state:
             wait_time = content['wait_time']
             players = content['pos']
             return '当前排队人数：' + str(players) + \
-                '\n预计排队时间：' + str(wait_time)
+                   '\n预计排队时间：' + str(wait_time)
         else:
             return '服务器又炸啦！'  # 破土豆服务器（
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/international.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/international.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
 import re
+from typing import Union
 
 import httpx
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 from ...utils_ import time_no_more, weibo_image
 
 
@@ -21,57 +21,61 @@
                       '-yT9jqnAOtRB6P_daaLXfdvYkPfvZhXy3bTeuLdBjWXF9;'  # 未登录时的cookie直接写死
         }
         self.copyright_ = ('------------'
                            '\r【数据来源：微博@光遇陈陈】\n'
                            '--本插件仅做数据展示之用，著作权归原文作者所有。'
                            '转载或转发请附文章作者微博--')
 
-    async def get_mblog(self, max_page):
+    async def get_mblog(self, max_page) -> Union[str, dict, None]:
         """获取微博 @光遇陈陈 国际服复刻先祖详情"""
 
         for page in range(1, max_page + 1):
             param = {
                 'page': str(page)
             }
             async with httpx.AsyncClient() as client:
                 response = await client.get(
                     url=self.url,
                     headers=self.headers,
                     params=param
                 )
-                content = json.loads(response.text)
-                overhead = content['data']['list']
-                for log in overhead:
-                    if (
-                            log.get('pic_infos') and
-                            re.findall(
-                                r'#(光遇)*([\u4e00-\u9fa5])*(先祖)*(复刻)+#',
-                                log['text_raw']
-                            ) and
-                            time_no_more(log.get('created_at'), 9, 50) and
-                            re.findall('【*?国.*?际.*?服】*?', log['text_raw'])
-                            # 错了再改
-                    ):
-                        return log
+                overhead = response.json().get('data')
+                if overhead:
+                    overhead = overhead.get('list')
+                    for log in overhead:
+                        if (
+                                log.get('pic_infos') and
+                                re.findall(
+                                    r'#(光遇)*([\u4e00-\u9fa5])*(先祖)*(复刻)+#',
+                                    log['text_raw']
+                                ) and
+                                time_no_more(log.get('created_at'), 9, 50) and
+                                re.findall('【*?国.*?际.*?服】*?', log['text_raw'])
+                                # 错了再改
+                        ):
+                            return log
+                else:
+                    return 'invalid'
         return None
 
 
-async def get_data():
+async def get_data() -> Union[str, None]:
     """获取复刻数据"""
+    results = ''
     travel = Travelling()
-    results = MessageSegment.text('')
-    overhead = await travel.get_mblog(100)
+    overhead = await travel.get_mblog(2)
+    if overhead == 'invalid':
+        return '超过未登录能获取页数的最大值：2'
     if overhead:
         pic_infos = overhead.get('pic_infos')
         if pic_infos:
             for pic in pic_infos:
                 large_url = pic_infos[pic]['largest']['url']
                 path = await weibo_image(large_url, pic)
-                img = MessageSegment.image(path)
-                results += img
+                results = path
         else:
-            results += overhead['text_raw']
+            results = None
     else:
         notice = '没有找到国际服复刻先祖的数据'
         logger.warning(notice)
-        results += MessageSegment.text(notice)
+        results = None
     return results
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/sky/travelling_spirit/national.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/national.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Union
 
 import httpx
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 
 from ...utils_ import time_no_more, weibo_image
 
@@ -14,60 +15,64 @@
         self.url = 'https://weibo.com/ajax/statuses/mymblog?uid=5685423899&feature=0'
         self.longtext = 'https://weibo.com/ajax/statuses/longtext?id='
         self.headers = {
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) '
                           'AppleWebKit/537.36 (KHTML, like Gecko) Chrome'
                           '/62.0.3202.9 Safari/537.36',
             'cookie': 'SUB=_2AkMUd3SHf8NxqwFRmP8Ty2Pna4VwywzEieKiK4VcJRMxHRl'
-                      '-yT9jqnAOtRB6P_daaLXfdvYkPfvZhXy3bTeuLdBjWXF9;'  # 未登录时的cookie直接写死
+                      '-yT9jqnAOtRB6P_daaLXfdvYkPfvZhXy3bTeuLdBjWXF9;'  # 未登录时的cookie直接写死 目前
         }
         self.copyright_ = ('------------'
                            '\r【数据来源：微博@光遇包包1号】\n'
                            '--本插件仅做数据展示之用，著作权归原文作者所有。'
                            '转载或转发请附文章作者微博--')
 
-    async def get_mblog(self, max_page):
+    async def get_mblog(self, max_page) -> Union[str, dict, None]:
         """获取微博 @光遇陈陈和包包 复刻先祖详情"""
 
         for page in range(1, max_page + 1):
             param = {
                 'page': str(page)
             }
             async with httpx.AsyncClient() as client:
                 response = await client.get(
                     url=self.url,
                     headers=self.headers,
                     params=param
                 )
-                content = response.json()
-                overhead = content['data']['list']
-                for log in overhead:
-                    if (
-                            log.get('pic_infos') and
-                            re.findall(
-                                r'#(光遇复刻)*([\u4e00-\u9fa5])*(先祖复刻)*([\u4e00-\u9fa5])*#',
-                                log['text_raw']
-                            ) and time_no_more(log.get('created_at'), 12, 30)
-                            # 为了包包我已经放弃了优雅。
-                    ):
-                        return log
+                overhead = response.json().get('data')
+                if overhead:
+                    overhead = overhead.get('list')
+                    for log in overhead:
+                        if (
+                                log.get('pic_infos') and
+                                re.findall(
+                                    r'#(光遇复刻)*([\u4e00-\u9fa5])*(先祖复刻)*([\u4e00-\u9fa5])*#',
+                                    log['text_raw']
+                                ) and time_no_more(log.get('created_at'), 12, 30)
+                                # 为了包包我已经放弃了优雅。
+                        ):
+                            return log
+                else:
+                    return 'invalid'
         return None
 
-    async def get_data(self):
+    async def get_data(self) -> Union[str, None]:
         """获取复刻数据"""
-        results = MessageSegment.text('')
-        overhead = await self.get_mblog(40)
+        results = ''
+        overhead = await self.get_mblog(2)
+        if overhead == 'invalid':
+            return '超过未登录能获取页数的最大值：2'
         if overhead:
             pic_infos = overhead.get('pic_infos')
             if pic_infos:
                 for pic in pic_infos:
                     large_url = pic_infos[pic]['largest']['url']
                     path = await weibo_image(large_url, pic)
-                    img = MessageSegment.image(path)
-                    results += img
+                    results = path
             else:
-                results += overhead['text_raw']
+                results = None
         else:
             notice = '没有找到国服复刻先祖的数据'
             logger.warning(notice)
-            results += MessageSegment.text(notice)
+            results = None
         return results
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/eating.jpg` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/eating.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_braid.gif` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_braid.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_bun.gif` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_bun.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_cat.gif` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_fox.gif` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_fox.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/helper_image/go.jpg` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/go.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/menu_image/menu.png` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu_image/menu.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/tools/scheduler.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from nonebot_plugin_apscheduler import scheduler
 import os
 import random
 
 from nonebot import require, get_bot, get_driver, on_command, logger
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.internal.matcher import Matcher
 from nonebot.params import CommandArg
 from ..config.command import get_cmd_alias
 from ..config.helper_at_all import *
 
 require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler
 
 Scheduler = on_command("-sc", aliases=get_cmd_alias('helper_name'))
 
 try:
     recv_group_id = get_driver().config.recv_group_id
     logger.success('[雨林干饭小助手] 以下群组已启用：%s' % recv_group_id)
 except Exception as e:
@@ -50,15 +50,18 @@
             await matcher.send('指令关键字错误请重新输入')
     except Exception as error:
         await matcher.send('发生错误：%s' % error)
 
     if is_on:
         # 设定提前五分钟提醒
         # 国服雨林干饭时间：整点的8,10,12,16,18,20
-        @scheduler.scheduled_job("cron", hour="7,9,11,15,17,19", minute="55", id="job_0")
+        @scheduler.scheduled_job("cron",
+                                 hour="7,9,11,15,17,19",
+                                 minute="55",
+                                 id="job_0")
         async def auto_run():
             try:
                 bot = get_bot()
             except Exception as p:
                 logger.error('您还未启动go-cqhttp | %s' % p)
 
             results_ = await go()
@@ -93,11 +96,12 @@
     ]
     text = random.sample(texts, 1)[0]
     abspath_ = os.path.abspath(__file__).strip('scheduler.py')
     path = abspath_ + 'helper_image/'
     image_list = os.listdir(path)
     file = random.sample(image_list, 1)[0]
     if at_all():
-        results = MessageSegment.at("all") + text + MessageSegment.image('file:///' + path + file)
+        results = MessageSegment.at(
+            "all") + text + MessageSegment.image('file:///' + path + file)
     else:
         results = text + MessageSegment.image('file:///' + path + file)
     return results
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/__init__.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/chain_reply.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/chain_reply.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/check_update.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/check_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 from nonebot import on_command, logger
 from ..config.command import get_cmd_alias
 
 logging.captureWarnings(True)  # 去掉建议使用SSL验证的显示
 
-Version = '2.2.7'  # 全局插件版本信息  （不用加v！）
+Version = '2.2.8'  # 全局插件版本信息  （不用加v！）
 
 
 async def get_datapack_ver():
     """
     检查本地数据包版本
     """
     try:
@@ -73,15 +73,15 @@
             res = await client.get(
                 url=url,
                 headers=headers
             )
             bs = BeautifulSoup(res.text, 'lxml')
             latest_ver = bs.find(
                 string=re.compile(
-                    'SkyDataPack-v(\d+.\d+.\d+)')
+                    'SkyDataPack-v(\\d+.\\d+.\\d+)')
             ).strip('SkyDataPack-v')
             return latest_ver
     except Exception as e:
         str(e)
         logger.error('获取数据包更新信息失败')
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/data_pack.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/data_pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
                     total = int(stream.headers['content-length']) / 1024 / 1024
                     with open('SkyDataPack.zip', 'wb') as f:
                         async for data in stream.aiter_bytes(
                                 chunk_size=chunk
                         ):
                             f.write(data)
                             size += len(data) / 1024 / 1024
-                            print('\r' + '[下载进度]: %0.2f MB/%0.2f MB' % (size, total), end='')
+                            print(
+                                '\r' + '[下载进度]: %0.2f MB/%0.2f MB' %
+                                (size, total), end='')
                             await sleep(1)
                     f.close()
                     logger.success('文件下载完成！')
         except (httpx.HTTPError, httpx.NetworkError):
             logger.error('数据包下载失败，请检查网络后重试')
 
 
@@ -103,15 +105,17 @@
     image_list = os.listdir('SkyDataPack/' + cmd_path)
     abs_path = os.path.abspath('SkyDataPack/' + cmd_path)
     for image in image_list:
         results += MessageSegment.image('file:///' + abs_path + "/" + image)
     return results
 
 
-Install = on_command("data_pack -install", aliases=get_cmd_alias('data_pack_install'))
+Install = on_command(
+    "data_pack -install",
+    aliases=get_cmd_alias('data_pack_install'))
 MenuV2 = on_command("menu v2", aliases=get_cmd_alias('menu_v2'))
 Cmd = on_command("-")
 
 
 @Install.handle()
 async def install_handle():
     """
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/json_cards.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/json_cards.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky/utils_/notice_board.py` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/notice_board.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/PKG-INFO` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.7
+Version: 2.2.8
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -180,21 +180,15 @@
 | `remain -in`/`国际服季节剩余` | 查询国际服最新季节的剩余时间                 |
 | `开启/关闭转发模式`           | 开启和关闭全局消息转发形式                 |
 | `开启/关闭艾特全体`           | 开启和关闭雨林干饭小助手的艾特全体消息           |
 | `安装数据包`               | 安装光遇相关攻略的静态资源数据包              |
 | `菜单v2`                | 查看数据包的文件名注入命令，这些命令都需要遵循命令前缀规则 |
 | `插件公告`               | 获取插件官方公告                         |
 | `check`/`检查更新`       | 检查插件、数据包版本是否有更新             |
-| `光遇绑定+[原id]`        | 仅私聊模式有效，绑定光遇原id用于蜡烛查询    |
-| `查询白蜡`               | 查询普通蜡烛的变化记录                    |
-| `查询季蜡`               | 查询季节蜡烛的变化记录                    |
-| `蜡烛`                  | 查询蜡烛总览                             |
 | `更新插件`               | 检查插件更新进行升级操作                 |
-| `光遇天气预报`/`sky天气`/`光遇天气` | 查询今日天气预报               |
-| `活动日历`               | 查询活动日历                           |
 
 </details>
 
 ### **任何情况下攻略最后的版权信息请勿私自移除**
 
 **【攻略数据来自微博@今天游离翻车了吗 @旧日与春 @光遇陈陈和包包 @张张幼稚园】**
 
@@ -286,14 +280,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.5.22 v2.2.8
+
+新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
+
 2023.4.30 v2.2.7
 
 1.在这个版本之后所有querytools命令均废弃不再生效。
 
 2.更新季节时间（暂时不是很准确
 
 2023.4.25 v2.2.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.7 Summary: nonebot2
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.8 Summary: nonebot2
 plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
 pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -71,21 +71,16 @@
 `å½éæå­£èå©ä½` | æ¥è¯¢å½éæææ°å­£èçå©ä½æ¶é´ | |
 `å¼å¯/å³é­è½¬åæ¨¡å¼` | å¼å¯åå³é­å¨å±æ¶æ¯è½¬åå½¢å¼ | |
 `å¼å¯/å³é­è¾ç¹å¨ä½` |
 å¼å¯åå³é­é¨æå¹²é¥­å°å©æçè¾ç¹å¨ä½æ¶æ¯ | | `å®è£æ°æ®å`
 | å®è£åéç¸å³æ»ç¥çéæèµæºæ°æ®å | | `èåv2` |
 æ¥çæ°æ®åçæä»¶åæ³¨å¥å½ä»¤ï¼è¿äºå½ä»¤é½éè¦éµå¾ªå½ä»¤åç¼è§å
 | | `æä»¶å¬å` | è·åæä»¶å®æ¹å¬å | | `check`/`æ£æ¥æ´æ°` |
-æ£æ¥æä»¶ãæ°æ®åçæ¬æ¯å¦ææ´æ° | | `åéç»å®+[åid]` |
-ä»ç§èæ¨¡å¼ææï¼ç»å®åéåidç¨äºè¡çæ¥è¯¢ | | `æ¥è¯¢ç½è¡`
-| æ¥è¯¢æ®éè¡ççååè®°å½ | | `æ¥è¯¢å­£è¡` |
-æ¥è¯¢å­£èè¡ççååè®°å½ | | `è¡ç` | æ¥è¯¢è¡çæ»è§ | |
-`æ´æ°æä»¶` | æ£æ¥æä»¶æ´æ°è¿è¡åçº§æä½ | | `åéå¤©æ°é¢æ¥`/
-`skyå¤©æ°`/`åéå¤©æ°` | æ¥è¯¢ä»æ¥å¤©æ°é¢æ¥ | | `æ´»å¨æ¥å` |
-æ¥è¯¢æ´»å¨æ¥å |  ###
+æ£æ¥æä»¶ãæ°æ®åçæ¬æ¯å¦ææ´æ° | | `æ´æ°æä»¶` |
+æ£æ¥æä»¶æ´æ°è¿è¡åçº§æä½ |  ###
 **ä»»ä½æåµä¸æ»ç¥æåççæä¿¡æ¯è¯·å¿ç§èªç§»é¤**
 **ãæ»ç¥æ°æ®æ¥èªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå @æ§æ¥ä¸æ¥
 @åéééååå @å¼ å¼ å¹¼ç¨å­ã** ## å¨å±ç¼å­ç®å½ï¼
 Noneboté¡¹ç®æä»¶å¤¹ä¸ç`sky/`ç®å½ ## --å¨å±å½ä»¤ç®¡ç-
 - å¨2.2çæ¬ä¸­å¼å¥äºãå¨å±å½ä»¤ç®¡çãåè½
 ä»¥ä¸æ¯ãå¨å±å½ä»¤æ¨¡æ¿ãçè·¯å¾ï¼ `Sky/cmd_template.txt`
 ä½ å¯ä»¥å¨ãå¨å±å½ä»¤æ¨¡æ¿ãä¸­èªå®ä¹èªå·±çå½ä»¤ï¼æ¯æ¬¡éå¯åé½ä¼èªå¨å¯¼å¥çæï¼ç¤ºä¾ï¼
@@ -111,15 +106,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.30 v2.2.7
+â¨æ´æ°æ¥å¿â¨ 2023.5.22 v2.2.8
+æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
+2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
```

### Comparing `nonebot-plugin-sky-2.2.7/nonebot_plugin_sky.egg-info/SOURCES.txt` & `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,8 +42,9 @@
 nonebot_plugin_sky/utils_/__init__.py
 nonebot_plugin_sky/utils_/bot_loader.py
 nonebot_plugin_sky/utils_/chain_reply.py
 nonebot_plugin_sky/utils_/check_update.py
 nonebot_plugin_sky/utils_/data_pack.py
 nonebot_plugin_sky/utils_/date_util.py
 nonebot_plugin_sky/utils_/json_cards.py
-nonebot_plugin_sky/utils_/notice_board.py
+nonebot_plugin_sky/utils_/notice_board.py
+nonebot_plugin_sky/utils_/travel_cycle.py
```

### Comparing `nonebot-plugin-sky-2.2.7/setup.py` & `nonebot-plugin-sky-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Files = get_files(r'nonebot_plugin_sky/tools/helper_image')
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
 setuptools.setup(
     name='nonebot-plugin-sky',
-    version='v2.2.7',
+    version='v2.2.8',
     author='Kaguya233qwq',
     author_email='1435608435@qq.com',
     keywords=["pip", "nonebot2", "nonebot", "sky光遇", "光遇"],
     url='https://github.com/Kaguya233qwq/nonebot_plugin_sky',
     description='''nonebot2 plugin sky''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```


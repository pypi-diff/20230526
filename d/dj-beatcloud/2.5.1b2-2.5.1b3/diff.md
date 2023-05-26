# Comparing `tmp/dj_beatcloud-2.5.1b2.tar.gz` & `tmp/dj_beatcloud-2.5.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.5.1b2.tar", last modified: Thu May 11 17:19:43 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.5.1b3.tar", last modified: Fri May 26 21:12:14 2023, max compression
```

## Comparing `dj_beatcloud-2.5.1b2.tar` & `dj_beatcloud-2.5.1b3.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.334572 dj_beatcloud-2.5.1b2/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b2/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-11 17:19:43.334661 dj_beatcloud-2.5.1b2/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-08 15:53:23.000000 dj_beatcloud-2.5.1b2/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.311206 dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-11 17:19:43.000000 dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1834 2023-05-11 17:19:43.000000 dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-11 17:19:43.000000 dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-11 17:19:43.000000 dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-11 17:19:43.000000 dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-11 17:19:43.000000 dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.313199 dj_beatcloud-2.5.1b2/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b2/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.316970 dj_beatcloud-2.5.1b2/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-06 19:49:39.000000 dj_beatcloud-2.5.1b2/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1241 2023-05-11 17:17:47.000000 dj_beatcloud-2.5.1b2/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13539 2023-05-11 17:13:12.000000 dj_beatcloud-2.5.1b2/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4504 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.317316 dj_beatcloud-2.5.1b2/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.322432 dj_beatcloud-2.5.1b2/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/playlist_combiner.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5338 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/test_shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.324209 dj_beatcloud-2.5.1b2/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.329957 dj_beatcloud-2.5.1b2/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b2/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      733 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-11 17:19:43.334406 dj_beatcloud-2.5.1b2/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b2/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b2/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b2/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-11 17:19:43.335134 dj_beatcloud-2.5.1b2/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2209 2023-05-11 17:16:53.000000 dj_beatcloud-2.5.1b2/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.909093 dj_beatcloud-2.5.1b3/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b3/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.5.1b3/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-26 21:12:14.909175 dj_beatcloud-2.5.1b3/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-08 15:53:23.000000 dj_beatcloud-2.5.1b3/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.895380 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1853 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-26 21:12:14.000000 dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.896520 dj_beatcloud-2.5.1b3/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2495 2023-05-26 20:25:44.000000 dj_beatcloud-2.5.1b3/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b3/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.899197 dj_beatcloud-2.5.1b3/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3691 2023-05-26 18:50:32.000000 dj_beatcloud-2.5.1b3/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1241 2023-05-26 20:51:33.000000 dj_beatcloud-2.5.1b3/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13779 2023-05-26 19:42:30.000000 dj_beatcloud-2.5.1b3/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-26 18:48:19.000000 dj_beatcloud-2.5.1b3/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4790 2023-05-26 20:56:40.000000 dj_beatcloud-2.5.1b3/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.899363 dj_beatcloud-2.5.1b3/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.902944 dj_beatcloud-2.5.1b3/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_combiner.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-06 19:49:46.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5338 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.904993 dj_beatcloud-2.5.1b3/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2288 2023-05-26 19:06:44.000000 dj_beatcloud-2.5.1b3/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.906709 dj_beatcloud-2.5.1b3/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b3/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      669 2023-05-26 20:29:52.000000 dj_beatcloud-2.5.1b3/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-26 21:12:14.908902 dj_beatcloud-2.5.1b3/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-05-26 20:24:46.000000 dj_beatcloud-2.5.1b3/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-05-11 17:06:22.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b3/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-05-26 20:33:17.000000 dj_beatcloud-2.5.1b3/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b3/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-26 21:12:14.909469 dj_beatcloud-2.5.1b3/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2425 2023-05-26 21:11:59.000000 dj_beatcloud-2.5.1b3/setup.py
```

### Comparing `dj_beatcloud-2.5.1b2/LICENSE` & `dj_beatcloud-2.5.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/PKG-INFO` & `dj_beatcloud-2.5.1b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.5.1b2
+Version: 2.5.1b3
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b2 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b3 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b2/README.md` & `dj_beatcloud-2.5.1b3/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.5.1b2
+Version: 2.5.1b3
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b2 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b3 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b2/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.5.1b3/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dj_beatcloud.egg-info/dependency_links.txt
 dj_beatcloud.egg-info/entry_points.txt
 dj_beatcloud.egg-info/requires.txt
 dj_beatcloud.egg-info/top_level.txt
 djtools/__init__.py
 djtools/__main__.py
 djtools/test_main.py
+djtools/version.py
 djtools/configs/__init__.py
 djtools/configs/config.py
 djtools/configs/config.yaml
 djtools/configs/helpers.py
 djtools/configs/logging.conf
 djtools/configs/rekordbox_playlists.yaml
 djtools/configs/spotify_playlists.yaml
```

### Comparing `dj_beatcloud-2.5.1b2/djtools/__init__.py` & `dj_beatcloud-2.5.1b3/djtools/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 )
 from .utils import (
     compare_tracks,
     initialize_logger,
     UTILS_OPERATIONS,
     url_download,
 )
+from .version import __version__
 
 
 __all__ = (
     "build_config",
     "build_playlists",
     "compare_tracks",
     "copy_playlists",
```

### Comparing `dj_beatcloud-2.5.1b2/djtools/__main__.py` & `dj_beatcloud-2.5.1b3/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/configs/config.yaml` & `dj_beatcloud-2.5.1b3/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/configs/helpers.py` & `dj_beatcloud-2.5.1b3/djtools/configs/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 using config.yaml. If command-line arguments are provided, this module
 overrides the corresponding configuration options with these arguments.
 """
 import argparse
 from argparse import ArgumentParser
 import logging
 from pathlib import Path
+import sys
 from typing import Any, Dict, List, Union
 
 import yaml
 
 from djtools.configs.config import BaseConfig
 from djtools.rekordbox.config import RekordboxConfig
 from djtools.spotify.config import SpotifyConfig
 from djtools.sync.config import SyncConfig
 from djtools.utils.config import UtilsConfig
+from djtools.version import __version__
 
 
 logger = logging.getLogger(__name__)
 
 pkg_cfg = {
     "configs": BaseConfig,
     "rekordbox": RekordboxConfig,
@@ -304,23 +306,32 @@
         "--verbosity",
         "-v",
         action="count",
         default=0,
         help="Logging verbosity",
     )
     parser.add_argument(
+        "--version",
+        action="store_true",
+        help="Display package version",
+    )
+    parser.add_argument(
         "--xml-path",
         type=convert_to_paths,
         help='Path to your exported Rekordbox XML database',
     )
     args = parser.parse_args()
 
     if args.log_level:
         logger.setLevel(args.log_level)
 
+    if args.version:
+        print(__version__)
+        sys.exit()
+
     if args.link_configs:
         args.link_configs = Path(args.link_configs)
         if args.link_configs.exists():
             msg = (
                 f"{args.link_configs} must be a directory that does not "
                 "already exist"
             )
```

### Comparing `dj_beatcloud-2.5.1b2/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.5.1b3/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/configs/test_config.py` & `dj_beatcloud-2.5.1b3/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/configs/test_helpers.py` & `dj_beatcloud-2.5.1b3/djtools/configs/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Testing for the helpers module."""
-from argparse import Namespace
 from pathlib import Path
 import re
 from typing import List
 from unittest import mock
 
 import pytest
 
@@ -13,66 +12,66 @@
     build_config,
     convert_to_paths,
     filter_dict,
     parse_yaml,
     pkg_cfg,
 )
 from djtools.utils.helpers import MockOpen
+from djtools.version import __version__
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
-def test_arg_parse_links_configs(mock_parse_args, tmpdir):
+def test_arg_parse_links_configs(mock_parse_args, tmpdir, namespace):
     """Test for the arg_parse function."""
     config_path = Path(tmpdir) / "test_dir"
-    mock_parse_args.return_value = Namespace(
-        link_configs=config_path, log_level="INFO"
-    )
+    namespace.link_configs = config_path
+    mock_parse_args.return_value = namespace
     arg_parse()
     assert config_path.is_symlink()
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
-def test_arg_parse_links_configs_dir_does_exist(mock_parse_args, tmpdir):
+def test_arg_parse_links_configs_dir_does_exist(
+    mock_parse_args, tmpdir, namespace
+):
     """Test for the arg_parse function."""
-    link_path = Path(tmpdir) / "new_dir" / "link_dir"
-    mock_parse_args.return_value = Namespace(
-        link_configs=link_path, log_level="INFO"
-    )
+    config_path = Path(tmpdir) / "new_dir" / "link_dir"
+    namespace.link_configs = config_path
+    mock_parse_args.return_value = namespace
     arg_parse()
-    assert link_path.exists()
-    assert link_path.is_symlink()
+    assert config_path.exists()
+    assert config_path.is_symlink()
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
-def test_arg_parse_links_configs_dir_does_not_exist(mock_parse_args, tmpdir):
+def test_arg_parse_links_configs_dir_does_not_exist(
+    mock_parse_args, tmpdir, namespace
+):
     """Test for the arg_parse function."""
-    link_path = str(tmpdir)
-    mock_parse_args.return_value = Namespace(
-        link_configs=link_path, log_level="INFO"
-    )
+    config_path = str(tmpdir)
+    namespace.link_configs = config_path
+    mock_parse_args.return_value = namespace
     with pytest.raises(
         ValueError,
         # NOTE(a-rich): WindowsPath needs to be escaped for `\` characters to
         # appear in the `match` argument.
         match=re.escape(
-            f'{link_path} must be a directory that does not already exist'
+            f'{config_path} must be a directory that does not already exist'
         ),
     ):
         arg_parse()
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
-def test_build_config():
+def test_build_config(namespace):
     """Test for the build_config function."""
     with mock.patch(
         "argparse.ArgumentParser.parse_args",
     ) as mock_parse_args:
-        mock_parse_args.return_value = Namespace(
-            link_configs="", log_level="INFO"
-        )
+        mock_parse_args.return_value = namespace
         config = build_config()
     assert isinstance(config, BaseConfig)
 
 
 @mock.patch("builtins.open", MockOpen(
     files=["config.yaml"],
     content="yaml_valid: {false",
@@ -83,27 +82,35 @@
     with pytest.raises(RuntimeError):
         build_config()
     assert 'Error reading "config.yaml"' in caplog.records[0].message
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
 @mock.patch("argparse.ArgumentParser.parse_args")
-def test_build_config_no_config_yaml(mock_parse_args):
+def test_build_config_no_config_yaml(mock_parse_args, namespace):
     """Test for the build_config function."""
-    mock_parse_args.return_value = Namespace(
-        link_configs="", log_level="INFO"
-    )
+    mock_parse_args.return_value = namespace
     config_dir = Path(__file__).parent.parent / "configs"
     config_file = config_dir / "config.yaml"
     with mock.patch.object(Path, "exists", return_value=False):
         assert not config_file.exists()
         build_config()
     assert config_file.exists()
 
 
+@mock.patch("argparse.ArgumentParser.parse_args")
+def test_build_config_version(mock_parse_args, namespace, capsys):
+    """Test for the build_config function."""
+    namespace.version = True
+    mock_parse_args.return_value = namespace
+    with pytest.raises(SystemExit):
+        build_config()
+    assert capsys.readouterr().out == f"{__version__}\n"
+
+
 @pytest.mark.parametrize("paths", ["path", ["path1", "path2"]])
 def test_convert_to_paths(paths):
     """Test for the convert_to_paths function."""
     paths = convert_to_paths(paths)
     if isinstance(paths, List):
         for path in paths:
             assert isinstance(path, Path)
```

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/config.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/playlist_combiner.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/playlist_combiner.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/shuffle_playlists.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/test_shuffle_playlists.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.5.1b3/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/spotify/__init__.py` & `dj_beatcloud-2.5.1b3/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/spotify/config.py` & `dj_beatcloud-2.5.1b3/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/spotify/helpers.py` & `dj_beatcloud-2.5.1b3/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.5.1b3/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/spotify/test_config.py` & `dj_beatcloud-2.5.1b3/djtools/spotify/test_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 
 from djtools.spotify.config import SpotifyConfig
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
 def test_spotifyconfig():
     """Test for the SpotifyConfig class."""
-    SpotifyConfig()
+    cfg = {
+        "AUTO_PLAYLIST_SUBREDDITS": [
+            {"name": "jungle"},
+            {"name": "darkpsy"},
+        ],
+    }
+    SpotifyConfig(**cfg)
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 def test_baseconfig_invalid_spotify_credentials(mock_spotify):
     """Test for the SpotifyConfig class."""
     mock_spotify.return_value.current_user.side_effect = Exception()
     cfg = {
```

### Comparing `dj_beatcloud-2.5.1b2/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.5.1b3/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.5.1b3/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/sync/__init__.py` & `dj_beatcloud-2.5.1b3/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/sync/config.py` & `dj_beatcloud-2.5.1b3/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/sync/helpers.py` & `dj_beatcloud-2.5.1b3/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/sync/sync_operations.py` & `dj_beatcloud-2.5.1b3/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/sync/test_config.py` & `dj_beatcloud-2.5.1b3/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/sync/test_helpers.py` & `dj_beatcloud-2.5.1b3/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.5.1b3/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/__init__.py` & `dj_beatcloud-2.5.1b3/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/check_tracks.py` & `dj_beatcloud-2.5.1b3/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/config.py` & `dj_beatcloud-2.5.1b3/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/helpers.py` & `dj_beatcloud-2.5.1b3/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.5.1b3/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/test_helpers.py` & `dj_beatcloud-2.5.1b3/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/test_url_download.py` & `dj_beatcloud-2.5.1b3/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/djtools/utils/url_download.py` & `dj_beatcloud-2.5.1b3/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b2/setup.py` & `dj_beatcloud-2.5.1b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Setup 'djtools' package.
 """
+from pathlib import Path
 from setuptools import setup
 
 
 with open('README.md', encoding='utf-8') as _file:
     LONG_DESCRIPTION = _file.read()
 
 REQUIREMENTS = [
@@ -42,17 +43,21 @@
     'Topic :: Other/Nonlisted Topic'
 ]
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
+version_path = Path(__file__).parent / "djtools" / "version.py"
+with open(version_path, mode="r", encoding="utf-8") as _file:
+    VERSION = _file.read().split("=")[-1].strip().replace('"', "")
+
 setup(
     name='dj_beatcloud',
-    version='2.5.1-b2',
+    version=VERSION,
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```


# Comparing `tmp/bdfrx-1.0.6.tar.gz` & `tmp/bdfrx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdfrx-1.0.6.tar", last modified: Mon May 15 00:22:33 2023, max compression
+gzip compressed data, was "bdfrx-1.0.7.tar", last modified: Fri May 26 00:41:05 2023, max compression
```

## Comparing `bdfrx-1.0.6.tar` & `bdfrx-1.0.7.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.021522 bdfrx-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-05-15 00:22:06.000000 bdfrx-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-15 00:22:33.021522 bdfrx-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-15 00:22:06.000000 bdfrx-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.013522 bdfrx-1.0.6/bdfrx/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/bdfrx.db
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/default_config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_authenticator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.017522 bdfrx-1.0.6/bdfrx/site_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/catbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/delay_for_reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/download_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/erome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.017522 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/gfycat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/imgur.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/pornhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/redgifs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/self_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/vidble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/vreddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-15 00:22:06.000000 bdfrx-1.0.6/bdfrx/site_downloaders/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.013522 bdfrx-1.0.6/bdfrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-15 00:22:33.000000 bdfrx-1.0.6/bdfrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 00:22:32.000000 bdfrx-1.0.6/bdfrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-15 00:22:06.000000 bdfrx-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 00:22:33.021522 bdfrx-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 00:22:33.021522 bdfrx-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-15 00:22:06.000000 bdfrx-1.0.6/tests/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.432501 bdfrx-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-05-26 00:40:49.000000 bdfrx-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-26 00:41:05.432501 bdfrx-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-05-26 00:40:49.000000 bdfrx-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.420501 bdfrx-1.0.7/bdfrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/bdfrx.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/default_config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_authenticator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.428501 bdfrx-1.0.7/bdfrx/site_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/catbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/delay_for_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/download_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/erome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.428501 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/gfycat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/imgchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/imgur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/pornhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/redgifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/self_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/vidble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/vreddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-26 00:40:49.000000 bdfrx-1.0.7/bdfrx/site_downloaders/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.424501 bdfrx-1.0.7/bdfrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 00:41:05.000000 bdfrx-1.0.7/bdfrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-26 00:40:49.000000 bdfrx-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:41:05.432501 bdfrx-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:05.428501 bdfrx-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-26 00:40:49.000000 bdfrx-1.0.7/tests/test_resource.py
```

### Comparing `bdfrx-1.0.6/LICENSE` & `bdfrx-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/PKG-INFO` & `bdfrx-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bdfrx-1.0.6/README.md` & `bdfrx-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/__main__.py` & `bdfrx-1.0.7/bdfrx/__main__.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/bdfrx.db` & `bdfrx-1.0.7/bdfrx/bdfrx.db`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/completion.py` & `bdfrx-1.0.7/bdfrx/completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/configuration.py` & `bdfrx-1.0.7/bdfrx/configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/connector.py` & `bdfrx-1.0.7/bdfrx/connector.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/download_filter.py` & `bdfrx-1.0.7/bdfrx/download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/downloader.py` & `bdfrx-1.0.7/bdfrx/downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/file_name_formatter.py` & `bdfrx-1.0.7/bdfrx/file_name_formatter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/oauth2.py` & `bdfrx-1.0.7/bdfrx/oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/resource.py` & `bdfrx-1.0.7/bdfrx/resource.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/base_downloader.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/catbox.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/catbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 
 class Catbox(BaseDownloader):
     def __init__(self, post: Submission) -> None:
         super().__init__(post)
 
     def find_resources(self, authenticator: Optional[SiteAuthenticator] = None) -> list[Resource]:
-        links = self.get_links(self.post.url)
+        links = self._get_links(self.post.url)
         if not links:
             raise SiteDownloaderError("Catbox parser could not find any links")
         links = [Resource(self.post, link, Resource.retry_download(link)) for link in links]
         return links
 
     @staticmethod
-    def get_links(url: str) -> set[str]:
+    def _get_links(url: str) -> set[str]:
         content = Catbox.retrieve_url(url)
         soup = bs4.BeautifulSoup(content.text, "html.parser")
         collection_div = soup.find("div", attrs={"class": "imagecontainer"})
         images = collection_div.find_all("a")
         images = [link.get("href") for link in images]
         videos = collection_div.find_all("video")
         videos = [link.get("src") for link in videos]
```

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/delay_for_reddit.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/delay_for_reddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/direct.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/direct.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/download_factory.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/download_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 from bdfrx.site_downloaders.catbox import Catbox
 from bdfrx.site_downloaders.delay_for_reddit import DelayForReddit
 from bdfrx.site_downloaders.direct import Direct
 from bdfrx.site_downloaders.erome import Erome
 from bdfrx.site_downloaders.fallback_downloaders.ytdlp_fallback import YtdlpFallback
 from bdfrx.site_downloaders.gallery import Gallery
 from bdfrx.site_downloaders.gfycat import Gfycat
+from bdfrx.site_downloaders.imgchest import Imgchest
 from bdfrx.site_downloaders.imgur import Imgur
 from bdfrx.site_downloaders.pornhub import PornHub
 from bdfrx.site_downloaders.redgifs import Redgifs
 from bdfrx.site_downloaders.self_post import SelfPost
 from bdfrx.site_downloaders.vidble import Vidble
 from bdfrx.site_downloaders.vreddit import VReddit
 from bdfrx.site_downloaders.youtube import Youtube
 
 
 class DownloadFactory:
     @staticmethod
     def pull_lever(url: str) -> type[BaseDownloader]:  # noqa: PLR0911,PLR0912
+        if not url:
+            raise NotADownloadableLinkError("No url provided by the reddit API")
         sanitised_url = DownloadFactory.sanitise_url(url).lower()
         if re.match(r"(i\.|m\.|o\.)?imgur", sanitised_url):
             return Imgur
         if re.match(r"(i\.|thumbs\d{1,2}\.|v\d\.)?(redgifs|gifdeliverynetwork)", sanitised_url):
             return Redgifs
         if re.match(r"(thumbs\.|giant\.)?gfycat\.", sanitised_url):
             return Gfycat
@@ -37,14 +40,16 @@
             return Erome
         if re.match(r"catbox\.moe", sanitised_url):
             return Catbox
         if re.match(r"delayforreddit\.com", sanitised_url):
             return DelayForReddit
         if re.match(r"reddit\.com/gallery/.*", sanitised_url) or re.match(r"patreon\.com.*", sanitised_url):
             return Gallery
+        if re.match(r"imgchest\.com/p/", sanitised_url):
+            return Imgchest
         if re.match(r"reddit\.com/r/", sanitised_url):
             return SelfPost
         if re.match(r"(m\.)?youtu\.?be", sanitised_url):
             return Youtube
         if re.match(r"i\.redd\.it.*", sanitised_url):
             return Direct
         if re.match(r"v\.redd\.it.*", sanitised_url):
```

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/erome.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/erome.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/gallery.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/gallery.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/gfycat.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/gfycat.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/imgur.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/imgur.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/pornhub.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/pornhub.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/redgifs.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/redgifs.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/self_post.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/self_post.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/vidble.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/vidble.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/vreddit.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/vreddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx/site_downloaders/youtube.py` & `bdfrx-1.0.7/bdfrx/site_downloaders/youtube.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/bdfrx.egg-info/PKG-INFO` & `bdfrx-1.0.7/bdfrx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bdfrx-1.0.6/bdfrx.egg-info/SOURCES.txt` & `bdfrx-1.0.7/bdfrx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 bdfrx/site_downloaders/catbox.py
 bdfrx/site_downloaders/delay_for_reddit.py
 bdfrx/site_downloaders/direct.py
 bdfrx/site_downloaders/download_factory.py
 bdfrx/site_downloaders/erome.py
 bdfrx/site_downloaders/gallery.py
 bdfrx/site_downloaders/gfycat.py
+bdfrx/site_downloaders/imgchest.py
 bdfrx/site_downloaders/imgur.py
 bdfrx/site_downloaders/pornhub.py
 bdfrx/site_downloaders/redgifs.py
 bdfrx/site_downloaders/self_post.py
 bdfrx/site_downloaders/vidble.py
 bdfrx/site_downloaders/vreddit.py
 bdfrx/site_downloaders/youtube.py
```

### Comparing `bdfrx-1.0.6/pyproject.toml` & `bdfrx-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_completion.py` & `bdfrx-1.0.7/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_configuration.py` & `bdfrx-1.0.7/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_connector.py` & `bdfrx-1.0.7/tests/test_connector.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_download_filter.py` & `bdfrx-1.0.7/tests/test_download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_downloader.py` & `bdfrx-1.0.7/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_file_name_formatter.py` & `bdfrx-1.0.7/tests/test_file_name_formatter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_oauth2.py` & `bdfrx-1.0.7/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.6/tests/test_resource.py` & `bdfrx-1.0.7/tests/test_resource.py`

 * *Files identical despite different names*


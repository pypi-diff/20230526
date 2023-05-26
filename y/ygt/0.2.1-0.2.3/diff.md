# Comparing `tmp/ygt-0.2.1.tar.gz` & `tmp/ygt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygt-0.2.1.tar", last modified: Thu May 11 22:03:18 2023, max compression
+gzip compressed data, was "ygt-0.2.3.tar", last modified: Fri May 26 02:52:38 2023, max compression
```

## Comparing `ygt-0.2.1.tar` & `ygt-0.2.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 22:03:18.809344 ygt-0.2.1/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.2.1/LICENSE
--rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.2.1/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     4156 2023-05-11 22:03:18.809218 ygt-0.2.1/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     3760 2023-05-10 10:57:33.000000 ygt-0.2.1/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      785 2023-05-11 22:01:56.000000 ygt-0.2.1/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-05-11 22:03:18.809379 ygt-0.2.1/setup.cfg
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.2.1/setup.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 22:03:18.792891 ygt-0.2.1/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 22:03:18.793333 ygt-0.2.1/src/hooks/
--rw-rw-r--   0 peterbaker   (504) staff       (20)      103 2023-05-04 12:22:22.000000 ygt-0.2.1/src/hooks/hook-freetype.py
--rw-r--r--   0 peterbaker   (504) staff       (20)      143 2023-05-07 08:59:05.000000 ygt-0.2.1/src/hooks/hook-xgridfit.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 22:03:18.799616 ygt-0.2.1/src/ygt/
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.2.1/src/ygt/__main__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.2.1/src/ygt/autohint_trash.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3721 2023-05-04 10:24:55.000000 ygt-0.2.1/src/ygt/cvGuesser.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     6108 2023-05-06 09:50:32.000000 ygt-0.2.1/src/ygt/fontViewDialog.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 22:03:18.800542 ygt-0.2.1/src/ygt/fonts/
--rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.2.1/src/ygt/fonts/SourceCodePro-Regular.ttf
--rw-r--r--   0 peterbaker   (504) staff       (20)    14419 2023-05-04 19:50:13.000000 ygt-0.2.1/src/ygt/freetypeFont.py
--rw-r--r--   0 peterbaker   (504) staff       (20)      492 2023-05-02 11:52:02.000000 ygt-0.2.1/src/ygt/harfbuzzFont.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 22:03:18.808893 ygt-0.2.1/src/ygt/icons/
--rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/align.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/anchor.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/black_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/cursor-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/cursor-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.2.1/src/ygt/icons/cv.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.2.1/src/ygt/icons/cv_guess.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/gray_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/hand-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/hand-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.2.1/src/ygt/icons/horizontal-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.2.1/src/ygt/icons/horizontal-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/interpolate.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/make_set.png
--rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.2.1/src/ygt/icons/program.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/shift.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.2.1/src/ygt/icons/stem_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.2.1/src/ygt/icons/vertical-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.2.1/src/ygt/icons/vertical-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.2.1/src/ygt/icons/white_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6030 2023-05-03 03:10:09.000000 ygt-0.2.1/src/ygt/macfuncDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    61400 2023-05-11 11:19:08.000000 ygt-0.2.1/src/ygt/makeCVDialog.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)    69578 2023-05-11 22:02:36.000000 ygt-0.2.1/src/ygt/window.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.2.1/src/ygt/ygError.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   118711 2023-05-07 08:05:34.000000 ygt-0.2.1/src/ygt/ygHintEditor.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   141199 2023-05-07 11:23:51.000000 ygt-0.2.1/src/ygt/ygModel.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)     9038 2023-05-11 15:28:45.000000 ygt-0.2.1/src/ygt/ygPreferences.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    24210 2023-05-05 23:01:15.000000 ygt-0.2.1/src/ygt/ygPreview.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    10146 2023-05-11 03:15:43.000000 ygt-0.2.1/src/ygt/ygSchema.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     5652 2023-05-02 21:03:38.000000 ygt-0.2.1/src/ygt/ygStems.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.2.1/src/ygt/ygYAMLEditor.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 22:03:18.800418 ygt-0.2.1/src/ygt.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     4156 2023-05-11 22:03:18.000000 ygt-0.2.1/src/ygt.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1335 2023-05-11 22:03:18.000000 ygt-0.2.1/src/ygt.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-05-11 22:03:18.000000 ygt-0.2.1/src/ygt.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-05-11 22:03:18.000000 ygt-0.2.1/src/ygt.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      158 2023-05-11 22:03:18.000000 ygt-0.2.1/src/ygt.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       27 2023-05-11 22:03:18.000000 ygt-0.2.1/src/ygt.egg-info/top_level.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       54 2023-05-06 10:50:11.000000 ygt-0.2.1/src/ygt.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.092718 ygt-0.2.3/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.2.3/LICENSE
+-rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.2.3/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4547 2023-05-26 02:52:38.092592 ygt-0.2.3/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4151 2023-05-26 02:30:51.000000 ygt-0.2.3/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      822 2023-05-26 02:40:12.000000 ygt-0.2.3/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-05-26 02:52:38.092750 ygt-0.2.3/setup.cfg
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.2.3/setup.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.076929 ygt-0.2.3/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.077472 ygt-0.2.3/src/hooks/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)      103 2023-05-04 12:22:22.000000 ygt-0.2.3/src/hooks/hook-freetype.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)      143 2023-05-07 08:59:05.000000 ygt-0.2.3/src/hooks/hook-xgridfit.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.084083 ygt-0.2.3/src/ygt/
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.2.3/src/ygt/__main__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.2.3/src/ygt/autohint_trash.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3721 2023-05-04 10:24:55.000000 ygt-0.2.3/src/ygt/cvGuesser.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6713 2023-05-25 12:17:29.000000 ygt-0.2.3/src/ygt/fontViewDialog.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.084929 ygt-0.2.3/src/ygt/fonts/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.2.3/src/ygt/fonts/SourceCodePro-Regular.ttf
+-rw-r--r--   0 peterbaker   (504) staff       (20)    14895 2023-05-25 20:13:01.000000 ygt-0.2.3/src/ygt/freetypeFont.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    12079 2023-05-25 20:16:51.000000 ygt-0.2.3/src/ygt/harfbuzzFont.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.092270 ygt-0.2.3/src/ygt/icons/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/align.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/anchor.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/black_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/cursor-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/cursor-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.2.3/src/ygt/icons/cv.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.2.3/src/ygt/icons/cv_guess.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/gray_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/hand-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/hand-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.2.3/src/ygt/icons/horizontal-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.2.3/src/ygt/icons/horizontal-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/interpolate.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/make_set.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.2.3/src/ygt/icons/program.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/shift.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.2.3/src/ygt/icons/stem_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.2.3/src/ygt/icons/vertical-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.2.3/src/ygt/icons/vertical-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.2.3/src/ygt/icons/white_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6030 2023-05-03 03:10:09.000000 ygt-0.2.3/src/ygt/macfuncDialog.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    61448 2023-05-25 00:47:12.000000 ygt-0.2.3/src/ygt/makeCVDialog.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)    73281 2023-05-25 21:05:10.000000 ygt-0.2.3/src/ygt/window.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.2.3/src/ygt/ygError.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   123606 2023-05-24 11:49:08.000000 ygt-0.2.3/src/ygt/ygHintEditor.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   142713 2023-05-23 14:04:27.000000 ygt-0.2.3/src/ygt/ygModel.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)     9038 2023-05-11 15:28:45.000000 ygt-0.2.3/src/ygt/ygPreferences.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26442 2023-05-25 20:13:17.000000 ygt-0.2.3/src/ygt/ygPreview.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10146 2023-05-11 03:15:43.000000 ygt-0.2.3/src/ygt/ygSchema.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     5652 2023-05-02 21:03:38.000000 ygt-0.2.3/src/ygt/ygStems.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13155 2023-05-17 23:57:49.000000 ygt-0.2.3/src/ygt/ygYAMLEditor.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-26 02:52:38.084825 ygt-0.2.3/src/ygt.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4547 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1335 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      184 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       27 2023-05-26 02:52:38.000000 ygt-0.2.3/src/ygt.egg-info/top_level.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       54 2023-05-06 10:50:11.000000 ygt-0.2.3/src/ygt.py
```

### Comparing `ygt-0.2.1/LICENSE` & `ygt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/PKG-INFO` & `ygt-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.2.1
+Version: 0.2.3
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -26,15 +26,33 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-### Verasion 0.2.0
+### Version 0.2.3 (2023-5-25)
+
+Enable OpenType features in string preview panel (via Harfbuzz).
+
+Better lcd/subpixel rendering in string preview panel.
+
+Touched points are tinted pink.
+
+Previews of composite glyphs can now be displayed.
+
+Editing panels are disabled when there are no outlines.
+
+Pyinstaller spec file for Linux added.
+
+### Version 0.2.1 (2023-5-11)
+
+Fixed a bug.
+
+### Version 0.2.0 (2023-5-11)
 
 Enabled merge (Ygt can add its hints to existing hints).
 
 Added files supporting creation of executables.
 
 Changed shortcuts: Ctrl-P = Hint Preview; Ctrl-L: Set Resolution.
```

### Comparing `ygt-0.2.1/README.md` & `ygt-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,33 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-### Verasion 0.2.0
+### Version 0.2.3 (2023-5-25)
+
+Enable OpenType features in string preview panel (via Harfbuzz).
+
+Better lcd/subpixel rendering in string preview panel.
+
+Touched points are tinted pink.
+
+Previews of composite glyphs can now be displayed.
+
+Editing panels are disabled when there are no outlines.
+
+Pyinstaller spec file for Linux added.
+
+### Version 0.2.1 (2023-5-11)
+
+Fixed a bug.
+
+### Version 0.2.0 (2023-5-11)
 
 Enabled merge (Ygt can add its hints to existing hints).
 
 Added files supporting creation of executables.
 
 Changed shortcuts: Ctrl-P = Hint Preview; Ctrl-L: Set Resolution.
```

### Comparing `ygt-0.2.1/pyproject.toml` & `ygt-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ygt"
-version = "0.2.1"
+version = "0.2.3"
 authors = [
     { name="Peter S. Baker", email="b.tarde@mail.com" },
 ]
 description = "A graphical hint editor for TrueType fonts"
 readme = "README.md"
 requires-python = ">=3.10.4"
 classifiers = [
@@ -23,12 +23,13 @@
     "defcon >= 0.10.1",
     "xgridfit >= 3.3.0",
     "setuptools >= 65.3.0",
     "PyYAML >= 6.0",
     "schema >= 0.7.5",
     "fs >= 2.4.15",
     "ufo2ft >= 2.28.0",
-    "numpy",
+    "numpy >= 1.22.4",
+    "uharfbuzz >= 0.25.0",
 ]
 
 [project.scripts]
     ygt = "ygt.window:main"
```

### Comparing `ygt-0.2.1/src/ygt/autohint_trash.py` & `ygt-0.2.3/src/ygt/autohint_trash.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/cvGuesser.py` & `ygt-0.2.3/src/ygt/cvGuesser.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/fontViewDialog.py` & `ygt-0.2.3/src/ygt/fontViewDialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from .freetypeFont import freetypeFont, RENDER_GRAYSCALE
+from .freetypeFont import freetypeFont, RENDER_LCD_1, RENDER_GRAYSCALE
 from fontTools import subset
 from .ygModel import ygFont
 from math import ceil
-from PyQt6.QtCore import Qt, QRect, pyqtSignal
-from PyQt6.QtWidgets import QWidget, QDialog, QGridLayout, QVBoxLayout, QScrollArea, QLabel
-from PyQt6.QtGui import QPainter, QBrush, QPen, QColor, QPalette, QPixmap
-import numpy
+from PyQt6.QtCore import pyqtSignal
+from PyQt6.QtWidgets import QWidget, QGridLayout, QVBoxLayout, QScrollArea, QLabel
+from PyQt6.QtGui import QPainter, QColor, QPalette, QPixmap
 from tempfile import SpooledTemporaryFile
 import copy
 
 
 # A window (not a dialog, despite the filename, retained to avoid complicating
 # the history in the repository) that displays all the non-composite glyphs
 # in the font, with those already hinted highlighted in blue. Click on any
@@ -32,28 +31,30 @@
         self.valid = True
         self.top_window = top_window
         self.setWindowTitle("Font View")
         self.glyph_name_list = []
         for g in glyph_list:
             self.glyph_name_list.append(g[1])
         self.yg_font = yg_font
-        if self.yg_font.source_file.source_type == "yaml":
-            self.face = freetypeFont(filename, size=24, render_mode=RENDER_GRAYSCALE)
-        else:
-            temp_font = copy.deepcopy(self.yg_font.preview_font)
-            tf = SpooledTemporaryFile(max_size=3000000, mode='b')
-            options = subset.Options(glyph_names=True)
-            options.layout_features = []
-            subsetter = subset.Subsetter(options)
-            subsetter.populate(glyphs=self.glyph_name_list)
-            subsetter.subset(temp_font)
-            temp_font.save(tf, 1)
-            tf.seek(0)
-            self.face = freetypeFont(tf, size=24, render_mode=RENDER_GRAYSCALE)
-            tf.close()
+        self.face = self.yg_font.freetype_font
+        self.face.set_size(24)
+        #if self.yg_font.source_file.source_type == "yaml":
+        #    self.face = freetypeFont(filename, size=24, render_mode=RENDER_LCD_1)
+        #else:
+        #    temp_font = copy.deepcopy(self.yg_font.preview_font)
+        #    tf = SpooledTemporaryFile(max_size=3000000, mode='b')
+        #    options = subset.Options(glyph_names=True)
+        #    options.layout_features = []
+        #    subsetter = subset.Subsetter(options)
+        #    subsetter.populate(glyphs=self.glyph_name_list)
+        #    subsetter.subset(temp_font)
+        #    temp_font.save(tf, 1)
+        #    tf.seek(0)
+        #    self.face = freetypeFont(tf, size=24, render_mode=RENDER_LCD_1)
+        #    tf.close()
         if not self.face.valid:
             self.valid = False
             return
         self.glyph_list = glyph_list
         self.glyph_index = {}
 
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
@@ -69,15 +70,14 @@
 
         self.sig_switch_to_glyph.connect(
             self.top_window.glyph_pane.switch_from_font_viewer
         )
 
     def update_cell(self, g):
         gc = self.glyph_index[g]
-        # print("via update_cell " + str(id(gc)))
         gc.make_pixmap()
         gc.update()
 
     def clicked_glyph(self, g: str) -> None:
         self.sig_switch_to_glyph.emit(g)
 
 
@@ -126,46 +126,63 @@
     def make_pixmap(self) -> None:
         """ Make a pixmap for this cell and draw the glyph on it.
             This makes for rapid painting and fast scrolling. If there's
             a change, simply repaint the pixmap and call update() on the
             cell.
         """
         # Test to see if we really need to paint the pixmap.
+        is_composite = self.dialog.yg_font.is_composite(self.glyph)
         has_hints_now = self.dialog.yg_font.has_hints(self.glyph)
         if self.pixmap != None and self.has_hints == has_hints_now:
             return
         else:
             self.has_hints = has_hints_now
 
         if self.pixmap == None:
             self.pixmap = QPixmap(36,36)
 
+        fill_color = None
+        alpha = 0.88
         if self.dialog.dark_theme:
-            if self.has_hints:
-                self.pixmap.fill(QColor(0, 0, 186, 128))
+            if is_composite:
+                # fill_color = QColor(169, 169, 169)
+                fill_color = QColor(64, 42, 9)
+                alpha = 0.96
+            elif self.has_hints:
+                fill_color = QColor(0, 0, 186, 128)
+                alpha = 0.95
             else:
-                self.pixmap.fill(QColor("black"))
+                fill_color = QColor("black")
+                alpha = 0.95
         else:
-            if self.has_hints:
-                self.pixmap.fill(QColor(186, 255, 255, 128))
+            if is_composite:
+                # fill_color = QColor(211, 211, 211)
+                fill_color = QColor(255, 239, 128)
+            elif self.has_hints:
+                fill_color = QColor(186, 255, 255, 128)
             else:
-                self.pixmap.fill(QColor("white"))
+                fill_color = QColor("white")
+        self.pixmap.fill(fill_color)
 
         painter = QPainter(self.pixmap)
 
-        ind = self.dialog.face.name_to_index(self.glyph)
+        # print("fontViewCell: " + self.glyph)
+        ind = self.dialog.face.name_to_index(self.glyph.encode(encoding="utf-8"))
+        self.dialog.face.set_render_mode(RENDER_LCD_1)
         self.dialog.face.set_char(ind)
         baseline = (
             round((36 - self.dialog.face.face_height) / 2) + self.dialog.face.ascender
         )
         xpos = round((36 - self.dialog.face.advance) / 2)
         self.dialog.face.draw_char(
-            painter, xpos, baseline, dark_theme = self.dialog.dark_theme
+            painter,
+            xpos,
+            baseline,
+            dark_theme = self.dialog.dark_theme
         )
 
         painter.end()
 
         self.setPixmap(self.pixmap)
 
     def mousePressEvent(self, event) -> None:
-        # print("Thie is " + str(id(self)))
         self.dialog.clicked_glyph(self.glyph)
```

### Comparing `ygt-0.2.1/src/ygt/fonts/SourceCodePro-Regular.ttf` & `ygt-0.2.3/src/ygt/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/freetypeFont.py` & `ygt-0.2.3/src/ygt/freetypeFont.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# from functools import lru_cache
 from typing import Optional
 import freetype as ft # type: ignore
 import numpy
 import copy
 from tempfile import SpooledTemporaryFile
-from PyQt6.QtGui import QColor, QPen
+from PyQt6.QtGui import QColor, QPen, QImage, QRegion, QBitmap, QPixmap, QPainter
 from PyQt6.QtCore import QRect, QLine
-import uharfbuzz as uhb
-
 
 RENDER_GRAYSCALE = 1
 RENDER_LCD_1 = 2
 RENDER_LCD_2 = 3
 
 
 class ygLetterBox:
@@ -50,48 +47,29 @@
 
     def __init__(
         self,
         font: SpooledTemporaryFile | str,
         size: int = 30,
         render_mode: int = RENDER_LCD_1,
         hinting_on: bool = True,
-        instance: str = None
+        instance: str = None,
+        keep_open: bool = False
     ) -> None:
         self.valid = True
         try:
             if type(font) is SpooledTemporaryFile:
                 font.seek(0)
                 self.face = ft.Face(font)
-                # Experimental code, for harfbuzz.
-                # Here's what we're going to have to do.
-                #    1. Load the whole font into Harfbuzz (shall we do this just once for
-                #       the session?)
-                #    2. Display features, let user choose.
-                #    3. Let hb.shape get us a new string
-                #    4. Get glyph names.
-                #    5. Send list of names to Xgridfit, get back list of indices.
-                #    6. Draw the glyphs.
-                #font.seek(0)
-                #font_data = font.read()
-                #hb_face = uhb.Face(font_data)
-                #hb_font = uhb.Font(hb_face)
-                #buf = uhb.Buffer()
-                #buf.add_str("first flat office")
-                #buf.guess_segment_properties()
-                #features = {"kern": True, "liga": True}
-                #uhb.shape(hb_font, buf, features)
-                #print(uhb._harfbuzz.ot_layout_language_get_feature_tags(hb_face, "GSUB"))
-                # End of harfbuzz experiment.
-                font.close()
-                #import uharfbuzz as hb
-                #test = hb.Blob(self.face)
-                #print(test)
+                if not keep_open:
+                    font.close()
             else:
                 self.face = ft.Face(font)
+
         except Exception as e:
+            print("Error in freetypeFont.__init__:")
             print(e.args)
             print(e)
             self.valid = False
             return
         self.char_size = size * 64
         self.size = 30
         self.ascender = 0
@@ -156,14 +134,17 @@
         self.hinting_on = not self.hinting_on
 
     def set_size(self, i):
         self.size = i
         self.face.set_char_size(i * 64)
         self._get_font_metrics()
 
+    def font_to_pixels(self, val):
+        return round(ft.FT_MulDiv(val, self.face.size.x_scale, 0x10000) / 64)
+
     def _get_font_metrics(self):
         """Populate class variables with basic metrics info for this font
         at the current size.
         """
         self.ascender = round(self.face.size.ascender / 64)
         self.descender = round(self.face.size.descender / 64)
         self.face_height = self.ascender + abs(self.descender)
@@ -195,147 +176,151 @@
         r = {}
         r["width"] = self.glyph_slot.bitmap.width
         r["rows"] = self.glyph_slot.bitmap.rows
         r["pitch"] = self.glyph_slot.bitmap.pitch
         r["bitmap_top"] = self.glyph_slot.bitmap_top
         r["bitmap_left"] = self.glyph_slot.bitmap_left
         r["advance"] = round(self.glyph_slot.advance.x / 64)
-        # r["advance_width"] = round(self.glyph_slot.linearHoriAdvance / 65536)
         return r
 
     def mk_array(self, metrics, render_mode):
         data = []
         rows = metrics["rows"]
         width = metrics["width"]
         pitch = metrics["pitch"]
         for i in range(rows):
             data.extend(self.glyph_slot.bitmap.buffer[i * pitch : i * pitch + width])
         if render_mode == RENDER_GRAYSCALE:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, width)
         else:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, int(width / 3), 3)
 
-    #@lru_cache(maxsize = 2048)
-    #def _get_lcd_color(self, rgb, dark_theme):
-    #    if dark_theme:
-    #        return QColor(rgb[0], rgb[1], rgb[2])
-    #    return QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
-
 
     def _draw_char_lcd(
             self,
             painter,
             x,
             y,
             spacing_mark = False,
             dark_theme = False,
-            is_target = False
+            is_target = False,
+            x_offset = 0,
+            y_offset = 0
         ):
         """Draws a bitmap with subpixel rendering (suitable for an lcd screen)
 
         Params:
 
         painter (QPainter): a Qt tool to draw with
 
         x (int): The left origin of the glyph
 
         y (int): The baseline
 
+        spacing_mark: Make nonspacing mark a spacing char.
+
+        dark_theme: true if letters lighter than background.
+
+        is_target: Whether this glyph matches the one in the big preview.
+
         """
         gdata = self._get_bitmap_metrics()
+
+        # Get the Freetype bitmap into a numpy array and get dimensions.
         Z = self.mk_array(gdata, RENDER_LCD_1)
-        ypos = y - gdata["bitmap_top"]
-        starting_ypos = ypos
-        is_mark = spacing_mark and gdata["advance"] == 0
+        height, width, channel = Z.shape
+        bytesPerLine = channel * width
+
+        have_outline = (not (0 in list(Z.shape)))
+
+        if not dark_theme:
+            Z = (255-Z)
+
+        # Get starting position and metrics. For zero-width marks, we expand the width,
+        # but only if spacing_mark=True.
+        starting_ypos = (y - gdata["bitmap_top"]) - y_offset
+        is_mark = spacing_mark and (gdata["advance"] == 0)
         if is_mark:
             starting_xpos = xpos = x
             xpos += 2
             gdata["advance"] = self.advance = round(gdata["width"] / 3) + 4
         else:
-            starting_xpos = xpos = x + gdata["bitmap_left"]
-        if dark_theme:
-            qp = QPen(QColor("white"))
-            white_color = QColor("black")
-        else:
-            qp = QPen(QColor("black"))
-            white_color = QColor("white")
-        qp.setWidth(1)
-        for row in Z:
-            xpos = starting_xpos
-            for col in row:
-                rgb = []
-                for elem in col:
-                    rgb.append(elem)
-                # The cached function doesn't help at all (timer produces about the same result).
-                # Look for other possibilities for optimization.
-                #qc = self._get_lcd_color(tuple(rgb), dark_theme)
-                if dark_theme:
-                    qc = QColor(rgb[0], rgb[1], rgb[2])
-                else:
-                    qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
-                if qc != white_color:
-                    qp.setColor(qc)
-                    painter.setPen(qp)
-                    painter.drawPoint(xpos, ypos)
-                xpos += 1
-            ypos += 1
+            starting_xpos = xpos = (x + gdata["bitmap_left"]) + x_offset
+
+        # Get QImage from Z; set composition mode; draw the glyph.
+        if have_outline:
+            img = QImage(Z.data, width, height, bytesPerLine, QImage.Format.Format_RGB888)
+            if dark_theme:
+                painter.setCompositionMode(QPainter.CompositionMode.CompositionMode_Screen)
+            else:
+                painter.setCompositionMode(QPainter.CompositionMode.CompositionMode_Multiply)
+            # painter.setRenderHint(QPainter.RenderHint.TextAntialiasing, on=False)
+            painter.drawImage(starting_xpos, starting_ypos, img)
+
+        # Draw a red line under target glyph (the one in the current resolution).
         ending_xpos = starting_xpos + round(gdata["advance"])
         ending_ypos = starting_ypos + gdata["rows"]
         if is_target:
             ul_y = ending_ypos + 4
             qc = QPen(QColor("red"))
             qc.setWidth(2)
             painter.setPen(qc)
             painter.drawLine(QLine(starting_xpos, ul_y, ending_xpos, ul_y))
         if abs(ending_ypos - starting_ypos) <= 5:
             starting_ypos -= 3
             ending_ypos += 3
+
+        # Get a QRect for this glyph (will be a target for clicks).
         self.rect_list.append(
             ygLetterBox(
                 starting_xpos,
                 starting_ypos,
                 ending_xpos,
                 ending_ypos,
                 glyph_index=self.glyph_index,
                 size=self.size,
                 gname=self.index_to_name(self.glyph_index),
             )
         )
         return gdata["advance"]
 
+
     def _draw_char_grayscale(
             self,
             painter,
             x,
             y,
             spacing_mark=False,
             dark_theme = False,
-            is_target = False):
+            is_target = False,
+            x_offset = 0,
+            y_offset = 0,
+        ):
         """Draws a bitmap with grayscale rendering
 
         Params:
 
         painter (QPainter): a Qt tool to draw with
 
         x (int): The left origin of the glyph
 
         y (int): The baseline
 
         """
         gdata = self._get_bitmap_metrics()
         Z = self.mk_array(gdata, RENDER_GRAYSCALE)
-        ypos = y - gdata["bitmap_top"]
+        ypos = (y - gdata["bitmap_top"]) - y_offset
         starting_ypos = ypos
-        is_mark = spacing_mark and gdata["advance"] == 0
+        is_mark = spacing_mark and (gdata["advance"] == 0)
         if is_mark:
             starting_xpos = xpos = x
             xpos += 2
             gdata["advance"] = self.advance = gdata["width"] + 4
         else:
-            starting_xpos = xpos = x + gdata["bitmap_left"]
+            starting_xpos = xpos = (x + gdata["bitmap_left"]) + x_offset
         qp = QPen(QColor("black"))
         qp.setWidth(1)
         for row in Z:
             xpos = starting_xpos
             for col in row:
                 if dark_theme:
                     qp.setColor(self.bw_colors_dark[col])
@@ -366,61 +351,103 @@
                 size=self.size,
                 gname=self.index_to_name(self.glyph_index),
             )
         )
         return gdata["advance"]
 
     def name_to_index(self, gname):
-        s = bytes(gname, "utf8")
+        if type(gname) is str:
+            gname = gname.encode()
         try:
-            return self.face.get_name_index(s)
+            r = self.face.get_name_index(gname)
+            return r
         except Exception as e:
-            print(e)
             return None
+        
+    def names_to_indices(self, l):
+        result = []
+        for n in l:
+            result.append(self.name_to_index(n))
+        return result
 
     def index_to_name(self, index):
         try:
             return self.face.get_glyph_name(index)
         except Exception as e:
+            print("Error in index_to_name:")
             print(e)
             return ".notdef"
+        
+    def indices_to_names(self, index_list):
+        result = []
+        for i in index_list:
+            result.append(self.index_to_name(i))
+        return result
+
 
     def char_to_index(self, char):
         try:
             return self.face.get_char_index(char)
-            # u = ord(char)
-            # return self.face.get_char_index(u)
         except Exception:
             return None
 
     def string_to_indices(self, s):
         indices = []
         for ss in s:
             try:
                 i = self.char_to_index(ss)
                 if i != None:
                     indices.append(i)
             except Exception:
                 pass
         return indices
 
-    def draw_string(self, painter, s, x, y, x_limit = 200, y_increment = 67, dark_theme = False):
+    def draw_string(self,
+                    painter,
+                    s: str | list,
+                    x,
+                    y,
+                    background_image: QImage,
+                    positions: list = [],
+                    x_limit = 200,
+                    y_increment = 67,
+                    dark_theme = False,
+        ):
+
         self.last_glyph_index = None
         self.reset_rect_list()
-        indices = self.string_to_indices(s)
+
+        if type(s) is str:
+            indices = self.string_to_indices(s)
+        else:
+            indices = self.names_to_indices(s)
+
         xpos = x
         ypos = y
-        for i in indices:
+        for count, i in enumerate(indices):
             self.set_char(i)
-            if self.last_glyph_index != None:
-                k = self.face.get_kerning(
-                    self.last_glyph_index, i, ft.FT_KERNING_DEFAULT
-                )
-                xpos += k.x
-            xpos += self.draw_char(painter, xpos, ypos, dark_theme = dark_theme)
+            x_offset = 0
+            y_offset = 0
+            x_advance = -1
+            # If possible, use positions from Harfbuzz. This will include kerning
+            # and correct positioning of diacritics.
+            if len(positions):
+                x_offset = self.font_to_pixels(positions[count].x_offset)
+                y_offset = self.font_to_pixels(positions[count].y_offset)
+                x_advance = self.font_to_pixels(positions[count].x_advance)
+
+            #if self.last_glyph_index != None:
+            #    k = self.face.get_kerning(
+            #        self.last_glyph_index, i, ft.FT_KERNING_DEFAULT
+            #    )
+            #    xpos += k.x
+            adv = self.draw_char(painter, xpos, ypos, dark_theme = dark_theme, x_offset = x_offset, y_offset = y_offset)
+            if x_advance >= 0:
+                adv = x_advance
+            xpos += adv
             if xpos >= x_limit:
                 xpos = x
                 ypos += y_increment
                 self.last_glyph_index = None
             if ypos > y + y_increment:
                 break
             self.last_glyph_index = i
```

### Comparing `ygt-0.2.1/src/ygt/icons/align.png` & `ygt-0.2.3/src/ygt/icons/align.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/anchor.png` & `ygt-0.2.3/src/ygt/icons/anchor.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/black_distance.png` & `ygt-0.2.3/src/ygt/icons/black_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/cursor-icon-off.png` & `ygt-0.2.3/src/ygt/icons/cursor-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/cursor-icon-on.png` & `ygt-0.2.3/src/ygt/icons/cursor-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/cv.png` & `ygt-0.2.3/src/ygt/icons/cv.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/cv_guess.png` & `ygt-0.2.3/src/ygt/icons/cv_guess.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/gray_distance.png` & `ygt-0.2.3/src/ygt/icons/gray_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/hand-icon-off.png` & `ygt-0.2.3/src/ygt/icons/hand-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/hand-icon-on.png` & `ygt-0.2.3/src/ygt/icons/hand-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/horizontal-off.png` & `ygt-0.2.3/src/ygt/icons/horizontal-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/horizontal-on.png` & `ygt-0.2.3/src/ygt/icons/horizontal-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/interpolate.png` & `ygt-0.2.3/src/ygt/icons/interpolate.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/make_set.png` & `ygt-0.2.3/src/ygt/icons/make_set.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/program.png` & `ygt-0.2.3/src/ygt/icons/program.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/shift.png` & `ygt-0.2.3/src/ygt/icons/shift.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/stem_distance.png` & `ygt-0.2.3/src/ygt/icons/stem_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/vertical-off.png` & `ygt-0.2.3/src/ygt/icons/vertical-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/vertical-on.png` & `ygt-0.2.3/src/ygt/icons/vertical-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/icons/white_distance.png` & `ygt-0.2.3/src/ygt/icons/white_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/macfuncDialog.py` & `ygt-0.2.3/src/ygt/macfuncDialog.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/makeCVDialog.py` & `ygt-0.2.3/src/ygt/makeCVDialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,16 +920,15 @@
         self.layout_obj.addWidget(self.cleartype, 3, 1)
         self.layout_obj.addWidget(self.assume_always_y, 4, 1)
         self.layout_obj.addWidget(self.counterclockwise, 1, 2)
         self.layout_obj.addWidget(self.mergemode, 2, 2)
         self.layout_obj.addWidget(self.replaceprep, 3, 2)
         self.functionbase.setFixedWidth(int(self.functionbase.width() /4))
         function_base_layout = QHBoxLayout()
-        # function_base_layout.setAlignment(Qt.AlignmentFlag.AlignLeft)
-        function_base_layout.addWidget(QLabel("function base"))
+        function_base_layout.addWidget(QLabel("Function base"))
         function_base_layout.addWidget(self.functionbase, alignment = Qt.AlignmentFlag.AlignLeft)
         self.layout_obj.addLayout(function_base_layout, 4, 2)
 
         self.setLayout(self.layout_obj)
 
         self.refresh()
 
@@ -1015,14 +1014,18 @@
 
         t = self.defaults.get_default("merge-mode")
         self.mergemode.setChecked(bool(t))
 
         t = self.defaults.get_default("replace-prep")
         self.replaceprep.setChecked(bool(t))
 
+        if not bool(t):
+            self.replaceprep.setEnabled(False)
+            self.functionbase.setEnabled(False)
+
         self.ignore_signal = False
 
 
 class makeCVDialog(QDialog, cvSource):
     """A dialog for creating a cv. This doesn't edit the cvt source
     directly, but instead works on a fragment of cv code to be
     added when the accept() function is called.
```

### Comparing `ygt-0.2.1/src/ygt/window.py` & `ygt-0.2.3/src/ygt/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# ApplicationSpecificRole
 # import inspect
 from typing import Any, TypeVar, Union, Optional
 import sys
 import os
 import copy
 import yaml
 from .ygModel import ygFont, ygGlyph, unicode_cat_names
@@ -49,21 +48,23 @@
     QPixmap,
     QActionGroup,
     QUndoStack,
     QUndoGroup,
     QCloseEvent,
     QAction,
     QFontDatabase,
+    QPainter,
 )
 from fontTools import ttLib, ufoLib # type: ignore
+from .harfbuzzFont import harfbuzzFont
 
 # FileNameVar = TypeVar("FileNameVar", str, tuple[str, Any])
 FileNameVar = Union[str, tuple[str, Any]]
 # FileNameVar = Any
-ygt_version = "0.2.1"
+ygt_version = "0.2.3"
 
 
 class ygPreviewFontMaker(QThread):
     """To be run from a QThread. This is because it can take the better
     part of a second to generate a preview, even on a pretty fast
     machine, and we want to be able to run this on a signal without
     making the GUI balky.
@@ -80,15 +81,21 @@
     sig_preview_ready = pyqtSignal(object)
     sig_preview_error = pyqtSignal()
 
     def __init__(self, font: ttLib.TTFont, source: dict, glyph_list: list) -> None:
         super().__init__()
         self.ft_font = font
         self.source = source
-        self.glyph_list = glyph_list
+        self.glyph_list = []
+        for g in glyph_list:
+            try:
+                self.glyph_list.append(g.decode(encoding="utf-8"))
+            except Exception:
+                self.glyph_list.append(g)
+        # self.glyph_list = glyph_list
         self.error = False
 
     def run(self) -> None:
         try:
             font = copy.deepcopy(self.ft_font)
             tmp_font, glyph_index, failed_glyph_list = compile_list(
                 font, self.source, self.glyph_list
@@ -135,15 +142,14 @@
         if cleartype:
             self.cleartype = "yes"
         self.use_truetype_defaults = use_truetype_defaults
 
     def run(self) -> None:
         try:
             font = copy.deepcopy(self.ft_font)
-            # failed_glyph_list = compile_all(font, self.source, self.output_font)
             err, failed_glyph_list = xgf_run(
                 font = font,
                 yaml = self.source,
                 outputfont = self.output_font,
                 quiet = 3,
                 mergemode = self.mergemode,
                 replaceprep = self.replaceprep,
@@ -171,18 +177,16 @@
         self.undo_group.cleanChanged.connect(self.clean_changed)
         self.error_manager = ygErrorMessages(self)
         if not win_list:
             self.win_list = [self]
         else:
             self.win_list = win_list
         self.filename = ""
-        # self.filename_extension = ""
         self.font_info_editor: Optional[fontInfoWindow] = None
         self.cvt_editor: Optional[editorDialog] = None
-        # self.cvar_editor = None
         self.prep_editor: Optional[editorDialog] = None
         self.function_editor: Optional[editorDialog] = None
         self.macro_editor: Optional[editorDialog] = None
         self.default_editor: Optional[editorDialog] = None
         self.font_viewer: Optional[fontViewWindow] = None
         self.statusbar = self.statusBar()
         self.statusbar_label = QLabel()
@@ -232,14 +236,21 @@
             self.get_preferences(ygPreferences())
         else:
             self.get_preferences(prefs)
 
         self.recents_display: list = []
         self.recents_actions: list = []
         self.instance_actions: list = []
+        self.script_actions: list = []
+        self.script_menu = None
+        self.language_actions: list = []
+        self.language_menu = None
+        self.feature_actions: list = []
+        self.feature_menu = None
+        self.feature_reset_action = None
         self.window_list: list = []
         self.preview_maker: Optional[ygPreviewFontMaker] = None
         self.font_generator: Optional[ygFontGenerator] = None
         self.auto_preview_update = True
 
         #
         # Build menus and toolbar
@@ -324,14 +335,20 @@
 
         #
         # Preview Menu
         #
 
         self.preview_menu = self.menu.addMenu("&Preview")
 
+        self.pv_show_hints_action = self.preview_menu.addAction("Hint preview")
+        self.pv_show_hints_action.setShortcut(QKeySequence("Ctrl+p"))
+        self.pv_show_hints_action.setCheckable(True)
+        self.pv_show_hints_action.setChecked(True)
+        self.pv_show_hints_action.setEnabled(False)
+
         self.save_current_glyph_action = self.preview_menu.addAction("Update Preview")
         self.save_current_glyph_action.setShortcut(QKeySequence("Ctrl+u"))
         self.save_current_glyph_action.setEnabled(False)
 
         self.toggle_auto_preview_action = self.preview_menu.addAction("Auto update")
         self.toggle_auto_preview_action.setCheckable(True)
         self.toggle_auto_preview_action.setChecked(True)
@@ -357,61 +374,66 @@
 
         self.pv_smaller_ten_action = self.preview_menu.addAction("Shrink by Ten")
         self.pv_smaller_ten_action.setShortcut(
             QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_Down) # type: ignore
         )
         self.pv_smaller_ten_action.setEnabled(False)
 
-        self.pv_show_hints_action = self.preview_menu.addAction("Hint preview")
-        self.pv_show_hints_action.setShortcut(QKeySequence("Ctrl+p"))
-        self.pv_show_hints_action.setCheckable(True)
-        self.pv_show_hints_action.setChecked(True)
-        self.pv_show_hints_action.setEnabled(False)
+        self.pv_set_size_action = self.preview_menu.addAction("Set size...")
+        self.pv_set_size_action.setShortcut(QKeySequence("Ctrl+l"))
+        self.pv_set_size_action.setEnabled(False)
+
+        self.preview_menu.addSeparator()
 
         self.pv_show_grid_action = self.preview_menu.addAction("Show grid")
         self.pv_show_grid_action.setCheckable(True)
         self.pv_show_grid_action.setChecked(True)
         self.pv_show_grid_action.setEnabled(False)
 
         self.instance_menu: Optional[QMenu] = None
 
-        self.preview_menu.addSeparator()
-
         self.pv_theme_menu = self.preview_menu.addMenu("Theme")
         self.pv_theme_auto_action = self.pv_theme_menu.addAction("Auto")
-        self.pv_theme_light_action = self.pv_theme_menu.addAction("Light")
-        self.pv_theme_dark_action = self.pv_theme_menu.addAction("Dark")
+        self.pv_theme_light_action = self.pv_theme_menu.addAction("Black on white")
+        self.pv_theme_dark_action = self.pv_theme_menu.addAction("White on black")
         self.theme_action_group = QActionGroup(self.pv_theme_menu)
         self.theme_action_group.addAction(self.pv_theme_auto_action)
         self.theme_action_group.addAction(self.pv_theme_light_action)
         self.theme_action_group.addAction(self.pv_theme_dark_action)
         self.pv_theme_auto_action.setCheckable(True)
         self.pv_theme_light_action.setCheckable(True)
         self.pv_theme_dark_action.setCheckable(True)
         self.pv_theme_auto_action.setChecked(True)
         self.pv_theme_menu.setEnabled(False)
 
-        self.pv_set_size_action = self.preview_menu.addAction("Set resolution...")
-        self.pv_set_size_action.setShortcut(QKeySequence("Ctrl+l"))
-        self.pv_set_size_action.setEnabled(False)
-
         self.pv_render_mode_menu = self.preview_menu.addMenu("Render mode")
         self.pv_mode_1_action = self.pv_render_mode_menu.addAction("Grayscale")
         self.pv_mode_2_action = self.pv_render_mode_menu.addAction("Subpixel (1)")
         self.pv_mode_3_action = self.pv_render_mode_menu.addAction("Subpixel (2)")
         self.render_action_group = QActionGroup(self.pv_render_mode_menu)
         self.render_action_group.addAction(self.pv_mode_1_action)
         self.render_action_group.addAction(self.pv_mode_2_action)
         self.render_action_group.addAction(self.pv_mode_3_action)
         self.pv_mode_1_action.setCheckable(True)
         self.pv_mode_2_action.setCheckable(True)
         self.pv_mode_2_action.setChecked(True)
         self.pv_mode_3_action.setCheckable(True)
         self.pv_render_mode_menu.setEnabled(False)
 
+        self.preview_menu.addSeparator()
+
+        self.script_menu = self.preview_menu.addMenu("Script")
+        self.script_menu.setEnabled(False)
+        self.language_menu = self.preview_menu.addMenu("Language")
+        self.language_menu.setEnabled(False)
+        self.feature_menu = self.preview_menu.addMenu("Features")
+        self.feature_menu.setEnabled(False)
+        self.feature_reset_action = self.preview_menu.addAction("Reset features")
+        self.feature_reset_action.setEnabled(False)
+
         self.preview_menu.aboutToShow.connect(self.preview_menu_about_to_show)
 
         #
         # View Menu
         #
 
         self.view_menu = self.menu.addMenu("&View")
@@ -701,19 +723,27 @@
             pass
         source = self.yg_font.source
         font = self.yg_font.preview_font
         self.preview_glyph_name = self.glyph_pane.yg_glyph_scene.yg_glyph.gname
         preview_text = self.yg_string_preview.panel._text
         self.preview_glyph_name_list = []
         if preview_text != None and len(preview_text) > 0:
-            l = self.yg_font.string_to_name_list(preview_text)
-            # l is the list with reduncancies removed.
+            l_full, p_full = self.yg_font.harfbuzz_font.get_shaped_names(preview_text)
+            l_full_fixed = [c.decode() for c in l_full]
+            # l is the list with redundancies removed (for making a subsetted font)
+            l = list(set(l_full_fixed))
             self.preview_glyph_name_list.extend(l)
+            # Store the full list for later use.
+            self.yg_string_preview.full_glyph_list = l_full_fixed
+            self.yg_string_preview.full_pos_list = p_full
         if not self.preview_glyph_name in self.preview_glyph_name_list:
             self.preview_glyph_name_list.append(self.preview_glyph_name)
+            self.preview_glyph_name_list.extend(
+                list(set(self.yg_font.additional_component_names([self.preview_glyph_name])))
+            )
 
         # What function does this line serve?
         self.yg_string_preview.set_face(self.yg_preview.face)
 
         self.preview_maker = ygPreviewFontMaker(
             font, source, self.preview_glyph_name_list
         )
@@ -739,14 +769,15 @@
     def update_string_preview(self, s) -> None:
         preview_text = self.yg_string_preview.panel._text
         if preview_text != None and len(preview_text) > 0:
             self.yg_string_preview.set_string_preview()
         else:
             self.yg_string_preview.set_size_array()
         self.yg_string_preview.set_face(self.yg_preview.face)
+        self.yg_string_preview.panel.make_pixmap()
         self.yg_string_preview.update()
 
     #
     # Font view window
     #
 
     @pyqtSlot()
@@ -779,14 +810,58 @@
         self.points_as_coords = True
         self.glyph_pane.yg_glyph_scene.set_point_display("coord")
 
     #
     # Prep for menu display
     #
 
+    def setup_script_menu(self):
+        if not self.yg_font:
+            return
+        self.script_menu.clear()
+        self.script_actions.clear()
+        scripts = self.yg_font.harfbuzz_font.sub_scripts
+        for s in scripts:
+            sa = self.script_menu.addAction(s)
+            sa.setCheckable(True)
+            sa.setChecked(s == self.yg_font.harfbuzz_font.current_script_tag)
+            sa.triggered.connect(self.set_script)
+            self.script_actions.append(sa)
+        self.script_menu.setEnabled(len(scripts) > 0)
+
+    def setup_language_menu(self):
+        if not self.yg_font:
+            return
+        self.language_menu.clear()
+        self.language_actions.clear()
+        languages = self.yg_font.harfbuzz_font.sub_languages
+        for l in languages:
+            la = self.language_menu.addAction(l)
+            la.setCheckable(True)
+            la.setChecked(l == self.yg_font.harfbuzz_font.current_language_tag)
+            la.triggered.connect(self.set_language)
+            self.language_actions.append(la)
+        self.language_menu.setEnabled(len(languages) > 0)
+
+    def setup_feature_menu(self):
+        if not self.yg_font:
+            return
+        self.feature_menu.clear()
+        self.feature_actions.clear()
+        features = self.yg_font.harfbuzz_font.sub_features
+        for f in features:
+            fa = self.feature_menu.addAction(harfbuzzFont.expanded_feature_name(f))
+            fa.setCheckable(True)
+            fa.setChecked(f in self.yg_font.harfbuzz_font._active_features)
+            fa.triggered.connect(self.toggle_feature)
+            self.feature_actions.append(fa)
+        self.feature_menu.setEnabled(len(features) > 0)
+        self.feature_reset_action.setEnabled(len(features) > 0)
+            
+
     @pyqtSlot()
     def view_menu_about_to_show(self) -> None:
         if self.points_as_coords:
             self.index_label_action.setEnabled(True)
             self.coord_label_action.setEnabled(False)
         else:
             self.index_label_action.setEnabled(False)
@@ -827,14 +902,18 @@
         if self.yg_preview != None:
             if self.yg_preview.face != None:
                 self.pv_render_mode_menu.setEnabled(True)
             self.pv_theme_menu.setEnabled(True)
             self.pv_show_hints_action.setChecked(self.yg_preview.hinting_on)
             self.pv_show_grid_action.setChecked(self.yg_preview.show_grid)
         self.toggle_auto_preview_action.setChecked(self.auto_preview_update)
+        self.setup_script_menu()
+        self.setup_language_menu()
+        self.setup_feature_menu()
+
 
     @pyqtSlot()
     def edit_menu_about_to_show(self) -> None:
         if self.undo_group.canUndo():
             self.undo_action.setEnabled(True)
             self.undo_action.setText("Undo " + self.undo_group.undoText())
         else:
@@ -886,24 +965,22 @@
         self.stem_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.anchor_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.interpolate_action.triggered.connect(
             self.glyph_pane.make_hint_from_selection
         )
         self.shift_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.align_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
-        # self.make_set_action.triggered.connect(self.glyph_pane.make_set)
         self.make_cv_action.triggered.connect(self.glyph_pane.make_control_value)
         self.make_cv_guess_action.triggered.connect(self.glyph_pane.guess_cv)
         self.vertical_action.toggled.connect(self.glyph_pane.switch_to_y)
         self.horizontal_action.toggled.connect(self.glyph_pane.switch_to_x)
 
     def setup_edit_connections(self) -> None:
         self.edit_cvt_action.triggered.connect(self.edit_cvt)
         self.edit_prep_action.triggered.connect(self.edit_prep)
-        # self.edit_cvar_action.triggered.connect(self.edit_cvar)
         self.edit_functions_action.triggered.connect(self.edit_functions)
         self.edit_macros_action.triggered.connect(self.edit_macros)
         self.edit_defaults_action.triggered.connect(self.edit_defaults)
         self.edit_names_action.triggered.connect(self.edit_names)
         self.edit_properties_action.triggered.connect(self.edit_properties)
         self.to_coords_action.triggered.connect(self.indices_to_coords)
         self.to_indices_action.triggered.connect(self.coords_to_indices)
@@ -920,14 +997,15 @@
         self.pv_mode_2_action.triggered.connect(self.yg_preview.render2)
         self.pv_mode_3_action.triggered.connect(self.yg_preview.render3)
         self.pv_theme_auto_action.triggered.connect(self.yg_preview.set_theme_auto)
         self.pv_theme_light_action.triggered.connect(self.yg_preview.set_theme_light)
         self.pv_theme_dark_action.triggered.connect(self.yg_preview.set_theme_dark)
         self.pv_show_hints_action.triggered.connect(self.yg_preview.toggle_show_hints)
         self.pv_show_grid_action.triggered.connect(self.yg_preview.toggle_grid)
+        self.feature_reset_action.triggered.connect(self.yg_font.harfbuzz_font.reset_features)
 
     def setup_preview_instance_connections(self) -> None:
         if self.yg_font.is_variable_font and self.instance_actions != None:
             self.prev_instance_action.triggered.connect(self.yg_preview.next_instance)
             self.next_instance_action.triggered.connect(self.yg_preview.prev_instance)
             for i in self.instance_actions:
                 i.triggered.connect(self.yg_preview.set_instance)
@@ -995,14 +1073,17 @@
                 instance_names.append(k)
             self.yg_preview.add_instances(self.yg_font.instances)
             self.yg_preview.instance = self.yg_font.default_instance
             self.prev_instance_action.setEnabled(False)
             self.next_instance_action.setEnabled(False)
             self.instance_menu.setEnabled(False)
 
+    def set_up_feature_list(self) -> None:
+        pass
+
     def set_size_and_position(self):
         """Set size and position of the main window."""
         if self.preferences.geometry_valid():
             self.setGeometry(
                 self.preferences["top_window_pos_x"],
                 self.preferences["top_window_pos_y"],
                 self.preferences["top_window_width"],
@@ -1012,21 +1093,19 @@
             qg = self.screen().availableGeometry()
             x = qg.x() + 20
             y = qg.y() + 20
             width = qg.width() * 0.66
             height = qg.height() * 0.75
             self.setGeometry(int(x), int(y), int(width), int(height))
 
-    def add_preview(self, previewer: ygPreview) -> None:
-        self.yg_preview = previewer
+    def add_preview(self) -> None:
+        self.yg_preview = ygPreview(self)
         self.yg_string_preview = ygStringPreview(self.yg_preview, self)
         self.yg_string_preview.set_go_to_signal(self.go_to_glyph)
-        self.preview_scroller = QScrollArea()
-        self.preview_scroller.setWidget(self.yg_preview)
-        ygpc = ygPreviewContainer(self.preview_scroller, self.yg_string_preview)
+        ygpc = ygPreviewContainer(self.yg_preview, self.yg_string_preview)
         self.qs.addWidget(ygpc)
         self.setup_preview_connections()
 
     def add_editor(self, editor: ygYAMLEditor):
         self.source_editor = editor
         self.source_editor.setup_error_signal(self.error_manager.new_message)
         self.qs.addWidget(self.source_editor)
@@ -1128,15 +1207,15 @@
         msg_box.setIcon(QMessageBox.Icon.Question)
         msg_box.setDefaultButton(QMessageBox.StandardButton.Save)
         ret = msg_box.exec()
         if ret == QMessageBox.StandardButton.Cancel:
             return
         mergemode = bool(self.yg_font.defaults.get_default("merge-mode"))
         replaceprep = bool(self.yg_font.defaults.get_default("replace-prep"))
-        initgraphics = bool(self.yg_font.defaults.get_default("init-graphics")) # ***
+        initgraphics = bool(self.yg_font.defaults.get_default("init-graphics"))
         assume_y = bool(self.yg_font.defaults.get_default("assume-always-y"))
         try:
             functionbase = int(self.yg_font.defaults.get_default("function-base"))
         except TypeError:
             functionbase = 0
         self.font_generator = ygFontGenerator(
             font,
@@ -1354,45 +1433,52 @@
                     u.close()
                     yaml_source = yaml.safe_load(y.decode("utf-8"))
                 except Exception:
                     yaml_source = self._initialize_source(filename, fn_base, extension)
 
             self.preferences["current_font"] = filename
 
-            self.yg_preview = ygPreview(self)
-            self.add_preview(self.yg_preview)
-            self.yg_preview.set_up_signal(self.update_string_preview)
-            self.source_editor = ygYAMLEditor(self.preferences)
-            self.add_editor(self.source_editor)
-
             # If opening ttf, we have both yaml_source and ygt_filename
             # If opening ufo, ygt_filename is the same as the font name
             # If opening yaml, we just pass the filename (since font is identified in the file)
             if len(yaml_source) > 0:
                 self.yg_font = ygFont(self, yaml_source, ygt_filename=ygt_filename)
             else:
                 self.yg_font = ygFont(self, filename)
             self.yg_font.setup_error_signal(self.error_manager.new_message)
 
+            self.setup_script_menu()
+            self.setup_language_menu()
+            self.setup_feature_menu()
+
+            self.add_preview()
+            self.yg_preview.set_up_signal(self.update_string_preview)
+
+            self.source_editor = ygYAMLEditor(self.preferences)
+            self.add_editor(self.source_editor)
+
             if (
                 "current_glyph" in self.preferences
                 and self.yg_font.full_name in self.preferences["current_glyph"]
             ):
                 initGlyph = self.preferences["current_glyph"][self.yg_font.full_name]
             else:
                 initGlyph = "A"
             modelGlyph = ygGlyph(self.preferences, self.yg_font, initGlyph)
             modelGlyph.set_yaml_editor(self.source_editor)
             yg_glyph_scene = ygGlyphScene(self.preferences, modelGlyph)
             view = ygGlyphView(self.preferences, yg_glyph_scene, self.yg_font)
             yg_glyph_scene.owner = view
             self.add_glyph_pane(view)
+            w = self.width()
+            self.qs.setSizes([int(w * 0.2961), int(w * 0.1497), int(w * 0.5542)])
             view.centerOn(view.yg_glyph_scene.center_x, view.sceneRect().center().y())
             self.set_window_title()
             self.set_up_instance_list()
+            self.set_up_feature_list()
             self.setup_editor_connections()
             self.setup_preview_instance_connections()
             self.setup_point_label_connections()
             # Should we send a signal for preview update from here?
             self._preview_current_glyph()
         return 0
 
@@ -1418,15 +1504,14 @@
         if selection_profile[0] == 0 and selection_profile[1] == 1:
             # enable anchor button
             self.anchor_action.setEnabled(True)
             self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
-            # self.make_set_action.setEnabled(False)
         elif selection_profile[0] == 1 and selection_profile[1] >= 1:
             if selection_profile[1] == 1:
                 self.stem_action.setEnabled(True)
             else:
                 self.stem_action.setEnabled(False)
             # shift_action and align_action if 1 pt touched and 1 or more untouched.
             if selection_profile[1] >= 1:
@@ -1448,15 +1533,14 @@
         else:
             # "Disable all hint editing buttons
             self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
             self.anchor_action.setEnabled(False)
-            #self.make_set_action.setEnabled(False)
 
     @pyqtSlot()
     def clean_changed(self):
         self.set_window_title()
 
     def set_window_title(self) -> None:
         """And also the status bar"""
@@ -1622,22 +1706,44 @@
     def go_to_glyph(self, g: str) -> None:
         self.glyph_pane.go_to_glyph(g)
 
     @pyqtSlot()
     def show_ppem_dialog(self):
         i, ok = QInputDialog().getInt(
             self,
-            "Set Points per Em",
-            "Points per em:",
-            value = 30,
+            "Set Size",
+            "Pixels per em:",
+            value = 25,
             min = 10,
             max = 400,
         )
         if ok:
             self.yg_preview.set_size(i)
+    
+    @pyqtSlot()
+    def toggle_feature(self):
+        f = harfbuzzFont.tag_only(self.sender().text())
+        if f in self.yg_font.harfbuzz_font.active_features:
+            self.yg_font.harfbuzz_font.deactivate_feature(f)
+        else:
+            self.yg_font.harfbuzz_font.activate_feature(f)
+
+    @pyqtSlot()
+    def set_script(self):
+        tag = self.sender().text()
+        self.yg_font.harfbuzz_font.select_script(tag)
+        for s in self.script_actions:
+            s.setChecked(tag == s.text())
+
+    @pyqtSlot()
+    def set_language(self):
+        tag = self.sender().text()
+        self.yg_font.harfbuzz_font.select_language(tag)
+        for l in self.language_actions:
+            l.setChecked(tag == l.text())
 
     #
     # Program exit
     #
 
     def save_query(self) -> int:
         msg_box = QMessageBox()
@@ -1693,15 +1799,14 @@
             self.set_preferences()
             self.preferences.save_config()
             self.app.quit()
         else:
             exiting = True
             del_list = []
             for w in self.win_list:
-                # if not w.yg_font.clean():
                 if not w.is_file_clean():
                     r = w.save_query()
                     if r in [0, 2]:
                         if r == 2:
                             w.set_all_clean()
                         del_list.append(w)
                     else:
@@ -1757,39 +1862,35 @@
         if event.type() == QEvent.Type.ActivationChange:
             if self.top_window.isActiveWindow():
                 self.top_window.preferences["top_window"] = self.top_window
         return super().eventFilter(source, event)
 
 
 def main():
-    #import uharfbuzz as hb
+    import uharfbuzz
     #from inspect import getfullargspec, signature
-    # print(dir(QMessageBox))
+    print(dir(uharfbuzz._harfbuzz.GlyphPosition))
+    # print(dir(QPainter))
     #print(dir(hb._harfbuzz.Font))
     #print(dir(hb._harfbuzz.Buffer))
 
     app = QApplication([])
 
     if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
-        # font_path = os.path.split(sys._MEIPASS)[0]
-        print(sys._MEIPASS)
         font_path = os.path.join(
             sys._MEIPASS,
             "fonts",
             "SourceCodePro-Regular.ttf"
         )
-        print(font_path)
-        # font_path += "/Resources/fonts/SourceCodePro-Regular.ttf"
     else:
         font_path = os.path.join(
             os.path.dirname(__file__),
             "fonts/SourceCodePro-Regular.ttf"
         )
-        #font_path = os.path.dirname(__file__) + "/fonts/SourceCodePro-Regular.ttf"
-    
+
     font_id = QFontDatabase.addApplicationFont(font_path)
     if font_id == -1:
         print("Can't find font Source Code Pro.")
     top_window = MainWindow(app)
     top_window.get_preferences(open_config(top_window))
     app.setWindowIcon(QIcon(top_window.icon_path + "program.png"))
     top_window.set_size_and_position()
```

### Comparing `ygt-0.2.1/src/ygt/ygError.py` & `ygt-0.2.3/src/ygt/ygError.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/ygHintEditor.py` & `ygt-0.2.3/src/ygt/ygHintEditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, TypeVar, Union, Optional, List, Dict, Callable, overload, Tuple
 import sys
+import numpy
 import uuid
 import copy
 from .macfuncDialog import macfuncDialog
 from .makeCVDialog import makeCVDialog
 from .ygModel import (
     ygFont,
     ygSet,
@@ -36,14 +37,17 @@
     QPen,
     QBrush,
     QColor,
     QPolygonF,
     QAction,
     QPainter,
     QPalette,
+    QImage,
+    QPixmap,
+    QBitmap,
 )
 from PyQt6.QtWidgets import (
     QWidget,
     QApplication,
     QGraphicsScene,
     QGraphicsView,
     QGraphicsItem,
@@ -55,17 +59,20 @@
     QMenu,
     QLabel,
     QDialog,
     QInputDialog,
     QLineEdit,
     QGraphicsProxyWidget,
     QStyleOptionGraphicsItem,
+    QHBoxLayout,
 )
 from fontTools.pens.basePen import BasePen  # type: ignore
+from fontTools.pens.freetypePen import FreeTypePen
 from .ygPreferences import ygPreferences
+# from .freetypeFont import freetypeFont
 
 
 HINT_ARROW_WIDTH = 3
 HINT_ANCHOR_WIDTH = 3
 HINT_LINK_WIDTH = 1
 HINT_ARROWHEAD_WIDTH = 2
 
@@ -95,30 +102,50 @@
 HINT_FUNC_SELECT_DARK = QColor(38, 191, 74, 192)
 
 HINT_INTERPOLATE_COLOR = QColor(255, 127, 0, 128)
 HINT_INTERPOLATE_DARK = QColor(212, 187, 106, 192)
 HINT_INTERPOLATE_SELECT_COLOR = QColor(215, 87, 0, 128)
 HINT_INTERPOLATE_SELECT_DARK = QColor(255, 195, 0, 192)
 
+PTFILL_COLOR = QColor("white")
+PTFILL_DARK = QColor("black")
+PTFILL_SELECT_COLOR = QColor(100, 105, 108, 192)
+PTFILL_SELECT_DARK = QColor(137, 207, 240)
+PTFILL_TOUCH_COLOR = QColor(255, 182, 193, 192)
+PTFILL_TOUCH_DARK = QColor(170, 51, 106, 192)
+PTFILL_TOUCH_SELECT_COLOR = QColor(138, 41, 86, 128)
+PTFILL_TOUCH_SELECT_DARK = QColor(255, 233, 236, 128)
+
 POINT_ONCURVE_OUTLINE = QColor("red")
-POINT_OFFCURVE_FILL = QColor("white")
-POINT_ONCURVE_FILL = QColor("white")
 POINT_OFFCURVE_OUTLINE = QColor(127, 127, 255, 255)
-POINT_OFFCURVE_SELECTED = QColor(127, 127, 255, 255)
-POINT_ONCURVE_SELECTED = QColor(127, 127, 255, 255)
+
+POINT_OFFCURVE_FILL = PTFILL_COLOR
+POINT_ONCURVE_FILL = PTFILL_COLOR
+#POINT_OFFCURVE_SELECTED = QColor(127, 127, 255, 255)
+#POINT_ONCURVE_SELECTED = QColor(127, 127, 255, 255)
+POINT_OFFCURVE_SELECTED = PTFILL_SELECT_COLOR
+POINT_ONCURVE_SELECTED = PTFILL_SELECT_COLOR
+POINT_TOUCHED = PTFILL_TOUCH_COLOR
+POINT_TOUCHED_SELECTED = PTFILL_TOUCH_SELECT_COLOR
+
 PREVIEW_BASE_COLOR = QColor(64, 33, 31, 255)
 POINT_OUTLINE_WIDTH = 1
 POINT_ANCHORED_OUTLINE_WIDTH = 3
 CHAR_OUTLINE_WIDTH = 1
 FUNC_BORDER_WIDTH = 2
 GLYPH_WIDGET_MARGIN = 50
 POINT_ONCURVE_DIA = 8
 POINT_OFFCURVE_DIA = 6
 HINT_BUTTON_DIA = 6
 
+PTFILL_ANCHOR_TOUCH_COLOR = QColor(255, 233, 236, 128)
+PTFILL_ANCHOR_TOUCH_DARK = QColor(170, 51, 106, 192)
+PTFILL_ANCHOR_TOUCH_SELECT_COLOR = QColor(255, 233, 236, 128)
+PTFILL_ANCHOR_TOUCH_SELECT_DARK = QColor(170, 51, 106, 192)
+
 HINT_COLOR = {}
 
 _HINT_COLOR = {
     "anchor": HINT_ANCHOR_COLOR,
     "align": HINT_ALIGN_COLOR,
     "shift": HINT_SHIFT_COLOR,
     "interpolate": HINT_INTERPOLATE_COLOR,
@@ -442,22 +469,26 @@
             elif type(p) is ygParams:
                 self._touch_untouch(self._get_macfunc_targets(p), touch)
             else:
                 pp = ptindex[p.id]
                 if touch:
                     try:
                         ptindex[p.id].touched = True
+                        if ptindex[p.id].changed:
+                            ptindex[p.id]._prepare_graphics()
                         ptindex[p.id].owners.append(self)
                     except Exception:
                         pass
                 else:
                     try:
                         ptindex[p.id].owners.remove(self)
                         if len(ptindex[p.id].owners) == 0:
                             ptindex[p.id].touched = False
+                            if ptindex[p.id].changed:
+                                ptindex[p.id]._prepare_graphics()
                     except Exception as e:
                         #print(str(e.args))
                         #print(str(e))
                         pass
 
     def _touch_all_points(self) -> None:
         """Mark each point affected by this hint as 'touched,' and record
@@ -1259,45 +1290,66 @@
         super().__init__(QRectF(self.glocation, QSizeF(self.diameter, self.diameter)))
         self.setCursor(Qt.CursorShape.CrossCursor)
         self.border_width = 1
         self.index = -1
         self.yg_glyph_scene = yg_glyph_scene
         self.point_number_label: Optional[QLabel] = None
         self.point_number_label_proxy: Optional[QGraphicsProxyWidget] = None
-        self.touched = False
+        self._touched = False
+        self._changed = False
         # These are the ygHintView objects that touch this point. When a hint
         # is removed from ygGlyphScene, remove the reference from this list.
         # If a hint being removed makes this list empty, remove the "touched"
         # flag from this ygPointView.
         self.owners: List[ygHintView] = []
 
+    @property
+    def touched(self) -> bool:
+        return self._touched
+
+    @touched.setter
+    def touched(self, b: bool) -> None:
+        if b != self._touched:
+            self._touched = b
+            self._changed = True
+        else:
+            self._changed = False
+
+    @property
+    def changed(self) -> bool:
+        return self._changed
+
     def attachment_point(self, pt: Any) -> QPointF:
         return self.glocation
 
     def center_point(self) -> QPointF:
         return self.glocation
 
     def _prepare_graphics(self) -> None:
         # For ygPointView
         if self.selected():
-            if self.yg_point.on_curve:
-                brushColor = POINT_ONCURVE_SELECTED
+            if self.touched:
+                brushColor = POINT_TOUCHED_SELECTED
             else:
-                brushColor = POINT_OFFCURVE_SELECTED
+                brushColor = POINT_ONCURVE_SELECTED
         else:
-            brushColor = POINT_ONCURVE_FILL
+            if self.touched:
+                brushColor = POINT_TOUCHED
+            else:
+                brushColor = POINT_ONCURVE_FILL
         if self.yg_point.on_curve:
             penColor = POINT_ONCURVE_OUTLINE
         else:
             penColor = POINT_OFFCURVE_OUTLINE
         pen = QPen(penColor)
         pen.setWidth(self.border_width)
         brush = QBrush(brushColor)
         self.setBrush(brush)
         self.setPen(pen)
+        self._changed = False
 
     #def get_scene(self) -> "ygGlyphScene":
     #    return self.yg_glyph_scene
 
     def has_label(self) -> bool:
         return self.point_number_label != None
 
@@ -1390,15 +1442,15 @@
     sig_name_points = pyqtSignal(object)
 
     def __init__(
             self, preferences: ygPreferences,
             yg_glyph: ygGlyph,
             owner: Optional["ygGlyphView"] = None) -> None:
         """yg_glyph is a ygGlyph object from ygModel."""
-        global HINT_COLOR, SELECTED_HINT_COLOR, POINT_OFFCURVE_FILL, POINT_ONCURVE_FILL, POINT_OFFCURVE_SELECTED, POINT_ONCURVE_SELECTED
+        global HINT_COLOR, SELECTED_HINT_COLOR, POINT_OFFCURVE_FILL, POINT_ONCURVE_FILL, POINT_OFFCURVE_SELECTED, POINT_ONCURVE_SELECTED, POINT_TOUCHED_SELECTED, POINT_TOUCHED
 
         self.preferences = preferences
 
         # Set up glyph info
 
         self.yg_glyph = yg_glyph
         self.owner = owner
@@ -1415,35 +1467,48 @@
 
         # Auto-detect if we have dark mode. We need to know so we can set
         # hint colors (not controlled by the system) to appropriate values.
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
         bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
         self.dark_theme = text_hsv_value > bg_hsv_value
         if self.dark_theme:
+            # These two are dicts
             HINT_COLOR = _HINT_DARK
             SELECTED_HINT_COLOR = _SELECTED_HINT_DARK
-            POINT_OFFCURVE_FILL = QColor("black")
-            POINT_ONCURVE_FILL = QColor("black")
-            POINT_OFFCURVE_SELECTED = QColor(QColor(137, 207, 240))
-            POINT_ONCURVE_SELECTED = QColor(QColor(137, 207, 240))
+            # Fill colors. We don't have to distinguish between fill for on-
+            # and off-curve points
+            POINT_OFFCURVE_FILL = PTFILL_DARK
+            POINT_ONCURVE_FILL = PTFILL_DARK
+            POINT_OFFCURVE_SELECTED = PTFILL_SELECT_DARK
+            POINT_ONCURVE_SELECTED = PTFILL_SELECT_DARK
+            POINT_TOUCHED = PTFILL_TOUCH_DARK
+            POINT_TOUCHED_SELECTED = PTFILL_TOUCH_SELECT_DARK
         else:
             HINT_COLOR = _HINT_COLOR
             SELECTED_HINT_COLOR = _SELECTED_HINT_COLOR
+            POINT_OFFCURVE_FILL = PTFILL_COLOR
+            POINT_ONCURVE_FILL = PTFILL_COLOR
+            POINT_OFFCURVE_SELECTED = PTFILL_SELECT_COLOR
+            POINT_ONCURVE_SELECTED = PTFILL_SELECT_COLOR
+            POINT_TOUCHED = PTFILL_TOUCH_COLOR
+            POINT_TOUCHED_SELECTED = PTFILL_TOUCH_SELECT_COLOR
         if self.preferences.top_window().show_off_curve_points != None:
             self.off_curve_points_showing = self.preferences.top_window().show_off_curve_points
         else:
             self.off_curve_points_showing = self.preferences.show_off_curve_points()
         self.point_numbers_showing = self.preferences.top_window().show_point_numbers
         self.zoom_factor = 1.0
         self.initial_zoom_factor = None
         self.canvas_size = self._calc_canvas_size()
         self.setSceneRect(QRectF(0, 0, self.canvas_size[0], self.canvas_size[1]))
         self.xTranslate = self.canvas_size[2]
         self.yTranslate = self.canvas_size[3]
 
+        # Used when we draw an image instead of rendering the glyph.
+        self.glyph_img = None
 
         # Try to get rid of ref to this scene in the model's ygGlyph class.
         # For now, we've got to ignore the type so as to avoid circular imports.
         self.yg_glyph.yg_glyph_scene = self  # type: ignore
 
         # Make graphical points
 
@@ -1456,14 +1521,15 @@
 
         self.adv = 0
         self.lsb = 0
         self.xTranslate = 0
         self.yTranslate = 0
         self.original_coordinates: Any = None
         self.center_x = self.xTranslate + round(self.adv / 2)
+        self.optimal_size = (0, 0)
 
         # Setup for selecting
 
         # selectionRect is the rubber band. None when no selection is underway.
         self.selectionRect: Optional[SelectionRect] = None
         # Set dragBeginPoint whenever left mouse button is pressed, in case of
         # rubber band selection.
@@ -1471,21 +1537,22 @@
         self.yg_selection = ygSelection(self)
         self.yg_selection.setup_selection_signal(
             self.preferences.top_window().selection_changed
         )
 
         # Add the points and manage their visibility.
 
-        for p in self.yg_point_view_list:
-            p._prepare_graphics()
-            if not p.yg_point.on_curve and not self.off_curve_points_showing:
-                p.hide()
-            if p.isVisible() and self.point_numbers_showing:
-                p.add_label()
-            self.addItem(p)
+        if not self.yg_glyph.is_composite:
+            for p in self.yg_point_view_list:
+                p._prepare_graphics()
+                if not p.yg_point.on_curve and not self.off_curve_points_showing:
+                    p.hide()
+                if p.isVisible() and self.point_numbers_showing:
+                    p.add_label()
+                self.addItem(p)
 
         # Set up connections.
 
         self.sig_new_hint.connect(self.add_hint)
         self.sig_change_cv.connect(self.change_cv)
         self.sig_reverse_hint.connect(self.reverse_hint)
         self.sig_swap_macfunc_points.connect(self.swap_macfunc_points)
@@ -1498,14 +1565,19 @@
         self.sig_round_hint.connect(self.toggle_hint_rounding)
         self.sig_min_dist.connect(self.toggle_min_dist)
         self.sig_name_points.connect(self.name_points)
 
         # Get and display the hints.
 
         self.install_hints(self.yg_glyph.hints)
+        # review the list of points and mark the ones that are touched.
+        if not self.yg_glyph.is_composite:
+            for p in self.yg_point_view_list:
+                if p.touched:
+                    p._prepare_graphics()
 
     #
     # Sizing and zooming
     #
 
     def size_report(self) -> None:
         """For diagnostics."""
@@ -1530,17 +1602,18 @@
         self.preferences.top_window().zoom_factor = self.zoom_factor
         self.scale_glyph()
         self.center_x = self.xTranslate + round(self.adv / 2)
         self.update()
         self.install_hints(self.yg_glyph.hints)
         # This will have the effect of moving point labels to the new positions
         # of the points. Affect only those already visible.
-        for p in self.yg_point_view_list:
-            if p.has_label():
-                p.add_label()
+        if not self.yg_glyph.is_composite:
+            for p in self.yg_point_view_list:
+                if p.has_label():
+                    p.add_label()
 
     def reset_scale(self) -> None:
         c = self.original_coordinates
         ft_font = self.yg_glyph.yg_font.ft_font
         ft_font["glyf"]._setCoordinates(
             self.yg_glyph.gname, c, ft_font["hmtx"].metrics
         )
@@ -1579,18 +1652,45 @@
                 p = self.yg_point_view_list[c_index]
                 p.glocation = self._font2Qt(cc[0], cc[1], p.yg_point.on_curve)
                 p.setPos(p.glocation)
             except IndexError as e:
                 # fontTools coordinate list has phantom points at the end, which we ignore.
                 pass
 
-        glyph_set = {self.yg_glyph.gname: self.yg_glyph.ft_glyph}
-        self.path = QPainterPath()
-        self.qt_pen = QtPen(glyph_set, path=self.path)
-        self.yg_glyph.ft_glyph.draw(self.qt_pen, self.yg_glyph.yg_font.ft_font["glyf"])
+        # glyph_set = {self.yg_glyph.gname: self.yg_glyph.ft_glyph}
+        glyph_set = self.yg_glyph.yg_font.ft_font.getGlyphSet()
+        glyph_table = self.yg_glyph.yg_font.ft_font["glyf"]
+        if self.yg_glyph.is_composite:
+            pass
+            #freetype_pen = FreeTypePen(glyph_set)
+            #print(type(freetype_pen))
+            #print(type(glyph_table))
+            #self.yg_glyph.ft_glyph.draw(freetype_pen, glyph_table)
+            #width, height = self.yg_glyph.dimensions()
+            # arr = freetype_pen.array(width = int((width * 64) * self.zoom_factor), height = int((height * 64) * self.zoom_factor))
+            #arr = freetype_pen.array(width * self.zoom_factor, height * self.zoom_factor)
+            #print("arr.shape: " + str(arr.shape))
+            #width, height = arr.shape
+            #self.glyph_img = QImage(arr, int(width * self.zoom_factor), int(height * self.zoom_factor), QImage.Format.Format_Mono)
+            #
+            #from matplotlib import pyplot as plt
+            #plt.imshow(arr)
+            #plt.show()
+            #
+            #qd = QDialog(self.preferences.top_window())
+            #layout = QHBoxLayout()
+            #l = QLabel()
+            #layout.addWidget(l)
+            #pm = QPixmap.fromImage(self.glyph_img)
+            #l.setPixmap(pm)
+            #qd.exec()
+        else:
+            self.path = QPainterPath()
+            self.qt_pen = QtPen(glyph_set, path=self.path)
+            self.yg_glyph.ft_glyph.draw(self.qt_pen, glyph_table)
 
     def _calc_canvas_size(self) -> Tuple[int, int, int, int]:
         """This calculates a canvas that will do for the entire font. The result
         can be awkward (see the absurd situation in Junicode, which has an
         extremely wide canvas because of one glyph, threeemdash (U+2E3B)).
         """
         f = self.yg_glyph.yg_font.ft_font
@@ -1648,14 +1748,15 @@
         global HINT_COLOR, SELECTED_HINT_COLOR
 
         if not self.initial_zoom_factor:
             visible_x = rect.width()
             visible_y = rect.height()
             optimal_x = round(visible_x * 0.8)
             optimal_y = round(visible_y * 0.8)
+            self.optimal_size = (optimal_x, optimal_y)
             width, height = self.yg_glyph.dimensions()
             if width != 0:
                 x_ratio = optimal_x / width
             else:
                 x_ratio = 1
             if height != 0:
                 y_ratio = optimal_y / height
@@ -1664,40 +1765,49 @@
             # Limit the initial zoom factor to max of 2.0. This prevents little glyphs
             # like period from becoming disconcertingly large.
             self.initial_zoom_factor = min(2.0, min(x_ratio, y_ratio))
             self.set_zoom_factor(self.initial_zoom_factor)
             if self.owner:
                 self.owner.centerOn(self.center_x, self.mid_point_y())
 
-
-        painter.scale(1.0, -1.0)
-        painter.translate(QPointF(self.xTranslate, self.yTranslate * -1))
+        # this_ft_glyph = self.yg_glyph.ft_glyph
+        if self.yg_glyph.is_composite:
+            pass
+        else:
+            painter.scale(1.0, -1.0)
+            painter.translate(QPointF(self.xTranslate, self.yTranslate * -1))
 
         pen = painter.pen()
 
-        if self.preferences["show_metrics"]:
-            pen.setWidth(1)
-            if self.dark_theme:
-                pen.setColor(QColor(220, 220, 220, 75))
-                HINT_COLOR = _HINT_DARK
-                SELECTED_HINT_COLOR = _SELECTED_HINT_DARK
-            else:
-                pen.setColor(QColor(50, 50, 50, 50))
-                HINT_COLOR = _HINT_COLOR
-                SELECTED_HINT_COLOR = _SELECTED_HINT_COLOR
+        if self.yg_glyph.is_composite:
+            pass
+            # For now, anyway, we're not displaying anything for composites in the
+            # main editing window. This should change, but don't get elaborate: this
+            # display is of much less interest than (e.g.) the preview.
+        else:
+            if self.preferences["show_metrics"]:
+                pen.setWidth(1)
+                if self.dark_theme:
+                    pen.setColor(QColor(220, 220, 220, 75))
+                    HINT_COLOR = _HINT_DARK
+                    SELECTED_HINT_COLOR = _SELECTED_HINT_DARK
+                else:
+                    pen.setColor(QColor(50, 50, 50, 50))
+                    HINT_COLOR = _HINT_COLOR
+                    SELECTED_HINT_COLOR = _SELECTED_HINT_COLOR
+                painter.setPen(pen)
+                painter.drawLine(QLine(-abs(self.xTranslate), 0, round(self.width()), 0))
+                ya = -abs(self.yTranslate)
+                painter.drawLine(QLine(0, ya, 0, round(self.height())))
+                painter.drawLine(QLine(self.adv, ya, self.adv, round(self.height())))
+
+            pen.setWidth(CHAR_OUTLINE_WIDTH)
+            pen.setColor(QColor("gray"))
             painter.setPen(pen)
-            painter.drawLine(QLine(-abs(self.xTranslate), 0, round(self.width()), 0))
-            ya = -abs(self.yTranslate)
-            painter.drawLine(QLine(0, ya, 0, round(self.height())))
-            painter.drawLine(QLine(self.adv, ya, self.adv, round(self.height())))
-
-        pen.setWidth(CHAR_OUTLINE_WIDTH)
-        pen.setColor(QColor("gray"))
-        painter.setPen(pen)
-        painter.drawPath(self.path)
+            painter.drawPath(self.path)
 
     #
     # Editing slots
     #
 
     @pyqtSlot()
     def guess_cv(self) -> None:
@@ -1727,15 +1837,15 @@
                 cv_name = self.yg_glyph.yg_font.cvt.get_closest_cv_name(
                     cv_list, selected_hint
                 )
                 selected_hint.set_cv(cv_name)
             except Exception:
                 pass
 
-    def guess_cv_for_hint(self, hint: ygHint) -> None:
+    def guess_cv_for_new_hint(self, hint: ygHint) -> None:
         """Like guess_cv(), but this is called as part of the process of constructing
         a hint, and therefore should not trigger a signal.
         """
         if hint != None:
             htn = self.get_hint_type_num(hint.hint_type)
             cv_type = "pos"
             if htn == 3:
@@ -1760,28 +1870,31 @@
         ed_dialog = macfuncDialog(hint)
         r = ed_dialog.exec()
         if r == QDialog.DialogCode.Accepted:
             hint.yg_hint.macfunc_other_args = ed_dialog.result_dict
 
     @pyqtSlot()
     def toggle_off_curve_visibility(self) -> None:
+        if self.yg_glyph.is_composite:
+            return
         self.off_curve_points_showing = not self.off_curve_points_showing
         self.preferences.top_window().show_off_curve_points = (
             self.off_curve_points_showing
         )
-        for p in self.yg_point_view_list:
-            if not p.yg_point.on_curve:
-                if self.off_curve_points_showing:
-                    p.show()
-                    if self.point_numbers_showing:
-                        p.add_label()
-                else:
-                    p.hide()
-                    if self.point_numbers_showing:
-                        p.del_label()
+        if not self.yg_glyph.is_composite:
+            for p in self.yg_point_view_list:
+                if not p.yg_point.on_curve:
+                    if self.off_curve_points_showing:
+                        p.show()
+                        if self.point_numbers_showing:
+                            p.add_label()
+                    else:
+                        p.hide()
+                        if self.point_numbers_showing:
+                            p.del_label()
 
     def make_control_value(self) -> None:
         """ With one or two points selected, launch a dialog for making a pos or dist CV.
         """
         sel = self.selected_objects(True)
         if len(sel) == 0:
             return
@@ -1815,15 +1928,17 @@
                     else "index"
                 )()
             )
 
     def untouch_all(self):
         for p in self.yg_point_view_list:
             p.touched = False
-            p.owners.clear()
+            if p.changed:
+                p.owners.clear()
+                p._prepare_graphics()
 
     @pyqtSlot(object)
     def change_hint_color(self, _params: dict) -> None:
         _params["hint"].yg_hint.change_hint_color(_params["color"])
 
     @pyqtSlot(object)
     def toggle_hint_rounding(self, hint: ygHintView) -> None:
@@ -1831,14 +1946,16 @@
 
     @pyqtSlot(object)
     def toggle_min_dist(self, hint: ygHintView) -> None:
         self._model_hint(hint).toggle_min_dist()
 
     @pyqtSlot()
     def toggle_point_numbers(self) -> None:
+        if self.yg_glyph.is_composite:
+            return
         self.point_numbers_showing = not self.point_numbers_showing
         self.preferences.top_window().show_point_numbers = self.point_numbers_showing
         for p in self.yg_point_view_list:
             if self.point_numbers_showing:
                 if p.isVisible():
                     p.add_label()
             else:
@@ -1851,14 +1968,16 @@
                 self.yg_glyph.props.del_property("category")
             except Exception:
                 pass
         else:
             self.yg_glyph.set_category(c)
 
     def set_point_display(self, pv: str) -> None:
+        if self.yg_glyph.is_composite:
+            return
         for p in self.yg_point_view_list:
             p.yg_point.label_pref = pv
             if self.point_numbers_showing:
                 if p.isVisible():
                     p.add_label()
 
     @pyqtSlot(object)
@@ -2341,15 +2460,15 @@
             if pplen >= 1:
                 h = {"ptid": self._model_point(pp[0]).preferred_label()}
                 new_yg_hint = ygHint(self.yg_glyph, h)
                 dr = self.get_round_default(new_yg_hint)
                 if dr != None:
                     new_yg_hint.set_round(dr)
                 if ctrl:
-                    self.guess_cv_for_hint(new_yg_hint)
+                    self.guess_cv_for_new_hint(new_yg_hint)
                 if shift:
                     new_yg_hint.set_round(True)
                 self.sig_new_hint.emit(new_yg_hint)
         if hint_type_num in [1, 3]:
             if pplen >= 2:
                 try:
                     if hint_type_num == 3:
@@ -2376,15 +2495,15 @@
                     return
                 h = {"ptid": tgt, "ref": ref_name, "rel": hint_type}
                 new_yg_hint = ygHint(self.yg_glyph, h)
                 dr = self.get_round_default(new_yg_hint)
                 if dr != None:
                     new_yg_hint.set_round(dr)
                 if ctrl and hint_type_num == 3:
-                    self.guess_cv_for_hint(new_yg_hint)
+                    self.guess_cv_for_new_hint(new_yg_hint)
                 if shift:
                     new_yg_hint.set_round(True)
                 self.sig_new_hint.emit(new_yg_hint)
         if hint_type_num == 2:
             if pplen >= 3:
                 # If two of the three selected points are touched, they are the
                 # reference points, and the untouched point is the target.
```

### Comparing `ygt-0.2.1/src/ygt/ygModel.py` & `ygt-0.2.3/src/ygt/ygModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 import os
 import pathlib
 import uuid
 import random
 import copy
 import unicodedata
 import abc
+from tempfile import SpooledTemporaryFile
 from .ygPreferences import ygPreferences
 from .cvGuesser import instanceChecker
+from .freetypeFont import freetypeFont
+from .harfbuzzFont import harfbuzzFont
 
 # from .ygSchema import error_message, set_error_message, is_cv_delta_valid
 import defcon # type: ignore
 from ufo2ft import compileTTF # type: ignore
 
 hint_type_nums = {
     "anchor": 0,
@@ -366,23 +369,33 @@
         fontfile = self.font_files.in_font
         if not fontfile:
             raise Exception("Need the name of an existing font")
             # Need to let user try again.
         split_fn = os.path.splitext(str(fontfile))
         extension = split_fn[1]
         ft_open_error = False
+        # self.freetype_font = None
+        # Here we get *two* copies of the font in memory: one in FontTools format,
+        # the other FreeType.
         if extension == ".ttf":
             try:
                 self.ft_font = ttLib.TTFont(fontfile)
+                self.freetype_font = freetypeFont(fontfile)
+                self.harfbuzz_font = harfbuzzFont(fontfile, self.freetype_font)
             except FileNotFoundError as ferr:
                 ft_open_error = True
         elif extension == ".ufo":
             try:
                 ufo = defcon.Font(fontfile)
                 self.ft_font = compileTTF(ufo, useProductionNames=False, reverseDirection=False)
+                tf = SpooledTemporaryFile(max_size=3000000, mode='b')
+                self.ft_font.save(tf, 1)
+                self.freetype_font = freetypeFont(tf, keep_open = True)
+                self.harfbuzz_font = harfbuzzFont(tf, self.freetype_font)
+                # tf.close()
             except Exception as e:
                 print(e)
                 ft_open_error = True
         if ft_open_error:
             raise Exception("Can't find font file " + str(fontfile))
             # Fix this! Need a dialog box and a chance to try again for a valid font.
             #
@@ -562,27 +575,27 @@
         self._clean = True
         glyph_names = self.ft_font.getGlyphNames()
 
         # dict of {glyph_name: unicode}.
         self.cmap = self.ft_font["cmap"].buildReversed()
 
         # This dict is for using a glyph name to look up a glyph's index.
-        # Composites are left out, since this program doesn't deal with them
-        # (may decide, though, to display previews of them)
         self.name_to_index = {}
         raw_order_list = self.ft_font.getGlyphOrder()
         for order_index, gn in enumerate(raw_order_list):
             self.name_to_index[gn] = order_index
 
         # Get a list of tuples containing unicodes and glyph names (still
         # omitting composites). Sort first by unicode, then by name. This
         # is our order for the font.
         for gn in glyph_names:
             g = self.ft_font["glyf"][gn]
-            if not g.isComposite():
+            # Remove this test if we're going to display composites.
+            # if not g.isComposite():
+            if True:
                 cc = g.getCoordinates(self.ft_font["glyf"])
                 if len(cc) > 0:
                     self.glyph_list.append((self.get_unicode(gn), gn))
         self.glyph_list.sort(key=lambda x: x[1])
         self.glyph_list.sort(key=lambda x: x[0])
 
         self.unicode_to_name = {}
@@ -697,14 +710,19 @@
             for g in no_hints:
                 del self.source["glyphs"][g]
         except Exception as e:
             self.send_error_message(
                 {"msg": "Error in cleanup_font: " + str(e), "mode": "console"}
             )
 
+    def is_composite(self, gname: str) -> bool:
+        if not gname in self.name_to_index:
+            return False
+        return self.ft_font['glyf'][gname].isComposite()
+
     def has_hints(self, gname: str) -> bool:
         if not gname in self.glyphs:
             return False
         glyph_program = self.glyphs[gname]
         if not ("y" in glyph_program or "x" in glyph_program):
             return False
         y_len = 0
@@ -739,25 +757,39 @@
             return self.name_to_index[gname]
 
     def get_glyph_name(self, char: str) -> str:
         try:
             return self.unicode_to_name[ord(char)]
         except Exception:
             return ".notdef"
+        
+    def additional_component_names(self, glyph_list):
+        """Get list of components for all the glyphs in glyph_list.
+           Recurse if necessary. Don't worry about redundancies in list.
+        """
+        result = []
+        for gn in glyph_list:
+            cn = self.ft_font['glyf'][gn].getComponentNames(self.ft_font['glyf'])
+            if len(cn):
+                for ccn in cn:
+                    result.append(ccn)
+                    result.extend(self.additional_component_names([ccn]))
+        return result
 
     def string_to_name_list(self, s: str) -> list:
         """Get the names of the glyphs needed to make string s
         from the current font.
         """
         result = []
         for c in s:
             gn = self.get_glyph_name(c)
             if not gn in result:
                 result.append(gn)
-        return result
+        result.extend(self.additional_component_names(result))
+        return list(set(result))
 
     def save_glyph_source(self, source: dict, axis: str, gname: str) -> None:
         """Save a y or x block to the in-memory source."""
         if not gname in self.glyphs:
             self.glyphs[gname] = {}
         self.glyphs[gname][axis] = source
 
@@ -2103,14 +2135,15 @@
             if "A" in l:
                 self.gname = "A"
             elif len(l) >= 2:
                 self.gname = l[1]
             else:
                 raise Exception("Tried to load nonexistent glyph " + self.gname)
             self.ft_glyph = yg_font.ft_font["glyf"][self.gname]
+        self.is_composite = self.ft_glyph.isComposite()
 
         # Initialize the source for this glyph.
 
         self._gsource = yg_font.get_glyph(self.gname)
         self.props = ygGlyphProperties(self)
         self.error = 0
 
@@ -2935,15 +2968,15 @@
         self.send_yaml_to_editor()
 
     def send_yaml_to_editor(self) -> None:
         """Sends yaml source for the current x or y block to the editor pane."""
         new_yaml = copy.deepcopy(self.current_block)
         self.yaml_strip_extraneous_nodes(new_yaml)
         self.sig_glyph_source_ready.emit(
-            yaml.dump(new_yaml, sort_keys=False, Dumper=Dumper)
+            [yaml.dump(new_yaml, sort_keys=False, Dumper=Dumper), self.is_composite]
         )
 
     def hint_changed(self, h: Union["ygHint", None]):
         """Called by signal from ygHint. Sends a list of hints in response."""
         self.set_dirty()
         self.sig_hints_changed.emit(self.hints)
         self.send_yaml_to_editor()
```

### Comparing `ygt-0.2.1/src/ygt/ygPreferences.py` & `ygt-0.2.3/src/ygt/ygPreferences.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/ygPreview.py` & `ygt-0.2.3/src/ygt/ygPreview.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 from typing import Callable, List, Optional
-from .freetypeFont import freetypeFont, RENDER_GRAYSCALE, RENDER_LCD_1, RENDER_LCD_2
+import copy
+from numpy import nditer
+from .freetypeFont import (
+    freetypeFont,
+    RENDER_GRAYSCALE,
+    RENDER_LCD_1,
+    RENDER_LCD_2,
+    #adjust_gamma,
+)
 from PyQt6.QtWidgets import (
     QWidget,
     QLabel,
     QLineEdit,
     QPushButton,
     QHBoxLayout,
     QVBoxLayout,
+    QScrollArea,
+    QSizePolicy,
 )
 from PyQt6.QtGui import QPainter, QBrush, QColor, QPalette, QPixmap
 from PyQt6.QtCore import Qt, QRect, pyqtSignal, pyqtSlot, QLine
+#import cv2
 
 
 PREVIEW_WIDTH = 450
-PREVIEW_HEIGHT = 700
-STRING_PREVIEW_HEIGHT = 150
+PREVIEW_HEIGHT = 500
+STRING_PREVIEW_HEIGHT = 200
 PREVIEW_HORI_MARGIN = 25
 PREVIEW_VERT_MARGIN = 50
 
 
-class ygPreviewContainer(QWidget):
+class ygPreviewContainer(QScrollArea):
     def __init__(self, preview, string_preview):
         super().__init__()
         self._layout = QVBoxLayout()
-        self._layout.setSpacing(0)
+        self._layout.setSpacing(10)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addWidget(preview)
         self._layout.addWidget(string_preview)
         self.setLayout(self._layout)
 
 
 class ygPreview(QLabel):
@@ -42,53 +53,60 @@
         self.glyph_index = 0
         self.char_size = 25
         self.label = QLabel()
         self.label.setStyleSheet("QLabel {background-color: transparent; color: red;}")
         self.label.setText(str(self.char_size) + "ppem")
         self.label.setParent(self)
         self.label.move(50, 30)
+
         self.minimum_x = PREVIEW_WIDTH
         self.minimum_y = PREVIEW_HEIGHT
-        self.setMinimumSize(self.minimum_x, self.minimum_y)
+        self.setFixedWidth(self.minimum_x)
+        self.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Expanding)
         self.vertical_margin = PREVIEW_VERT_MARGIN
         self.horizontal_margin = PREVIEW_HORI_MARGIN
+
         self.max_pixel_size = 12
         self.pixel_size = 12
         # absolute height of the glyph, from top pixel to bottom pixel.
         self.current_glyph_height = 0
         # Corresponds to font's ascender number
         self.ascender = 0
         # Corresponds to the font's descender number
         self.descender = 0
-        # The height of the glyph above the baseline. Should be able to subtract
-        # this from self.ascender to get where on the grid we should start laying
-        # down pixels. If the result of the subtraction is negative, we need to
+        # The height of the glyph above the baseline. Subtract this from
+        # self.ascender to get where on the grid we should start laying down
+        # pixels. If the result of the subtraction is negative, we need to
         # display grid above the ascender number.
         self.bitmap_top = 0
         self.grid_height = 0
         self.total_height = 0
         # The top of the grid should be offset this far from self.vertical_margin
         self.top_grid_offset = 0
         # The pixels of the glyph start this far down.
         self.top_char_margin = 0
         self.show_grid = True
+
         # Two- or three-dimensional array shaped by numpy.
         self.Z: list = []
         self.instance_dict: Optional[dict] = None
         self.instance: Optional[str] = None
+
+        # Figure out if we have a dark or a light theme.
         text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
         self.background_color = self.default_background = self.palette().color(QPalette.ColorRole.Base)
         bg_hsv_value = self.background_color.value()
         self.dark_theme = text_hsv_value > bg_hsv_value
         self.theme_choice = "auto"
         self.colors = None
         self.change_theme(self.theme_choice)
 
         self.render_mode = RENDER_LCD_1
         self.hinting_on = True
+
         # We display the preview by painting on a QPixmap and adding that to this widget.
         # There are three methods for grayscale, lcd1, and lcd2. These are assigned to
         # self.make_pixmap, which can be called whenever display needs to be refreshed--
         # but we don't call the actual methods directly.
         self.make_pixmap = self.make_pixmap_lcd1
 
         self.pixmap = None
@@ -122,15 +140,16 @@
         if self.theme_choice == "auto":
             dark_theme = self.dark_theme
 
         for count, c in enumerate(l):
             if dark_theme:
                 l[count] = QColor(255, 255, 255, count) # type: ignore
             else:
-                l[count] = QColor(101, 53, 15, count) # type: ignore
+                # l[count] = QColor(101, 53, 15, count) # type: ignore
+                l[count] = QColor(0, 0, 0, count) # type: ignore
         return l # type: ignore
 
     def fetch_glyph(self, font, glyph_index):
         """Get a temporary FreeType font, then build the specified glyph.
 
         params:
 
@@ -174,18 +193,18 @@
             if abs(glyph_descent) > abs(self.face.descender):
                 self.total_height += abs(glyph_descent) - abs(self.face.descender)
 
         self.pixel_size = self.max_pixel_size
         char_width = ft_width
         if self.render_mode != RENDER_GRAYSCALE:
             char_width = ft_width / 3
-        preview_display_width = PREVIEW_WIDTH - (PREVIEW_HORI_MARGIN * 2)
+        preview_display_width = self.width() - (PREVIEW_HORI_MARGIN * 2)
         if char_width * self.pixel_size > preview_display_width:
             self.pixel_size = round(preview_display_width / char_width)
-        preview_display_height = PREVIEW_HEIGHT - (PREVIEW_VERT_MARGIN * 2)
+        preview_display_height = self.height() - (PREVIEW_VERT_MARGIN * 2)
         if self.total_height * self.pixel_size > preview_display_height:
             self.pixel_size = round(preview_display_height / self.total_height)
         if self.render_mode == RENDER_LCD_2:
             nn = self.pixel_size % 3
             if nn != 0:
                 self.pixel_size -= nn
             if self.pixel_size < 3:
@@ -384,14 +403,15 @@
             else:
                 pen.setColor(QColor(50, 50, 50, 50))
             painter.setPen(pen)
             for i, r in enumerate(range(grid_width)):
                 painter.drawLine(QLine(left, y_top, left, y_bot))
                 left += self.pixel_size
 
+
     def make_pixmap_grayscale(self) -> None:
         """Paint grayscale glyph."""
         dark_theme = (self.theme_choice == "dark")
         if self.theme_choice == "auto":
             dark_theme = self.dark_theme
 
         if self.pixmap == None:
@@ -416,15 +436,18 @@
             xposition = self.horizontal_margin
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
         self.setPixmap(self.pixmap)
         self.sig_preview_paint_done.emit(None)
 
+
     def make_pixmap_lcd1(self) -> None:
+        """ Make glyph rendered as subpixel 1
+        """
         dark_theme = (self.theme_choice == "dark")
         if self.theme_choice == "auto":
             dark_theme = self.dark_theme
 
         if self.pixmap == None:
             self.pixmap = QPixmap(self.width(), self.height())
         self.pixmap.fill(self.background_color)
@@ -432,32 +455,33 @@
 
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
             painter.end()
             return
+        # Get a copy of the pre-corrected bitmap to use as a mask. We'll skip drawing any
+        # pixels with color 0,0,0.
+        mask = copy.deepcopy(self.Z)
+
         xposition = self.horizontal_margin
         yposition = self.vertical_margin + (self.top_char_margin * self.pixel_size)
 
-        if dark_theme:
-            skippable = QColor("black")
-        else:
-            skippable = QColor("white")
-
-        for row in self.Z:
-            for col in row:
-                rgb = []
-                for elem in col:
-                    rgb.append(elem)
-                if dark_theme:
-                    qc = QColor(rgb[0], rgb[1], rgb[2])
-                else:
-                    qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
-                if qc != skippable:
+        for i, row in enumerate(self.Z):
+            for ii, col in enumerate(row):
+                # If any of the (rgb) bytes for this pixel are non-zero in the mask,
+                # draw the pixel. Otherwise skip.
+                if mask[i][ii].any():
+                    rgb = []
+                    for elem in col:
+                        rgb.append(elem)
+                    if dark_theme:
+                        qc = QColor(rgb[0], rgb[1], rgb[2])
+                    else:
+                        qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
                     qr = QRect(xposition, yposition, self.pixel_size, self.pixel_size)
                     painter.fillRect(qr, qc)
                 xposition += self.pixel_size
             yposition += self.pixel_size
             xposition = self.horizontal_margin
 
         if self.show_grid:
@@ -465,16 +489,18 @@
 
         painter.end()
 
         self.setPixmap(self.pixmap)
 
         self.sig_preview_paint_done.emit(None)
 
+
     def make_pixmap_lcd2(self) -> None:
-        """Paint subpixel rendering with rgb pixel trios."""
+        """ Make glyph rendered as subpixel 1
+        """
         dark_theme = (self.theme_choice == "dark")
         if self.theme_choice == "auto":
             dark_theme = self.dark_theme
 
         if self.pixmap == None:
             self.pixmap = QPixmap(self.width(), self.height())
         self.pixmap.fill(self.background_color)
@@ -521,40 +547,44 @@
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
         self.setPixmap(self.pixmap)
         self.sig_preview_paint_done.emit(None)
 
 
-class ygStringPreviewPanel(QWidget):
+class ygStringPreviewPanel(QLabel):
     sig_go_to_glyph = pyqtSignal(object)
 
     def __init__(self, yg_preview: ygPreview, top_window) -> None:
         super().__init__()
         self.yg_preview = yg_preview
         self.top_window = top_window
         self.face = self.yg_preview.face
         self._text = ""
         self.minimum_x = PREVIEW_WIDTH
         self.minimum_y = 200
-        self.setMinimumSize(self.minimum_x, self.minimum_y)
-        self.paintEvent = self.paintEvent_a # type: ignore
+        self.setFixedSize(PREVIEW_WIDTH, STRING_PREVIEW_HEIGHT)
+        self.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
         self.rect_list: list = []
+        self._full_glyph_list = []
+        self._full_pos_list = []
+        self.make_pixmap = self.make_pixmap_a
+        self.pixmap = None
 
     def set_go_to_signal(self, func: Callable) -> None:
         self.sig_go_to_glyph.connect(func)
 
     def set_face(self, face) -> None:
         self.face = face
 
     def set_text(self, t: str) -> None:
         self._text = t
 
     def string_to_glyph_list(self, s: str) -> list:
-        """Get a list of glyph names needed for string s."""
+        """Get a list of glyph names (no dupicates) needed for string s."""
         yg_font = self.top_window.glyph_pane.yg_glyph_scene.yg_glyph.yg_font
         result = []
         for c in s:
             try:
                 if not c in result:
                     result.append(yg_font.unicode_to_name[ord(c)])
             except Exception:
@@ -564,17 +594,22 @@
     def _fill_background(self, painter: QPainter) -> None:
         brush = QBrush()
         brush.setColor(self.yg_preview.background_color)
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
 
-    def paintEvent_a(self, event) -> None:
+    def make_pixmap_a(self) -> None:
+        """ Draw the size array.
+        """
         target_size = self.yg_preview.char_size
-        painter = QPainter(self)
+        if self.pixmap == None:
+            self.pixmap = QPixmap(self.width(), self.height())
+        self.pixmap.fill(self.yg_preview.background_color)
+        painter = QPainter(self.pixmap)
         self._fill_background(painter)
         if self.face == None:
             painter.end()
             return
         if not self.yg_preview:
             return
         self.face.reset_rect_list()
@@ -596,73 +631,89 @@
             )
             advance = self.face.draw_char(
                 painter,
                 xposition,
                 yposition,
                 spacing_mark = True,
                 dark_theme = dark_theme,
-                is_target=this_is_target
+                is_target=this_is_target,
             )
             xposition += advance
             if xposition + advance > (PREVIEW_WIDTH - 50):
                 if yposition == 66:
                     xposition = 25
                     yposition = 133
                 else:
                     break
         self.rect_list = self.face.rect_list
         painter.end()
+        self.setPixmap(self.pixmap)
 
-    def paintEvent_b(self, event) -> None:
-        painter = QPainter(self)
+    def make_pixmap_b(self) -> None:
+        """ Draw a string. """
+        if self.pixmap == None:
+            self.pixmap == QPixmap(self.width(), self.height())
+        self.pixmap.fill(self.yg_preview.background_color)
+        painter = QPainter(self.pixmap)
         self._fill_background(painter)
         if not self.yg_preview:
             return
         xposition = 25
         yposition = 66
         self.face = self.yg_preview.face
         dark_theme = (self.yg_preview.theme_choice == "dark")
         if self.yg_preview.theme_choice == "auto":
             dark_theme = self.yg_preview.dark_theme
         self.rect_list = self.face.draw_string(
             painter,
-            self._text,
+            # self._text,
+            self._full_glyph_list,
             xposition,
             yposition,
+            self.pixmap.toImage(),
+            positions = self._full_pos_list,
             x_limit = PREVIEW_WIDTH - 50,
             dark_theme = dark_theme
         )
         painter.end()
+        self.setPixmap(self.pixmap)
 
     def mousePressEvent(self, event) -> None:
         qp = event.position()
         x = int(qp.x())
         y = int(qp.y())
         rr = None
         for r in self.rect_list:
             if r.contains(x, y):
                 rr = r
                 break
         if rr != None:
-            if self.paintEvent == self.paintEvent_a:
+            if self.make_pixmap == self.make_pixmap_a:
                 self.yg_preview.set_size(rr.size)
             else:
                 self.sig_go_to_glyph.emit(rr.gname.decode())
 
 
 class ygStringPreview(QWidget):
 
     sig_string_changed = pyqtSignal(object)
 
     def __init__(self, yg_preview: ygPreview, top_window) -> None:
         super().__init__()
         self.yg_preview = yg_preview
         self.top_window = top_window
 
+        self.vertical_margin = PREVIEW_VERT_MARGIN
+        self.horizontal_margin = PREVIEW_HORI_MARGIN
+
         self._layout = QVBoxLayout()
+        self._layout.setContentsMargins(0,0,0,0)
+
+        self.setFixedWidth(PREVIEW_WIDTH)
+        self.setMinimumHeight(STRING_PREVIEW_HEIGHT)
 
         self.panel = ygStringPreviewPanel(yg_preview, top_window)
 
         self.button_widget = QWidget()
         self.button_widget_layout = QHBoxLayout()
         self.button_widget_layout.addWidget(QLabel("Text:"))
         self.qle = QLineEdit()
@@ -676,22 +727,44 @@
         self.qle.editingFinished.connect(self.got_string)
 
         self._layout.addWidget(self.panel)
         self._layout.addWidget(self.button_widget)
 
         self.setLayout(self._layout)
 
+        # list of glyph names correspond
+        
+    @property
+    def full_glyph_list(self):
+        return self.panel._full_glyph_list
+    
+    @full_glyph_list.setter
+    def full_glyph_list(self, l):
+        self.panel._full_glyph_list.clear()
+        for ll in l:
+            self.panel._full_glyph_list.append(ll)
+
+    @property
+    def full_pos_list(self):
+        return self.panel._full_pos_list
+
+    @full_pos_list.setter
+    def full_pos_list(self, l):
+        self.panel._full_pos_list = l
+
     def set_go_to_signal(self, func: Callable) -> None:
         self.panel.set_go_to_signal(func)
 
     def set_string_preview(self) -> None:
-        self.panel.paintEvent = self.panel.paintEvent_b # type: ignore
+        self.panel.make_pixmap = self.panel.make_pixmap_b
+        # self.panel.paintEvent = self.panel.paintEvent_b # type: ignore
 
     def set_size_array(self) -> None:
-        self.panel.paintEvent = self.panel.paintEvent_a # type: ignore
+        self.panel.make_pixmap = self.panel.make_pixmap_a
+        # self.panel.paintEvent = self.panel.paintEvent_a # type: ignore
 
     def set_face(self, f: freetypeFont) -> None:
         if self.panel != None:
             self.panel.face = f
 
     def got_string(self) -> None:
         self.panel.set_text(self.qle.text())
```

### Comparing `ygt-0.2.1/src/ygt/ygSchema.py` & `ygt-0.2.3/src/ygt/ygSchema.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/ygStems.py` & `ygt-0.2.3/src/ygt/ygStems.py`

 * *Files identical despite different names*

### Comparing `ygt-0.2.1/src/ygt/ygYAMLEditor.py` & `ygt-0.2.3/src/ygt/ygYAMLEditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,20 @@
         self.code_valid = True
         self.setup_editor()
 
     def setup_error_signal(self, f: Callable) -> None:
         self.sig_error.connect(f)
 
     @pyqtSlot(object)
-    def install_source(self, text: str) -> None:
-        self.setPlainText(text)
+    def install_source(self, l: list) -> None:
+        self.setPlainText(l[0])
+        if l[1]:
+            self.setEnabled(False)
+            return
+        self.setEnabled(True)
 
     @pyqtSlot()
     def yaml_source(self) -> None:
         err = False
         # msg = ""
         s = ""
         try:
```

### Comparing `ygt-0.2.1/src/ygt.egg-info/PKG-INFO` & `ygt-0.2.3/src/ygt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.2.1
+Version: 0.2.3
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
@@ -26,15 +26,33 @@
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
 
 ## Changes
 
-### Verasion 0.2.0
+### Version 0.2.3 (2023-5-25)
+
+Enable OpenType features in string preview panel (via Harfbuzz).
+
+Better lcd/subpixel rendering in string preview panel.
+
+Touched points are tinted pink.
+
+Previews of composite glyphs can now be displayed.
+
+Editing panels are disabled when there are no outlines.
+
+Pyinstaller spec file for Linux added.
+
+### Version 0.2.1 (2023-5-11)
+
+Fixed a bug.
+
+### Version 0.2.0 (2023-5-11)
 
 Enabled merge (Ygt can add its hints to existing hints).
 
 Added files supporting creation of executables.
 
 Changed shortcuts: Ctrl-P = Hint Preview; Ctrl-L: Set Resolution.
```

### Comparing `ygt-0.2.1/src/ygt.egg-info/SOURCES.txt` & `ygt-0.2.3/src/ygt.egg-info/SOURCES.txt`

 * *Files identical despite different names*


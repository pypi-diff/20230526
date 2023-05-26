# Comparing `tmp/FuncsForSPO-4.43.0.tar.gz` & `tmp/FuncsForSPO-4.44.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.43.0.tar", last modified: Thu May 25 14:08:07 2023, max compression
+gzip compressed data, was "FuncsForSPO-4.44.0.tar", last modified: Fri May 26 15:15:12 2023, max compression
```

## Comparing `FuncsForSPO-4.43.0.tar` & `FuncsForSPO-4.44.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.566792 FuncsForSPO-4.43.0/
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.016280 FuncsForSPO-4.43.0/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.095946 FuncsForSPO-4.43.0/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.43.0/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.43.0/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.113478 FuncsForSPO-4.43.0/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.43.0/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.130394 FuncsForSPO-4.43.0/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.43.0/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.147693 FuncsForSPO-4.43.0/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.43.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.007293 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.177732 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.209882 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.219080 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.250825 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5017 2023-05-08 20:46:58.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.270617 FuncsForSPO-4.43.0/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.283339 FuncsForSPO-4.43.0/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    68204 2023-05-25 14:06:54.000000 FuncsForSPO-4.43.0/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.323190 FuncsForSPO-4.43.0/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.43.0/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.349089 FuncsForSPO-4.43.0/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.43.0/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.367573 FuncsForSPO-4.43.0/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.43.0/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.43.0/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.383997 FuncsForSPO-4.43.0/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.43.0/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.43.0/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.468719 FuncsForSPO-4.43.0/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.43.0/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:08:07.074534 FuncsForSPO-4.43.0/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-05-25 14:08:06.000000 FuncsForSPO-4.43.0/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-05-25 14:08:06.000000 FuncsForSPO-4.43.0/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:08:06.000000 FuncsForSPO-4.43.0/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-05-25 14:08:06.000000 FuncsForSPO-4.43.0/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-05-25 14:08:06.000000 FuncsForSPO-4.43.0/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.43.0/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-05-25 14:08:07.563302 FuncsForSPO-4.43.0/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.43.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 14:08:07.567327 FuncsForSPO-4.43.0/setup.cfg
--rw-rw-rw-   0        0        0     2177 2023-05-25 14:07:50.000000 FuncsForSPO-4.43.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.427635 FuncsForSPO-4.44.0/
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.062951 FuncsForSPO-4.44.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.115445 FuncsForSPO-4.44.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.44.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.44.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.127133 FuncsForSPO-4.44.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.44.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.137655 FuncsForSPO-4.44.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.44.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.148550 FuncsForSPO-4.44.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.44.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.054356 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.193821 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.212320 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.219327 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.236706 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5017 2023-05-08 20:46:58.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.245227 FuncsForSPO-4.44.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.254236 FuncsForSPO-4.44.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-4.44.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.266348 FuncsForSPO-4.44.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.44.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.275973 FuncsForSPO-4.44.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.44.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.287561 FuncsForSPO-4.44.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.44.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.295384 FuncsForSPO-4.44.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.44.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.44.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.302088 FuncsForSPO-4.44.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.44.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:15:12.105297 FuncsForSPO-4.44.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-05-26 15:15:11.000000 FuncsForSPO-4.44.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-05-26 15:15:11.000000 FuncsForSPO-4.44.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:15:11.000000 FuncsForSPO-4.44.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-05-26 15:15:11.000000 FuncsForSPO-4.44.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      350 2023-05-26 15:15:11.000000 FuncsForSPO-4.44.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.44.0/LICENSE
+-rw-rw-rw-   0        0        0     8027 2023-05-26 15:15:12.422855 FuncsForSPO-4.44.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.44.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:15:12.427635 FuncsForSPO-4.44.0/setup.cfg
+-rw-rw-rw-   0        0        0     2177 2023-05-26 15:15:00.000000 FuncsForSPO-4.44.0/setup.py
```

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/femails/femails.py` & `FuncsForSPO-4.44.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files 0% similar despite different names*

```diff
@@ -1571,14 +1571,19 @@
         fjson.write("""from FuncsForSPO.fpdf.focr.orc import *
 from FuncsForSPO.fpdf.fcompress.compress import *
 from FuncsForSPO.fpdf.fimgpdf.img_to_pdf import *
 from FuncsForSPO.fpysimplegui.functions_for_sg import *
 from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.fregex.functions_re import *
 from FuncsForSPO.fselenium.functions_selenium import *
+import sys
+import os
+
+root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+sys.path.append(root_dir)
 
 # SEMPRE COLOQUE O QUE A FUNÇÃO TEM QUE FAZER EXPLICITAMENTE
 """)
 
     # cria diretório base
     if create_base_dir:
         cria_dir_no_dir_de_trabalho_atual('base')
```

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-4.44.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO/utils/utils.py` & `FuncsForSPO-4.44.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-4.44.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.43.0
+Version: 4.44.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.43.0/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-4.44.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/LICENSE` & `FuncsForSPO-4.44.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/PKG-INFO` & `FuncsForSPO-4.44.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.43.0
+Version: 4.44.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.43.0/README.md` & `FuncsForSPO-4.44.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.43.0/setup.py` & `FuncsForSPO-4.44.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.43.0'
+version = '4.44.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```


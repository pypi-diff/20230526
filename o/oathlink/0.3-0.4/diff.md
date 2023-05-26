# Comparing `tmp/oathlink-0.3.tar.gz` & `tmp/oathlink-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oathlink-0.3.tar", last modified: Fri May 26 20:28:57 2023, max compression
+gzip compressed data, was "oathlink-0.4.tar", last modified: Fri May 26 20:39:36 2023, max compression
```

## Comparing `oathlink-0.3.tar` & `oathlink-0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.378870 oathlink-0.3/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.3/LICENSE
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      687 2023-05-26 20:28:57.378958 oathlink-0.3/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.3/README.md
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.3/pyproject.toml
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      822 2023-05-26 20:28:57.379270 oathlink-0.3/setup.cfg
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.372070 oathlink-0.3/src/
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.373536 oathlink-0.3/src/oathlink/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       40 2023-05-26 20:06:46.000000 oathlink-0.3/src/oathlink/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.374586 oathlink-0.3/src/oathlink/main/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/main/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     4727 2023-05-26 20:12:25.000000 oathlink-0.3/src/oathlink/main/oathlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.374918 oathlink-0.3/src/oathlink/services/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/services/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.375154 oathlink-0.3/src/oathlink/services/agent/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/services/agent/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.375981 oathlink-0.3/src/oathlink/services/agent/account/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/services/agent/account/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/agent/account/create.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/agent/account/link.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/agent/account/unlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.376438 oathlink-0.3/src/oathlink/services/agent/ip/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/services/agent/ip/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/agent/ip/add.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/agent/ip/remove.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/hello.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.377433 oathlink-0.3/src/oathlink/services/record/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/services/record/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/record/archive.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/record/cancel.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      897 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/record/decrypt.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/record/download.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1273 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/record/upload.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.377958 oathlink-0.3/src/oathlink/services/report/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/services/report/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/report/history.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/report/outstanding.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.3/src/oathlink/services/report/record.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.378126 oathlink-0.3/src/oathlink/util/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/util/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.378457 oathlink-0.3/src/oathlink/util/crypto/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.3/src/oathlink/util/crypto/Fernet.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/util/crypto/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.378636 oathlink-0.3/src/oathlink/util/https/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.3/src/oathlink/util/https/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1976 2023-03-10 16:20:28.000000 oathlink-0.3/src/oathlink/util/https/https.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:28:57.374384 oathlink-0.3/src/oathlink.egg-info/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      687 2023-05-26 20:28:57.000000 oathlink-0.3/src/oathlink.egg-info/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-05-26 20:28:57.000000 oathlink-0.3/src/oathlink.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-05-26 20:28:57.000000 oathlink-0.3/src/oathlink.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-05-26 20:28:57.000000 oathlink-0.3/src/oathlink.egg-info/requires.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-05-26 20:28:57.000000 oathlink-0.3/src/oathlink.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.120235 oathlink-0.4/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.4/LICENSE
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      687 2023-05-26 20:39:36.120314 oathlink-0.4/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.4/README.md
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.4/pyproject.toml
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      822 2023-05-26 20:39:36.120564 oathlink-0.4/setup.cfg
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.112879 oathlink-0.4/src/
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.114073 oathlink-0.4/src/oathlink/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       36 2023-05-26 20:32:55.000000 oathlink-0.4/src/oathlink/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.115108 oathlink-0.4/src/oathlink/main/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/main/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     4727 2023-05-26 20:12:25.000000 oathlink-0.4/src/oathlink/main/oathlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.115450 oathlink-0.4/src/oathlink/services/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/services/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.115686 oathlink-0.4/src/oathlink/services/agent/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/services/agent/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.116500 oathlink-0.4/src/oathlink/services/agent/account/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/services/agent/account/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/agent/account/create.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/agent/account/link.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/agent/account/unlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.117181 oathlink-0.4/src/oathlink/services/agent/ip/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/services/agent/ip/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/agent/ip/add.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/agent/ip/remove.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/hello.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.118356 oathlink-0.4/src/oathlink/services/record/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/services/record/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/record/archive.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/record/cancel.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      897 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/record/decrypt.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/record/download.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1273 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/record/upload.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.119239 oathlink-0.4/src/oathlink/services/report/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/services/report/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/report/history.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/report/outstanding.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.4/src/oathlink/services/report/record.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.119395 oathlink-0.4/src/oathlink/util/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/util/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.119754 oathlink-0.4/src/oathlink/util/crypto/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.4/src/oathlink/util/crypto/Fernet.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/util/crypto/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.119984 oathlink-0.4/src/oathlink/util/https/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.4/src/oathlink/util/https/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1976 2023-03-10 16:20:28.000000 oathlink-0.4/src/oathlink/util/https/https.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:39:36.114909 oathlink-0.4/src/oathlink.egg-info/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      687 2023-05-26 20:39:36.000000 oathlink-0.4/src/oathlink.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-05-26 20:39:36.000000 oathlink-0.4/src/oathlink.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-05-26 20:39:36.000000 oathlink-0.4/src/oathlink.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-05-26 20:39:36.000000 oathlink-0.4/src/oathlink.egg-info/requires.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-05-26 20:39:36.000000 oathlink-0.4/src/oathlink.egg-info/top_level.txt
```

### Comparing `oathlink-0.3/LICENSE` & `oathlink-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/setup.cfg` & `oathlink-0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oathlink
-version = 0.3
+version = 0.4
 author = oathlink
 author_email = oathlink@bfi.lat
 description = This repository holds the Oathlink user Python package (client source code).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 project_urls =
```

### Comparing `oathlink-0.3/src/oathlink/main/oathlink.py` & `oathlink-0.4/src/oathlink/main/oathlink.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/agent/account/create.py` & `oathlink-0.4/src/oathlink/services/agent/account/create.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/agent/account/link.py` & `oathlink-0.4/src/oathlink/services/agent/account/link.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/agent/account/unlink.py` & `oathlink-0.4/src/oathlink/services/agent/account/unlink.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/agent/ip/add.py` & `oathlink-0.4/src/oathlink/services/agent/ip/add.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/agent/ip/remove.py` & `oathlink-0.4/src/oathlink/services/agent/ip/remove.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/hello.py` & `oathlink-0.4/src/oathlink/services/hello.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/record/archive.py` & `oathlink-0.4/src/oathlink/services/record/archive.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/record/cancel.py` & `oathlink-0.4/src/oathlink/services/record/cancel.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/record/decrypt.py` & `oathlink-0.4/src/oathlink/services/record/decrypt.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/record/download.py` & `oathlink-0.4/src/oathlink/services/record/download.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/record/upload.py` & `oathlink-0.4/src/oathlink/services/record/upload.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/report/history.py` & `oathlink-0.4/src/oathlink/services/report/history.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/report/outstanding.py` & `oathlink-0.4/src/oathlink/services/report/outstanding.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/services/report/record.py` & `oathlink-0.4/src/oathlink/services/report/record.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/util/crypto/Fernet.py` & `oathlink-0.4/src/oathlink/util/crypto/Fernet.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink/util/https/https.py` & `oathlink-0.4/src/oathlink/util/https/https.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.3/src/oathlink.egg-info/SOURCES.txt` & `oathlink-0.4/src/oathlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*


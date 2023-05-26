# Comparing `tmp/KPAPI-1.0.0.tar.gz` & `tmp/KPAPI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\KPAPI-1.0.0.tar", last modified: Fri May 26 09:35:57 2023, max compression
+gzip compressed data, was "dist\KPAPI-1.0.1.tar", last modified: Fri May 26 10:08:11 2023, max compression
```

## Comparing `KPAPI-1.0.0.tar` & `KPAPI-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 09:35:57.081734 KPAPI-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-26 09:35:57.014001 KPAPI-1.0.0/KPAPI/
--rw-rw-rw-   0        0        0      231 2023-05-26 08:49:51.000000 KPAPI-1.0.0/KPAPI/__init__.py
--rw-rw-rw-   0        0        0      393 2023-05-26 08:52:37.000000 KPAPI-1.0.0/KPAPI/seen.py
--rw-rw-rw-   0        0        0      697 2023-05-26 04:46:17.000000 KPAPI-1.0.0/KPAPI/sendMedia.py
--rw-rw-rw-   0        0        0      469 2023-05-26 04:46:58.000000 KPAPI-1.0.0/KPAPI/sendMsg.py
--rw-rw-rw-   0        0        0      399 2023-05-26 04:48:42.000000 KPAPI-1.0.0/KPAPI/typingOff.py
--rw-rw-rw-   0        0        0      397 2023-05-26 04:48:15.000000 KPAPI-1.0.0/KPAPI/typingOn.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:35:57.077735 KPAPI-1.0.0/KPAPI.egg-info/
--rw-rw-rw-   0        0        0      322 2023-05-26 09:35:55.000000 KPAPI-1.0.0/KPAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-05-26 09:35:55.000000 KPAPI-1.0.0/KPAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 09:35:55.000000 KPAPI-1.0.0/KPAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 09:35:55.000000 KPAPI-1.0.0/KPAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2023-05-26 08:55:03.000000 KPAPI-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      322 2023-05-26 09:35:57.079734 KPAPI-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-05-26 09:01:53.000000 KPAPI-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 09:35:57.082739 KPAPI-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      402 2023-05-26 09:32:31.000000 KPAPI-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:08:11.371544 KPAPI-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-26 10:08:11.349542 KPAPI-1.0.1/KPAPI/
+-rw-rw-rw-   0        0        0      231 2023-05-26 08:49:51.000000 KPAPI-1.0.1/KPAPI/__init__.py
+-rw-rw-rw-   0        0        0      393 2023-05-26 08:52:37.000000 KPAPI-1.0.1/KPAPI/seen.py
+-rw-rw-rw-   0        0        0      697 2023-05-26 04:46:17.000000 KPAPI-1.0.1/KPAPI/sendMedia.py
+-rw-rw-rw-   0        0        0      469 2023-05-26 04:46:58.000000 KPAPI-1.0.1/KPAPI/sendMsg.py
+-rw-rw-rw-   0        0        0      399 2023-05-26 04:48:42.000000 KPAPI-1.0.1/KPAPI/typingOff.py
+-rw-rw-rw-   0        0        0      397 2023-05-26 04:48:15.000000 KPAPI-1.0.1/KPAPI/typingOn.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:08:11.367539 KPAPI-1.0.1/KPAPI.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-05-26 10:08:08.000000 KPAPI-1.0.1/KPAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-05-26 10:08:09.000000 KPAPI-1.0.1/KPAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 10:08:08.000000 KPAPI-1.0.1/KPAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 10:08:08.000000 KPAPI-1.0.1/KPAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-05-26 08:55:03.000000 KPAPI-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      956 2023-05-26 10:08:11.369544 KPAPI-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2023-05-26 09:43:31.000000 KPAPI-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 10:08:11.371544 KPAPI-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      502 2023-05-26 10:04:37.000000 KPAPI-1.0.1/setup.py
```

### Comparing `KPAPI-1.0.0/KPAPI/sendMedia.py` & `KPAPI-1.0.1/KPAPI/sendMedia.py`

 * *Files identical despite different names*

### Comparing `KPAPI-1.0.0/LICENSE` & `KPAPI-1.0.1/LICENSE`

 * *Files identical despite different names*


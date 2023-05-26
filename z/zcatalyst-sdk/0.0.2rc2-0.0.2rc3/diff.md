# Comparing `tmp/zcatalyst_sdk-0.0.2rc2.tar.gz` & `tmp/zcatalyst_sdk-0.0.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcatalyst_sdk-0.0.2rc2.tar", last modified: Thu Apr 13 07:54:35 2023, max compression
+gzip compressed data, was "zcatalyst_sdk-0.0.2rc3.tar", last modified: Fri May 26 13:22:32 2023, max compression
```

## Comparing `zcatalyst_sdk-0.0.2rc2.tar` & `zcatalyst_sdk-0.0.2rc3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      639 2023-03-07 13:18:06.000000 zcatalyst_sdk-0.0.2rc2/LICENSE
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       98 2023-03-30 10:55:22.000000 zcatalyst_sdk-0.0.2rc2/MANIFEST.in
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/PKG-INFO
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1441 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/README.md
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       16 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/requirements.txt
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       38 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/setup.cfg
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1129 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/setup.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6151 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       57 2023-04-13 07:52:53.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/__version__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3525 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_constants.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7485 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_http_client.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      519 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_thread_util.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7851 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/authentication.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1675 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3589 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/_segment.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6190 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/catalyst_app.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2183 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/circuit.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2397 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4064 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/_connector.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)    11824 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/credentials.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3313 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cron.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1599 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3092 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_bulk_job.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     5552 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_table.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2611 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/email.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3539 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/exceptions.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2001 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4544 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/_folder.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1140 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/functions.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      794 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1280 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_mobile_notification.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1035 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_web_notificaton.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1203 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/search.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4027 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/smart_browz.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.949810 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7235 2023-03-29 09:36:20.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/__init__.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1630 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/smart_browz.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2999 2023-03-28 05:45:09.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/zia.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     8879 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/validator.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1073 2023-04-10 07:00:22.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zcql.py
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     8247 2023-04-13 07:10:21.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zia.py
-drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-04-13 07:54:35.945812 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1285 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)        1 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       17 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/requires.txt
--rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       14 2023-04-13 07:54:35.000000 zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.141976 zcatalyst_sdk-0.0.2rc3/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      639 2023-03-07 13:18:06.000000 zcatalyst_sdk-0.0.2rc3/LICENSE
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       98 2023-03-30 10:55:22.000000 zcatalyst_sdk-0.0.2rc3/MANIFEST.in
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-05-26 13:22:32.141976 zcatalyst_sdk-0.0.2rc3/PKG-INFO
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1441 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/README.md
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       16 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/requirements.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       38 2023-05-26 13:22:32.141976 zcatalyst_sdk-0.0.2rc3/setup.cfg
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1129 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/setup.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.137977 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6317 2023-05-26 12:03:09.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       57 2023-05-26 12:04:49.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/__version__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3525 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/_constants.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7485 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/_http_client.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      708 2023-05-26 12:03:09.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/_thread_util.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      463 2023-05-26 12:03:09.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/_util.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7852 2023-05-26 13:20:16.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/authentication.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.137977 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/cache/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1675 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/cache/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3589 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/cache/_segment.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     6190 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/catalyst_app.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2183 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/circuit.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.137977 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/connection/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2397 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/connection/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4091 2023-05-26 13:20:16.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/connection/_connector.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)    11824 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/credentials.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3313 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/cron.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.137977 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/datastore/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1599 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/datastore/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3092 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/datastore/_bulk_job.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     5552 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/datastore/_table.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2611 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/email.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     3539 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/exceptions.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.137977 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/filestore/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2001 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/filestore/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4544 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/filestore/_folder.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1140 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/functions.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.137977 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/push_notification/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)      794 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/push_notification/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1280 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/push_notification/_mobile_notification.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1035 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/push_notification/_web_notificaton.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1203 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/search.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     4027 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/smart_browz.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.141976 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/types/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     7235 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/types/__init__.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1630 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/types/smart_browz.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2999 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/types/zia.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     8879 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/validator.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1073 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/zcql.py
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     8247 2023-04-19 11:05:58.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/zia.py
+drwxr-xr-x   0 mahesh-pt4947 (618233756) domain^users (618136065)        0 2023-05-26 13:22:32.137977 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     2118 2023-05-26 13:22:32.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)     1308 2023-05-26 13:22:32.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)        1 2023-05-26 13:22:32.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       17 2023-05-26 13:22:32.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/requires.txt
+-rw-r--r--   0 mahesh-pt4947 (618233756) domain^users (618136065)       14 2023-05-26 13:22:32.000000 zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/top_level.txt
```

### Comparing `zcatalyst_sdk-0.0.2rc2/LICENSE` & `zcatalyst_sdk-0.0.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/PKG-INFO` & `zcatalyst_sdk-0.0.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcatalyst_sdk
-Version: 0.0.2rc2
+Version: 0.0.2rc3
 Summary: Zoho Catalyst SDK for Python
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcatalyst_sdk Version: 0.0.2rc2 Summary: Zoho
+Metadata-Version: 2.1 Name: zcatalyst_sdk Version: 0.0.2rc3 Summary: Zoho
 Catalyst SDK for Python Home-page: https://catalyst.zoho.com/ Author: Catalyst
 by Zoho Author-email: support@zohocatalyst.com License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Requires-Python: >= 3.9
```

### Comparing `zcatalyst_sdk-0.0.2rc2/README.md` & `zcatalyst_sdk-0.0.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/setup.py` & `zcatalyst_sdk-0.0.2rc3/setup.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/__init__.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,42 +20,49 @@
 from .types import ICatalystOptions
 from . import credentials
 from .catalyst_app import CatalystApp
 from ._thread_util import ZCThreadUtil, get_attr
 from .exceptions import CatalystAppError
 from . import _constants as APIConstants
 from ._constants import ProjectHeader, CredentialHeader
+from ._util import parse_headers_from_request
 
 _app_collection = {}
 _app_lock = threading.RLock()
 
 _DEFAULT_APP_NAME = '[DEFAULT]'
 CatalystScopes = Literal['admin', 'user']
 
 
 def initialize(
     name=_DEFAULT_APP_NAME,
-    scope: CatalystScopes = None
+    scope: CatalystScopes = None,
+    req = None
 ):
     """
     Initializes a new CatalystApp from request
 
     Args:
         name: Name of the catalyst app (optional).
             If app name is None, default name will be used.
         scope: The scope in which the app gets initialized (optional).
             If no scope provided, catalyst will switch scopes automatically.
+        req: Request object to initialize the SDK
 
     Returns:
         CatalystApp: A newly initialized catalyst app instance.
 
     Raises:
         CatalystAppError: If the given scope or other app properties are invalid.
         CatalystCredentialError: If the credentials are missing.
     """
+
+    if req:
+        parse_headers_from_request(req)
+
     thread_obj = ZCThreadUtil()
     catalyst_headers: Dict = thread_obj.get_value("catalyst_headers")
 
     if not catalyst_headers:
         raise CatalystAppError(
             'FATAL ERROR',
             'Catalyst headers are empty'
```

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_constants.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/_constants.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_http_client.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/_http_client.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/_thread_util.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/_thread_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import threading
 from typing import Any
 
 
 class ZCThreadUtil:
     def __init__(self) -> None:
-        self.__zclocal = getattr(threading.current_thread(), '__zc_local', {})
+        try:
+            self.__zclocal = getattr(threading.current_thread(), '__zc_local')
+        except AttributeError:
+            setattr(threading.current_thread(), '__zc_local', {})
+            self.__zclocal = getattr(threading.current_thread(), '__zc_local')
 
     def get_value(self, key: str):
         return self.__zclocal.get(key)
 
     def put_value(self, key: str, val: Any):
         self.__zclocal[key] = val
```

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/authentication.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,11 +218,11 @@
         validator.is_non_empty_dict(
             custom_token_details, 'custom_token_details', CatalystAuthenticationError
         )
         resp = self._requester.request(
             method=RequestMethod.POST,
             path='/authentication/custom-token',
             json=custom_token_details,
-            user=CredentialUser.USER
+            user=CredentialUser.ADMIN
         )
         resp_json = resp.response_json
         return resp_json.get('data')
```

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/__init__.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cache/_segment.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/cache/_segment.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/catalyst_app.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/catalyst_app.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/circuit.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/circuit.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/__init__.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/connection/_connector.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/connection/_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,17 @@
 
     def get_access_token(self):
         cached_token = self._app.cache().segment().get(self._connector_name)
         value = cached_token['cache_value']
 
         if value:
             time = 3600000 - int(cached_token['ttl_in_milliseconds'])
-            if self.expires_in and time < (self.expires_in * 1000):
-                # returning from cache
+            if not self.expires_in:
+                return value
+            if self.expires_in and time <= (self.expires_in * 1000):
                 return value
 
         validator.is_non_empty_string(self.refresh_token, 'refresh_token', CatalystConnectorError)
 
         resp = self._requester.request(
             method=RequestMethod.POST,
             url=self.refresh_url,
```

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/credentials.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/credentials.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/cron.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/cron.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/__init__.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_bulk_job.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/datastore/_bulk_job.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/datastore/_table.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/datastore/_table.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/email.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/email.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/exceptions.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/__init__.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/filestore/_folder.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/filestore/_folder.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/functions.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/functions.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/__init__.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/push_notification/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_mobile_notification.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/push_notification/_mobile_notification.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/push_notification/_web_notificaton.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/push_notification/_web_notificaton.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/search.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/search.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/smart_browz.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/smart_browz.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/__init__.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/smart_browz.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/types/smart_browz.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/types/zia.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/types/zia.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/validator.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/validator.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zcql.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/zcql.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk/zia.py` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk/zia.py`

 * *Files identical despite different names*

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/PKG-INFO` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcatalyst-sdk
-Version: 0.0.2rc2
+Version: 0.0.2rc3
 Summary: Zoho Catalyst SDK for Python
 Home-page: https://catalyst.zoho.com/
 Author: Catalyst by Zoho
 Author-email: support@zohocatalyst.com
 License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zcatalyst-sdk Version: 0.0.2rc2 Summary: Zoho
+Metadata-Version: 2.1 Name: zcatalyst-sdk Version: 0.0.2rc3 Summary: Zoho
 Catalyst SDK for Python Home-page: https://catalyst.zoho.com/ Author: Catalyst
 by Zoho Author-email: support@zohocatalyst.com License: Apache License 2.0
 Keywords: zcatalyst,zoho,catalyst,serverless,cloud,SDK,development Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Requires-Python: >= 3.9
```

### Comparing `zcatalyst_sdk-0.0.2rc2/zcatalyst_sdk.egg-info/SOURCES.txt` & `zcatalyst_sdk-0.0.2rc3/zcatalyst_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requirements.txt
 setup.py
 zcatalyst_sdk/__init__.py
 zcatalyst_sdk/__version__.py
 zcatalyst_sdk/_constants.py
 zcatalyst_sdk/_http_client.py
 zcatalyst_sdk/_thread_util.py
+zcatalyst_sdk/_util.py
 zcatalyst_sdk/authentication.py
 zcatalyst_sdk/catalyst_app.py
 zcatalyst_sdk/circuit.py
 zcatalyst_sdk/credentials.py
 zcatalyst_sdk/cron.py
 zcatalyst_sdk/email.py
 zcatalyst_sdk/exceptions.py
```


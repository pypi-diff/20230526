# Comparing `tmp/huscy.consents-0.8.0a20.tar.gz` & `tmp/huscy.consents-0.8.0a21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.consents-0.8.0a20.tar", last modified: Thu May 25 15:55:28 2023, max compression
+gzip compressed data, was "huscy.consents-0.8.0a21.tar", last modified: Fri May 26 17:29:45 2023, max compression
```

## Comparing `huscy.consents-0.8.0a20.tar` & `huscy.consents-0.8.0a21.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.8.0a20/MANIFEST.in
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a20/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy/consents/
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-05-25 10:06:04.000000 huscy.consents-0.8.0a20/huscy/consents/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a20/huscy/consents/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/api_urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a20/huscy/consents/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/forms.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy/consents/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2023-05-25 15:55:27.000000 huscy.consents-0.8.0a20/huscy/consents/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      638 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a20/huscy/consents/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6695 2023-05-25 10:06:04.000000 huscy.consents-0.8.0a20/huscy/consents/services.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/consents/static/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/consents/static/consents/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy/consents/static/consents/css/
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic.min.css
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic2.9.0.min.css
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.323811 huscy.consents-0.8.0a20/huscy/consents/static/consents/img/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/img/logo.svg
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.327811 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic2.9.0.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery3.6.1.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper1.16.1.min.js
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/consents/templates/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.331811 huscy.consents-0.8.0a20/huscy/consents/templates/consents/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/base.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/create_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/sign_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/signed_consent.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/success.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/checkbox.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      113 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/heading.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/markdown.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/paragraph.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/huscy/consents/templates/consents/widgets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/widgets/select_date.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/huscy/consents/templatetags/
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/templatetags/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/templatetags/dict_extras.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/views.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/viewsets.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy.consents.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1685 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      208 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/setup.cfg
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1766 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a20/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.8.0a21/MANIFEST.in
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a21/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a21/huscy/consents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a21/huscy/consents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/api_urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a21/huscy/consents/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/forms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1800 2023-05-26 17:29:44.000000 huscy.consents-0.8.0a21/huscy/consents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1085 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a21/huscy/consents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6948 2023-05-26 11:36:57.000000 huscy.consents-0.8.0a21/huscy/consents/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/static/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/static/consents/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.341955 huscy.consents-0.8.0a21/huscy/consents/static/consents/css/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic.min.css
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic2.9.0.min.css
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.341955 huscy.consents-0.8.0a21/huscy/consents/static/consents/img/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/img/logo.svg
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.345955 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic2.9.0.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery3.6.1.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper1.16.1.min.js
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy/consents/templates/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.349955 huscy.consents-0.8.0a21/huscy/consents/templates/consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/base.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/create_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/sign_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/signed_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/success.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.349955 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/checkbox.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      113 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/heading.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/markdown.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/text_fragments/paragraph.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.349955 huscy.consents-0.8.0a21/huscy/consents/templates/consents/widgets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/templates/consents/widgets/select_date.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/huscy/consents/templatetags/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/templatetags/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/templatetags/dict_extras.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a21/huscy/consents/urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a21/huscy/consents/views.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a21/huscy/consents/viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-26 17:29:45.337955 huscy.consents-0.8.0a21/huscy.consents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1685 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      208 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-05-26 17:29:45.000000 huscy.consents-0.8.0a21/huscy.consents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-05-26 17:29:45.353955 huscy.consents-0.8.0a21/setup.cfg
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1766 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a21/setup.py
```

### Comparing `huscy.consents-0.8.0a20/PKG-INFO` & `huscy.consents-0.8.0a21/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.8.0a20
+Version: 0.8.0a21
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.8.0a20/huscy/consents/admin.py` & `huscy.consents-0.8.0a21/huscy/consents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/forms.py` & `huscy.consents-0.8.0a21/huscy/consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/migrations/0001_initial.py` & `huscy.consents-0.8.0a21/huscy/consents/migrations/0001_initial.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 from django.db import migrations, models
 import django.db.models.deletion
+import huscy.consents.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
     ]
 
     operations = [
         migrations.CreateModel(
             name='Consent',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=128)),
                 ('text_fragments', models.JSONField()),
                 ('version', models.PositiveIntegerField(default=1)),
+                ('name', models.CharField(max_length=128)),
             ],
+            options={
+                'abstract': False,
+            },
         ),
         migrations.CreateModel(
             name='ConsentCategory',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=128)),
-                ('template_text_fragments', models.JSONField(default=list)),
+                ('template_text_fragments', models.JSONField()),
             ],
+            options={
+                'abstract': False,
+            },
         ),
         migrations.CreateModel(
             name='ConsentFile',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('consent_version', models.PositiveIntegerField()),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
-                ('filehandle', models.FileField(upload_to='')),
+                ('filehandle', models.FileField(upload_to=huscy.consents.models.get_consent_file_upload_path)),
                 ('consent', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='consents.consent')),
             ],
+            options={
+                'abstract': False,
+            },
         ),
     ]
```

### Comparing `huscy.consents-0.8.0a20/huscy/consents/serializer.py` & `huscy.consents-0.8.0a21/huscy/consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/services.py` & `huscy.consents-0.8.0a21/huscy/consents/services.py`

 * *Files 9% similar despite different names*

```diff
@@ -168,35 +168,53 @@
             {"$ref": "#/$defs/paragraph"},
         ],
     },
     "minItems": 1,
 }
 
 
-def create_consent(name, text_fragments):
-    jsonschema.validate(text_fragments, TEXT_FRAGMENTS_SCHEMA)
-    return Consent.objects.create(name=name, text_fragments=text_fragments)
-
-
 def create_consent_category(name, template_text_fragments):
     jsonschema.validate(template_text_fragments, TEXT_FRAGMENTS_SCHEMA)
     return ConsentCategory.objects.create(
         name=name,
         template_text_fragments=template_text_fragments,
     )
 
 
+def create_consent(name, text_fragments):
+    jsonschema.validate(text_fragments, TEXT_FRAGMENTS_SCHEMA)
+    return Consent.objects.create(name=name, text_fragments=text_fragments)
+
+
 def create_consent_file(consent, filehandle):
     return ConsentFile.objects.create(
         consent=consent,
         consent_version=consent.version,
         filehandle=filehandle,
     )
 
 
+def update_consent_category(consent_category, name=None, template_text_fragments=None):
+    update_fields = []
+
+    if name is not None and name != consent_category.name:
+        consent_category.name = name
+        update_fields.append('name')
+
+    if (template_text_fragments is not None
+            and template_text_fragments != consent_category.template_text_fragments):
+        jsonschema.validate(template_text_fragments, TEXT_FRAGMENTS_SCHEMA)
+        consent_category.template_text_fragments = template_text_fragments
+        update_fields.append('template_text_fragments')
+
+    consent_category.save(update_fields=update_fields)
+
+    return consent_category
+
+
 def update_consent(consent, name=None, text_fragments=None):
     update_fields = []
 
     if name is not None and name != consent.name:
         consent.name = name
         update_fields.append('name')
 
@@ -207,16 +225,7 @@
 
     if update_fields:
         consent.version += 1
         update_fields.append('version')
         consent.save(update_fields=update_fields)
 
     return consent
-
-
-def update_consent_category(consent_category, name=None, template_text_fragments=None):
-    consent_category.name = consent_category.name if name is None else name
-    if template_text_fragments is not None:
-        jsonschema.validate(template_text_fragments, TEXT_FRAGMENTS_SCHEMA)
-        consent_category.template_text_fragments = template_text_fragments
-    consent_category.save()
-    return consent_category
```

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic.min.css` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic2.9.0.min.css` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/css/fomantic2.9.0.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/img/logo.svg` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/img/logo.svg`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic.min.js` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic2.9.0.min.js` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/fomantic2.9.0.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery.min.js` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery3.6.1.min.js` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/jquery3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper.min.js` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper1.16.1.min.js` & `huscy.consents-0.8.0a21/huscy/consents/static/consents/js/popper1.16.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/templates/consents/base.html` & `huscy.consents-0.8.0a21/huscy/consents/templates/consents/base.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/templates/consents/create_consent.html` & `huscy.consents-0.8.0a21/huscy/consents/templates/consents/create_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/templates/consents/sign_consent.html` & `huscy.consents-0.8.0a21/huscy/consents/templates/consents/sign_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/templates/consents/signed_consent.html` & `huscy.consents-0.8.0a21/huscy/consents/templates/consents/signed_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/views.py` & `huscy.consents-0.8.0a21/huscy/consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy/consents/viewsets.py` & `huscy.consents-0.8.0a21/huscy/consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/huscy.consents.egg-info/PKG-INFO` & `huscy.consents-0.8.0a21/huscy.consents.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.8.0a20
+Version: 0.8.0a21
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.8.0a20/huscy.consents.egg-info/SOURCES.txt` & `huscy.consents-0.8.0a21/huscy.consents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a20/setup.py` & `huscy.consents-0.8.0a21/setup.py`

 * *Files identical despite different names*


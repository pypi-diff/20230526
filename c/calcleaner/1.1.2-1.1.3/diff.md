# Comparing `tmp/calcleaner-1.1.2.tar.gz` & `tmp/calcleaner-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcleaner-1.1.2.tar", last modified: Wed May 24 11:56:48 2023, max compression
+gzip compressed data, was "calcleaner-1.1.3.tar", last modified: Fri May 26 11:35:24 2023, max compression
```

## Comparing `calcleaner-1.1.2.tar` & `calcleaner-1.1.3.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.052017 calcleaner-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-24 11:56:33.000000 calcleaner-1.1.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-24 11:56:33.000000 calcleaner-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-24 11:56:48.052017 calcleaner-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-24 11:56:33.000000 calcleaner-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.036017 calcleaner-1.1.2/calcleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/account_edit_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/accounts_manage_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/caldav_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/calendar_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.028017 calcleaner-1.1.2/calcleaner/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.044017 calcleaner-1.1.2/calcleaner/data/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_128.png
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_256.png
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/images/calcleaner_64.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.044017 calcleaner-1.1.2/calcleaner/data/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/hr/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.024017 calcleaner-1.1.2/calcleaner/data/locales/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-24 11:56:45.000000 calcleaner-1.1.2/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/style/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/style/calcleaner.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.048017 calcleaner-1.1.2/calcleaner/data/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/ui/account-edit-dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/ui/accounts-manage-dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data/ui/main-window.glade
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/data_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-24 11:56:33.000000 calcleaner-1.1.2/calcleaner/translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:56:48.044017 calcleaner-1.1.2/calcleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-24 11:56:48.000000 calcleaner-1.1.2/calcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 11:56:47.000000 calcleaner-1.1.2/calcleaner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:56:48.052017 calcleaner-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-24 11:56:33.000000 calcleaner-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.871320 calcleaner-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 11:35:12.000000 calcleaner-1.1.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 11:35:12.000000 calcleaner-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-26 11:35:24.871320 calcleaner-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-26 11:35:12.000000 calcleaner-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.859320 calcleaner-1.1.3/calcleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/account_edit_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/accounts_manage_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/caldav_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/calendar_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.847320 calcleaner-1.1.3/calcleaner/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.867320 calcleaner-1.1.3/calcleaner/data/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/images/calcleaner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/images/calcleaner_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/images/calcleaner_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/images/calcleaner_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/images/calcleaner_64.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.847320 calcleaner-1.1.3/calcleaner/data/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.839320 calcleaner-1.1.3/calcleaner/data/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.867320 calcleaner-1.1.3/calcleaner/data/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-26 11:35:23.000000 calcleaner-1.1.3/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.839320 calcleaner-1.1.3/calcleaner/data/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.867320 calcleaner-1.1.3/calcleaner/data/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-26 11:35:23.000000 calcleaner-1.1.3/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.839320 calcleaner-1.1.3/calcleaner/data/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.867320 calcleaner-1.1.3/calcleaner/data/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-26 11:35:23.000000 calcleaner-1.1.3/calcleaner/data/locales/hr/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.847320 calcleaner-1.1.3/calcleaner/data/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.867320 calcleaner-1.1.3/calcleaner/data/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-26 11:35:23.000000 calcleaner-1.1.3/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.847320 calcleaner-1.1.3/calcleaner/data/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.871320 calcleaner-1.1.3/calcleaner/data/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-26 11:35:23.000000 calcleaner-1.1.3/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.847320 calcleaner-1.1.3/calcleaner/data/locales/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.871320 calcleaner-1.1.3/calcleaner/data/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-26 11:35:23.000000 calcleaner-1.1.3/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.847320 calcleaner-1.1.3/calcleaner/data/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.871320 calcleaner-1.1.3/calcleaner/data/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-26 11:35:23.000000 calcleaner-1.1.3/calcleaner/data/locales/tr/LC_MESSAGES/org.flozz.calcleaner.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.871320 calcleaner-1.1.3/calcleaner/data/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/style/calcleaner.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.871320 calcleaner-1.1.3/calcleaner/data/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/ui/account-edit-dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/ui/accounts-manage-dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data/ui/main-window.glade
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/data_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-26 11:35:12.000000 calcleaner-1.1.3/calcleaner/translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:35:24.867320 calcleaner-1.1.3/calcleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-26 11:35:24.000000 calcleaner-1.1.3/calcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 11:35:24.000000 calcleaner-1.1.3/calcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:35:24.000000 calcleaner-1.1.3/calcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 11:35:24.000000 calcleaner-1.1.3/calcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 11:35:24.000000 calcleaner-1.1.3/calcleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 11:35:24.000000 calcleaner-1.1.3/calcleaner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:35:24.871320 calcleaner-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-26 11:35:12.000000 calcleaner-1.1.3/setup.py
```

### Comparing `calcleaner-1.1.2/COPYING` & `calcleaner-1.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/PKG-INFO` & `calcleaner-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcleaner
-Version: 1.1.2
+Version: 1.1.3
 Summary: A simple graphical tool to purge old events from CalDAV calendars
 Home-page: https://calcleaner.flozz.org/
 Author: Fabien LOISON
 License: GPLv3
 Project-URL: Source Code, https://github.com/flozz/calcleaner
 Project-URL: Changelog, https://github.com/flozz/calcleaner#changelog
 Project-URL: Issues, https://github.com/flozz/calcleaner/issues
@@ -128,20 +128,16 @@
 
 
 Translating Calcleaner
 ~~~~~~~~~~~~~~~~~~~~~~
 
 If the software is not available in your language, you can help translate it.
 
-To translate Calcleaner, you can:
-
-* submit your translations using a Pull Request on Github,
-* or translate online using POEditor:
-
-  * → https://poeditor.com/join/project/He30lKMTwO
+To translate Calcleaner, you can submit your translations using a Pull Request
+on Github,
 
 Do not forget to add your name as the translation of the ``translator-credits``
 key (one name per line, e-mail is optional)::
 
     msgid "translator-credits"
     msgstr ""
     "John DOE\n"
@@ -243,14 +239,18 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` but not released yet):
 
   * Nothing yet ;)
 
+* **v1.1.3:**
+
+  * Added Turkish translation (@sabriunal, #8)
+
 * **v1.1.2:**
 
   * Added Croatian translation (@milotype, #7)
   * Added Python 3.11 support
 
 * **v1.1.1:**
```

### Comparing `calcleaner-1.1.2/README.rst` & `calcleaner-1.1.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -112,20 +112,16 @@
 
 
 Translating Calcleaner
 ~~~~~~~~~~~~~~~~~~~~~~
 
 If the software is not available in your language, you can help translate it.
 
-To translate Calcleaner, you can:
-
-* submit your translations using a Pull Request on Github,
-* or translate online using POEditor:
-
-  * → https://poeditor.com/join/project/He30lKMTwO
+To translate Calcleaner, you can submit your translations using a Pull Request
+on Github,
 
 Do not forget to add your name as the translation of the ``translator-credits``
 key (one name per line, e-mail is optional)::
 
     msgid "translator-credits"
     msgstr ""
     "John DOE\n"
@@ -227,14 +223,18 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` but not released yet):
 
   * Nothing yet ;)
 
+* **v1.1.3:**
+
+  * Added Turkish translation (@sabriunal, #8)
+
 * **v1.1.2:**
 
   * Added Croatian translation (@milotype, #7)
   * Added Python 3.11 support
 
 * **v1.1.1:**
```

### Comparing `calcleaner-1.1.2/calcleaner/about_dialog.py` & `calcleaner-1.1.3/calcleaner/about_dialog.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/account_edit_dialog.py` & `calcleaner-1.1.3/calcleaner/account_edit_dialog.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/accounts.py` & `calcleaner-1.1.3/calcleaner/accounts.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/accounts_manage_dialog.py` & `calcleaner-1.1.3/calcleaner/accounts_manage_dialog.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/application.py` & `calcleaner-1.1.3/calcleaner/application.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/caldav_helpers.py` & `calcleaner-1.1.3/calcleaner/caldav_helpers.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/calendar_store.py` & `calcleaner-1.1.3/calcleaner/calendar_store.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/images/calcleaner.svg` & `calcleaner-1.1.3/calcleaner/data/images/calcleaner.svg`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/images/calcleaner_128.png` & `calcleaner-1.1.3/calcleaner/data/images/calcleaner_128.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/images/calcleaner_256.png` & `calcleaner-1.1.3/calcleaner/data/images/calcleaner_256.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/images/calcleaner_32.png` & `calcleaner-1.1.3/calcleaner/data/images/calcleaner_32.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/images/calcleaner_64.png` & `calcleaner-1.1.3/calcleaner/data/images/calcleaner_64.png`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.3/calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.3/calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/locales/hr/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.3/calcleaner/data/locales/hr/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.3/calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.3/calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo` & `calcleaner-1.1.3/calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/ui/account-edit-dialog.glade` & `calcleaner-1.1.3/calcleaner/data/ui/account-edit-dialog.glade`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/ui/accounts-manage-dialog.glade` & `calcleaner-1.1.3/calcleaner/data/ui/accounts-manage-dialog.glade`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/data/ui/main-window.glade` & `calcleaner-1.1.3/calcleaner/data/ui/main-window.glade`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/main_window.py` & `calcleaner-1.1.3/calcleaner/main_window.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner/translation.py` & `calcleaner-1.1.3/calcleaner/translation.py`

 * *Files identical despite different names*

### Comparing `calcleaner-1.1.2/calcleaner.egg-info/PKG-INFO` & `calcleaner-1.1.3/calcleaner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcleaner
-Version: 1.1.2
+Version: 1.1.3
 Summary: A simple graphical tool to purge old events from CalDAV calendars
 Home-page: https://calcleaner.flozz.org/
 Author: Fabien LOISON
 License: GPLv3
 Project-URL: Source Code, https://github.com/flozz/calcleaner
 Project-URL: Changelog, https://github.com/flozz/calcleaner#changelog
 Project-URL: Issues, https://github.com/flozz/calcleaner/issues
@@ -128,20 +128,16 @@
 
 
 Translating Calcleaner
 ~~~~~~~~~~~~~~~~~~~~~~
 
 If the software is not available in your language, you can help translate it.
 
-To translate Calcleaner, you can:
-
-* submit your translations using a Pull Request on Github,
-* or translate online using POEditor:
-
-  * → https://poeditor.com/join/project/He30lKMTwO
+To translate Calcleaner, you can submit your translations using a Pull Request
+on Github,
 
 Do not forget to add your name as the translation of the ``translator-credits``
 key (one name per line, e-mail is optional)::
 
     msgid "translator-credits"
     msgstr ""
     "John DOE\n"
@@ -243,14 +239,18 @@
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` but not released yet):
 
   * Nothing yet ;)
 
+* **v1.1.3:**
+
+  * Added Turkish translation (@sabriunal, #8)
+
 * **v1.1.2:**
 
   * Added Croatian translation (@milotype, #7)
   * Added Python 3.11 support
 
 * **v1.1.1:**
```

### Comparing `calcleaner-1.1.2/calcleaner.egg-info/SOURCES.txt` & `calcleaner-1.1.3/calcleaner.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,11 +28,12 @@
 calcleaner/data/images/calcleaner_64.png
 calcleaner/data/locales/de/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/fr/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/hr/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/it/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/nl/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/locales/pt_BR/LC_MESSAGES/org.flozz.calcleaner.mo
+calcleaner/data/locales/tr/LC_MESSAGES/org.flozz.calcleaner.mo
 calcleaner/data/style/calcleaner.css
 calcleaner/data/ui/account-edit-dialog.glade
 calcleaner/data/ui/accounts-manage-dialog.glade
 calcleaner/data/ui/main-window.glade
```

### Comparing `calcleaner-1.1.2/setup.py` & `calcleaner-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 long_description = ""
 if os.path.isfile("README.rst"):
     long_description = open("README.rst", "r", encoding="UTF-8").read()
 
 
 setup(
     name="calcleaner",
-    version="1.1.2",
+    version="1.1.3",
     description="A simple graphical tool to purge old events from CalDAV calendars",
     url="https://calcleaner.flozz.org/",
     project_urls={
         "Source Code": "https://github.com/flozz/calcleaner",
         "Changelog": "https://github.com/flozz/calcleaner#changelog",
         "Issues": "https://github.com/flozz/calcleaner/issues",
         "Chat": "https://discord.gg/P77sWhuSs4",
```


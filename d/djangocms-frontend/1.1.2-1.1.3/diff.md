# Comparing `tmp/djangocms-frontend-1.1.2.tar.gz` & `tmp/djangocms-frontend-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-frontend-1.1.2.tar", last modified: Tue Apr 25 21:55:50 2023, max compression
+gzip compressed data, was "djangocms-frontend-1.1.3.tar", last modified: Fri May 26 17:21:32 2023, max compression
```

## Comparing `djangocms-frontend-1.1.2.tar` & `djangocms-frontend-1.1.3.tar`

### file list

```diff
@@ -1,686 +1,686 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.699537 djangocms-frontend-1.1.2/djangocms_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/background.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.711537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.711537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.735538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.735538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.755538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
--rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
--rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
--rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.787538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.787538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/bootstrap4_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/stale_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/icon_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/styled_link_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/
--rw-r--r--   0 runner    (1001) docker     (123)    93523 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/div_select.css
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/select2.css
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
--rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/html_container.html
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templatetags/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.699537 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33033 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/accordion/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/accordion/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/alert/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/alert/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/badge/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/badge/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/card/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/card/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/carousel/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/carousel/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/collapse/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/collapse/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/content/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/content/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/grid/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/grid/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/icon/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/icon/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/image/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/image/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/jumbotron/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/jumbotron/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/link/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/link/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/link/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/listgroup/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/listgroup/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/media/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/media/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/navigation/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/navigation/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/tabs/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/tabs/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/utilities/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/utilities/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/title.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.534249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.534249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.586250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/bootstrap4_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/stale_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/icon_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/styled_link_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    93571 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/div_select.css
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/html_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templatetags/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33033 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/tests/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/accordion/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/accordion/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/alert/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/alert/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/badge/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/badge/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/card/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/card/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/carousel/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/carousel/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/collapse/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/collapse/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/content/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/content/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/grid/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/grid/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/icon/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/icon/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/image/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/image/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/jumbotron/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/jumbotron/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/link/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/link/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/listgroup/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/listgroup/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/media/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/media/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/navigation/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/navigation/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/tabs/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/tabs/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/utilities/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/utilities/test_plugins.py
```

### Comparing `djangocms-frontend-1.1.2/LICENSE` & `djangocms-frontend-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/PKG-INFO` & `djangocms-frontend-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.2
+Version: 1.1.3
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.2/README.rst` & `djangocms-frontend-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/__init__.py` & `djangocms-frontend-1.1.3/djangocms_frontend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
  9. git push
 10. Assure that all tests pass on https://github.com/django-cms/djangocms-frontend/actions
 11. Create a new release on https://github.com/django-cms/djangocms-frontend/releases/new
 12. Publish the release when ready
 13. Github actions will publish the new package to pypi
 """
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
```

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/common/attributes.py` & `djangocms-frontend-1.1.3/djangocms_frontend/common/attributes.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/background.py` & `djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/background.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/responsive.py` & `djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/responsive.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/sizing.py` & `djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/sizing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/common/spacing.py` & `djangocms-frontend-1.1.3/djangocms_frontend/common/spacing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/common/title.py` & `djangocms-frontend-1.1.3/djangocms_frontend/common/title.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/constants.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/foundation6.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/constants.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/constants.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/foundation6.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/conf.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/conf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/fields.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/icon_tags.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/icon_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/cms_plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
     name = _("Picture / Image")
     module = _("Frontend")
 
     model = models.Image
     form = forms.ImageForm
 
+    text_enabled = True
+
     change_form_template = "djangocms_frontend/admin/image.html"
 
     fieldsets = [
         (
             None,
             {
                 "fields": (
```

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/apps.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/constants.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/helpers.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/views.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/constants.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/cms_plugins.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/forms.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html` & `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/fields.py` & `djangocms-frontend-1.1.3/djangocms_frontend/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.3/djangocms_frontend/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/helpers.py` & `djangocms-frontend-1.1.3/djangocms_frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/bootstrap4_migration.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/bootstrap4_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/frontend.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/base.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/frequency_analysis.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/migrate.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/migrate.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/stale_references.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/stale_references.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/sync_permissions.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/icon_migration.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/icon_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/management/styled_link_migration.py` & `djangocms-frontend-1.1.3/djangocms_frontend/management/styled_link_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/migrations/0001_initial.py` & `djangocms-frontend-1.1.3/djangocms_frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/models.py` & `djangocms-frontend-1.1.3/djangocms_frontend/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/settings.py` & `djangocms-frontend-1.1.3/djangocms_frontend/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/base.css`

 * *Files 0% similar despite different names*

```diff
@@ -2564,3283 +2564,3286 @@
 0000a030: 5f63 6f6c 735f 7873 202e 6669 656c 642d  _cols_xs .field-
 0000a040: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
 0000a050: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
 0000a060: 6d2d 726f 772e 6669 656c 642d 726f 775f  m-row.field-row_
 0000a070: 636f 6c73 5f78 7320 2e66 6965 6c64 426f  cols_xs .fieldBo
 0000a080: 787b 706f 7369 7469 6f6e 3a72 656c 6174  x{position:relat
 0000a090: 6976 653b 7769 6474 683a 3130 3070 7821  ive;width:100px!
-0000a0a0: 696d 706f 7274 616e 743b 7061 6464 696e  important;paddin
-0000a0b0: 673a 3135 7078 2031 3070 783b 6d61 7267  g:15px 10px;marg
-0000a0c0: 696e 3a30 2169 6d70 6f72 7461 6e74 3b62  in:0!important;b
-0000a0d0: 6f72 6465 722d 626f 7474 6f6d 3a31 7078  order-bottom:1px
-0000a0e0: 2073 6f6c 6964 2023 6565 653b 666c 6f61   solid #eee;floa
-0000a0f0: 743a 6c65 6674 2169 6d70 6f72 7461 6e74  t:left!important
-0000a100: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
-0000a110: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000a120: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
-0000a130: 735f 7873 202e 6669 656c 642d 626f 7820  s_xs .field-box 
-0000a140: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000a150: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000a160: 6f72 6d2d 726f 772e 6669 656c 642d 726f  orm-row.field-ro
-0000a170: 775f 636f 6c73 5f78 7320 2e66 6965 6c64  w_cols_xs .field
-0000a180: 426f 7820 696e 7075 747b 7465 7874 2d61  Box input{text-a
-0000a190: 6c69 676e 3a72 6967 6874 3b70 6164 6469  lign:right;paddi
-0000a1a0: 6e67 2d72 6967 6874 3a35 7078 2169 6d70  ng-right:5px!imp
-0000a1b0: 6f72 7461 6e74 3b62 6f78 2d73 697a 696e  ortant;box-sizin
-0000a1c0: 673a 626f 7264 6572 2d62 6f78 3b77 6964  g:border-box;wid
-0000a1d0: 7468 3a31 3030 257d 2e64 6a61 6e67 6f63  th:100%}.djangoc
-0000a1e0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000a1f0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000a200: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
-0000a210: 6c64 2d62 6f78 206c 6162 656c 2c2e 646a  ld-box label,.dj
-0000a220: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000a230: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000a240: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
-0000a250: 202e 6669 656c 6442 6f78 206c 6162 656c   .fieldBox label
-0000a260: 7b66 6f6e 742d 7369 7a65 3a31 3270 7821  {font-size:12px!
-0000a270: 696d 706f 7274 616e 743b 666f 6e74 2d77  important;font-w
-0000a280: 6569 6768 743a 3430 3021 696d 706f 7274  eight:400!import
-0000a290: 616e 743b 636f 6c6f 723a 2363 6363 2169  ant;color:#ccc!i
-0000a2a0: 6d70 6f72 7461 6e74 3b70 6f73 6974 696f  mportant;positio
-0000a2b0: 6e3a 6162 736f 6c75 7465 3b6c 6566 743a  n:absolute;left:
-0000a2c0: 3135 7078 3b62 6f74 746f 6d3a 3137 7078  15px;bottom:17px
-0000a2d0: 3b74 6578 742d 7472 616e 7366 6f72 6d3a  ;text-transform:
-0000a2e0: 6c6f 7765 7263 6173 657d 2e64 6a61 6e67  lowercase}.djang
-0000a2f0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000a300: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000a310: 642d 726f 775f 636f 6c73 5f78 7320 2e66  d-row_cols_xs .f
-0000a320: 6965 6c64 2d62 6f78 202e 6469 7361 626c  ield-box .disabl
-0000a330: 6564 2c2e 646a 616e 676f 636d 732d 6672  ed,.djangocms-fr
-0000a340: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-0000a350: 2d72 6f77 2e66 6965 6c64 2d72 6f77 5f63  -row.field-row_c
-0000a360: 6f6c 735f 7873 202e 6669 656c 6442 6f78  ols_xs .fieldBox
-0000a370: 202e 6469 7361 626c 6564 7b63 6f6c 6f72   .disabled{color
-0000a380: 3a23 6363 633b 6261 636b 6772 6f75 6e64  :#ccc;background
-0000a390: 3a23 6565 657d 2e64 6a61 6e67 6f63 6d73  :#eee}.djangocms
-0000a3a0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000a3b0: 6f72 6d2d 726f 772e 6669 656c 642d 726f  orm-row.field-ro
-0000a3c0: 775f 636f 6c73 5f78 7320 2e66 6965 6c64  w_cols_xs .field
-0000a3d0: 2d62 6f78 3a6c 6173 742d 6368 696c 642c  -box:last-child,
-0000a3e0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000a3f0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000a400: 772e 6669 656c 642d 726f 775f 636f 6c73  w.field-row_cols
-0000a410: 5f78 7320 2e66 6965 6c64 426f 783a 6c61  _xs .fieldBox:la
-0000a420: 7374 2d63 6869 6c64 7b62 6f72 6465 722d  st-child{border-
-0000a430: 7269 6768 743a 6e6f 6e65 7d2e 646a 616e  right:none}.djan
-0000a440: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000a450: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000a460: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
-0000a470: 6572 726f 7273 7b6d 6172 6769 6e2d 626f  errors{margin-bo
-0000a480: 7474 6f6d 3a30 7d2e 646a 616e 676f 636d  ttom:0}.djangocm
-0000a490: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000a4a0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d72  form-row.field-r
-0000a4b0: 6f77 5f63 6f6c 735f 7873 202e 6669 656c  ow_cols_xs .fiel
-0000a4c0: 642d 626f 782d 6c61 6265 6c7b 6469 7370  d-box-label{disp
-0000a4d0: 6c61 793a 2d6d 732d 666c 6578 626f 783b  lay:-ms-flexbox;
-0000a4e0: 6469 7370 6c61 793a 666c 6578 3b6d 6172  display:flex;mar
-0000a4f0: 6769 6e2d 746f 703a 6175 746f 3b63 6f6c  gin-top:auto;col
-0000a500: 6f72 3a23 3939 397d 2e64 6a61 6e67 6f63  or:#999}.djangoc
-0000a510: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000a520: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000a530: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
-0000a540: 6c64 2d62 6f78 2d6c 6162 656c 2061 7b77  ld-box-label a{w
-0000a550: 6964 7468 3a31 3030 253b 6d61 7267 696e  idth:100%;margin
-0000a560: 2d74 6f70 3a61 7574 6f7d 2e64 6a61 6e67  -top:auto}.djang
-0000a570: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000a580: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000a590: 642d 726f 775f 636f 6c73 5f78 7320 2e66  d-row_cols_xs .f
-0000a5a0: 6965 6c64 2d62 6f78 2d6c 6162 656c 202e  ield-box-label .
-0000a5b0: 6963 6f6e 7b70 6f73 6974 696f 6e3a 7265  icon{position:re
-0000a5c0: 6c61 7469 7665 3b74 6f70 3a33 7078 7d2e  lative;top:3px}.
-0000a5d0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000a5e0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000a5f0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000a600: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000a610: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000a620: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000a630: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000a640: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000a650: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000a660: 6d73 2c2e 646a 616e 676f 636d 732d 6672  ms,.djangocms-fr
-0000a670: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000a680: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000a690: 5f6f 6666 7365 742c 2e64 6a61 6e67 6f63  _offset,.djangoc
-0000a6a0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000a6b0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000a6c0: 6c64 2d78 735f 6f72 6465 722c 2e64 6a61  ld-xs_order,.dja
-0000a6d0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000a6e0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000a6f0: 656c 642d 7873 5f63 6f6c 2c2e 646a 616e  eld-xs_col,.djan
-0000a700: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000a710: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000a720: 6c64 2d78 735f 6d65 2c2e 646a 616e 676f  ld-xs_me,.django
-0000a730: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000a740: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000a750: 2d78 735f 6d73 2c2e 646a 616e 676f 636d  -xs_ms,.djangocm
-0000a760: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000a770: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000a780: 735f 6f66 6673 6574 2c2e 646a 616e 676f  s_offset,.django
-0000a790: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000a7a0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000a7b0: 2d78 735f 6f72 6465 727b 706f 7369 7469  -xs_order{positi
-0000a7c0: 6f6e 3a72 656c 6174 6976 653b 6469 7370  on:relative;disp
-0000a7d0: 6c61 793a 2d6d 732d 666c 6578 626f 783b  lay:-ms-flexbox;
-0000a7e0: 6469 7370 6c61 793a 666c 6578 3b70 6164  display:flex;pad
-0000a7f0: 6469 6e67 3a30 3b6d 696e 2d77 6964 7468  ding:0;min-width
-0000a800: 3a38 3030 7078 7d2e 646a 616e 676f 636d  :800px}.djangocm
-0000a810: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000a820: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000a830: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-0000a840: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
-0000a850: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000a860: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000a870: 735f 636f 6c20 2e66 6965 6c64 426f 782c  s_col .fieldBox,
-0000a880: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000a890: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000a8a0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000a8b0: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
-0000a8c0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000a8d0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000a8e0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000a8f0: 656c 6442 6f78 2c2e 646a 616e 676f 636d  eldBox,.djangocm
-0000a900: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000a910: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000a920: 642d 7873 5f6d 7320 2e66 6965 6c64 2d62  d-xs_ms .field-b
-0000a930: 6f78 2c2e 646a 616e 676f 636d 732d 6672  ox,.djangocms-fr
-0000a940: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000a950: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000a960: 5f6d 7320 2e66 6965 6c64 426f 782c 2e64  _ms .fieldBox,.d
-0000a970: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000a980: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000a990: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000a9a0: 6574 202e 6669 656c 642d 626f 782c 2e64  et .field-box,.d
-0000a9b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000a9c0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000a9d0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000a9e0: 6574 202e 6669 656c 6442 6f78 2c2e 646a  et .fieldBox,.dj
-0000a9f0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000aa00: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000aa10: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000aa20: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
-0000aa30: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000aa40: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000aa50: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
-0000aa60: 2e66 6965 6c64 426f 782c 2e64 6a61 6e67  .fieldBox,.djang
-0000aa70: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000aa80: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000aa90: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-0000aaa0: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
-0000aab0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000aac0: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000aad0: 6f6c 202e 6669 656c 6442 6f78 2c2e 646a  ol .fieldBox,.dj
-0000aae0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000aaf0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000ab00: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000ab10: 642d 626f 782c 2e64 6a61 6e67 6f63 6d73  d-box,.djangocms
-0000ab20: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000ab30: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000ab40: 5f6d 6520 2e66 6965 6c64 426f 782c 2e64  _me .fieldBox,.d
-0000ab50: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000ab60: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000ab70: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
-0000ab80: 6c64 2d62 6f78 2c2e 646a 616e 676f 636d  ld-box,.djangocm
-0000ab90: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000aba0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000abb0: 735f 6d73 202e 6669 656c 6442 6f78 2c2e  s_ms .fieldBox,.
-0000abc0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000abd0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000abe0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-0000abf0: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
-0000ac00: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000ac10: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000ac20: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000ac30: 6965 6c64 426f 782c 2e64 6a61 6e67 6f63  ieldBox,.djangoc
-0000ac40: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000ac50: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000ac60: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-0000ac70: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
-0000ac80: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000ac90: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000aca0: 7264 6572 202e 6669 656c 6442 6f78 7b70  rder .fieldBox{p
-0000acb0: 6f73 6974 696f 6e3a 7265 6c61 7469 7665  osition:relative
-0000acc0: 3b77 6964 7468 3a31 3030 7078 2169 6d70  ;width:100px!imp
-0000acd0: 6f72 7461 6e74 3b70 6164 6469 6e67 3a31  ortant;padding:1
-0000ace0: 3570 7820 3130 7078 3b6d 6172 6769 6e3a  5px 10px;margin:
-0000acf0: 3021 696d 706f 7274 616e 743b 626f 7264  0!important;bord
-0000ad00: 6572 2d62 6f74 746f 6d3a 3170 7820 736f  er-bottom:1px so
-0000ad10: 6c69 6420 2365 6565 3b66 6c6f 6174 3a6c  lid #eee;float:l
-0000ad20: 6566 7421 696d 706f 7274 616e 747d 2e64  eft!important}.d
-0000ad30: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000ad40: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000ad50: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000ad60: 2e66 6965 6c64 2d62 6f78 2069 6e70 7574  .field-box input
-0000ad70: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000ad80: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000ad90: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000ada0: 6f6c 202e 6669 656c 6442 6f78 2069 6e70  ol .fieldBox inp
-0000adb0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-0000adc0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000add0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000ade0: 5f6d 6520 2e66 6965 6c64 2d62 6f78 2069  _me .field-box i
-0000adf0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-0000ae00: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000ae10: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000ae20: 7873 5f6d 6520 2e66 6965 6c64 426f 7820  xs_me .fieldBox 
-0000ae30: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000ae40: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000ae50: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000ae60: 2d78 735f 6d73 202e 6669 656c 642d 626f  -xs_ms .field-bo
-0000ae70: 7820 696e 7075 742c 2e64 6a61 6e67 6f63  x input,.djangoc
-0000ae80: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000ae90: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000aea0: 6c64 2d78 735f 6d73 202e 6669 656c 6442  ld-xs_ms .fieldB
-0000aeb0: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
-0000aec0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000aed0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000aee0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000aef0: 6965 6c64 2d62 6f78 2069 6e70 7574 2c2e  ield-box input,.
-0000af00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000af10: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000af20: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
-0000af30: 7365 7420 2e66 6965 6c64 426f 7820 696e  set .fieldBox in
-0000af40: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-0000af50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000af60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000af70: 735f 6f72 6465 7220 2e66 6965 6c64 2d62  s_order .field-b
-0000af80: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
-0000af90: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000afa0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000afb0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000afc0: 656c 6442 6f78 2069 6e70 7574 2c2e 646a  eldBox input,.dj
-0000afd0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000afe0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000aff0: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-0000b000: 6c64 2d62 6f78 2069 6e70 7574 2c2e 646a  ld-box input,.dj
-0000b010: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b020: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000b030: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-0000b040: 6c64 426f 7820 696e 7075 742c 2e64 6a61  ldBox input,.dja
-0000b050: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000b060: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000b070: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-0000b080: 2d62 6f78 2069 6e70 7574 2c2e 646a 616e  -box input,.djan
-0000b090: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000b0a0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000b0b0: 6c64 2d78 735f 6d65 202e 6669 656c 6442  ld-xs_me .fieldB
-0000b0c0: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
-0000b0d0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000b0e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000b0f0: 2d78 735f 6d73 202e 6669 656c 642d 626f  -xs_ms .field-bo
-0000b100: 7820 696e 7075 742c 2e64 6a61 6e67 6f63  x input,.djangoc
-0000b110: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000b120: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000b130: 7873 5f6d 7320 2e66 6965 6c64 426f 7820  xs_ms .fieldBox 
-0000b140: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000b150: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000b160: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000b170: 5f6f 6666 7365 7420 2e66 6965 6c64 2d62  _offset .field-b
-0000b180: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
-0000b190: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000b1a0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000b1b0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000b1c0: 6442 6f78 2069 6e70 7574 2c2e 646a 616e  dBox input,.djan
-0000b1d0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000b1e0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000b1f0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000b200: 6c64 2d62 6f78 2069 6e70 7574 2c2e 646a  ld-box input,.dj
-0000b210: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b220: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000b230: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
-0000b240: 6965 6c64 426f 7820 696e 7075 747b 7465  ieldBox input{te
-0000b250: 7874 2d61 6c69 676e 3a72 6967 6874 3b70  xt-align:right;p
-0000b260: 6164 6469 6e67 2d72 6967 6874 3a35 7078  adding-right:5px
-0000b270: 2169 6d70 6f72 7461 6e74 3b62 6f78 2d73  !important;box-s
-0000b280: 697a 696e 673a 626f 7264 6572 2d62 6f78  izing:border-box
-0000b290: 3b77 6964 7468 3a31 3030 257d 2e64 6a61  ;width:100%}.dja
-0000b2a0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000b2b0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000b2c0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000b2d0: 6965 6c64 2d62 6f78 206c 6162 656c 2c2e  ield-box label,.
-0000b2e0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000b2f0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000b300: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000b310: 202e 6669 656c 6442 6f78 206c 6162 656c   .fieldBox label
-0000b320: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000b330: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000b340: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000b350: 6520 2e66 6965 6c64 2d62 6f78 206c 6162  e .field-box lab
-0000b360: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-0000b370: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000b380: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000b390: 5f6d 6520 2e66 6965 6c64 426f 7820 6c61  _me .fieldBox la
-0000b3a0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000b3b0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000b3c0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000b3d0: 735f 6d73 202e 6669 656c 642d 626f 7820  s_ms .field-box 
-0000b3e0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000b3f0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000b400: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000b410: 2d78 735f 6d73 202e 6669 656c 6442 6f78  -xs_ms .fieldBox
-0000b420: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000b430: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000b440: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000b450: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000b460: 6c64 2d62 6f78 206c 6162 656c 2c2e 646a  ld-box label,.dj
-0000b470: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b480: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000b490: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
-0000b4a0: 7420 2e66 6965 6c64 426f 7820 6c61 6265  t .fieldBox labe
-0000b4b0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000b4c0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000b4d0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000b4e0: 6f72 6465 7220 2e66 6965 6c64 2d62 6f78  order .field-box
-0000b4f0: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000b500: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000b510: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000b520: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-0000b530: 6442 6f78 206c 6162 656c 2c2e 646a 616e  dBox label,.djan
-0000b540: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000b550: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000b560: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-0000b570: 2d62 6f78 206c 6162 656c 2c2e 646a 616e  -box label,.djan
-0000b580: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000b590: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000b5a0: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-0000b5b0: 426f 7820 6c61 6265 6c2c 2e64 6a61 6e67  Box label,.djang
-0000b5c0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000b5d0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000b5e0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
-0000b5f0: 6f78 206c 6162 656c 2c2e 646a 616e 676f  ox label,.django
-0000b600: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000b610: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000b620: 2d78 735f 6d65 202e 6669 656c 6442 6f78  -xs_me .fieldBox
-0000b630: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000b640: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000b650: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000b660: 735f 6d73 202e 6669 656c 642d 626f 7820  s_ms .field-box 
-0000b670: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000b680: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000b690: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000b6a0: 5f6d 7320 2e66 6965 6c64 426f 7820 6c61  _ms .fieldBox la
-0000b6b0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000b6c0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000b6d0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000b6e0: 6666 7365 7420 2e66 6965 6c64 2d62 6f78  ffset .field-box
-0000b6f0: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000b700: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000b710: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000b720: 735f 6f66 6673 6574 202e 6669 656c 6442  s_offset .fieldB
-0000b730: 6f78 206c 6162 656c 2c2e 646a 616e 676f  ox label,.django
-0000b740: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000b750: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000b760: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
-0000b770: 2d62 6f78 206c 6162 656c 2c2e 646a 616e  -box label,.djan
-0000b780: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000b790: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000b7a0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000b7b0: 6c64 426f 7820 6c61 6265 6c7b 666f 6e74  ldBox label{font
-0000b7c0: 2d73 697a 653a 3132 7078 2169 6d70 6f72  -size:12px!impor
-0000b7d0: 7461 6e74 3b66 6f6e 742d 7765 6967 6874  tant;font-weight
-0000b7e0: 3a34 3030 2169 6d70 6f72 7461 6e74 3b63  :400!important;c
-0000b7f0: 6f6c 6f72 3a23 6363 6321 696d 706f 7274  olor:#ccc!import
-0000b800: 616e 743b 706f 7369 7469 6f6e 3a61 6273  ant;position:abs
-0000b810: 6f6c 7574 653b 6c65 6674 3a31 3570 783b  olute;left:15px;
-0000b820: 626f 7474 6f6d 3a31 3770 783b 7465 7874  bottom:17px;text
-0000b830: 2d74 7261 6e73 666f 726d 3a6c 6f77 6572  -transform:lower
-0000b840: 6361 7365 7d2e 646a 616e 676f 636d 732d  case}.djangocms-
-0000b850: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000b860: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000b870: 7873 5f63 6f6c 202e 6669 656c 642d 626f  xs_col .field-bo
-0000b880: 7820 2e64 6973 6162 6c65 642c 2e64 6a61  x .disabled,.dja
-0000b890: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000b8a0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000b8b0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000b8c0: 6965 6c64 426f 7820 2e64 6973 6162 6c65  ieldBox .disable
-0000b8d0: 642c 2e64 6a61 6e67 6f63 6d73 2d66 726f  d,.djangocms-fro
-0000b8e0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000b8f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000b900: 6d65 202e 6669 656c 642d 626f 7820 2e64  me .field-box .d
-0000b910: 6973 6162 6c65 642c 2e64 6a61 6e67 6f63  isabled,.djangoc
-0000b920: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000b930: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000b940: 6c64 2d78 735f 6d65 202e 6669 656c 6442  ld-xs_me .fieldB
-0000b950: 6f78 202e 6469 7361 626c 6564 2c2e 646a  ox .disabled,.dj
-0000b960: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b970: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000b980: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
-0000b990: 6965 6c64 2d62 6f78 202e 6469 7361 626c  ield-box .disabl
-0000b9a0: 6564 2c2e 646a 616e 676f 636d 732d 6672  ed,.djangocms-fr
-0000b9b0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000b9c0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000b9d0: 5f6d 7320 2e66 6965 6c64 426f 7820 2e64  _ms .fieldBox .d
-0000b9e0: 6973 6162 6c65 642c 2e64 6a61 6e67 6f63  isabled,.djangoc
-0000b9f0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000ba00: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000ba10: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000ba20: 656c 642d 626f 7820 2e64 6973 6162 6c65  eld-box .disable
-0000ba30: 642c 2e64 6a61 6e67 6f63 6d73 2d66 726f  d,.djangocms-fro
-0000ba40: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000ba50: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000ba60: 6f66 6673 6574 202e 6669 656c 6442 6f78  offset .fieldBox
-0000ba70: 202e 6469 7361 626c 6564 2c2e 646a 616e   .disabled,.djan
-0000ba80: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000ba90: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000baa0: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000bab0: 6669 656c 642d 626f 7820 2e64 6973 6162  field-box .disab
-0000bac0: 6c65 642c 2e64 6a61 6e67 6f63 6d73 2d66  led,.djangocms-f
-0000bad0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000bae0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000baf0: 735f 6f72 6465 7220 2e66 6965 6c64 426f  s_order .fieldBo
-0000bb00: 7820 2e64 6973 6162 6c65 642c 2e64 6a61  x .disabled,.dja
-0000bb10: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000bb20: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000bb30: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-0000bb40: 642d 626f 7820 2e64 6973 6162 6c65 642c  d-box .disabled,
-0000bb50: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000bb60: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000bb70: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-0000bb80: 6669 656c 6442 6f78 202e 6469 7361 626c  fieldBox .disabl
-0000bb90: 6564 2c2e 646a 616e 676f 636d 732d 6672  ed,.djangocms-fr
-0000bba0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-0000bbb0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000bbc0: 202e 6669 656c 642d 626f 7820 2e64 6973   .field-box .dis
-0000bbd0: 6162 6c65 642c 2e64 6a61 6e67 6f63 6d73  abled,.djangocms
-0000bbe0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000bbf0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000bc00: 5f6d 6520 2e66 6965 6c64 426f 7820 2e64  _me .fieldBox .d
-0000bc10: 6973 6162 6c65 642c 2e64 6a61 6e67 6f63  isabled,.djangoc
-0000bc20: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000bc30: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000bc40: 7873 5f6d 7320 2e66 6965 6c64 2d62 6f78  xs_ms .field-box
-0000bc50: 202e 6469 7361 626c 6564 2c2e 646a 616e   .disabled,.djan
-0000bc60: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000bc70: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000bc80: 6c64 2d78 735f 6d73 202e 6669 656c 6442  ld-xs_ms .fieldB
-0000bc90: 6f78 202e 6469 7361 626c 6564 2c2e 646a  ox .disabled,.dj
-0000bca0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000bcb0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000bcc0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
-0000bcd0: 6669 656c 642d 626f 7820 2e64 6973 6162  field-box .disab
-0000bce0: 6c65 642c 2e64 6a61 6e67 6f63 6d73 2d66  led,.djangocms-f
-0000bcf0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000bd00: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000bd10: 6666 7365 7420 2e66 6965 6c64 426f 7820  ffset .fieldBox 
-0000bd20: 2e64 6973 6162 6c65 642c 2e64 6a61 6e67  .disabled,.djang
-0000bd30: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000bd40: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000bd50: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-0000bd60: 642d 626f 7820 2e64 6973 6162 6c65 642c  d-box .disabled,
-0000bd70: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000bd80: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000bd90: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000bda0: 202e 6669 656c 6442 6f78 202e 6469 7361   .fieldBox .disa
-0000bdb0: 626c 6564 7b63 6f6c 6f72 3a23 6363 633b  bled{color:#ccc;
-0000bdc0: 6261 636b 6772 6f75 6e64 3a23 6565 657d  background:#eee}
-0000bdd0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000bde0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000bdf0: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000be00: 6c20 2e66 6965 6c64 2d62 6f78 3a6c 6173  l .field-box:las
-0000be10: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
-0000be20: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000be30: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000be40: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-0000be50: 426f 783a 6c61 7374 2d63 6869 6c64 2c2e  Box:last-child,.
-0000be60: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000be70: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000be80: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
-0000be90: 2e66 6965 6c64 2d62 6f78 3a6c 6173 742d  .field-box:last-
-0000bea0: 6368 696c 642c 2e64 6a61 6e67 6f63 6d73  child,.djangocms
-0000beb0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000bec0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000bed0: 2d78 735f 6d65 202e 6669 656c 6442 6f78  -xs_me .fieldBox
-0000bee0: 3a6c 6173 742d 6368 696c 642c 2e64 6a61  :last-child,.dja
-0000bef0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000bf00: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000bf10: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000bf20: 656c 642d 626f 783a 6c61 7374 2d63 6869  eld-box:last-chi
-0000bf30: 6c64 2c2e 646a 616e 676f 636d 732d 6672  ld,.djangocms-fr
-0000bf40: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000bf50: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000bf60: 5f6d 7320 2e66 6965 6c64 426f 783a 6c61  _ms .fieldBox:la
-0000bf70: 7374 2d63 6869 6c64 2c2e 646a 616e 676f  st-child,.django
-0000bf80: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000bf90: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000bfa0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000bfb0: 6965 6c64 2d62 6f78 3a6c 6173 742d 6368  ield-box:last-ch
-0000bfc0: 696c 642c 2e64 6a61 6e67 6f63 6d73 2d66  ild,.djangocms-f
-0000bfd0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000bfe0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000bff0: 735f 6f66 6673 6574 202e 6669 656c 6442  s_offset .fieldB
-0000c000: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
-0000c010: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c020: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000c030: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-0000c040: 7220 2e66 6965 6c64 2d62 6f78 3a6c 6173  r .field-box:las
-0000c050: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
-0000c060: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000c070: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000c080: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000c090: 6c64 426f 783a 6c61 7374 2d63 6869 6c64  ldBox:last-child
-0000c0a0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000c0b0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000c0c0: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000c0d0: 2e66 6965 6c64 2d62 6f78 3a6c 6173 742d  .field-box:last-
-0000c0e0: 6368 696c 642c 2e64 6a61 6e67 6f63 6d73  child,.djangocms
-0000c0f0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000c100: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000c110: 5f63 6f6c 202e 6669 656c 6442 6f78 3a6c  _col .fieldBox:l
-0000c120: 6173 742d 6368 696c 642c 2e64 6a61 6e67  ast-child,.djang
-0000c130: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000c140: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000c150: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
-0000c160: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
-0000c170: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c180: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000c190: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
-0000c1a0: 6c64 426f 783a 6c61 7374 2d63 6869 6c64  ldBox:last-child
-0000c1b0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000c1c0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000c1d0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000c1e0: 6669 656c 642d 626f 783a 6c61 7374 2d63  field-box:last-c
-0000c1f0: 6869 6c64 2c2e 646a 616e 676f 636d 732d  hild,.djangocms-
-0000c200: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000c210: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000c220: 6d73 202e 6669 656c 6442 6f78 3a6c 6173  ms .fieldBox:las
-0000c230: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
-0000c240: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000c250: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000c260: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
-0000c270: 2d62 6f78 3a6c 6173 742d 6368 696c 642c  -box:last-child,
-0000c280: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000c290: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000c2a0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
-0000c2b0: 7420 2e66 6965 6c64 426f 783a 6c61 7374  t .fieldBox:last
-0000c2c0: 2d63 6869 6c64 2c2e 646a 616e 676f 636d  -child,.djangocm
-0000c2d0: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000c2e0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000c2f0: 735f 6f72 6465 7220 2e66 6965 6c64 2d62  s_order .field-b
-0000c300: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
-0000c310: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c320: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000c330: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000c340: 6669 656c 6442 6f78 3a6c 6173 742d 6368  fieldBox:last-ch
-0000c350: 696c 647b 626f 7264 6572 2d72 6967 6874  ild{border-right
-0000c360: 3a6e 6f6e 657d 2e64 6a61 6e67 6f63 6d73  :none}.djangocms
-0000c370: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000c380: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000c390: 2d78 735f 636f 6c20 2e65 7272 6f72 732c  -xs_col .errors,
-0000c3a0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000c3b0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000c3c0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000c3d0: 202e 6572 726f 7273 2c2e 646a 616e 676f   .errors,.django
-0000c3e0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000c3f0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000c400: 656c 642d 7873 5f6d 7320 2e65 7272 6f72  eld-xs_ms .error
-0000c410: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000c420: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000c430: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000c440: 6f66 6673 6574 202e 6572 726f 7273 2c2e  offset .errors,.
-0000c450: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000c460: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000c470: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-0000c480: 6572 202e 6572 726f 7273 2c2e 646a 616e  er .errors,.djan
-0000c490: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000c4a0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000c4b0: 6c64 2d78 735f 636f 6c20 2e65 7272 6f72  ld-xs_col .error
-0000c4c0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000c4d0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000c4e0: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
-0000c4f0: 2e65 7272 6f72 732c 2e64 6a61 6e67 6f63  .errors,.djangoc
-0000c500: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000c510: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000c520: 7873 5f6d 7320 2e65 7272 6f72 732c 2e64  xs_ms .errors,.d
-0000c530: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c540: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000c550: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
-0000c560: 2e65 7272 6f72 732c 2e64 6a61 6e67 6f63  .errors,.djangoc
-0000c570: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000c580: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000c590: 7873 5f6f 7264 6572 202e 6572 726f 7273  xs_order .errors
-0000c5a0: 7b6d 6172 6769 6e2d 626f 7474 6f6d 3a30  {margin-bottom:0
-0000c5b0: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
-0000c5c0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000c5d0: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000c5e0: 6f6c 202e 6572 726f 726c 6973 742c 2e64  ol .errorlist,.d
-0000c5f0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c600: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000c610: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
-0000c620: 6572 726f 726c 6973 742c 2e64 6a61 6e67  errorlist,.djang
-0000c630: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000c640: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000c650: 6965 6c64 2d78 735f 6d73 202e 6572 726f  ield-xs_ms .erro
-0000c660: 726c 6973 742c 2e64 6a61 6e67 6f63 6d73  rlist,.djangocms
-0000c670: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000c680: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000c690: 2d78 735f 6f66 6673 6574 202e 6572 726f  -xs_offset .erro
-0000c6a0: 726c 6973 742c 2e64 6a61 6e67 6f63 6d73  rlist,.djangocms
-0000c6b0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000c6c0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000c6d0: 2d78 735f 6f72 6465 7220 2e65 7272 6f72  -xs_order .error
-0000c6e0: 6c69 7374 2c2e 646a 616e 676f 636d 732d  list,.djangocms-
-0000c6f0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000c700: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000c710: 636f 6c20 2e65 7272 6f72 6c69 7374 2c2e  col .errorlist,.
-0000c720: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000c730: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000c740: 2e66 6965 6c64 2d78 735f 6d65 202e 6572  .field-xs_me .er
-0000c750: 726f 726c 6973 742c 2e64 6a61 6e67 6f63  rorlist,.djangoc
-0000c760: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000c770: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000c780: 7873 5f6d 7320 2e65 7272 6f72 6c69 7374  xs_ms .errorlist
-0000c790: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000c7a0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000c7b0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000c7c0: 6574 202e 6572 726f 726c 6973 742c 2e64  et .errorlist,.d
-0000c7d0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c7e0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000c7f0: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000c800: 6572 726f 726c 6973 747b 706f 7369 7469  errorlist{positi
-0000c810: 6f6e 3a61 6273 6f6c 7574 6521 696d 706f  on:absolute!impo
-0000c820: 7274 616e 743b 7769 6474 683a 3170 7821  rtant;width:1px!
-0000c830: 696d 706f 7274 616e 743b 6865 6967 6874  important;height
-0000c840: 3a31 7078 2169 6d70 6f72 7461 6e74 3b70  :1px!important;p
-0000c850: 6164 6469 6e67 3a30 2169 6d70 6f72 7461  adding:0!importa
-0000c860: 6e74 3b6d 6172 6769 6e3a 2d31 7078 2169  nt;margin:-1px!i
-0000c870: 6d70 6f72 7461 6e74 3b6f 7665 7266 6c6f  mportant;overflo
-0000c880: 773a 6869 6464 656e 2169 6d70 6f72 7461  w:hidden!importa
-0000c890: 6e74 3b63 6c69 703a 7265 6374 2830 2c30  nt;clip:rect(0,0
-0000c8a0: 2c30 2c30 2921 696d 706f 7274 616e 743b  ,0,0)!important;
-0000c8b0: 7768 6974 652d 7370 6163 653a 6e6f 7772  white-space:nowr
-0000c8c0: 6170 2169 6d70 6f72 7461 6e74 3b62 6f72  ap!important;bor
-0000c8d0: 6465 723a 3021 696d 706f 7274 616e 747d  der:0!important}
-0000c8e0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000c8f0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000c900: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000c910: 6c2e 6669 656c 642d 7873 5f6d 6520 2e66  l.field-xs_me .f
-0000c920: 6965 6c64 2d62 6f78 2c2e 646a 616e 676f  ield-box,.django
-0000c930: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000c940: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000c950: 656c 642d 7873 5f6d 652e 6669 656c 642d  eld-xs_me.field-
-0000c960: 7873 5f6d 6520 2e66 6965 6c64 2d62 6f78  xs_me .field-box
-0000c970: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000c980: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000c990: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000c9a0: 732e 6669 656c 642d 7873 5f6d 6520 2e66  s.field-xs_me .f
-0000c9b0: 6965 6c64 2d62 6f78 2c2e 646a 616e 676f  ield-box,.django
-0000c9c0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000c9d0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000c9e0: 656c 642d 7873 5f6f 6666 7365 742e 6669  eld-xs_offset.fi
-0000c9f0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-0000ca00: 2d62 6f78 2c2e 646a 616e 676f 636d 732d  -box,.djangocms-
-0000ca10: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000ca20: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000ca30: 7873 5f6f 7264 6572 2e66 6965 6c64 2d78  xs_order.field-x
-0000ca40: 735f 6d65 202e 6669 656c 642d 626f 782c  s_me .field-box,
-0000ca50: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000ca60: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000ca70: 772e 6669 656c 642d 7873 5f63 6f6c 2e66  w.field-xs_col.f
-0000ca80: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000ca90: 642d 626f 782c 2e64 6a61 6e67 6f63 6d73  d-box,.djangocms
-0000caa0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000cab0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000cac0: 5f6d 652e 6669 656c 642d 7873 5f6d 6520  _me.field-xs_me 
-0000cad0: 2e66 6965 6c64 2d62 6f78 2c2e 646a 616e  .field-box,.djan
-0000cae0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000caf0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000cb00: 6c64 2d78 735f 6d73 2e66 6965 6c64 2d78  ld-xs_ms.field-x
-0000cb10: 735f 6d65 202e 6669 656c 642d 626f 782c  s_me .field-box,
-0000cb20: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000cb30: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000cb40: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
-0000cb50: 742e 6669 656c 642d 7873 5f6d 6520 2e66  t.field-xs_me .f
-0000cb60: 6965 6c64 2d62 6f78 2c2e 646a 616e 676f  ield-box,.django
-0000cb70: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000cb80: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000cb90: 2d78 735f 6f72 6465 722e 6669 656c 642d  -xs_order.field-
-0000cba0: 7873 5f6d 6520 2e66 6965 6c64 2d62 6f78  xs_me .field-box
-0000cbb0: 7b62 6f72 6465 722d 626f 7474 6f6d 3a6e  {border-bottom:n
-0000cbc0: 6f6e 657d 2e64 6a61 6e67 6f63 6d73 2d66  one}.djangocms-f
-0000cbd0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000cbe0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000cbf0: 735f 636f 6c20 2e66 6965 6c64 2d62 6f78  s_col .field-box
-0000cc00: 2d6c 6162 656c 2c2e 646a 616e 676f 636d  -label,.djangocm
-0000cc10: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000cc20: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000cc30: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
-0000cc40: 6f78 2d6c 6162 656c 2c2e 646a 616e 676f  ox-label,.django
-0000cc50: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000cc60: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000cc70: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
-0000cc80: 2d62 6f78 2d6c 6162 656c 2c2e 646a 616e  -box-label,.djan
-0000cc90: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000cca0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000ccb0: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
-0000ccc0: 2e66 6965 6c64 2d62 6f78 2d6c 6162 656c  .field-box-label
-0000ccd0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000cce0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000ccf0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000cd00: 7264 6572 202e 6669 656c 642d 626f 782d  rder .field-box-
-0000cd10: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000cd20: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000cd30: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000cd40: 5f63 6f6c 202e 6669 656c 642d 626f 782d  _col .field-box-
-0000cd50: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000cd60: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000cd70: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000cd80: 5f6d 6520 2e66 6965 6c64 2d62 6f78 2d6c  _me .field-box-l
-0000cd90: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000cda0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000cdb0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000cdc0: 6d73 202e 6669 656c 642d 626f 782d 6c61  ms .field-box-la
-0000cdd0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000cde0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000cdf0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000ce00: 6666 7365 7420 2e66 6965 6c64 2d62 6f78  ffset .field-box
-0000ce10: 2d6c 6162 656c 2c2e 646a 616e 676f 636d  -label,.djangocm
-0000ce20: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000ce30: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000ce40: 735f 6f72 6465 7220 2e66 6965 6c64 2d62  s_order .field-b
-0000ce50: 6f78 2d6c 6162 656c 7b64 6973 706c 6179  ox-label{display
-0000ce60: 3a2d 6d73 2d66 6c65 7862 6f78 3b64 6973  :-ms-flexbox;dis
-0000ce70: 706c 6179 3a66 6c65 783b 6d61 7267 696e  play:flex;margin
-0000ce80: 2d74 6f70 3a61 7574 6f3b 636f 6c6f 723a  -top:auto;color:
-0000ce90: 2339 3939 7d2e 646a 616e 676f 636d 732d  #999}.djangocms-
-0000cea0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000ceb0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000cec0: 7873 5f63 6f6c 202e 6669 656c 642d 626f  xs_col .field-bo
-0000ced0: 782d 6c61 6265 6c20 612c 2e64 6a61 6e67  x-label a,.djang
-0000cee0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000cef0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000cf00: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000cf10: 642d 626f 782d 6c61 6265 6c20 612c 2e64  d-box-label a,.d
-0000cf20: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000cf30: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000cf40: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000cf50: 6669 656c 642d 626f 782d 6c61 6265 6c20  field-box-label 
-0000cf60: 612c 2e64 6a61 6e67 6f63 6d73 2d66 726f  a,.djangocms-fro
-0000cf70: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000cf80: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000cf90: 6f66 6673 6574 202e 6669 656c 642d 626f  offset .field-bo
-0000cfa0: 782d 6c61 6265 6c20 612c 2e64 6a61 6e67  x-label a,.djang
-0000cfb0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000cfc0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000cfd0: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
-0000cfe0: 6965 6c64 2d62 6f78 2d6c 6162 656c 2061  ield-box-label a
-0000cff0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000d000: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000d010: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000d020: 2e66 6965 6c64 2d62 6f78 2d6c 6162 656c  .field-box-label
-0000d030: 2061 2c2e 646a 616e 676f 636d 732d 6672   a,.djangocms-fr
-0000d040: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-0000d050: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000d060: 202e 6669 656c 642d 626f 782d 6c61 6265   .field-box-labe
-0000d070: 6c20 612c 2e64 6a61 6e67 6f63 6d73 2d66  l a,.djangocms-f
-0000d080: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000d090: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000d0a0: 7320 2e66 6965 6c64 2d62 6f78 2d6c 6162  s .field-box-lab
-0000d0b0: 656c 2061 2c2e 646a 616e 676f 636d 732d  el a,.djangocms-
-0000d0c0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000d0d0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000d0e0: 6f66 6673 6574 202e 6669 656c 642d 626f  offset .field-bo
-0000d0f0: 782d 6c61 6265 6c20 612c 2e64 6a61 6e67  x-label a,.djang
-0000d100: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000d110: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000d120: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-0000d130: 642d 626f 782d 6c61 6265 6c20 617b 7769  d-box-label a{wi
-0000d140: 6474 683a 3130 3025 3b6d 6172 6769 6e2d  dth:100%;margin-
-0000d150: 746f 703a 6175 746f 7d2e 646a 616e 676f  top:auto}.django
-0000d160: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000d170: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000d180: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-0000d190: 642d 626f 782d 6c61 6265 6c20 2e69 636f  d-box-label .ico
-0000d1a0: 6e2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  n,.djangocms-fro
-0000d1b0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000d1c0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000d1d0: 6d65 202e 6669 656c 642d 626f 782d 6c61  me .field-box-la
-0000d1e0: 6265 6c20 2e69 636f 6e2c 2e64 6a61 6e67  bel .icon,.djang
-0000d1f0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000d200: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000d210: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-0000d220: 642d 626f 782d 6c61 6265 6c20 2e69 636f  d-box-label .ico
-0000d230: 6e2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  n,.djangocms-fro
-0000d240: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000d250: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000d260: 6f66 6673 6574 202e 6669 656c 642d 626f  offset .field-bo
-0000d270: 782d 6c61 6265 6c20 2e69 636f 6e2c 2e64  x-label .icon,.d
-0000d280: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000d290: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000d2a0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-0000d2b0: 7220 2e66 6965 6c64 2d62 6f78 2d6c 6162  r .field-box-lab
-0000d2c0: 656c 202e 6963 6f6e 2c2e 646a 616e 676f  el .icon,.django
-0000d2d0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000d2e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000d2f0: 2d78 735f 636f 6c20 2e66 6965 6c64 2d62  -xs_col .field-b
-0000d300: 6f78 2d6c 6162 656c 202e 6963 6f6e 2c2e  ox-label .icon,.
-0000d310: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000d320: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000d330: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000d340: 656c 642d 626f 782d 6c61 6265 6c20 2e69  eld-box-label .i
-0000d350: 636f 6e2c 2e64 6a61 6e67 6f63 6d73 2d66  con,.djangocms-f
-0000d360: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000d370: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000d380: 7320 2e66 6965 6c64 2d62 6f78 2d6c 6162  s .field-box-lab
-0000d390: 656c 202e 6963 6f6e 2c2e 646a 616e 676f  el .icon,.django
-0000d3a0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000d3b0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000d3c0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000d3d0: 642d 626f 782d 6c61 6265 6c20 2e69 636f  d-box-label .ico
-0000d3e0: 6e2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  n,.djangocms-fro
-0000d3f0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000d400: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-0000d410: 6572 202e 6669 656c 642d 626f 782d 6c61  er .field-box-la
-0000d420: 6265 6c20 2e69 636f 6e7b 706f 7369 7469  bel .icon{positi
-0000d430: 6f6e 3a72 656c 6174 6976 653b 746f 703a  on:relative;top:
-0000d440: 3370 787d 2e64 6a61 6e67 6f63 6d73 2d66  3px}.djangocms-f
-0000d450: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000d460: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000d470: 735f 636f 6c20 2e66 6965 6c64 2d6c 675f  s_col .field-lg_
-0000d480: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
-0000d490: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000d4a0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000d4b0: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
-0000d4c0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000d4d0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000d4e0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000d4f0: 636f 6c20 2e66 6965 6c64 2d6d 645f 6d65  col .field-md_me
-0000d500: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000d510: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000d520: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000d530: 6f6c 202e 6669 656c 642d 6d64 5f6d 732c  ol .field-md_ms,
-0000d540: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000d550: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000d560: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000d570: 6c20 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  l .field-sm_me,.
-0000d580: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000d590: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000d5a0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000d5b0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
-0000d5c0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000d5d0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000d5e0: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000d5f0: 2e66 6965 6c64 2d78 6c5f 6d65 2c2e 646a  .field-xl_me,.dj
-0000d600: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000d610: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000d620: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-0000d630: 6669 656c 642d 786c 5f6d 732c 2e64 6a61  field-xl_ms,.dja
-0000d640: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000d650: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000d660: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000d670: 6965 6c64 2d78 735f 6d65 2c2e 646a 616e  ield-xs_me,.djan
-0000d680: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000d690: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000d6a0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-0000d6b0: 656c 642d 7873 5f6d 732c 2e64 6a61 6e67  eld-xs_ms,.djang
-0000d6c0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000d6d0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000d6e0: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-0000d6f0: 6c64 2d78 786c 5f6d 652c 2e64 6a61 6e67  ld-xxl_me,.djang
-0000d700: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000d710: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000d720: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-0000d730: 6c64 2d78 786c 5f6d 732c 2e64 6a61 6e67  ld-xxl_ms,.djang
-0000d740: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000d750: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000d760: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000d770: 642d 6c67 5f6d 652c 2e64 6a61 6e67 6f63  d-lg_me,.djangoc
-0000d780: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000d790: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000d7a0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000d7b0: 6c67 5f6d 732c 2e64 6a61 6e67 6f63 6d73  lg_ms,.djangocms
-0000d7c0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000d7d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000d7e0: 2d78 735f 6d65 202e 6669 656c 642d 6d64  -xs_me .field-md
-0000d7f0: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
-0000d800: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000d810: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000d820: 735f 6d65 202e 6669 656c 642d 6d64 5f6d  s_me .field-md_m
-0000d830: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000d840: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000d850: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000d860: 6d65 202e 6669 656c 642d 736d 5f6d 652c  me .field-sm_me,
-0000d870: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000d880: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000d890: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000d8a0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
-0000d8b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000d8c0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000d8d0: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
-0000d8e0: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
-0000d8f0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000d900: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000d910: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000d920: 656c 642d 786c 5f6d 732c 2e64 6a61 6e67  eld-xl_ms,.djang
-0000d930: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000d940: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000d950: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000d960: 642d 7873 5f6d 652c 2e64 6a61 6e67 6f63  d-xs_me,.djangoc
-0000d970: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000d980: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000d990: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000d9a0: 7873 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xs_ms,.djangocms
-0000d9b0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000d9c0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000d9d0: 2d78 735f 6d65 202e 6669 656c 642d 7878  -xs_me .field-xx
-0000d9e0: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
-0000d9f0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000da00: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000da10: 7873 5f6d 6520 2e66 6965 6c64 2d78 786c  xs_me .field-xxl
-0000da20: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000da30: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000da40: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000da50: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
-0000da60: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000da70: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000da80: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000da90: 6d73 202e 6669 656c 642d 6c67 5f6d 732c  ms .field-lg_ms,
-0000daa0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000dab0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000dac0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000dad0: 202e 6669 656c 642d 6d64 5f6d 652c 2e64   .field-md_me,.d
-0000dae0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000daf0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000db00: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000db10: 6669 656c 642d 6d64 5f6d 732c 2e64 6a61  field-md_ms,.dja
-0000db20: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000db30: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000db40: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000db50: 656c 642d 736d 5f6d 652c 2e64 6a61 6e67  eld-sm_me,.djang
-0000db60: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000db70: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000db80: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-0000db90: 642d 736d 5f6d 732c 2e64 6a61 6e67 6f63  d-sm_ms,.djangoc
-0000dba0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000dbb0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000dbc0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
-0000dbd0: 786c 5f6d 652c 2e64 6a61 6e67 6f63 6d73  xl_me,.djangocms
-0000dbe0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000dbf0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000dc00: 2d78 735f 6d73 202e 6669 656c 642d 786c  -xs_ms .field-xl
-0000dc10: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000dc20: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000dc30: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000dc40: 735f 6d73 202e 6669 656c 642d 7873 5f6d  s_ms .field-xs_m
-0000dc50: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000dc60: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000dc70: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000dc80: 6d73 202e 6669 656c 642d 7873 5f6d 732c  ms .field-xs_ms,
-0000dc90: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000dca0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000dcb0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000dcc0: 202e 6669 656c 642d 7878 6c5f 6d65 2c2e   .field-xxl_me,.
-0000dcd0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000dce0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000dcf0: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
-0000dd00: 2e66 6965 6c64 2d78 786c 5f6d 732c 2e64  .field-xxl_ms,.d
-0000dd10: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000dd20: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000dd30: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000dd40: 6574 202e 6669 656c 642d 6c67 5f6d 652c  et .field-lg_me,
-0000dd50: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000dd60: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000dd70: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000dd80: 6673 6574 202e 6669 656c 642d 6c67 5f6d  fset .field-lg_m
-0000dd90: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000dda0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000ddb0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000ddc0: 6f66 6673 6574 202e 6669 656c 642d 6d64  offset .field-md
-0000ddd0: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
-0000dde0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000ddf0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000de00: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-0000de10: 6d64 5f6d 732c 2e64 6a61 6e67 6f63 6d73  md_ms,.djangocms
-0000de20: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000de30: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000de40: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000de50: 642d 736d 5f6d 652c 2e64 6a61 6e67 6f63  d-sm_me,.djangoc
-0000de60: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000de70: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000de80: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000de90: 656c 642d 736d 5f6d 732c 2e64 6a61 6e67  eld-sm_ms,.djang
-0000dea0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000deb0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000dec0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
-0000ded0: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
-0000dee0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000def0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000df00: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-0000df10: 202e 6669 656c 642d 786c 5f6d 732c 2e64   .field-xl_ms,.d
-0000df20: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000df30: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000df40: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000df50: 6574 202e 6669 656c 642d 7873 5f6d 652c  et .field-xs_me,
-0000df60: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000df70: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000df80: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000df90: 6673 6574 202e 6669 656c 642d 7873 5f6d  fset .field-xs_m
-0000dfa0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000dfb0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000dfc0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000dfd0: 6f66 6673 6574 202e 6669 656c 642d 7878  offset .field-xx
-0000dfe0: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
-0000dff0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000e000: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000e010: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
-0000e020: 2d78 786c 5f6d 732c 2e64 6a61 6e67 6f63  -xxl_ms,.djangoc
-0000e030: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000e040: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000e050: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000e060: 6c64 2d6c 675f 6d65 2c2e 646a 616e 676f  ld-lg_me,.django
-0000e070: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000e080: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000e090: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000e0a0: 656c 642d 6c67 5f6d 732c 2e64 6a61 6e67  eld-lg_ms,.djang
-0000e0b0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000e0c0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000e0d0: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
-0000e0e0: 6965 6c64 2d6d 645f 6d65 2c2e 646a 616e  ield-md_me,.djan
-0000e0f0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000e100: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000e110: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000e120: 6669 656c 642d 6d64 5f6d 732c 2e64 6a61  field-md_ms,.dja
-0000e130: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000e140: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000e150: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
-0000e160: 2e66 6965 6c64 2d73 6d5f 6d65 2c2e 646a  .field-sm_me,.dj
-0000e170: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000e180: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000e190: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000e1a0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
-0000e1b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e1c0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000e1d0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-0000e1e0: 7220 2e66 6965 6c64 2d78 6c5f 6d65 2c2e  r .field-xl_me,.
-0000e1f0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000e200: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000e210: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-0000e220: 6572 202e 6669 656c 642d 786c 5f6d 732c  er .field-xl_ms,
-0000e230: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000e240: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000e250: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
-0000e260: 6465 7220 2e66 6965 6c64 2d78 735f 6d65  der .field-xs_me
-0000e270: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000e280: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000e290: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000e2a0: 7264 6572 202e 6669 656c 642d 7873 5f6d  rder .field-xs_m
-0000e2b0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000e2c0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000e2d0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000e2e0: 6f72 6465 7220 2e66 6965 6c64 2d78 786c  order .field-xxl
-0000e2f0: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
-0000e300: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000e310: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000e320: 735f 6f72 6465 7220 2e66 6965 6c64 2d78  s_order .field-x
-0000e330: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
-0000e340: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000e350: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000e360: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
-0000e370: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000e380: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000e390: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000e3a0: 202e 6669 656c 642d 6c67 5f6d 732c 2e64   .field-lg_ms,.d
-0000e3b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e3c0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000e3d0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-0000e3e0: 656c 642d 6d64 5f6d 652c 2e64 6a61 6e67  eld-md_me,.djang
-0000e3f0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000e400: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000e410: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-0000e420: 6d64 5f6d 732c 2e64 6a61 6e67 6f63 6d73  md_ms,.djangocms
-0000e430: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000e440: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000e450: 5f63 6f6c 202e 6669 656c 642d 736d 5f6d  _col .field-sm_m
-0000e460: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000e470: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000e480: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000e490: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
-0000e4a0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e4b0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000e4c0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-0000e4d0: 656c 642d 786c 5f6d 652c 2e64 6a61 6e67  eld-xl_me,.djang
-0000e4e0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000e4f0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000e500: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-0000e510: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
-0000e520: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000e530: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000e540: 5f63 6f6c 202e 6669 656c 642d 7873 5f6d  _col .field-xs_m
-0000e550: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000e560: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000e570: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000e580: 202e 6669 656c 642d 7873 5f6d 732c 2e64   .field-xs_ms,.d
-0000e590: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e5a0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000e5b0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-0000e5c0: 656c 642d 7878 6c5f 6d65 2c2e 646a 616e  eld-xxl_me,.djan
-0000e5d0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000e5e0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000e5f0: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-0000e600: 2d78 786c 5f6d 732c 2e64 6a61 6e67 6f63  -xxl_ms,.djangoc
-0000e610: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000e620: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000e630: 7873 5f6d 6520 2e66 6965 6c64 2d6c 675f  xs_me .field-lg_
-0000e640: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
-0000e650: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-0000e660: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000e670: 202e 6669 656c 642d 6c67 5f6d 732c 2e64   .field-lg_ms,.d
-0000e680: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e690: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000e6a0: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
-0000e6b0: 6c64 2d6d 645f 6d65 2c2e 646a 616e 676f  ld-md_me,.django
-0000e6c0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000e6d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000e6e0: 2d78 735f 6d65 202e 6669 656c 642d 6d64  -xs_me .field-md
-0000e6f0: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000e700: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000e710: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000e720: 6520 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  e .field-sm_me,.
-0000e730: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000e740: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000e750: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000e760: 656c 642d 736d 5f6d 732c 2e64 6a61 6e67  eld-sm_ms,.djang
-0000e770: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000e780: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000e790: 642d 7873 5f6d 6520 2e66 6965 6c64 2d78  d-xs_me .field-x
-0000e7a0: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
-0000e7b0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000e7c0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000e7d0: 6d65 202e 6669 656c 642d 786c 5f6d 732c  me .field-xl_ms,
-0000e7e0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000e7f0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000e800: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
-0000e810: 6965 6c64 2d78 735f 6d65 2c2e 646a 616e  ield-xs_me,.djan
-0000e820: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000e830: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000e840: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000e850: 7873 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xs_ms,.djangocms
-0000e860: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000e870: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000e880: 5f6d 6520 2e66 6965 6c64 2d78 786c 5f6d  _me .field-xxl_m
-0000e890: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000e8a0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000e8b0: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
-0000e8c0: 2e66 6965 6c64 2d78 786c 5f6d 732c 2e64  .field-xxl_ms,.d
-0000e8d0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e8e0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000e8f0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
-0000e900: 6c64 2d6c 675f 6d65 2c2e 646a 616e 676f  ld-lg_me,.django
-0000e910: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000e920: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000e930: 2d78 735f 6d73 202e 6669 656c 642d 6c67  -xs_ms .field-lg
-0000e940: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000e950: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000e960: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000e970: 7320 2e66 6965 6c64 2d6d 645f 6d65 2c2e  s .field-md_me,.
-0000e980: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000e990: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000e9a0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000e9b0: 656c 642d 6d64 5f6d 732c 2e64 6a61 6e67  eld-md_ms,.djang
-0000e9c0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000e9d0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000e9e0: 642d 7873 5f6d 7320 2e66 6965 6c64 2d73  d-xs_ms .field-s
-0000e9f0: 6d5f 6d65 2c2e 646a 616e 676f 636d 732d  m_me,.djangocms-
-0000ea00: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000ea10: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000ea20: 6d73 202e 6669 656c 642d 736d 5f6d 732c  ms .field-sm_ms,
-0000ea30: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000ea40: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000ea50: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
-0000ea60: 6965 6c64 2d78 6c5f 6d65 2c2e 646a 616e  ield-xl_me,.djan
-0000ea70: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000ea80: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000ea90: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
-0000eaa0: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
-0000eab0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000eac0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000ead0: 5f6d 7320 2e66 6965 6c64 2d78 735f 6d65  _ms .field-xs_me
-0000eae0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000eaf0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000eb00: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000eb10: 6669 656c 642d 7873 5f6d 732c 2e64 6a61  field-xs_ms,.dja
-0000eb20: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000eb30: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000eb40: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
-0000eb50: 2d78 786c 5f6d 652c 2e64 6a61 6e67 6f63  -xxl_me,.djangoc
-0000eb60: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000eb70: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000eb80: 7873 5f6d 7320 2e66 6965 6c64 2d78 786c  xs_ms .field-xxl
-0000eb90: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000eba0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000ebb0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000ebc0: 6666 7365 7420 2e66 6965 6c64 2d6c 675f  ffset .field-lg_
-0000ebd0: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
-0000ebe0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-0000ebf0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000ec00: 6673 6574 202e 6669 656c 642d 6c67 5f6d  fset .field-lg_m
-0000ec10: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000ec20: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000ec30: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
-0000ec40: 7365 7420 2e66 6965 6c64 2d6d 645f 6d65  set .field-md_me
-0000ec50: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000ec60: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000ec70: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000ec80: 6574 202e 6669 656c 642d 6d64 5f6d 732c  et .field-md_ms,
-0000ec90: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000eca0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000ecb0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
-0000ecc0: 7420 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  t .field-sm_me,.
-0000ecd0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000ece0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000ecf0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-0000ed00: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
-0000ed10: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000ed20: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000ed30: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
-0000ed40: 2e66 6965 6c64 2d78 6c5f 6d65 2c2e 646a  .field-xl_me,.dj
-0000ed50: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000ed60: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000ed70: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
-0000ed80: 6669 656c 642d 786c 5f6d 732c 2e64 6a61  field-xl_ms,.dja
-0000ed90: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000eda0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000edb0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000edc0: 6965 6c64 2d78 735f 6d65 2c2e 646a 616e  ield-xs_me,.djan
-0000edd0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000ede0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000edf0: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000ee00: 656c 642d 7873 5f6d 732c 2e64 6a61 6e67  eld-xs_ms,.djang
-0000ee10: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000ee20: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000ee30: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000ee40: 6c64 2d78 786c 5f6d 652c 2e64 6a61 6e67  ld-xxl_me,.djang
-0000ee50: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000ee60: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000ee70: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000ee80: 6c64 2d78 786c 5f6d 732c 2e64 6a61 6e67  ld-xxl_ms,.djang
-0000ee90: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000eea0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000eeb0: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-0000eec0: 642d 6c67 5f6d 652c 2e64 6a61 6e67 6f63  d-lg_me,.djangoc
-0000eed0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000eee0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000eef0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-0000ef00: 6c67 5f6d 732c 2e64 6a61 6e67 6f63 6d73  lg_ms,.djangocms
-0000ef10: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000ef20: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000ef30: 5f6f 7264 6572 202e 6669 656c 642d 6d64  _order .field-md
-0000ef40: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
-0000ef50: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000ef60: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000ef70: 7264 6572 202e 6669 656c 642d 6d64 5f6d  rder .field-md_m
-0000ef80: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000ef90: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000efa0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-0000efb0: 6572 202e 6669 656c 642d 736d 5f6d 652c  er .field-sm_me,
-0000efc0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000efd0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000efe0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000eff0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
-0000f000: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000f010: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000f020: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000f030: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
-0000f040: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000f050: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000f060: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000f070: 656c 642d 786c 5f6d 732c 2e64 6a61 6e67  eld-xl_ms,.djang
-0000f080: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000f090: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000f0a0: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-0000f0b0: 642d 7873 5f6d 652c 2e64 6a61 6e67 6f63  d-xs_me,.djangoc
-0000f0c0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000f0d0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000f0e0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-0000f0f0: 7873 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xs_ms,.djangocms
-0000f100: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000f110: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000f120: 5f6f 7264 6572 202e 6669 656c 642d 7878  _order .field-xx
-0000f130: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
-0000f140: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000f150: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000f160: 6f72 6465 7220 2e66 6965 6c64 2d78 786c  order .field-xxl
-0000f170: 5f6d 737b 7465 7874 2d61 6c69 676e 3a6c  _ms{text-align:l
-0000f180: 6566 747d 2e64 6a61 6e67 6f63 6d73 2d66  eft}.djangocms-f
-0000f190: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000f1a0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000f1b0: 735f 636f 6c20 2e66 6965 6c64 2d6c 675f  s_col .field-lg_
-0000f1c0: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-0000f1d0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000f1e0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000f1f0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-0000f200: 642d 6c67 5f6d 7320 6c61 6265 6c2c 2e64  d-lg_ms label,.d
-0000f210: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000f220: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000f230: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000f240: 2e66 6965 6c64 2d6d 645f 6d65 206c 6162  .field-md_me lab
-0000f250: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-0000f260: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000f270: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000f280: 5f63 6f6c 202e 6669 656c 642d 6d64 5f6d  _col .field-md_m
-0000f290: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
-0000f2a0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f2b0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f2c0: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-0000f2d0: 2d73 6d5f 6d65 206c 6162 656c 2c2e 646a  -sm_me label,.dj
-0000f2e0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000f2f0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000f300: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-0000f310: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
-0000f320: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000f330: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000f340: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000f350: 636f 6c20 2e66 6965 6c64 2d78 6c5f 6d65  col .field-xl_me
-0000f360: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000f370: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000f380: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000f390: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-0000f3a0: 786c 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xl_ms label,.dja
-0000f3b0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000f3c0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000f3d0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000f3e0: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
-0000f3f0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000f400: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000f410: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000f420: 6f6c 202e 6669 656c 642d 7873 5f6d 7320  ol .field-xs_ms 
-0000f430: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000f440: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000f450: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000f460: 2d78 735f 636f 6c20 2e66 6965 6c64 2d78  -xs_col .field-x
-0000f470: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
-0000f480: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000f490: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000f4a0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000f4b0: 6965 6c64 2d78 786c 5f6d 7320 6c61 6265  ield-xxl_ms labe
-0000f4c0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000f4d0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000f4e0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000f4f0: 6d65 202e 6669 656c 642d 6c67 5f6d 6520  me .field-lg_me 
-0000f500: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000f510: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000f520: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000f530: 2d78 735f 6d65 202e 6669 656c 642d 6c67  -xs_me .field-lg
-0000f540: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-0000f550: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000f560: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000f570: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000f580: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
-0000f590: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000f5a0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000f5b0: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
-0000f5c0: 6669 656c 642d 6d64 5f6d 7320 6c61 6265  field-md_ms labe
-0000f5d0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000f5e0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000f5f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000f600: 6d65 202e 6669 656c 642d 736d 5f6d 6520  me .field-sm_me 
-0000f610: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000f620: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000f630: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000f640: 2d78 735f 6d65 202e 6669 656c 642d 736d  -xs_me .field-sm
-0000f650: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-0000f660: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000f670: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000f680: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000f690: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
-0000f6a0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000f6b0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000f6c0: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
-0000f6d0: 6669 656c 642d 786c 5f6d 7320 6c61 6265  field-xl_ms labe
-0000f6e0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000f6f0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000f700: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000f710: 6d65 202e 6669 656c 642d 7873 5f6d 6520  me .field-xs_me 
-0000f720: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000f730: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000f740: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000f750: 2d78 735f 6d65 202e 6669 656c 642d 7873  -xs_me .field-xs
-0000f760: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-0000f770: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000f780: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000f790: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000f7a0: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
-0000f7b0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000f7c0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000f7d0: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
-0000f7e0: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
-0000f7f0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000f800: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000f810: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000f820: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
-0000f830: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
-0000f840: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f850: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f860: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
-0000f870: 6c67 5f6d 7320 6c61 6265 6c2c 2e64 6a61  lg_ms label,.dja
-0000f880: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000f890: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000f8a0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000f8b0: 656c 642d 6d64 5f6d 6520 6c61 6265 6c2c  eld-md_me label,
-0000f8c0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f8d0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f8e0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000f8f0: 202e 6669 656c 642d 6d64 5f6d 7320 6c61   .field-md_ms la
-0000f900: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000f910: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000f920: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000f930: 735f 6d73 202e 6669 656c 642d 736d 5f6d  s_ms .field-sm_m
-0000f940: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
-0000f950: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f960: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f970: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
-0000f980: 736d 5f6d 7320 6c61 6265 6c2c 2e64 6a61  sm_ms label,.dja
-0000f990: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000f9a0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000f9b0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000f9c0: 656c 642d 786c 5f6d 6520 6c61 6265 6c2c  eld-xl_me label,
-0000f9d0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f9e0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f9f0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000fa00: 202e 6669 656c 642d 786c 5f6d 7320 6c61   .field-xl_ms la
-0000fa10: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000fa20: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000fa30: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000fa40: 735f 6d73 202e 6669 656c 642d 7873 5f6d  s_ms .field-xs_m
-0000fa50: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
-0000fa60: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000fa70: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000fa80: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
-0000fa90: 7873 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xs_ms label,.dja
-0000faa0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000fab0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000fac0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000fad0: 656c 642d 7878 6c5f 6d65 206c 6162 656c  eld-xxl_me label
-0000fae0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000faf0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000fb00: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000fb10: 7320 2e66 6965 6c64 2d78 786c 5f6d 7320  s .field-xxl_ms 
-0000fb20: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000fb30: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000fb40: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000fb50: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000fb60: 642d 6c67 5f6d 6520 6c61 6265 6c2c 2e64  d-lg_me label,.d
-0000fb70: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000fb80: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000fb90: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000fba0: 6574 202e 6669 656c 642d 6c67 5f6d 7320  et .field-lg_ms 
-0000fbb0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000fbc0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000fbd0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000fbe0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000fbf0: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
-0000fc00: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000fc10: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000fc20: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000fc30: 6574 202e 6669 656c 642d 6d64 5f6d 7320  et .field-md_ms 
-0000fc40: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000fc50: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000fc60: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000fc70: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000fc80: 642d 736d 5f6d 6520 6c61 6265 6c2c 2e64  d-sm_me label,.d
-0000fc90: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000fca0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000fcb0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000fcc0: 6574 202e 6669 656c 642d 736d 5f6d 7320  et .field-sm_ms 
-0000fcd0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000fce0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000fcf0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000fd00: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000fd10: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
-0000fd20: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000fd30: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000fd40: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000fd50: 6574 202e 6669 656c 642d 786c 5f6d 7320  et .field-xl_ms 
-0000fd60: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000fd70: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000fd80: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000fd90: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000fda0: 642d 7873 5f6d 6520 6c61 6265 6c2c 2e64  d-xs_me label,.d
-0000fdb0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000fdc0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000fdd0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000fde0: 6574 202e 6669 656c 642d 7873 5f6d 7320  et .field-xs_ms 
-0000fdf0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000fe00: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000fe10: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000fe20: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000fe30: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
-0000fe40: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000fe50: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000fe60: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
-0000fe70: 7365 7420 2e66 6965 6c64 2d78 786c 5f6d  set .field-xxl_m
-0000fe80: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
-0000fe90: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000fea0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000feb0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000fec0: 6c64 2d6c 675f 6d65 206c 6162 656c 2c2e  ld-lg_me label,.
-0000fed0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000fee0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000fef0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-0000ff00: 6572 202e 6669 656c 642d 6c67 5f6d 7320  er .field-lg_ms 
-0000ff10: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000ff20: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000ff30: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000ff40: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
-0000ff50: 2d6d 645f 6d65 206c 6162 656c 2c2e 646a  -md_me label,.dj
-0000ff60: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000ff70: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000ff80: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000ff90: 202e 6669 656c 642d 6d64 5f6d 7320 6c61   .field-md_ms la
-0000ffa0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000ffb0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000ffc0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000ffd0: 735f 6f72 6465 7220 2e66 6965 6c64 2d73  s_order .field-s
-0000ffe0: 6d5f 6d65 206c 6162 656c 2c2e 646a 616e  m_me label,.djan
-0000fff0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-00010000: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-00010010: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-00010020: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
-00010030: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010040: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-00010050: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-00010060: 6f72 6465 7220 2e66 6965 6c64 2d78 6c5f  order .field-xl_
-00010070: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-00010080: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-00010090: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-000100a0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-000100b0: 656c 642d 786c 5f6d 7320 6c61 6265 6c2c  eld-xl_ms label,
-000100c0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-000100d0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-000100e0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
-000100f0: 6465 7220 2e66 6965 6c64 2d78 735f 6d65  der .field-xs_me
-00010100: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-00010110: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-00010120: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-00010130: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-00010140: 642d 7873 5f6d 7320 6c61 6265 6c2c 2e64  d-xs_ms label,.d
-00010150: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00010160: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-00010170: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-00010180: 7220 2e66 6965 6c64 2d78 786c 5f6d 6520  r .field-xxl_me 
-00010190: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-000101a0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-000101b0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-000101c0: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
-000101d0: 2d78 786c 5f6d 7320 6c61 6265 6c2c 2e64  -xxl_ms label,.d
-000101e0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-000101f0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00010200: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-00010210: 656c 642d 6c67 5f6d 6520 6c61 6265 6c2c  eld-lg_me label,
-00010220: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00010230: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00010240: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-00010250: 6669 656c 642d 6c67 5f6d 7320 6c61 6265  field-lg_ms labe
-00010260: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010270: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00010280: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-00010290: 202e 6669 656c 642d 6d64 5f6d 6520 6c61   .field-md_me la
-000102a0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-000102b0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-000102c0: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-000102d0: 6f6c 202e 6669 656c 642d 6d64 5f6d 7320  ol .field-md_ms 
-000102e0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-000102f0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00010300: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00010310: 5f63 6f6c 202e 6669 656c 642d 736d 5f6d  _col .field-sm_m
-00010320: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
-00010330: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00010340: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00010350: 7873 5f63 6f6c 202e 6669 656c 642d 736d  xs_col .field-sm
-00010360: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-00010370: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-00010380: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-00010390: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-000103a0: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
-000103b0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-000103c0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-000103d0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-000103e0: 642d 786c 5f6d 7320 6c61 6265 6c2c 2e64  d-xl_ms label,.d
-000103f0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00010400: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00010410: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-00010420: 656c 642d 7873 5f6d 6520 6c61 6265 6c2c  eld-xs_me label,
-00010430: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00010440: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00010450: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-00010460: 6669 656c 642d 7873 5f6d 7320 6c61 6265  field-xs_ms labe
-00010470: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010480: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00010490: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-000104a0: 202e 6669 656c 642d 7878 6c5f 6d65 206c   .field-xxl_me l
-000104b0: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-000104c0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-000104d0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-000104e0: 636f 6c20 2e66 6965 6c64 2d78 786c 5f6d  col .field-xxl_m
-000104f0: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
-00010500: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00010510: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00010520: 7873 5f6d 6520 2e66 6965 6c64 2d6c 675f  xs_me .field-lg_
-00010530: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-00010540: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-00010550: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-00010560: 2d78 735f 6d65 202e 6669 656c 642d 6c67  -xs_me .field-lg
-00010570: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-00010580: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-00010590: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-000105a0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d6d  d-xs_me .field-m
-000105b0: 645f 6d65 206c 6162 656c 2c2e 646a 616e  d_me label,.djan
-000105c0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-000105d0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-000105e0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-000105f0: 6d64 5f6d 7320 6c61 6265 6c2c 2e64 6a61  md_ms label,.dja
-00010600: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00010610: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00010620: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-00010630: 2d73 6d5f 6d65 206c 6162 656c 2c2e 646a  -sm_me label,.dj
-00010640: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-00010650: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-00010660: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-00010670: 642d 736d 5f6d 7320 6c61 6265 6c2c 2e64  d-sm_ms label,.d
-00010680: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00010690: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-000106a0: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
-000106b0: 6c64 2d78 6c5f 6d65 206c 6162 656c 2c2e  ld-xl_me label,.
-000106c0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-000106d0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-000106e0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-000106f0: 656c 642d 786c 5f6d 7320 6c61 6265 6c2c  eld-xl_ms label,
-00010700: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00010710: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00010720: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
-00010730: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
-00010740: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-00010750: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-00010760: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
-00010770: 6669 656c 642d 7873 5f6d 7320 6c61 6265  field-xs_ms labe
-00010780: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010790: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-000107a0: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
-000107b0: 2e66 6965 6c64 2d78 786c 5f6d 6520 6c61  .field-xxl_me la
-000107c0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-000107d0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-000107e0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-000107f0: 6520 2e66 6965 6c64 2d78 786c 5f6d 7320  e .field-xxl_ms 
-00010800: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-00010810: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00010820: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00010830: 5f6d 7320 2e66 6965 6c64 2d6c 675f 6d65  _ms .field-lg_me
-00010840: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-00010850: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-00010860: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00010870: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
-00010880: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
-00010890: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-000108a0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-000108b0: 7873 5f6d 7320 2e66 6965 6c64 2d6d 645f  xs_ms .field-md_
-000108c0: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-000108d0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-000108e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-000108f0: 2d78 735f 6d73 202e 6669 656c 642d 6d64  -xs_ms .field-md
-00010900: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-00010910: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-00010920: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-00010930: 642d 7873 5f6d 7320 2e66 6965 6c64 2d73  d-xs_ms .field-s
-00010940: 6d5f 6d65 206c 6162 656c 2c2e 646a 616e  m_me label,.djan
-00010950: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-00010960: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-00010970: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
-00010980: 736d 5f6d 7320 6c61 6265 6c2c 2e64 6a61  sm_ms label,.dja
-00010990: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-000109a0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-000109b0: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
-000109c0: 2d78 6c5f 6d65 206c 6162 656c 2c2e 646a  -xl_me label,.dj
-000109d0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-000109e0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-000109f0: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-00010a00: 642d 786c 5f6d 7320 6c61 6265 6c2c 2e64  d-xl_ms label,.d
-00010a10: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00010a20: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00010a30: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
-00010a40: 6c64 2d78 735f 6d65 206c 6162 656c 2c2e  ld-xs_me label,.
-00010a50: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-00010a60: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-00010a70: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-00010a80: 656c 642d 7873 5f6d 7320 6c61 6265 6c2c  eld-xs_ms label,
-00010a90: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00010aa0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00010ab0: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
-00010ac0: 6965 6c64 2d78 786c 5f6d 6520 6c61 6265  ield-xxl_me labe
-00010ad0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010ae0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00010af0: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
-00010b00: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
-00010b10: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-00010b20: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-00010b30: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-00010b40: 6666 7365 7420 2e66 6965 6c64 2d6c 675f  ffset .field-lg_
-00010b50: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-00010b60: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-00010b70: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-00010b80: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-00010b90: 642d 6c67 5f6d 7320 6c61 6265 6c2c 2e64  d-lg_ms label,.d
-00010ba0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00010bb0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00010bc0: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
-00010bd0: 2e66 6965 6c64 2d6d 645f 6d65 206c 6162  .field-md_me lab
-00010be0: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-00010bf0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-00010c00: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-00010c10: 6673 6574 202e 6669 656c 642d 6d64 5f6d  fset .field-md_m
-00010c20: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
-00010c30: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00010c40: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00010c50: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
-00010c60: 2d73 6d5f 6d65 206c 6162 656c 2c2e 646a  -sm_me label,.dj
-00010c70: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-00010c80: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-00010c90: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
-00010ca0: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
-00010cb0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010cc0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00010cd0: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
-00010ce0: 7365 7420 2e66 6965 6c64 2d78 6c5f 6d65  set .field-xl_me
-00010cf0: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-00010d00: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-00010d10: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00010d20: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-00010d30: 786c 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xl_ms label,.dja
-00010d40: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00010d50: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00010d60: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-00010d70: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
-00010d80: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-00010d90: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-00010da0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-00010db0: 6574 202e 6669 656c 642d 7873 5f6d 7320  et .field-xs_ms 
-00010dc0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-00010dd0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00010de0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00010df0: 5f6f 6666 7365 7420 2e66 6965 6c64 2d78  _offset .field-x
-00010e00: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
-00010e10: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00010e20: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00010e30: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-00010e40: 6965 6c64 2d78 786c 5f6d 7320 6c61 6265  ield-xxl_ms labe
-00010e50: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010e60: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00010e70: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-00010e80: 6572 202e 6669 656c 642d 6c67 5f6d 6520  er .field-lg_me 
-00010e90: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-00010ea0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00010eb0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00010ec0: 5f6f 7264 6572 202e 6669 656c 642d 6c67  _order .field-lg
-00010ed0: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-00010ee0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-00010ef0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-00010f00: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-00010f10: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
-00010f20: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00010f30: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00010f40: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-00010f50: 6669 656c 642d 6d64 5f6d 7320 6c61 6265  field-md_ms labe
-00010f60: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00010f70: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00010f80: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-00010f90: 6572 202e 6669 656c 642d 736d 5f6d 6520  er .field-sm_me 
-00010fa0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-00010fb0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00010fc0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00010fd0: 5f6f 7264 6572 202e 6669 656c 642d 736d  _order .field-sm
-00010fe0: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-00010ff0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-00011000: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-00011010: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-00011020: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
-00011030: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00011040: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00011050: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-00011060: 6669 656c 642d 786c 5f6d 7320 6c61 6265  field-xl_ms labe
-00011070: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-00011080: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00011090: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-000110a0: 6572 202e 6669 656c 642d 7873 5f6d 6520  er .field-xs_me 
-000110b0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-000110c0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-000110d0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-000110e0: 5f6f 7264 6572 202e 6669 656c 642d 7873  _order .field-xs
-000110f0: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
-00011100: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-00011110: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-00011120: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-00011130: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
-00011140: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-00011150: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-00011160: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
-00011170: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
-00011180: 6265 6c7b 6c65 6674 3a33 3070 783b 626f  bel{left:30px;bo
-00011190: 7474 6f6d 3a31 3470 787d 2e64 6a61 6e67  ttom:14px}.djang
-000111a0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-000111b0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-000111c0: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-000111d0: 6c64 2d6c 675f 6d65 2069 6e70 7574 2c2e  ld-lg_me input,.
-000111e0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-000111f0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-00011200: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-00011210: 202e 6669 656c 642d 6c67 5f6d 7320 696e   .field-lg_ms in
-00011220: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00011230: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-00011240: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00011250: 735f 636f 6c20 2e66 6965 6c64 2d6d 645f  s_col .field-md_
-00011260: 6d65 2069 6e70 7574 2c2e 646a 616e 676f  me input,.django
-00011270: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-00011280: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-00011290: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-000112a0: 642d 6d64 5f6d 7320 696e 7075 742c 2e64  d-md_ms input,.d
-000112b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-000112c0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-000112d0: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-000112e0: 2e66 6965 6c64 2d73 6d5f 6d65 2069 6e70  .field-sm_me inp
-000112f0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-00011300: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-00011310: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00011320: 5f63 6f6c 202e 6669 656c 642d 736d 5f6d  _col .field-sm_m
-00011330: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00011340: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-00011350: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-00011360: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-00011370: 2d78 6c5f 6d65 2069 6e70 7574 2c2e 646a  -xl_me input,.dj
-00011380: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-00011390: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-000113a0: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-000113b0: 6669 656c 642d 786c 5f6d 7320 696e 7075  field-xl_ms inpu
-000113c0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-000113d0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-000113e0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-000113f0: 636f 6c20 2e66 6965 6c64 2d78 735f 6d65  col .field-xs_me
-00011400: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
-00011410: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-00011420: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-00011430: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-00011440: 7873 5f6d 7320 696e 7075 742c 2e64 6a61  xs_ms input,.dja
-00011450: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011460: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011470: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-00011480: 6965 6c64 2d78 786c 5f6d 6520 696e 7075  ield-xxl_me inpu
-00011490: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-000114a0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-000114b0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-000114c0: 636f 6c20 2e66 6965 6c64 2d78 786c 5f6d  col .field-xxl_m
-000114d0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-000114e0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-000114f0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-00011500: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-00011510: 6c67 5f6d 6520 696e 7075 742c 2e64 6a61  lg_me input,.dja
-00011520: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011530: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011540: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-00011550: 656c 642d 6c67 5f6d 7320 696e 7075 742c  eld-lg_ms input,
-00011560: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00011570: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-00011580: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-00011590: 202e 6669 656c 642d 6d64 5f6d 6520 696e   .field-md_me in
-000115a0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-000115b0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-000115c0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-000115d0: 735f 6d65 202e 6669 656c 642d 6d64 5f6d  s_me .field-md_m
-000115e0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-000115f0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-00011600: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-00011610: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-00011620: 736d 5f6d 6520 696e 7075 742c 2e64 6a61  sm_me input,.dja
-00011630: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011640: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011650: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-00011660: 656c 642d 736d 5f6d 7320 696e 7075 742c  eld-sm_ms input,
-00011670: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00011680: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-00011690: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-000116a0: 202e 6669 656c 642d 786c 5f6d 6520 696e   .field-xl_me in
-000116b0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-000116c0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-000116d0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-000116e0: 735f 6d65 202e 6669 656c 642d 786c 5f6d  s_me .field-xl_m
-000116f0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00011700: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-00011710: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-00011720: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-00011730: 7873 5f6d 6520 696e 7075 742c 2e64 6a61  xs_me input,.dja
-00011740: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011750: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011760: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-00011770: 656c 642d 7873 5f6d 7320 696e 7075 742c  eld-xs_ms input,
-00011780: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00011790: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-000117a0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-000117b0: 202e 6669 656c 642d 7878 6c5f 6d65 2069   .field-xxl_me i
-000117c0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-000117d0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-000117e0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-000117f0: 7873 5f6d 6520 2e66 6965 6c64 2d78 786c  xs_me .field-xxl
-00011800: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-00011810: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-00011820: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-00011830: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-00011840: 642d 6c67 5f6d 6520 696e 7075 742c 2e64  d-lg_me input,.d
-00011850: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00011860: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-00011870: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-00011880: 6669 656c 642d 6c67 5f6d 7320 696e 7075  field-lg_ms inpu
-00011890: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-000118a0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-000118b0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-000118c0: 6d73 202e 6669 656c 642d 6d64 5f6d 6520  ms .field-md_me 
-000118d0: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-000118e0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-000118f0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-00011900: 2d78 735f 6d73 202e 6669 656c 642d 6d64  -xs_ms .field-md
-00011910: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-00011920: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-00011930: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-00011940: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-00011950: 642d 736d 5f6d 6520 696e 7075 742c 2e64  d-sm_me input,.d
-00011960: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00011970: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-00011980: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-00011990: 6669 656c 642d 736d 5f6d 7320 696e 7075  field-sm_ms inpu
-000119a0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-000119b0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-000119c0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-000119d0: 6d73 202e 6669 656c 642d 786c 5f6d 6520  ms .field-xl_me 
-000119e0: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-000119f0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-00011a00: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-00011a10: 2d78 735f 6d73 202e 6669 656c 642d 786c  -xs_ms .field-xl
-00011a20: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-00011a30: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-00011a40: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-00011a50: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-00011a60: 642d 7873 5f6d 6520 696e 7075 742c 2e64  d-xs_me input,.d
-00011a70: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00011a80: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-00011a90: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-00011aa0: 6669 656c 642d 7873 5f6d 7320 696e 7075  field-xs_ms inpu
-00011ab0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-00011ac0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-00011ad0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-00011ae0: 6d73 202e 6669 656c 642d 7878 6c5f 6d65  ms .field-xxl_me
-00011af0: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
-00011b00: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-00011b10: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-00011b20: 642d 7873 5f6d 7320 2e66 6965 6c64 2d78  d-xs_ms .field-x
-00011b30: 786c 5f6d 7320 696e 7075 742c 2e64 6a61  xl_ms input,.dja
-00011b40: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011b50: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011b60: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-00011b70: 202e 6669 656c 642d 6c67 5f6d 6520 696e   .field-lg_me in
-00011b80: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00011b90: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-00011ba0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00011bb0: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-00011bc0: 6c67 5f6d 7320 696e 7075 742c 2e64 6a61  lg_ms input,.dja
-00011bd0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011be0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011bf0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-00011c00: 202e 6669 656c 642d 6d64 5f6d 6520 696e   .field-md_me in
-00011c10: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00011c20: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-00011c30: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00011c40: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-00011c50: 6d64 5f6d 7320 696e 7075 742c 2e64 6a61  md_ms input,.dja
-00011c60: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011c70: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011c80: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-00011c90: 202e 6669 656c 642d 736d 5f6d 6520 696e   .field-sm_me in
-00011ca0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00011cb0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-00011cc0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00011cd0: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-00011ce0: 736d 5f6d 7320 696e 7075 742c 2e64 6a61  sm_ms input,.dja
-00011cf0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011d00: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011d10: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-00011d20: 202e 6669 656c 642d 786c 5f6d 6520 696e   .field-xl_me in
-00011d30: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00011d40: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-00011d50: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00011d60: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-00011d70: 786c 5f6d 7320 696e 7075 742c 2e64 6a61  xl_ms input,.dja
-00011d80: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011d90: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011da0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-00011db0: 202e 6669 656c 642d 7873 5f6d 6520 696e   .field-xs_me in
-00011dc0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00011dd0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-00011de0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00011df0: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-00011e00: 7873 5f6d 7320 696e 7075 742c 2e64 6a61  xs_ms input,.dja
-00011e10: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011e20: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011e30: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-00011e40: 202e 6669 656c 642d 7878 6c5f 6d65 2069   .field-xxl_me i
-00011e50: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-00011e60: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-00011e70: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00011e80: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
-00011e90: 2d78 786c 5f6d 7320 696e 7075 742c 2e64  -xxl_ms input,.d
-00011ea0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00011eb0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-00011ec0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-00011ed0: 7220 2e66 6965 6c64 2d6c 675f 6d65 2069  r .field-lg_me i
-00011ee0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-00011ef0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-00011f00: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00011f10: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-00011f20: 6c67 5f6d 7320 696e 7075 742c 2e64 6a61  lg_ms input,.dja
-00011f30: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00011f40: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-00011f50: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
-00011f60: 2e66 6965 6c64 2d6d 645f 6d65 2069 6e70  .field-md_me inp
-00011f70: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-00011f80: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-00011f90: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00011fa0: 5f6f 7264 6572 202e 6669 656c 642d 6d64  _order .field-md
-00011fb0: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-00011fc0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-00011fd0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-00011fe0: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
-00011ff0: 6965 6c64 2d73 6d5f 6d65 2069 6e70 7574  ield-sm_me input
-00012000: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-00012010: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-00012020: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-00012030: 7264 6572 202e 6669 656c 642d 736d 5f6d  rder .field-sm_m
-00012040: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00012050: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-00012060: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-00012070: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-00012080: 6c64 2d78 6c5f 6d65 2069 6e70 7574 2c2e  ld-xl_me input,.
-00012090: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-000120a0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-000120b0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-000120c0: 6572 202e 6669 656c 642d 786c 5f6d 7320  er .field-xl_ms 
-000120d0: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-000120e0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-000120f0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-00012100: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
-00012110: 2d78 735f 6d65 2069 6e70 7574 2c2e 646a  -xs_me input,.dj
-00012120: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-00012130: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-00012140: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-00012150: 202e 6669 656c 642d 7873 5f6d 7320 696e   .field-xs_ms in
-00012160: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00012170: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-00012180: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00012190: 735f 6f72 6465 7220 2e66 6965 6c64 2d78  s_order .field-x
-000121a0: 786c 5f6d 6520 696e 7075 742c 2e64 6a61  xl_me input,.dja
-000121b0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-000121c0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-000121d0: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
-000121e0: 2e66 6965 6c64 2d78 786c 5f6d 7320 696e  .field-xxl_ms in
-000121f0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00012200: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-00012210: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-00012220: 6f6c 202e 6669 656c 642d 6c67 5f6d 6520  ol .field-lg_me 
-00012230: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-00012240: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00012250: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00012260: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
-00012270: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00012280: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00012290: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-000122a0: 7873 5f63 6f6c 202e 6669 656c 642d 6d64  xs_col .field-md
-000122b0: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
-000122c0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-000122d0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-000122e0: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-000122f0: 6d64 5f6d 7320 696e 7075 742c 2e64 6a61  md_ms input,.dja
-00012300: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00012310: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00012320: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-00012330: 642d 736d 5f6d 6520 696e 7075 742c 2e64  d-sm_me input,.d
-00012340: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00012350: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00012360: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-00012370: 656c 642d 736d 5f6d 7320 696e 7075 742c  eld-sm_ms input,
-00012380: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00012390: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-000123a0: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-000123b0: 6669 656c 642d 786c 5f6d 6520 696e 7075  field-xl_me inpu
-000123c0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-000123d0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-000123e0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-000123f0: 202e 6669 656c 642d 786c 5f6d 7320 696e   .field-xl_ms in
-00012400: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00012410: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-00012420: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-00012430: 6f6c 202e 6669 656c 642d 7873 5f6d 6520  ol .field-xs_me 
-00012440: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-00012450: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00012460: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00012470: 5f63 6f6c 202e 6669 656c 642d 7873 5f6d  _col .field-xs_m
-00012480: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00012490: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-000124a0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-000124b0: 7873 5f63 6f6c 202e 6669 656c 642d 7878  xs_col .field-xx
-000124c0: 6c5f 6d65 2069 6e70 7574 2c2e 646a 616e  l_me input,.djan
-000124d0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-000124e0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-000124f0: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-00012500: 2d78 786c 5f6d 7320 696e 7075 742c 2e64  -xxl_ms input,.d
-00012510: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00012520: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00012530: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
-00012540: 6c64 2d6c 675f 6d65 2069 6e70 7574 2c2e  ld-lg_me input,.
-00012550: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-00012560: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-00012570: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-00012580: 656c 642d 6c67 5f6d 7320 696e 7075 742c  eld-lg_ms input,
-00012590: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-000125a0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-000125b0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
-000125c0: 6965 6c64 2d6d 645f 6d65 2069 6e70 7574  ield-md_me input
-000125d0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-000125e0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-000125f0: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
-00012600: 6669 656c 642d 6d64 5f6d 7320 696e 7075  field-md_ms inpu
-00012610: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-00012620: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00012630: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
-00012640: 2e66 6965 6c64 2d73 6d5f 6d65 2069 6e70  .field-sm_me inp
-00012650: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-00012660: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-00012670: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-00012680: 202e 6669 656c 642d 736d 5f6d 7320 696e   .field-sm_ms in
-00012690: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-000126a0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-000126b0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-000126c0: 6520 2e66 6965 6c64 2d78 6c5f 6d65 2069  e .field-xl_me i
-000126d0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-000126e0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-000126f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-00012700: 6d65 202e 6669 656c 642d 786c 5f6d 7320  me .field-xl_ms 
-00012710: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-00012720: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00012730: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00012740: 5f6d 6520 2e66 6965 6c64 2d78 735f 6d65  _me .field-xs_me
-00012750: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
-00012760: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-00012770: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00012780: 735f 6d65 202e 6669 656c 642d 7873 5f6d  s_me .field-xs_m
-00012790: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-000127a0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-000127b0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-000127c0: 7873 5f6d 6520 2e66 6965 6c64 2d78 786c  xs_me .field-xxl
-000127d0: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
-000127e0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-000127f0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-00012800: 642d 7873 5f6d 6520 2e66 6965 6c64 2d78  d-xs_me .field-x
-00012810: 786c 5f6d 7320 696e 7075 742c 2e64 6a61  xl_ms input,.dja
-00012820: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00012830: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00012840: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
-00012850: 2d6c 675f 6d65 2069 6e70 7574 2c2e 646a  -lg_me input,.dj
-00012860: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-00012870: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-00012880: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-00012890: 642d 6c67 5f6d 7320 696e 7075 742c 2e64  d-lg_ms input,.d
-000128a0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-000128b0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-000128c0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
-000128d0: 6c64 2d6d 645f 6d65 2069 6e70 7574 2c2e  ld-md_me input,.
-000128e0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-000128f0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-00012900: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-00012910: 656c 642d 6d64 5f6d 7320 696e 7075 742c  eld-md_ms input,
-00012920: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00012930: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00012940: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
-00012950: 6965 6c64 2d73 6d5f 6d65 2069 6e70 7574  ield-sm_me input
-00012960: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-00012970: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-00012980: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-00012990: 6669 656c 642d 736d 5f6d 7320 696e 7075  field-sm_ms inpu
-000129a0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-000129b0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-000129c0: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
-000129d0: 2e66 6965 6c64 2d78 6c5f 6d65 2069 6e70  .field-xl_me inp
-000129e0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-000129f0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-00012a00: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-00012a10: 202e 6669 656c 642d 786c 5f6d 7320 696e   .field-xl_ms in
-00012a20: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00012a30: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-00012a40: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-00012a50: 7320 2e66 6965 6c64 2d78 735f 6d65 2069  s .field-xs_me i
-00012a60: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-00012a70: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-00012a80: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-00012a90: 6d73 202e 6669 656c 642d 7873 5f6d 7320  ms .field-xs_ms 
-00012aa0: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-00012ab0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-00012ac0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-00012ad0: 5f6d 7320 2e66 6965 6c64 2d78 786c 5f6d  _ms .field-xxl_m
-00012ae0: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
-00012af0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00012b00: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00012b10: 7873 5f6d 7320 2e66 6965 6c64 2d78 786c  xs_ms .field-xxl
-00012b20: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-00012b30: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-00012b40: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-00012b50: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-00012b60: 6c64 2d6c 675f 6d65 2069 6e70 7574 2c2e  ld-lg_me input,.
-00012b70: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-00012b80: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-00012b90: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-00012ba0: 202e 6669 656c 642d 6c67 5f6d 7320 696e   .field-lg_ms in
-00012bb0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00012bc0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-00012bd0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-00012be0: 6666 7365 7420 2e66 6965 6c64 2d6d 645f  ffset .field-md_
-00012bf0: 6d65 2069 6e70 7574 2c2e 646a 616e 676f  me input,.django
-00012c00: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-00012c10: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-00012c20: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-00012c30: 642d 6d64 5f6d 7320 696e 7075 742c 2e64  d-md_ms input,.d
-00012c40: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00012c50: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-00012c60: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
-00012c70: 2e66 6965 6c64 2d73 6d5f 6d65 2069 6e70  .field-sm_me inp
-00012c80: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-00012c90: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-00012ca0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-00012cb0: 6673 6574 202e 6669 656c 642d 736d 5f6d  fset .field-sm_m
-00012cc0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00012cd0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00012ce0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00012cf0: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
-00012d00: 2d78 6c5f 6d65 2069 6e70 7574 2c2e 646a  -xl_me input,.dj
-00012d10: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-00012d20: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-00012d30: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
-00012d40: 6669 656c 642d 786c 5f6d 7320 696e 7075  field-xl_ms inpu
-00012d50: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-00012d60: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00012d70: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
-00012d80: 7365 7420 2e66 6965 6c64 2d78 735f 6d65  set .field-xs_me
-00012d90: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
-00012da0: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-00012db0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-00012dc0: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-00012dd0: 7873 5f6d 7320 696e 7075 742c 2e64 6a61  xs_ms input,.dja
-00012de0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00012df0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00012e00: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-00012e10: 6965 6c64 2d78 786c 5f6d 6520 696e 7075  ield-xxl_me inpu
-00012e20: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-00012e30: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-00012e40: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
-00012e50: 7365 7420 2e66 6965 6c64 2d78 786c 5f6d  set .field-xxl_m
-00012e60: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00012e70: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00012e80: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00012e90: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-00012ea0: 6c67 5f6d 6520 696e 7075 742c 2e64 6a61  lg_me input,.dja
-00012eb0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00012ec0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00012ed0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-00012ee0: 656c 642d 6c67 5f6d 7320 696e 7075 742c  eld-lg_ms input,
-00012ef0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00012f00: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00012f10: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-00012f20: 202e 6669 656c 642d 6d64 5f6d 6520 696e   .field-md_me in
-00012f30: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00012f40: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-00012f50: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-00012f60: 7264 6572 202e 6669 656c 642d 6d64 5f6d  rder .field-md_m
-00012f70: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00012f80: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-00012f90: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00012fa0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-00012fb0: 736d 5f6d 6520 696e 7075 742c 2e64 6a61  sm_me input,.dja
-00012fc0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00012fd0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-00012fe0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-00012ff0: 656c 642d 736d 5f6d 7320 696e 7075 742c  eld-sm_ms input,
-00013000: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00013010: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00013020: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-00013030: 202e 6669 656c 642d 786c 5f6d 6520 696e   .field-xl_me in
-00013040: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-00013050: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-00013060: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-00013070: 7264 6572 202e 6669 656c 642d 786c 5f6d  rder .field-xl_m
-00013080: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-00013090: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-000130a0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-000130b0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-000130c0: 7873 5f6d 6520 696e 7075 742c 2e64 6a61  xs_me input,.dja
-000130d0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-000130e0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-000130f0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-00013100: 656c 642d 7873 5f6d 7320 696e 7075 742c  eld-xs_ms input,
-00013110: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00013120: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-00013130: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-00013140: 202e 6669 656c 642d 7878 6c5f 6d65 2069   .field-xxl_me i
-00013150: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-00013160: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-00013170: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-00013180: 6f72 6465 7220 2e66 6965 6c64 2d78 786c  order .field-xxl
-00013190: 5f6d 7320 696e 7075 747b 706f 7369 7469  _ms input{positi
-000131a0: 6f6e 3a72 656c 6174 6976 653b 626f 782d  on:relative;box-
-000131b0: 7369 7a69 6e67 3a62 6f72 6465 722d 626f  sizing:border-bo
-000131c0: 783b 746f 703a 2d33 7078 7d2e 646a 616e  x;top:-3px}.djan
-000131d0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-000131e0: 6f6c 756d 6e20 2e67 7269 642d 7265 7365  olumn .grid-rese
-000131f0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-00013200: 6e74 656e 642d 726f 7720 2e67 7269 642d  ntend-row .grid-
-00013210: 7265 7365 747b 706f 7369 7469 6f6e 3a61  reset{position:a
-00013220: 6273 6f6c 7574 653b 7269 6768 743a 3570  bsolute;right:5p
-00013230: 783b 746f 703a 307d 2e64 6a61 6e67 6f63  x;top:0}.djangoc
-00013240: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-00013250: 6d6e 202e 6963 6f6e 2d74 6865 6164 2c2e  mn .icon-thead,.
-00013260: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-00013270: 6e64 2d72 6f77 202e 6963 6f6e 2d74 6865  nd-row .icon-the
-00013280: 6164 7b74 6578 742d 616c 6967 6e3a 6365  ad{text-align:ce
-00013290: 6e74 6572 3b6d 6172 6769 6e2d 626f 7474  nter;margin-bott
-000132a0: 6f6d 3a31 3570 787d 2e64 6a61 6e67 6f63  om:15px}.djangoc
-000132b0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-000132c0: 6d6e 202e 6963 6f6e 2d74 6865 6164 202e  mn .icon-thead .
-000132d0: 6963 6f6e 2c2e 646a 616e 676f 636d 732d  icon,.djangocms-
-000132e0: 6672 6f6e 7465 6e64 2d72 6f77 202e 6963  frontend-row .ic
-000132f0: 6f6e 2d74 6865 6164 202e 6963 6f6e 7b66  on-thead .icon{f
-00013300: 6f6e 742d 7369 7a65 3a33 3070 787d 2e64  ont-size:30px}.d
-00013310: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00013320: 642d 636f 6c75 6d6e 202e 6963 6f6e 2d74  d-column .icon-t
-00013330: 6865 6164 202e 6963 6f6e 2d73 697a 652d  head .icon-size-
-00013340: 736d 2c2e 646a 616e 676f 636d 732d 6672  sm,.djangocms-fr
-00013350: 6f6e 7465 6e64 2d72 6f77 202e 6963 6f6e  ontend-row .icon
-00013360: 2d74 6865 6164 202e 6963 6f6e 2d73 697a  -thead .icon-siz
-00013370: 652d 736d 7b74 7261 6e73 666f 726d 3a72  e-sm{transform:r
-00013380: 6f74 6174 6528 3930 6465 6729 7d2e 646a  otate(90deg)}.dj
-00013390: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-000133a0: 2d63 6f6c 756d 6e20 2e69 636f 6e2d 7469  -column .icon-ti
-000133b0: 746c 652c 2e64 6a61 6e67 6f63 6d73 2d66  tle,.djangocms-f
-000133c0: 726f 6e74 656e 642d 726f 7720 2e69 636f  rontend-row .ico
-000133d0: 6e2d 7469 746c 657b 6469 7370 6c61 793a  n-title{display:
-000133e0: 626c 6f63 6b3b 666f 6e74 2d73 697a 653a  block;font-size:
-000133f0: 3132 7078 3b63 6f6c 6f72 3a23 3939 393b  12px;color:#999;
-00013400: 7061 6464 696e 673a 3570 7820 3020 307d  padding:5px 0 0}
-00013410: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00013420: 656e 642d 7072 6576 6965 777b 706f 7369  end-preview{posi
-00013430: 7469 6f6e 3a66 6978 6564 3b74 6f70 3a30  tion:fixed;top:0
-00013440: 3b72 6967 6874 3a30 3b7a 2d69 6e64 6578  ;right:0;z-index
-00013450: 3a31 303b 7465 7874 2d61 6c69 676e 3a63  :10;text-align:c
-00013460: 656e 7465 723b 626f 7264 6572 2d72 6164  enter;border-rad
-00013470: 6975 733a 3020 3020 3020 3370 783b 7061  ius:0 0 0 3px;pa
-00013480: 6464 696e 673a 3130 7078 2032 3070 7820  dding:10px 20px 
-00013490: 3237 7078 3b62 6f72 6465 723a 3170 7820  27px;border:1px 
-000134a0: 736f 6c69 6420 7661 7228 2d2d 6463 612d  solid var(--dca-
-000134b0: 6772 6179 2c76 6172 282d 2d68 6169 726c  gray,var(--hairl
-000134c0: 696e 652d 636f 6c6f 722c 2363 6363 2929  ine-color,#ccc))
-000134d0: 3b62 6f72 6465 722d 746f 703a 6e6f 6e65  ;border-top:none
-000134e0: 3b62 6f72 6465 722d 7269 6768 743a 6e6f  ;border-right:no
-000134f0: 6e65 3b62 6163 6b67 726f 756e 643a 7661  ne;background:va
-00013500: 7228 2d2d 626f 6479 2d62 672c 2366 6666  r(--body-bg,#fff
-00013510: 297d 406d 6564 6961 2028 7072 6566 6572  )}@media (prefer
-00013520: 732d 636f 6c6f 722d 7363 6865 6d65 3a64  s-color-scheme:d
-00013530: 6172 6b29 7b2e 646a 616e 676f 636d 732d  ark){.djangocms-
-00013540: 6672 6f6e 7465 6e64 2d70 7265 7669 6577  frontend-preview
-00013550: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
-00013560: 2d2d 626f 6479 2d62 672c 2330 3030 297d  --body-bg,#000)}
-00013570: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
-00013580: 7465 6e64 2d70 7265 7669 6577 2068 327b  tend-preview h2{
-00013590: 666f 6e74 2d73 697a 653a 3134 7078 3b6d  font-size:14px;m
-000135a0: 696e 2d77 6964 7468 3a31 3530 7078 3b6d  in-width:150px;m
-000135b0: 6172 6769 6e3a 3020 3020 3132 7078 7d2e  argin:0 0 12px}.
-000135c0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-000135d0: 6e64 2d70 7265 7669 6577 202e 6234 2d70  nd-preview .b4-p
-000135e0: 7265 7669 6577 7b6d 6172 6769 6e3a 3020  review{margin:0 
-000135f0: 3020 2d31 3570 787d 2e64 6a61 6e67 6f63  0 -15px}.djangoc
-00013600: 6d73 2d66 726f 6e74 656e 642d 7072 6576  ms-frontend-prev
-00013610: 6965 7720 2e62 342d 636c 6f73 657b 706f  iew .b4-close{po
-00013620: 7369 7469 6f6e 3a61 6273 6f6c 7574 653b  sition:absolute;
-00013630: 7269 6768 743a 3130 7078 3b74 6f70 3a38  right:10px;top:8
-00013640: 7078 3b7a 2d69 6e64 6578 3a31 3030 3b64  px;z-index:100;d
-00013650: 6973 706c 6179 3a62 6c6f 636b 3b63 6f6c  isplay:block;col
-00013660: 6f72 3a23 3565 3565 3565 3b66 6f6e 742d  or:#5e5e5e;font-
-00013670: 7369 7a65 3a31 3270 783b 6c69 6e65 2d68  size:12px;line-h
-00013680: 6569 6768 743a 3230 7078 3b66 6f6e 742d  eight:20px;font-
-00013690: 7765 6967 6874 3a37 3030 3b74 6578 742d  weight:700;text-
-000136a0: 7472 616e 7366 6f72 6d3a 7570 7065 7263  transform:upperc
-000136b0: 6173 653b 7769 6474 683a 3230 7078 3b68  ase;width:20px;h
-000136c0: 6569 6768 743a 3230 7078 3b62 6f72 6465  eight:20px;borde
-000136d0: 722d 7261 6469 7573 3a33 7078 3b62 6163  r-radius:3px;bac
-000136e0: 6b67 726f 756e 643a 2364 6464 7d2e 646a  kground:#ddd}.dj
-000136f0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-00013700: 2d70 7265 7669 6577 202e 6234 2d63 6c6f  -preview .b4-clo
-00013710: 7365 3a68 6f76 6572 7b63 6f6c 6f72 3a23  se:hover{color:#
-00013720: 6666 6621 696d 706f 7274 616e 743b 7465  fff!important;te
-00013730: 7874 2d64 6563 6f72 6174 696f 6e3a 6e6f  xt-decoration:no
-00013740: 6e65 3b62 6163 6b67 726f 756e 643a 2330  ne;background:#0
-00013750: 6266 7d2e 646a 616e 676f 636d 732d 6672  bf}.djangocms-fr
-00013760: 6f6e 7465 6e64 2d70 7265 7669 6577 202e  ontend-preview .
-00013770: 6274 6e3e 7370 616e 7b76 6572 7469 6361  btn>span{vertica
-00013780: 6c2d 616c 6967 6e3a 6d69 6464 6c65 7d2e  l-align:middle}.
-00013790: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-000137a0: 6e64 2d70 7265 7669 6577 202e 6274 6e3e  nd-preview .btn>
-000137b0: 7370 616e 3e2e 6963 6f6e 7b76 6572 7469  span>.icon{verti
-000137c0: 6361 6c2d 616c 6967 6e3a 6d69 6464 6c65  cal-align:middle
-000137d0: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
-000137e0: 7465 6e64 2d70 7265 7669 6577 202e 6274  tend-preview .bt
-000137f0: 6e3e 7370 616e 2073 7667 2c2e 646a 616e  n>span svg,.djan
-00013800: 676f 636d 732d 6672 6f6e 7465 6e64 2d70  gocms-frontend-p
-00013810: 7265 7669 6577 202e 6274 6e3e 7370 616e  review .btn>span
-00013820: 2075 7365 7b66 696c 6c3a 6375 7272 656e   use{fill:curren
-00013830: 7443 6f6c 6f72 7d2e 646a 616e 676f 636d  tColor}.djangocm
-00013840: 732d 6672 6f6e 7465 6e64 2d62 6c6f 636b  s-frontend-block
-00013850: 7175 6f74 6520 7465 7874 6172 6561 7b68  quote textarea{h
-00013860: 6569 6768 743a 3131 3070 787d 2369 645f  eight:110px}#id_
-00013870: 6c69 6e6b 5f74 7970 657b 7061 6464 696e  link_type{paddin
-00013880: 673a 303b 6d61 7267 696e 3a30 3b62 6f72  g:0;margin:0;bor
-00013890: 6465 723a 6e6f 6e65 7d23 6964 5f6c 696e  der:none}#id_lin
-000138a0: 6b5f 7479 7065 206c 697b 7061 6464 696e  k_type li{paddin
-000138b0: 673a 303b 6d61 7267 696e 3a30 2031 3570  g:0;margin:0 15p
-000138c0: 7820 3570 7820 303b 626f 7264 6572 3a6e  x 5px 0;border:n
-000138d0: 6f6e 657d 2369 645f 6c69 6e6b 5f74 7970  one}#id_link_typ
-000138e0: 6520 6c61 6265 6c20 696e 7075 747b 706f  e label input{po
-000138f0: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
-00013900: 746f 703a 2d34 7078 7d61 5b64 6174 612d  top:-4px}a[data-
-00013910: 706b 5d7b 706f 7369 7469 6f6e 3a72 656c  pk]{position:rel
-00013920: 6174 6976 657d 615b 6461 7461 2d70 6b5d  ative}a[data-pk]
-00013930: 3a61 6674 6572 7b63 6f6e 7465 6e74 3a61  :after{content:a
-00013940: 7474 7228 6461 7461 2d70 6b29 3b76 6973  ttr(data-pk);vis
-00013950: 6962 696c 6974 793a 6869 6464 656e 3b77  ibility:hidden;w
-00013960: 6964 7468 3a61 7574 6f3b 666f 6e74 2d77  idth:auto;font-w
-00013970: 6569 6768 743a 3430 303b 666f 6e74 2d73  eight:400;font-s
-00013980: 697a 653a 3830 253b 6261 636b 6772 6f75  ize:80%;backgrou
-00013990: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d64  nd-color:var(--d
-000139a0: 6361 2d77 6869 7465 2c76 6172 282d 2d62  ca-white,var(--b
-000139b0: 6f64 792d 6267 2c23 6666 6629 293b 636f  ody-bg,#fff));co
-000139c0: 6c6f 723a 7661 7228 2d2d 6463 612d 6772  lor:var(--dca-gr
-000139d0: 6179 2c76 6172 282d 2d62 6f64 792d 6667  ay,var(--body-fg
-000139e0: 2c23 3333 3329 293b 626f 7264 6572 3a73  ,#333));border:s
-000139f0: 6f6c 6964 2031 7078 2076 6172 282d 2d64  olid 1px var(--d
-00013a00: 6361 2d67 7261 792c 7661 7228 2d2d 626f  ca-gray,var(--bo
-00013a10: 6479 2d66 672c 2333 3333 2929 3b74 6578  dy-fg,#333));tex
-00013a20: 742d 616c 6967 6e3a 6365 6e74 6572 3b70  t-align:center;p
-00013a30: 6164 6469 6e67 3a35 7078 2031 3070 783b  adding:5px 10px;
-00013a40: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
-00013a50: 653b 7a2d 696e 6465 783a 313b 746f 703a  e;z-index:1;top:
-00013a60: 3131 3025 3b6c 6566 743a 3530 253b 6d61  110%;left:50%;ma
-00013a70: 7267 696e 2d6c 6566 743a 2d35 3025 7d61  rgin-left:-50%}a
-00013a80: 5b64 6174 612d 706b 5d3a 686f 7665 723a  [data-pk]:hover:
-00013a90: 6166 7465 727b 7669 7369 6269 6c69 7479  after{visibility
-00013aa0: 3a76 6973 6962 6c65 7d2e 646a 616e 676f  :visible}.django
-00013ab0: 636d 732d 6164 6d69 6e2d 7374 796c 6520  cms-admin-style 
-00013ac0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-00013ad0: 706c 7567 696e 5f74 6974 6c65 2069 6e70  plugin_title inp
-00013ae0: 7574 5b6e 616d 653d 706c 7567 696e 5f74  ut[name=plugin_t
-00013af0: 6974 6c65 5f30 5d7b 6d61 7267 696e 2d62  itle_0]{margin-b
-00013b00: 6f74 746f 6d3a 2e35 656d 2169 6d70 6f72  ottom:.5em!impor
-00013b10: 7461 6e74 7d2e 646a 616e 676f 636d 732d  tant}.djangocms-
-00013b20: 6164 6d69 6e2d 7374 796c 6520 2e66 6f72  admin-style .for
-00013b30: 6d2d 726f 772e 6669 656c 642d 706c 7567  m-row.field-plug
-00013b40: 696e 5f74 6974 6c65 2069 6e70 7574 5b6e  in_title input[n
-00013b50: 616d 653d 706c 7567 696e 5f74 6974 6c65  ame=plugin_title
-00013b60: 5f31 5d7b 7769 6474 683a 6361 6c63 2831  _1]{width:calc(1
-00013b70: 3030 2520 2d20 3265 6d29 2169 6d70 6f72  00% - 2em)!impor
-00013b80: 7461 6e74 7d62 6f64 793a 6e6f 7428 2e64  tant}body:not(.d
-00013b90: 6a61 6e67 6f63 6d73 2d61 646d 696e 2d73  jangocms-admin-s
-00013ba0: 7479 6c65 2920 2e66 6f72 6d2d 726f 772e  tyle) .form-row.
-00013bb0: 6669 656c 642d 706c 7567 696e 5f74 6974  field-plugin_tit
-00013bc0: 6c65 2069 6e70 7574 5b6e 616d 653d 706c  le input[name=pl
-00013bd0: 7567 696e 5f74 6974 6c65 5f31 5d7b 7769  ugin_title_1]{wi
-00013be0: 6474 683a 6361 6c63 2831 3030 2520 2d20  dth:calc(100% - 
-00013bf0: 3230 3070 7820 2d20 3165 6d29 2169 6d70  200px - 1em)!imp
-00013c00: 6f72 7461 6e74 3b6d 6172 6769 6e2d 6c65  ortant;margin-le
-00013c10: 6674 3a31 656d 7d2e 6672 6f6e 7465 6e64  ft:1em}.frontend
-00013c20: 2d69 636f 6e2d 7069 636b 6572 7b74 6578  -icon-picker{tex
-00013c30: 742d 616c 6967 6e3a 6365 6e74 6572 3b64  t-align:center;d
-00013c40: 6973 706c 6179 3a69 6e6c 696e 652d 626c  isplay:inline-bl
-00013c50: 6f63 6b7d 2e66 726f 6e74 656e 642d 6963  ock}.frontend-ic
-00013c60: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
-00013c70: 636f 6e74 6169 6e65 727b 706f 7369 7469  container{positi
-00013c80: 6f6e 3a72 656c 6174 6976 653b 6d61 7267  on:relative;marg
-00013c90: 696e 2d62 6f74 746f 6d3a 2e35 656d 3b6d  in-bottom:.5em;m
-00013ca0: 6172 6769 6e2d 6c65 6674 3a61 7574 6f3b  argin-left:auto;
-00013cb0: 6d61 7267 696e 2d72 6967 6874 3a61 7574  margin-right:aut
-00013cc0: 6f3b 7769 6474 683a 3765 6d3b 6865 6967  o;width:7em;heig
-00013cd0: 6874 3a37 656d 3b62 6f72 6465 723a 3170  ht:7em;border:1p
-00013ce0: 7820 7661 7228 2d2d 6463 612d 6772 6179  x var(--dca-gray
-00013cf0: 2d6c 6967 6874 2c76 6172 282d 2d62 6f72  -light,var(--bor
-00013d00: 6465 722d 636f 6c6f 722c 2364 3364 3364  der-color,#d3d3d
-00013d10: 3329 2920 736f 6c69 643b 7472 616e 7369  3)) solid;transi
-00013d20: 7469 6f6e 3a62 6163 6b67 726f 756e 642d  tion:background-
-00013d30: 636f 6c6f 7220 2e31 3573 2c63 6f6c 6f72  color .15s,color
-00013d40: 202e 3135 737d 2e66 726f 6e74 656e 642d   .15s}.frontend-
-00013d50: 6963 6f6e 2d70 6963 6b65 7220 2e69 636f  icon-picker .ico
-00013d60: 6e2d 636f 6e74 6169 6e65 7220 2e69 636f  n-container .ico
-00013d70: 6e2d 7072 6576 6965 777b 7769 6474 683a  n-preview{width:
-00013d80: 3765 6d3b 6865 6967 6874 3a37 656d 3b64  7em;height:7em;d
-00013d90: 6973 706c 6179 3a2d 6d73 2d66 6c65 7862  isplay:-ms-flexb
-00013da0: 6f78 3b64 6973 706c 6179 3a66 6c65 783b  ox;display:flex;
-00013db0: 2d6d 732d 666c 6578 2d64 6972 6563 7469  -ms-flex-directi
-00013dc0: 6f6e 3a63 6f6c 756d 6e3b 666c 6578 2d64  on:column;flex-d
-00013dd0: 6972 6563 7469 6f6e 3a63 6f6c 756d 6e3b  irection:column;
-00013de0: 2d6d 732d 666c 6578 2d70 6163 6b3a 6365  -ms-flex-pack:ce
-00013df0: 6e74 6572 3b6a 7573 7469 6679 2d63 6f6e  nter;justify-con
-00013e00: 7465 6e74 3a63 656e 7465 727d 2e66 726f  tent:center}.fro
-00013e10: 6e74 656e 642d 6963 6f6e 2d70 6963 6b65  ntend-icon-picke
-00013e20: 7220 2e69 636f 6e2d 636f 6e74 6169 6e65  r .icon-containe
-00013e30: 7220 2e69 636f 6e2d 7072 6576 6965 7720  r .icon-preview 
-00013e40: 2e69 636f 6e2d 626f 787b 666f 6e74 2d73  .icon-box{font-s
-00013e50: 697a 653a 3530 3025 3b6c 696e 652d 6865  ize:500%;line-he
-00013e60: 6967 6874 3a31 2e33 3b6d 6172 6769 6e3a  ight:1.3;margin:
-00013e70: 303b 7465 7874 2d61 6c69 676e 3a63 656e  0;text-align:cen
-00013e80: 7465 727d 2e66 726f 6e74 656e 642d 6963  ter}.frontend-ic
-00013e90: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
-00013ea0: 636f 6e74 6169 6e65 7220 2e69 636f 6e2d  container .icon-
-00013eb0: 7072 6576 6965 7720 2e69 636f 6e2d 626f  preview .icon-bo
-00013ec0: 7820 692c 2e66 726f 6e74 656e 642d 6963  x i,.frontend-ic
-00013ed0: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
-00013ee0: 636f 6e74 6169 6e65 7220 2e69 636f 6e2d  container .icon-
-00013ef0: 7072 6576 6965 7720 2e69 636f 6e2d 626f  preview .icon-bo
-00013f00: 7820 7370 616e 7b66 6f6e 742d 7369 7a65  x span{font-size
-00013f10: 3a75 6e73 6574 7d2e 6672 6f6e 7465 6e64  :unset}.frontend
-00013f20: 2d69 636f 6e2d 7069 636b 6572 202e 6963  -icon-picker .ic
-00013f30: 6f6e 2d63 6f6e 7461 696e 6572 202e 6963  on-container .ic
-00013f40: 6f6e 2d70 7265 7669 6577 202e 656d 7074  on-preview .empt
-00013f50: 792d 626f 787b 7465 7874 2d61 6c69 676e  y-box{text-align
-00013f60: 3a63 656e 7465 723b 6f76 6572 666c 6f77  :center;overflow
-00013f70: 3a68 6964 6465 6e3b 7465 7874 2d6f 7665  :hidden;text-ove
-00013f80: 7266 6c6f 773a 656c 6c69 7073 6973 3b6c  rflow:ellipsis;l
-00013f90: 696e 652d 6865 6967 6874 3a31 3b66 6f6e  ine-height:1;fon
-00013fa0: 742d 7369 7a65 3a31 3030 257d 2e66 726f  t-size:100%}.fro
-00013fb0: 6e74 656e 642d 6963 6f6e 2d70 6963 6b65  ntend-icon-picke
-00013fc0: 7220 2e69 636f 6e2d 636f 6e74 6169 6e65  r .icon-containe
-00013fd0: 7220 2e69 636f 6e2d 7072 6576 6965 7720  r .icon-preview 
-00013fe0: 2e65 6d70 7479 2d62 6f78 2e68 6964 6465  .empty-box.hidde
-00013ff0: 6e7b 6469 7370 6c61 793a 6e6f 6e65 7d2e  n{display:none}.
-00014000: 6672 6f6e 7465 6e64 2d69 636f 6e2d 7069  frontend-icon-pi
-00014010: 636b 6572 202e 6963 6f6e 2d63 6f6e 7461  cker .icon-conta
-00014020: 696e 6572 202e 6963 6f6e 2d70 7265 7669  iner .icon-previ
-00014030: 6577 3a68 6f76 6572 7b62 6163 6b67 726f  ew:hover{backgro
-00014040: 756e 643a 7661 7228 2d2d 6463 612d 6772  und:var(--dca-gr
-00014050: 6179 2d6c 6967 6874 2c76 6172 282d 2d62  ay-light,var(--b
-00014060: 6f72 6465 722d 636f 6c6f 722c 2364 3364  order-color,#d3d
-00014070: 3364 3329 293b 6375 7273 6f72 3a70 6f69  3d3));cursor:poi
-00014080: 6e74 6572 7d2e 6672 6f6e 7465 6e64 2d69  nter}.frontend-i
-00014090: 636f 6e2d 7069 636b 6572 202e 6963 6f6e  con-picker .icon
-000140a0: 2d63 6f6e 7461 696e 6572 202e 6963 6f6e  -container .icon
-000140b0: 2d63 6c6f 7365 2d69 6e64 6963 6174 6f72  -close-indicator
-000140c0: 7b64 6973 706c 6179 3a62 6c6f 636b 3b62  {display:block;b
-000140d0: 6f72 6465 722d 7261 6469 7573 3a35 3025  order-radius:50%
-000140e0: 3b63 6f6c 6f72 3a76 6172 282d 2d64 6361  ;color:var(--dca
-000140f0: 2d62 6c61 636b 2c76 6172 282d 2d62 6f64  -black,var(--bod
-00014100: 792d 6667 2c23 3030 3029 293b 6261 636b  y-fg,#000));back
-00014110: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
-00014120: 282d 2d64 6361 2d77 6869 7465 2c76 6172  (--dca-white,var
-00014130: 282d 2d62 6f64 792d 6267 2c23 6666 6629  (--body-bg,#fff)
-00014140: 293b 7061 6464 696e 673a 2e35 7265 6d3b  );padding:.5rem;
-00014150: 626f 7264 6572 3a31 7078 2073 6f6c 6964  border:1px solid
-00014160: 2076 6172 282d 2d64 6361 2d62 6c61 636b   var(--dca-black
-00014170: 2c76 6172 282d 2d62 6f64 792d 6667 2c23  ,var(--body-fg,#
-00014180: 3030 3029 293b 7472 616e 7366 6f72 6d3a  000));transform:
-00014190: 7472 616e 736c 6174 6528 2d35 3025 2c2d  translate(-50%,-
-000141a0: 3530 2529 3b74 6f70 3a30 3b6c 6566 743a  50%);top:0;left:
-000141b0: 3130 3025 3b77 6964 7468 3a2e 3665 6d3b  100%;width:.6em;
-000141c0: 6865 6967 6874 3a2e 3665 6d3b 6c69 6e65  height:.6em;line
-000141d0: 2d68 6569 6768 743a 2e35 656d 3b70 6f73  -height:.5em;pos
-000141e0: 6974 696f 6e3a 6162 736f 6c75 7465 3b74  ition:absolute;t
-000141f0: 7261 6e73 6974 696f 6e3a 6261 636b 6772  ransition:backgr
-00014200: 6f75 6e64 2d63 6f6c 6f72 202e 3135 737d  ound-color .15s}
-00014210: 2e66 726f 6e74 656e 642d 6963 6f6e 2d70  .frontend-icon-p
-00014220: 6963 6b65 7220 2e69 636f 6e2d 636f 6e74  icker .icon-cont
-00014230: 6169 6e65 7220 2e69 636f 6e2d 636c 6f73  ainer .icon-clos
-00014240: 652d 696e 6469 6361 746f 723a 6265 666f  e-indicator:befo
-00014250: 7265 7b63 6f6e 7465 6e74 3a22 c397 227d  re{content:".."}
-00014260: 2e66 726f 6e74 656e 642d 6963 6f6e 2d70  .frontend-icon-p
-00014270: 6963 6b65 7220 2e69 636f 6e2d 636f 6e74  icker .icon-cont
-00014280: 6169 6e65 7220 2e69 636f 6e2d 636c 6f73  ainer .icon-clos
-00014290: 652d 696e 6469 6361 746f 723a 686f 7665  e-indicator:hove
-000142a0: 727b 6261 636b 6772 6f75 6e64 3a76 6172  r{background:var
-000142b0: 282d 2d64 656c 6574 652d 6275 7474 6f6e  (--delete-button
-000142c0: 2d62 672c 7265 6429 3b63 6f6c 6f72 3a76  -bg,red);color:v
-000142d0: 6172 282d 2d64 656c 6574 652d 6275 7474  ar(--delete-butt
-000142e0: 6f6e 2d66 672c 2366 6666 293b 6375 7273  on-fg,#fff);curs
-000142f0: 6f72 3a70 6f69 6e74 6572 7d2e 7569 702d  or:pointer}.uip-
-00014300: 6d6f 6461 6c7b 706f 7369 7469 6f6e 3a66  modal{position:f
-00014310: 6978 6564 3b68 6569 6768 743a 3130 3025  ixed;height:100%
-00014320: 3b77 6964 7468 3a31 3030 253b 626f 7474  ;width:100%;bott
-00014330: 6f6d 3a30 3b6c 6566 743a 303b 6261 636b  om:0;left:0;back
-00014340: 6772 6f75 6e64 2d63 6f6c 6f72 3a72 6762  ground-color:rgb
-00014350: 6128 302c 302c 302c 2e38 293b 7a2d 696e  a(0,0,0,.8);z-in
-00014360: 6465 783a 3939 3939 3b2d 7765 626b 6974  dex:9999;-webkit
-00014370: 2d75 7365 722d 7365 6c65 6374 3a6e 6f6e  -user-select:non
-00014380: 653b 2d6d 732d 7573 6572 2d73 656c 6563  e;-ms-user-selec
-00014390: 743a 6e6f 6e65 3b75 7365 722d 7365 6c65  t:none;user-sele
-000143a0: 6374 3a6e 6f6e 653b 6469 7370 6c61 793a  ct:none;display:
-000143b0: 2d6d 732d 666c 6578 626f 783b 6469 7370  -ms-flexbox;disp
-000143c0: 6c61 793a 666c 6578 3b2d 6d73 2d66 6c65  lay:flex;-ms-fle
-000143d0: 782d 616c 6967 6e3a 6365 6e74 6572 3b61  x-align:center;a
-000143e0: 6c69 676e 2d69 7465 6d73 3a63 656e 7465  lign-items:cente
-000143f0: 727d 2e75 6970 2d6d 6f64 616c 202a 2c2e  r}.uip-modal *,.
-00014400: 7569 702d 6d6f 6461 6c20 3a61 6674 6572  uip-modal :after
-00014410: 2c2e 7569 702d 6d6f 6461 6c20 3a62 6566  ,.uip-modal :bef
-00014420: 6f72 657b 626f 782d 7369 7a69 6e67 3a62  ore{box-sizing:b
-00014430: 6f72 6465 722d 626f 787d 2e75 6970 2d6d  order-box}.uip-m
-00014440: 6f64 616c 2e75 6970 2d63 6c6f 7365 7b6f  odal.uip-close{o
-00014450: 7061 6369 7479 3a30 3b76 6973 6962 696c  pacity:0;visibil
-00014460: 6974 793a 6869 6464 656e 3b74 7261 6e73  ity:hidden;trans
-00014470: 6974 696f 6e3a 616c 6c20 2e34 7320 6561  ition:all .4s ea
-00014480: 7365 2d69 6e2d 6f75 747d 2e75 6970 2d6d  se-in-out}.uip-m
-00014490: 6f64 616c 2e75 6970 2d6f 7065 6e7b 6f70  odal.uip-open{op
-000144a0: 6163 6974 793a 313b 7669 7369 6269 6c69  acity:1;visibili
-000144b0: 7479 3a76 6973 6962 6c65 3b74 7261 6e73  ty:visible;trans
-000144c0: 6974 696f 6e3a 616c 6c20 2e34 7320 6561  ition:all .4s ea
-000144d0: 7365 2d69 6e2d 6f75 747d 2e75 6970 2d6d  se-in-out}.uip-m
-000144e0: 6f64 616c 202e 7569 702d 6d6f 6461 6c2d  odal .uip-modal-
-000144f0: 2d63 6f6e 7465 6e74 7b70 6f73 6974 696f  -content{positio
-00014500: 6e3a 6162 736f 6c75 7465 3b62 6f72 6465  n:absolute;borde
-00014510: 722d 7261 6469 7573 3a33 7078 3b62 6f78  r-radius:3px;box
-00014520: 2d73 6861 646f 773a 3270 7820 3870 7820  -shadow:2px 8px 
-00014530: 3233 7078 2033 7078 2072 6762 6128 302c  23px 3px rgba(0,
-00014540: 302c 302c 2e32 293b 6f76 6572 666c 6f77  0,0,.2);overflow
-00014550: 3a68 6964 6465 6e3b 666f 6e74 2d66 616d  :hidden;font-fam
-00014560: 696c 793a 526f 626f 746f 2c41 7269 616c  ily:Roboto,Arial
-00014570: 2c48 656c 7665 7469 6361 2c56 6572 6461  ,Helvetica,Verda
-00014580: 6e61 2c73 616e 732d 7365 7269 663b 6261  na,sans-serif;ba
-00014590: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-000145a0: 6172 282d 2d64 6361 2d67 7261 792d 6c69  ar(--dca-gray-li
-000145b0: 6768 7465 7374 2c76 6172 282d 2d64 6172  ghtest,var(--dar
-000145c0: 6b65 6e65 642d 6267 2c23 6638 6638 6638  kened-bg,#f8f8f8
-000145d0: 2929 3b77 6964 7468 3a31 3030 253b 6d61  ));width:100%;ma
-000145e0: 7267 696e 3a61 7574 6f3b 6c65 6674 3a30  rgin:auto;left:0
-000145f0: 3b72 6967 6874 3a30 3b6d 6172 6769 6e2d  ;right:0;margin-
-00014600: 626f 7474 6f6d 3a32 656d 7d2e 7569 702d  bottom:2em}.uip-
-00014610: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
-00014620: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
-00014630: 6f64 616c 2d2d 6865 6164 6572 7b70 6164  odal--header{pad
-00014640: 6469 6e67 3a31 3570 7820 3135 7078 3b62  ding:15px 15px;b
-00014650: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00014660: 7661 7228 2d2d 6463 612d 7768 6974 652c  var(--dca-white,
-00014670: 7661 7228 2d2d 6267 2d63 6f6c 6f72 2c23  var(--bg-color,#
-00014680: 6666 6629 293b 626f 782d 7368 6164 6f77  fff));box-shadow
-00014690: 3a30 2030 2038 7078 2072 6762 6128 302c  :0 0 8px rgba(0,
-000146a0: 302c 302c 2e31 293b 706f 7369 7469 6f6e  0,0,.1);position
-000146b0: 3a72 656c 6174 6976 653b 7a2d 696e 6465  :relative;z-inde
-000146c0: 783a 313b 666f 6e74 2d73 697a 653a 3135  x:1;font-size:15
-000146d0: 7078 3b63 6f6c 6f72 3a76 6172 282d 2d64  px;color:var(--d
-000146e0: 6361 2d67 7261 792c 7661 7228 2d2d 626f  ca-gray,var(--bo
-000146f0: 6479 2d71 7569 6574 2d63 6f6c 6f72 2c23  dy-quiet-color,#
-00014700: 3636 3629 293b 666f 6e74 2d77 6569 6768  666));font-weigh
-00014710: 743a 3530 303b 6469 7370 6c61 793a 2d6d  t:500;display:-m
-00014720: 732d 666c 6578 626f 783b 6469 7370 6c61  s-flexbox;displa
-00014730: 793a 666c 6578 3b2d 6d73 2d66 6c65 782d  y:flex;-ms-flex-
-00014740: 616c 6967 6e3a 6365 6e74 6572 3b61 6c69  align:center;ali
-00014750: 676e 2d69 7465 6d73 3a63 656e 7465 723b  gn-items:center;
-00014760: 2d6d 732d 666c 6578 2d70 6163 6b3a 6a75  -ms-flex-pack:ju
-00014770: 7374 6966 793b 6a75 7374 6966 792d 636f  stify;justify-co
-00014780: 6e74 656e 743a 7370 6163 652d 6265 7477  ntent:space-betw
-00014790: 6565 6e7d 2e75 6970 2d6d 6f64 616c 202e  een}.uip-modal .
-000147a0: 7569 702d 6d6f 6461 6c2d 2d63 6f6e 7465  uip-modal--conte
-000147b0: 6e74 202e 7569 702d 6d6f 6461 6c2d 2d68  nt .uip-modal--h
-000147c0: 6561 6465 7220 2e75 6970 2d6d 6f64 616c  eader .uip-modal
-000147d0: 2d2d 6865 6164 6572 2d6c 6f67 6f2d 7469  --header-logo-ti
-000147e0: 746c 657b 7061 6464 696e 672d 746f 703a  tle{padding-top:
-000147f0: 3270 783b 6c69 6e65 2d68 6569 6768 743a  2px;line-height:
-00014800: 313b 7465 7874 2d74 7261 6e73 666f 726d  1;text-transform
-00014810: 3a75 7070 6572 6361 7365 3b66 6f6e 742d  :uppercase;font-
-00014820: 7765 6967 6874 3a37 3030 3b63 7572 736f  weight:700;curso
-00014830: 723a 706f 696e 7465 727d 2e75 6970 2d6d  r:pointer}.uip-m
-00014840: 6f64 616c 202e 7569 702d 6d6f 6461 6c2d  odal .uip-modal-
-00014850: 2d63 6f6e 7465 6e74 202e 7569 702d 6d6f  -content .uip-mo
-00014860: 6461 6c2d 2d68 6561 6465 7220 2e75 6970  dal--header .uip
-00014870: 2d6d 6f64 616c 2d2d 6865 6164 6572 2d63  -modal--header-c
-00014880: 6c6f 7365 2d62 746e 7b63 7572 736f 723a  lose-btn{cursor:
-00014890: 706f 696e 7465 727d 2e75 6970 2d6d 6f64  pointer}.uip-mod
-000148a0: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
-000148b0: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
-000148c0: 6c2d 2d62 6f64 797b 666f 6e74 2d73 697a  l--body{font-siz
-000148d0: 653a 3132 7078 3b6c 696e 652d 6865 6967  e:12px;line-heig
-000148e0: 6874 3a31 2e35 3b62 6f78 2d73 697a 696e  ht:1.5;box-sizin
-000148f0: 673a 626f 7264 6572 2d62 6f78 3b70 6164  g:border-box;pad
-00014900: 6469 6e67 3a30 3b68 6569 6768 743a 3730  ding:0;height:70
-00014910: 7668 3b64 6973 706c 6179 3a2d 6d73 2d66  vh;display:-ms-f
-00014920: 6c65 7862 6f78 3b64 6973 706c 6179 3a66  lexbox;display:f
-00014930: 6c65 783b 6d69 6e2d 6865 6967 6874 3a35  lex;min-height:5
-00014940: 3070 783b 6d61 782d 6865 6967 6874 3a38  0px;max-height:8
-00014950: 3576 683b 6f76 6572 666c 6f77 3a61 7574  5vh;overflow:aut
-00014960: 6f7d 2e75 6970 2d6d 6f64 616c 202e 7569  o}.uip-modal .ui
-00014970: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
-00014980: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
-00014990: 7920 2e75 6970 2d6d 6f64 616c 2d2d 7369  y .uip-modal--si
-000149a0: 6465 6261 727b 2d6d 732d 666c 6578 2d6e  debar{-ms-flex-n
-000149b0: 6567 6174 6976 653a 303b 666c 6578 2d73  egative:0;flex-s
-000149c0: 6872 696e 6b3a 303b 6d61 782d 7769 6474  hrink:0;max-widt
-000149d0: 683a 3235 257d 2e75 6970 2d6d 6f64 616c  h:25%}.uip-modal
-000149e0: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
-000149f0: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
-00014a00: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
-00014a10: 2d2d 7369 6465 6261 7220 2e75 6970 2d6d  --sidebar .uip-m
-00014a20: 6f64 616c 2d2d 7369 6465 6261 722d 7461  odal--sidebar-ta
-00014a30: 6273 7b6d 6172 6769 6e2d 746f 703a 3330  bs{margin-top:30
-00014a40: 7078 7d2e 7569 702d 6d6f 6461 6c20 2e75  px}.uip-modal .u
-00014a50: 6970 2d6d 6f64 616c 2d2d 636f 6e74 656e  ip-modal--conten
-00014a60: 7420 2e75 6970 2d6d 6f64 616c 2d2d 626f  t .uip-modal--bo
-00014a70: 6479 202e 7569 702d 6d6f 6461 6c2d 2d73  dy .uip-modal--s
-00014a80: 6964 6562 6172 202e 7569 702d 6d6f 6461  idebar .uip-moda
-00014a90: 6c2d 2d73 6964 6562 6172 2d74 6162 7320  l--sidebar-tabs 
-00014aa0: 2e75 6970 2d6d 6f64 616c 2d2d 7369 6465  .uip-modal--side
-00014ab0: 6261 722d 7461 622d 6974 656d 7b70 6164  bar-tab-item{pad
-00014ac0: 6469 6e67 3a31 3570 783b 666f 6e74 2d73  ding:15px;font-s
-00014ad0: 697a 653a 3134 7078 3b63 6f6c 6f72 3a76  ize:14px;color:v
-00014ae0: 6172 282d 2d64 6361 2d67 7261 792c 7661  ar(--dca-gray,va
-00014af0: 7228 2d2d 626f 6479 2d71 7569 6574 2d63  r(--body-quiet-c
-00014b00: 6f6c 6f72 2c23 3636 3629 293b 7465 7874  olor,#666));text
-00014b10: 2d61 6c69 676e 3a6c 6566 743b 6375 7273  -align:left;curs
-00014b20: 6f72 3a70 6f69 6e74 6572 3b70 6f73 6974  or:pointer;posit
-00014b30: 696f 6e3a 7265 6c61 7469 7665 3b64 6973  ion:relative;dis
-00014b40: 706c 6179 3a2d 6d73 2d66 6c65 7862 6f78  play:-ms-flexbox
-00014b50: 3b64 6973 706c 6179 3a66 6c65 783b 2d6d  ;display:flex;-m
-00014b60: 732d 666c 6578 2d61 6c69 676e 3a63 656e  s-flex-align:cen
-00014b70: 7465 723b 616c 6967 6e2d 6974 656d 733a  ter;align-items:
-00014b80: 6365 6e74 6572 3b74 6578 742d 7472 616e  center;text-tran
-00014b90: 7366 6f72 6d3a 6361 7069 7461 6c69 7a65  sform:capitalize
-00014ba0: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
-00014bb0: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
-00014bc0: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
-00014bd0: 202e 7569 702d 6d6f 6461 6c2d 2d73 6964   .uip-modal--sid
-00014be0: 6562 6172 202e 7569 702d 6d6f 6461 6c2d  ebar .uip-modal-
-00014bf0: 2d73 6964 6562 6172 2d74 6162 7320 2e75  -sidebar-tabs .u
-00014c00: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
-00014c10: 722d 7461 622d 6974 656d 2069 7b66 6f6e  r-tab-item i{fon
-00014c20: 742d 7369 7a65 3a32 3070 783b 7061 6464  t-size:20px;padd
-00014c30: 696e 672d 7269 6768 743a 3135 7078 3b63  ing-right:15px;c
-00014c40: 6f6c 6f72 3a76 6172 282d 2d64 6361 2d67  olor:var(--dca-g
-00014c50: 7261 792d 6c69 6768 7465 722c 7661 7228  ray-lighter,var(
-00014c60: 2d2d 626f 7264 6572 2d63 6f6c 6f72 2c23  --border-color,#
-00014c70: 6363 6329 297d 2e75 6970 2d6d 6f64 616c  ccc))}.uip-modal
-00014c80: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
-00014c90: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
-00014ca0: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
-00014cb0: 2d2d 7369 6465 6261 7220 2e75 6970 2d6d  --sidebar .uip-m
-00014cc0: 6f64 616c 2d2d 7369 6465 6261 722d 7461  odal--sidebar-ta
-00014cd0: 6273 202e 7569 702d 6d6f 6461 6c2d 2d73  bs .uip-modal--s
-00014ce0: 6964 6562 6172 2d74 6162 2d69 7465 6d20  idebar-tab-item 
-00014cf0: 696d 677b 7061 6464 696e 672d 7269 6768  img{padding-righ
-00014d00: 743a 3135 7078 7d2e 7569 702d 6d6f 6461  t:15px}.uip-moda
-00014d10: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
-00014d20: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
-00014d30: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
-00014d40: 6c2d 2d73 6964 6562 6172 202e 7569 702d  l--sidebar .uip-
-00014d50: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
-00014d60: 6162 7320 2e75 6970 2d6d 6f64 616c 2d2d  abs .uip-modal--
-00014d70: 7369 6465 6261 722d 7461 622d 6974 656d  sidebar-tab-item
-00014d80: 2e75 6e69 7665 7273 616c 2d61 6374 6976  .universal-activ
-00014d90: 657b 6261 636b 6772 6f75 6e64 2d63 6f6c  e{background-col
-00014da0: 6f72 3a76 6172 282d 2d64 6361 2d77 6869  or:var(--dca-whi
-00014db0: 7465 2c76 6172 282d 2d62 672d 636f 6c6f  te,var(--bg-colo
-00014dc0: 722c 2366 6666 2929 3b62 6f78 2d73 6861  r,#fff));box-sha
-00014dd0: 646f 773a 3020 3670 7820 3230 7078 2030  dow:0 6px 20px 0
-00014de0: 2072 6762 6128 302c 302c 302c 2e31 297d   rgba(0,0,0,.1)}
-00014df0: 2e75 6970 2d6d 6f64 616c 202e 7569 702d  .uip-modal .uip-
-00014e00: 6d6f 6461 6c2d 2d63 6f6e 7465 6e74 202e  modal--content .
-00014e10: 7569 702d 6d6f 6461 6c2d 2d62 6f64 7920  uip-modal--body 
-00014e20: 2e75 6970 2d6d 6f64 616c 2d2d 7369 6465  .uip-modal--side
-00014e30: 6261 7220 2e75 6970 2d6d 6f64 616c 2d2d  bar .uip-modal--
-00014e40: 7369 6465 6261 722d 7461 6273 202e 7569  sidebar-tabs .ui
-00014e50: 702d 6d6f 6461 6c2d 2d73 6964 6562 6172  p-modal--sidebar
-00014e60: 2d74 6162 2d69 7465 6d2e 756e 6976 6572  -tab-item.univer
-00014e70: 7361 6c2d 6163 7469 7665 3a61 6674 6572  sal-active:after
-00014e80: 7b63 6f6e 7465 6e74 3a22 223b 706f 7369  {content:"";posi
-00014e90: 7469 6f6e 3a61 6273 6f6c 7574 653b 6865  tion:absolute;he
-00014ea0: 6967 6874 3a31 3030 253b 7769 6474 683a  ight:100%;width:
-00014eb0: 3570 783b 746f 703a 303b 6c65 6674 3a30  5px;top:0;left:0
-00014ec0: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
-00014ed0: 723a 2330 6266 7d2e 7569 702d 6d6f 6461  r:#0bf}.uip-moda
-00014ee0: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
-00014ef0: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
-00014f00: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
-00014f10: 6c2d 2d73 6964 6562 6172 202e 7569 702d  l--sidebar .uip-
-00014f20: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
-00014f30: 6162 7320 2e75 6970 2d6d 6f64 616c 2d2d  abs .uip-modal--
-00014f40: 7369 6465 6261 722d 7461 622d 6974 656d  sidebar-tab-item
-00014f50: 2e75 6e69 7665 7273 616c 2d61 6374 6976  .universal-activ
-00014f60: 6520 697b 636f 6c6f 723a 2330 6266 7d2e  e i{color:#0bf}.
-00014f70: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-00014f80: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
-00014f90: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
-00014fa0: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
-00014fb0: 6172 202e 7569 702d 6d6f 6461 6c2d 2d73  ar .uip-modal--s
-00014fc0: 6964 6562 6172 2d74 6162 7320 2e75 6970  idebar-tabs .uip
-00014fd0: 2d6d 6f64 616c 2d2d 7369 6465 6261 722d  -modal--sidebar-
-00014fe0: 7461 622d 6974 656d 3a6f 6e6c 792d 6368  tab-item:only-ch
-00014ff0: 696c 647b 6469 7370 6c61 793a 6e6f 6e65  ild{display:none
-00015000: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
-00015010: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
-00015020: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
-00015030: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
-00015040: 6e2d 7072 6576 6965 772d 7772 6170 7b64  n-preview-wrap{d
-00015050: 6973 706c 6179 3a2d 6d73 2d66 6c65 7862  isplay:-ms-flexb
-00015060: 6f78 3b64 6973 706c 6179 3a66 6c65 783b  ox;display:flex;
-00015070: 2d6d 732d 666c 6578 2d64 6972 6563 7469  -ms-flex-directi
-00015080: 6f6e 3a63 6f6c 756d 6e3b 666c 6578 2d64  on:column;flex-d
-00015090: 6972 6563 7469 6f6e 3a63 6f6c 756d 6e3b  irection:column;
-000150a0: 7061 6464 696e 673a 3330 7078 2038 3070  padding:30px 80p
-000150b0: 7820 303b 7769 6474 683a 3130 3025 7d2e  x 0;width:100%}.
-000150c0: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-000150d0: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
-000150e0: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
-000150f0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-00015100: 7072 6576 6965 772d 7772 6170 202e 7569  preview-wrap .ui
-00015110: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7072  p-modal--icon-pr
-00015120: 6576 6965 772d 696e 6e65 727b 6f76 6572  eview-inner{over
-00015130: 666c 6f77 3a61 7574 6f3b 6d61 7267 696e  flow:auto;margin
-00015140: 3a32 3570 7820 2d31 3570 7820 303b 7061  :25px -15px 0;pa
-00015150: 6464 696e 673a 3020 3135 7078 2031 3570  dding:0 15px 15p
-00015160: 787d 2e75 6970 2d6d 6f64 616c 202e 7569  x}.uip-modal .ui
-00015170: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
-00015180: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
-00015190: 7920 2e75 6970 2d6d 6f64 616c 2d2d 6963  y .uip-modal--ic
-000151a0: 6f6e 2d70 7265 7669 6577 2d77 7261 7020  on-preview-wrap 
-000151b0: 2e75 6970 2d6d 6f64 616c 2d2d 6963 6f6e  .uip-modal--icon
-000151c0: 2d70 7265 7669 6577 2d69 6e6e 6572 202e  -preview-inner .
-000151d0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-000151e0: 7072 6576 6965 777b 6469 7370 6c61 793a  preview{display:
-000151f0: 2d6d 732d 6772 6964 3b64 6973 706c 6179  -ms-grid;display
-00015200: 3a67 7269 643b 6772 6964 2d67 6170 3a32  :grid;grid-gap:2
-00015210: 3070 783b 6d61 7267 696e 3a32 3070 7820  0px;margin:20px 
-00015220: 307d 2e75 6970 2d6d 6f64 616c 202e 7569  0}.uip-modal .ui
-00015230: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
-00015240: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
-00015250: 7920 2e75 6970 2d6d 6f64 616c 2d2d 6963  y .uip-modal--ic
-00015260: 6f6e 2d70 7265 7669 6577 2d77 7261 7020  on-preview-wrap 
-00015270: 2e75 6970 2d6d 6f64 616c 2d2d 6963 6f6e  .uip-modal--icon
-00015280: 2d70 7265 7669 6577 2d69 6e6e 6572 202e  -preview-inner .
-00015290: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-000152a0: 7072 6576 6965 7720 2e75 6970 2d69 636f  preview .uip-ico
-000152b0: 6e2d 6974 656d 7b70 6f73 6974 696f 6e3a  n-item{position:
-000152c0: 7265 6c61 7469 7665 3b70 6164 6469 6e67  relative;padding
-000152d0: 3a31 3070 783b 6261 636b 6772 6f75 6e64  :10px;background
-000152e0: 2d63 6f6c 6f72 3a76 6172 282d 2d64 6361  -color:var(--dca
-000152f0: 2d77 6869 7465 2c76 6172 282d 2d62 672d  -white,var(--bg-
-00015300: 636f 6c6f 722c 2366 6666 2929 3b62 6f78  color,#fff));box
-00015310: 2d73 6861 646f 773a 3020 3170 7820 3132  -shadow:0 1px 12
-00015320: 7078 2072 6762 6128 302c 302c 302c 2e30  px rgba(0,0,0,.0
-00015330: 3529 3b62 6f72 6465 722d 7261 6469 7573  5);border-radius
-00015340: 3a33 7078 3b63 7572 736f 723a 706f 696e  :3px;cursor:poin
-00015350: 7465 723b 7472 616e 7369 7469 6f6e 3a61  ter;transition:a
-00015360: 6c6c 202e 3373 3b6f 7665 7266 6c6f 773a  ll .3s;overflow:
-00015370: 6869 6464 656e 7d2e 7569 702d 6d6f 6461  hidden}.uip-moda
-00015380: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
-00015390: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
-000153a0: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
-000153b0: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
-000153c0: 7772 6170 202e 7569 702d 6d6f 6461 6c2d  wrap .uip-modal-
-000153d0: 2d69 636f 6e2d 7072 6576 6965 772d 696e  -icon-preview-in
-000153e0: 6e65 7220 2e75 6970 2d6d 6f64 616c 2d2d  ner .uip-modal--
-000153f0: 6963 6f6e 2d70 7265 7669 6577 202e 7569  icon-preview .ui
-00015400: 702d 6963 6f6e 2d69 7465 6d3a 686f 7665  p-icon-item:hove
-00015410: 727b 626f 782d 7368 6164 6f77 3a30 2031  r{box-shadow:0 1
-00015420: 7078 2031 3470 7820 7267 6261 2830 2c30  px 14px rgba(0,0
-00015430: 2c30 2c2e 3136 297d 2e75 6970 2d6d 6f64  ,0,.16)}.uip-mod
-00015440: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
-00015450: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
-00015460: 6c2d 2d62 6f64 7920 2e75 6970 2d6d 6f64  l--body .uip-mod
-00015470: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
-00015480: 2d77 7261 7020 2e75 6970 2d6d 6f64 616c  -wrap .uip-modal
-00015490: 2d2d 6963 6f6e 2d70 7265 7669 6577 2d69  --icon-preview-i
-000154a0: 6e6e 6572 202e 7569 702d 6d6f 6461 6c2d  nner .uip-modal-
-000154b0: 2d69 636f 6e2d 7072 6576 6965 7720 2e75  -icon-preview .u
-000154c0: 6970 2d69 636f 6e2d 6974 656d 2e75 6e69  ip-icon-item.uni
-000154d0: 7665 7273 616c 2d73 656c 6563 7465 647b  versal-selected{
-000154e0: 626f 782d 7368 6164 6f77 3a30 2031 7078  box-shadow:0 1px
-000154f0: 2031 3270 7820 7267 6261 2830 2c30 2c30   12px rgba(0,0,0
-00015500: 2c2e 3035 292c 3020 3020 3020 3370 7820  ,.05),0 0 0 3px 
-00015510: 2330 6266 7d2e 7569 702d 6d6f 6461 6c20  #0bf}.uip-modal 
-00015520: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
-00015530: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
-00015540: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
-00015550: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
-00015560: 6170 202e 7569 702d 6d6f 6461 6c2d 2d69  ap .uip-modal--i
-00015570: 636f 6e2d 7072 6576 6965 772d 696e 6e65  con-preview-inne
-00015580: 7220 2e75 6970 2d6d 6f64 616c 2d2d 6963  r .uip-modal--ic
-00015590: 6f6e 2d70 7265 7669 6577 202e 7569 702d  on-preview .uip-
-000155a0: 6963 6f6e 2d69 7465 6d20 2e75 6970 2d69  icon-item .uip-i
-000155b0: 636f 6e2d 6974 656d 2d69 6e6e 6572 7b64  con-item-inner{d
-000155c0: 6973 706c 6179 3a2d 6d73 2d66 6c65 7862  isplay:-ms-flexb
-000155d0: 6f78 3b64 6973 706c 6179 3a66 6c65 783b  ox;display:flex;
-000155e0: 2d6d 732d 666c 6578 2d64 6972 6563 7469  -ms-flex-directi
-000155f0: 6f6e 3a63 6f6c 756d 6e3b 666c 6578 2d64  on:column;flex-d
-00015600: 6972 6563 7469 6f6e 3a63 6f6c 756d 6e3b  irection:column;
-00015610: 2d6d 732d 666c 6578 2d61 6c69 676e 3a63  -ms-flex-align:c
-00015620: 656e 7465 723b 616c 6967 6e2d 6974 656d  enter;align-item
-00015630: 733a 6365 6e74 6572 3b70 6164 6469 6e67  s:center;padding
-00015640: 3a31 7078 7d2e 7569 702d 6d6f 6461 6c20  :1px}.uip-modal 
-00015650: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
-00015660: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
-00015670: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
-00015680: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
-00015690: 6170 202e 7569 702d 6d6f 6461 6c2d 2d69  ap .uip-modal--i
-000156a0: 636f 6e2d 7072 6576 6965 772d 696e 6e65  con-preview-inne
-000156b0: 7220 2e75 6970 2d6d 6f64 616c 2d2d 6963  r .uip-modal--ic
-000156c0: 6f6e 2d70 7265 7669 6577 202e 7569 702d  on-preview .uip-
-000156d0: 6963 6f6e 2d69 7465 6d20 2e75 6970 2d69  icon-item .uip-i
-000156e0: 636f 6e2d 6974 656d 2d69 6e6e 6572 202e  con-item-inner .
-000156f0: 7569 702d 6963 6f6e 2d69 7465 6d5f 5f69  uip-icon-item__i
-00015700: 636f 6e2c 2e75 6970 2d6d 6f64 616c 202e  con,.uip-modal .
-00015710: 7569 702d 6d6f 6461 6c2d 2d63 6f6e 7465  uip-modal--conte
-00015720: 6e74 202e 7569 702d 6d6f 6461 6c2d 2d62  nt .uip-modal--b
-00015730: 6f64 7920 2e75 6970 2d6d 6f64 616c 2d2d  ody .uip-modal--
-00015740: 6963 6f6e 2d70 7265 7669 6577 2d77 7261  icon-preview-wra
-00015750: 7020 2e75 6970 2d6d 6f64 616c 2d2d 6963  p .uip-modal--ic
-00015760: 6f6e 2d70 7265 7669 6577 2d69 6e6e 6572  on-preview-inner
-00015770: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
-00015780: 6e2d 7072 6576 6965 7720 2e75 6970 2d69  n-preview .uip-i
-00015790: 636f 6e2d 6974 656d 202e 7569 702d 6963  con-item .uip-ic
-000157a0: 6f6e 2d69 7465 6d2d 696e 6e65 7220 697b  on-item-inner i{
-000157b0: 666f 6e74 2d73 697a 653a 3235 7078 3b63  font-size:25px;c
-000157c0: 6f6c 6f72 3a76 6172 282d 2d64 6361 2d67  olor:var(--dca-g
-000157d0: 7261 792d 6461 726b 6573 742c 7661 7228  ray-darkest,var(
-000157e0: 2d2d 626f 6479 2d66 672c 2333 3333 2929  --body-fg,#333))
-000157f0: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
-00015800: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
-00015810: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
-00015820: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
-00015830: 6e2d 7072 6576 6965 772d 7772 6170 202e  n-preview-wrap .
-00015840: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-00015850: 7072 6576 6965 772d 696e 6e65 7220 2e75  preview-inner .u
-00015860: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
-00015870: 7265 7669 6577 202e 7569 702d 6963 6f6e  review .uip-icon
-00015880: 2d69 7465 6d20 2e75 6970 2d69 636f 6e2d  -item .uip-icon-
-00015890: 6974 656d 2d69 6e6e 6572 202e 7569 702d  item-inner .uip-
-000158a0: 6963 6f6e 2d69 7465 6d2d 6e61 6d65 7b63  icon-item-name{c
-000158b0: 6f6c 6f72 3a76 6172 282d 2d64 6361 2d67  olor:var(--dca-g
-000158c0: 7261 792c 7661 7228 2d2d 626f 6479 2d71  ray,var(--body-q
-000158d0: 7569 6574 2d63 6f6c 6f72 2c23 3636 3629  uiet-color,#666)
-000158e0: 293b 666f 6e74 2d73 697a 653a 3131 7078  );font-size:11px
-000158f0: 3b70 6164 6469 6e67 3a31 3370 7820 3020  ;padding:13px 0 
-00015900: 303b 6d61 782d 7769 6474 683a 3130 3025  0;max-width:100%
-00015910: 3b77 6869 7465 2d73 7061 6365 3a6e 6f77  ;white-space:now
-00015920: 7261 703b 7465 7874 2d6f 7665 7266 6c6f  rap;text-overflo
-00015930: 773a 656c 6c69 7073 6973 3b6f 7665 7266  w:ellipsis;overf
-00015940: 6c6f 773a 6869 6464 656e 3b74 6578 742d  low:hidden;text-
-00015950: 7472 616e 7366 6f72 6d3a 6361 7069 7461  transform:capita
-00015960: 6c69 7a65 7d2e 7569 702d 6d6f 6461 6c20  lize}.uip-modal 
-00015970: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
-00015980: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
-00015990: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
-000159a0: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
-000159b0: 6170 202e 7569 702d 6d6f 6461 6c2d 2d69  ap .uip-modal--i
-000159c0: 636f 6e2d 7365 6172 6368 7b70 6f73 6974  con-search{posit
-000159d0: 696f 6e3a 7265 6c61 7469 7665 7d2e 7569  ion:relative}.ui
-000159e0: 702d 6d6f 6461 6c20 2e75 6970 2d6d 6f64  p-modal .uip-mod
-000159f0: 616c 2d2d 636f 6e74 656e 7420 2e75 6970  al--content .uip
-00015a00: 2d6d 6f64 616c 2d2d 626f 6479 202e 7569  -modal--body .ui
-00015a10: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7072  p-modal--icon-pr
-00015a20: 6576 6965 772d 7772 6170 202e 7569 702d  eview-wrap .uip-
-00015a30: 6d6f 6461 6c2d 2d69 636f 6e2d 7365 6172  modal--icon-sear
-00015a40: 6368 2069 6e70 7574 7b77 6964 7468 3a31  ch input{width:1
-00015a50: 3030 253b 7061 6464 696e 673a 3870 7820  00%;padding:8px 
-00015a60: 3135 7078 3b62 6163 6b67 726f 756e 642d  15px;background-
-00015a70: 636f 6c6f 723a 7661 7228 2d2d 6463 612d  color:var(--dca-
-00015a80: 7768 6974 652c 7661 7228 2d2d 6267 2d63  white,var(--bg-c
-00015a90: 6f6c 6f72 2c23 6666 6629 293b 626f 7264  olor,#fff));bord
-00015aa0: 6572 3a6e 6f6e 657d 2e75 6970 2d6d 6f64  er:none}.uip-mod
-00015ab0: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
-00015ac0: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
-00015ad0: 6c2d 2d62 6f64 7920 2e75 6970 2d6d 6f64  l--body .uip-mod
-00015ae0: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
-00015af0: 2d77 7261 7020 2e75 6970 2d6d 6f64 616c  -wrap .uip-modal
-00015b00: 2d2d 6963 6f6e 2d73 6561 7263 6820 696e  --icon-search in
-00015b10: 7075 743a 2d6d 732d 696e 7075 742d 706c  put:-ms-input-pl
-00015b20: 6163 6568 6f6c 6465 727b 666f 6e74 2d73  aceholder{font-s
-00015b30: 7479 6c65 3a69 7461 6c69 637d 2e75 6970  tyle:italic}.uip
-00015b40: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
-00015b50: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
-00015b60: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
-00015b70: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
-00015b80: 7669 6577 2d77 7261 7020 2e75 6970 2d6d  view-wrap .uip-m
-00015b90: 6f64 616c 2d2d 6963 6f6e 2d73 6561 7263  odal--icon-searc
-00015ba0: 6820 696e 7075 743a 3a70 6c61 6365 686f  h input::placeho
-00015bb0: 6c64 6572 7b66 6f6e 742d 7374 796c 653a  lder{font-style:
-00015bc0: 6974 616c 6963 7d2e 7569 702d 6d6f 6461  italic}.uip-moda
-00015bd0: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
-00015be0: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
-00015bf0: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
-00015c00: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
-00015c10: 7772 6170 202e 7569 702d 6d6f 6461 6c2d  wrap .uip-modal-
-00015c20: 2d69 636f 6e2d 7365 6172 6368 2069 6d67  -icon-search img
-00015c30: 7b70 6f73 6974 696f 6e3a 6162 736f 6c75  {position:absolu
-00015c40: 7465 3b74 6f70 3a35 3025 3b74 7261 6e73  te;top:50%;trans
-00015c50: 666f 726d 3a74 7261 6e73 6c61 7465 5928  form:translateY(
-00015c60: 2d35 3025 293b 7269 6768 743a 3130 7078  -50%);right:10px
-00015c70: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
-00015c80: 2d6d 6f64 616c 2d2d 666f 6f74 6572 7b62  -modal--footer{b
-00015c90: 6f72 6465 722d 746f 703a 3170 7820 736f  order-top:1px so
-00015ca0: 6c69 6420 7661 7228 2d2d 6463 612d 6772  lid var(--dca-gr
-00015cb0: 6179 2d6c 6967 6874 6572 2c76 6172 282d  ay-lighter,var(-
-00015cc0: 2d62 6f72 6465 722d 636f 6c6f 722c 2363  -border-color,#c
-00015cd0: 6363 2929 3b74 6578 742d 616c 6967 6e3a  cc));text-align:
-00015ce0: 6365 6e74 6572 3b62 6163 6b67 726f 756e  center;backgroun
-00015cf0: 642d 636f 6c6f 723a 7661 7228 2d2d 6463  d-color:var(--dc
-00015d00: 612d 7768 6974 652c 7661 7228 2d2d 6267  a-white,var(--bg
-00015d10: 2d63 6f6c 6f72 2c23 6666 6629 293b 626f  -color,#fff));bo
-00015d20: 7264 6572 3a6e 6f6e 653b 6469 7370 6c61  rder:none;displa
-00015d30: 793a 6e6f 6e65 3b2d 6d73 2d66 6c65 782d  y:none;-ms-flex-
-00015d40: 7061 636b 3a65 6e64 3b6a 7573 7469 6679  pack:end;justify
-00015d50: 2d63 6f6e 7465 6e74 3a66 6c65 782d 656e  -content:flex-en
-00015d60: 643b 7061 6464 696e 673a 3570 783b 626f  d;padding:5px;bo
-00015d70: 782d 7368 6164 6f77 3a30 2030 2038 7078  x-shadow:0 0 8px
-00015d80: 2072 6762 6128 302c 302c 302c 2e31 293b   rgba(0,0,0,.1);
-00015d90: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
-00015da0: 653b 6469 7370 6c61 793a 2d6d 732d 666c  e;display:-ms-fl
-00015db0: 6578 626f 783b 6469 7370 6c61 793a 666c  exbox;display:fl
-00015dc0: 6578 7d2e 7569 702d 6d6f 6461 6c20 2e75  ex}.uip-modal .u
-00015dd0: 6970 2d6d 6f64 616c 2d2d 666f 6f74 6572  ip-modal--footer
-00015de0: 2062 7574 746f 6e2e 7569 702d 696e 7365   button.uip-inse
-00015df0: 7274 2d69 636f 6e2d 6275 7474 6f6e 7b70  rt-icon-button{p
-00015e00: 6164 6469 6e67 3a31 3070 7820 3335 7078  adding:10px 35px
-00015e10: 2169 6d70 6f72 7461 6e74 3b63 6f6c 6f72  !important;color
-00015e20: 3a76 6172 282d 2d64 6361 2d77 6869 7465  :var(--dca-white
-00015e30: 2c76 6172 282d 2d62 672d 636f 6c6f 722c  ,var(--bg-color,
-00015e40: 2366 6666 2929 2169 6d70 6f72 7461 6e74  #fff))!important
-00015e50: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
-00015e60: 723a 2330 6266 2169 6d70 6f72 7461 6e74  r:#0bf!important
-00015e70: 3b62 6f72 6465 723a 6e6f 6e65 3b63 7572  ;border:none;cur
-00015e80: 736f 723a 706f 696e 7465 723b 6f75 746c  sor:pointer;outl
-00015e90: 696e 653a 307d 2e75 6970 2d6d 6f64 616c  ine:0}.uip-modal
-00015ea0: 202e 7569 702d 6d6f 6461 6c2d 2d66 6f6f   .uip-modal--foo
-00015eb0: 7465 7220 2e75 6e69 7665 7273 616c 2d62  ter .universal-b
-00015ec0: 7574 746f 6e7b 6865 6967 6874 3a34 3070  utton{height:40p
-00015ed0: 783b 6d61 7267 696e 2d6c 6566 743a 3570  x;margin-left:5p
-00015ee0: 787d 2e75 6970 2d6d 6f64 616c 202e 7569  x}.uip-modal .ui
-00015ef0: 702d 6d6f 6461 6c2d 2d66 6f6f 7465 7220  p-modal--footer 
-00015f00: 2e75 6e69 7665 7273 616c 2d62 7574 746f  .universal-butto
-00015f10: 6e2d 7375 6363 6573 737b 7061 6464 696e  n-success{paddin
-00015f20: 673a 3132 7078 2033 3670 783b 636f 6c6f  g:12px 36px;colo
-00015f30: 723a 7661 7228 2d2d 6463 612d 7768 6974  r:var(--dca-whit
-00015f40: 652c 7661 7228 2d2d 6267 2d63 6f6c 6f72  e,var(--bg-color
-00015f50: 2c23 6666 6629 293b 7769 6474 683a 696e  ,#fff));width:in
-00015f60: 6974 6961 6c7d 2e75 6970 2d6d 6f64 616c  itial}.uip-modal
-00015f70: 202e 7569 702d 6d6f 6461 6c2d 2d66 6f6f   .uip-modal--foo
-00015f80: 7465 7220 2e75 6e69 7665 7273 616c 2d62  ter .universal-b
-00015f90: 7574 746f 6e2d 7375 6363 6573 733a 686f  utton-success:ho
-00015fa0: 7665 727b 6261 636b 6772 6f75 6e64 2d63  ver{background-c
-00015fb0: 6f6c 6f72 3a23 3062 667d 406d 6564 6961  olor:#0bf}@media
-00015fc0: 2028 6d69 6e2d 7769 6474 683a 3134 3430   (min-width:1440
-00015fd0: 7078 297b 626f 6479 3a6e 6f74 282e 636d  px){body:not(.cm
-00015fe0: 732d 6164 6d69 6e2d 6d6f 6461 6c29 202e  s-admin-modal) .
-00015ff0: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-00016000: 6f64 616c 2d2d 636f 6e74 656e 747b 6d61  odal--content{ma
-00016010: 782d 7769 6474 683a 3132 3030 7078 7d7d  x-width:1200px}}
-00016020: 406d 6564 6961 2028 6d61 782d 7769 6474  @media (max-widt
-00016030: 683a 3134 3339 7078 297b 626f 6479 3a6e  h:1439px){body:n
-00016040: 6f74 282e 636d 732d 6164 6d69 6e2d 6d6f  ot(.cms-admin-mo
-00016050: 6461 6c29 202e 7569 702d 6d6f 6461 6c20  dal) .uip-modal 
-00016060: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
-00016070: 656e 747b 6d61 782d 7769 6474 683a 3939  ent{max-width:99
-00016080: 3070 787d 2e75 6970 2d6d 6f64 616c 2d2d  0px}.uip-modal--
-00016090: 6963 6f6e 2d70 7265 7669 6577 2d77 7261  icon-preview-wra
-000160a0: 707b 7061 6464 696e 673a 3330 7078 2035  p{padding:30px 5
-000160b0: 3070 7820 307d 7d40 6d65 6469 6120 286d  0px 0}}@media (m
-000160c0: 6178 2d77 6964 7468 3a31 3032 3370 7829  ax-width:1023px)
-000160d0: 7b62 6f64 793a 6e6f 7428 2e63 6d73 2d61  {body:not(.cms-a
-000160e0: 646d 696e 2d6d 6f64 616c 2920 2e75 6970  dmin-modal) .uip
-000160f0: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
-00016100: 6c2d 2d63 6f6e 7465 6e74 7b6d 6178 2d77  l--content{max-w
-00016110: 6964 7468 3a37 3430 7078 7d7d 406d 6564  idth:740px}}@med
-00016120: 6961 2028 6d61 782d 7769 6474 683a 3736  ia (max-width:76
-00016130: 3770 7829 7b2e 7569 702d 6d6f 6461 6c2d  7px){.uip-modal-
-00016140: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
-00016150: 6170 7b70 6164 6469 6e67 3a31 3570 7821  ap{padding:15px!
-00016160: 696d 706f 7274 616e 747d 2e75 6970 2d6d  important}.uip-m
-00016170: 6f64 616c 2d2d 7369 6465 6261 727b 6469  odal--sidebar{di
-00016180: 7370 6c61 793a 6e6f 6e65 7d7d 406d 6564  splay:none}}@med
-00016190: 6961 2028 6d69 6e2d 7769 6474 683a 3134  ia (min-width:14
-000161a0: 3430 7078 297b 2e75 6970 2d6d 6f64 616c  40px){.uip-modal
-000161b0: 2d2d 6963 6f6e 2d70 7265 7669 6577 7b2d  --icon-preview{-
-000161c0: 6d73 2d67 7269 642d 636f 6c75 6d6e 733a  ms-grid-columns:
-000161d0: 2831 6672 295b 375d 3b67 7269 642d 7465  (1fr)[7];grid-te
-000161e0: 6d70 6c61 7465 2d63 6f6c 756d 6e73 3a72  mplate-columns:r
-000161f0: 6570 6561 7428 372c 3166 7229 7d7d 406d  epeat(7,1fr)}}@m
-00016200: 6564 6961 2028 6d61 782d 7769 6474 683a  edia (max-width:
-00016210: 3134 3339 7078 297b 2e75 6970 2d6d 6f64  1439px){.uip-mod
-00016220: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
-00016230: 7b2d 6d73 2d67 7269 642d 636f 6c75 6d6e  {-ms-grid-column
-00016240: 733a 2831 6672 295b 365d 3b67 7269 642d  s:(1fr)[6];grid-
-00016250: 7465 6d70 6c61 7465 2d63 6f6c 756d 6e73  template-columns
-00016260: 3a72 6570 6561 7428 362c 3166 7229 7d7d  :repeat(6,1fr)}}
-00016270: 406d 6564 6961 2028 6d61 782d 7769 6474  @media (max-widt
-00016280: 683a 3130 3234 7078 297b 2e75 6970 2d6d  h:1024px){.uip-m
-00016290: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
-000162a0: 6577 7b2d 6d73 2d67 7269 642d 636f 6c75  ew{-ms-grid-colu
-000162b0: 6d6e 733a 2831 6672 295b 355d 3b67 7269  mns:(1fr)[5];gri
-000162c0: 642d 7465 6d70 6c61 7465 2d63 6f6c 756d  d-template-colum
-000162d0: 6e73 3a72 6570 6561 7428 352c 3166 7229  ns:repeat(5,1fr)
-000162e0: 7d7d 406d 6564 6961 2028 6d61 782d 7769  }}@media (max-wi
-000162f0: 6474 683a 3736 3770 7829 7b2e 7569 702d  dth:767px){.uip-
-00016300: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
-00016310: 6965 777b 2d6d 732d 6772 6964 2d63 6f6c  iew{-ms-grid-col
-00016320: 756d 6e73 3a28 3166 7229 5b34 5d3b 6772  umns:(1fr)[4];gr
-00016330: 6964 2d74 656d 706c 6174 652d 636f 6c75  id-template-colu
-00016340: 6d6e 733a 7265 7065 6174 2834 2c31 6672  mns:repeat(4,1fr
-00016350: 297d 7d40 6d65 6469 6120 286d 6178 2d77  )}}@media (max-w
-00016360: 6964 7468 3a34 3739 7078 297b 2e75 6970  idth:479px){.uip
-00016370: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
-00016380: 7669 6577 7b2d 6d73 2d67 7269 642d 636f  view{-ms-grid-co
-00016390: 6c75 6d6e 733a 2831 6672 295b 335d 3b67  lumns:(1fr)[3];g
-000163a0: 7269 642d 7465 6d70 6c61 7465 2d63 6f6c  rid-template-col
-000163b0: 756d 6e73 3a72 6570 6561 7428 332c 3166  umns:repeat(3,1f
-000163c0: 7229 7d7d 406d 6564 6961 2028 6d61 782d  r)}}@media (max-
-000163d0: 7769 6474 683a 3134 3339 7078 297b 2e75  width:1439px){.u
-000163e0: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
-000163f0: 722d 7461 622d 6974 656d 7b70 6164 6469  r-tab-item{paddi
-00016400: 6e67 3a31 3570 7820 3135 7078 2031 3570  ng:15px 15px 15p
-00016410: 7820 3235 7078 3b66 6f6e 742d 7369 7a65  x 25px;font-size
-00016420: 3a31 3170 787d 2e75 6970 2d6d 6f64 616c  :11px}.uip-modal
-00016430: 2d2d 7369 6465 6261 722d 7461 622d 6974  --sidebar-tab-it
-00016440: 656d 2069 7b66 6f6e 742d 7369 7a65 3a31  em i{font-size:1
-00016450: 3570 787d 7d40 6d65 6469 6120 286d 6178  5px}}@media (max
-00016460: 2d77 6964 7468 3a31 3032 3470 7829 7b2e  -width:1024px){.
-00016470: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
-00016480: 6172 2d74 6162 2d69 7465 6d20 692c 2e75  ar-tab-item i,.u
-00016490: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
-000164a0: 722d 7461 622d 6974 656d 2069 6d67 7b64  r-tab-item img{d
-000164b0: 6973 706c 6179 3a6e 6f6e 657d 7d2e 7372  isplay:none}}.sr
-000164c0: 2d6f 6e6c 797b 706f 7369 7469 6f6e 3a61  -only{position:a
-000164d0: 6273 6f6c 7574 6521 696d 706f 7274 616e  bsolute!importan
-000164e0: 743b 7769 6474 683a 3170 7821 696d 706f  t;width:1px!impo
-000164f0: 7274 616e 743b 6865 6967 6874 3a31 7078  rtant;height:1px
-00016500: 2169 6d70 6f72 7461 6e74 3b70 6164 6469  !important;paddi
-00016510: 6e67 3a30 2169 6d70 6f72 7461 6e74 3b6d  ng:0!important;m
-00016520: 6172 6769 6e3a 2d31 7078 2169 6d70 6f72  argin:-1px!impor
-00016530: 7461 6e74 3b6f 7665 7266 6c6f 773a 6869  tant;overflow:hi
-00016540: 6464 656e 2169 6d70 6f72 7461 6e74 3b63  dden!important;c
-00016550: 6c69 703a 7265 6374 2830 2c30 2c30 2c30  lip:rect(0,0,0,0
-00016560: 2921 696d 706f 7274 616e 743b 7768 6974  )!important;whit
-00016570: 652d 7370 6163 653a 6e6f 7772 6170 2169  e-space:nowrap!i
-00016580: 6d70 6f72 7461 6e74 3b62 6f72 6465 723a  mportant;border:
-00016590: 3021 696d 706f 7274 616e 747d 756c 2e6e  0!important}ul.n
-000165a0: 6176 7b6d 6172 6769 6e2d 626f 7474 6f6d  av{margin-bottom
-000165b0: 3a31 656d 7d75 6c2e 6e61 763e 6c69 2e6e  :1em}ul.nav>li.n
-000165c0: 6176 2d69 7465 6d7b 6c69 7374 2d73 7479  av-item{list-sty
-000165d0: 6c65 2d74 7970 653a 6e6f 6e65 3b70 6164  le-type:none;pad
-000165e0: 6469 6e67 3a69 6e68 6572 6974 7d2e 636f  ding:inherit}.co
-000165f0: 6c4d 2075 6c3a 6e6f 7428 2e6f 626a 6563  lM ul:not(.objec
-00016600: 742d 746f 6f6c 7329 2e6e 6176 7b6d 6172  t-tools).nav{mar
-00016610: 6769 6e2d 746f 703a 303b 6d61 7267 696e  gin-top:0;margin
-00016620: 2d62 6f74 746f 6d3a 3230 7078 7d75 6c2e  -bottom:20px}ul.
-00016630: 6e61 7620 2e6e 6176 2d69 7465 6d7b 6d61  nav .nav-item{ma
-00016640: 7267 696e 2d72 6967 6874 3a31 7265 6d7d  rgin-right:1rem}
-00016650: 756c 2e6e 6176 202e 6e61 762d 6c69 6e6b  ul.nav .nav-link
-00016660: 7b70 6f73 6974 696f 6e3a 7265 6c61 7469  {position:relati
-00016670: 7665 3b74 6578 742d 6465 636f 7261 7469  ve;text-decorati
-00016680: 6f6e 3a6e 6f6e 657d 756c 2e6e 6176 202e  on:none}ul.nav .
-00016690: 6e61 762d 6c69 6e6b 2073 7061 6e2e 696e  nav-link span.in
-000166a0: 6469 6361 746f 727b 6469 7370 6c61 793a  dicator{display:
-000166b0: 6e6f 6e65 3b62 6f72 6465 722d 7261 6469  none;border-radi
-000166c0: 7573 3a35 3025 3b70 6164 6469 6e67 3a2e  us:50%;padding:.
-000166d0: 3572 656d 3b62 6f72 6465 723a 3170 7820  5rem;border:1px 
-000166e0: 736f 6c69 6420 7661 7228 2d2d 6463 612d  solid var(--dca-
-000166f0: 7768 6974 652c 7661 7228 2d2d 626f 6479  white,var(--body
-00016700: 2d62 672c 2366 6666 2929 3b74 7261 6e73  -bg,#fff));trans
-00016710: 666f 726d 3a74 7261 6e73 6c61 7465 282d  form:translate(-
-00016720: 3530 252c 2d35 3025 293b 746f 703a 303b  50%,-50%);top:0;
-00016730: 6c65 6674 3a31 3030 253b 706f 7369 7469  left:100%;positi
-00016740: 6f6e 3a61 6273 6f6c 7574 657d 756c 2e6e  on:absolute}ul.n
-00016750: 6176 202e 6e61 762d 6c69 6e6b 2073 7061  av .nav-link spa
-00016760: 6e2e 696e 6469 6361 746f 722e 6572 726f  n.indicator.erro
-00016770: 727b 6261 636b 6772 6f75 6e64 2d63 6f6c  r{background-col
-00016780: 6f72 3a76 6172 282d 2d62 732d 6461 6e67  or:var(--bs-dang
-00016790: 6572 297d 756c 2e6e 6176 202e 6e61 762d  er)}ul.nav .nav-
-000167a0: 6c69 6e6b 2073 7061 6e2e 696e 6469 6361  link span.indica
-000167b0: 746f 722e 6174 7472 6962 7574 6573 7b62  tor.attributes{b
-000167c0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-000167d0: 7661 7228 2d2d 6273 2d69 6e66 6f29 3b64  var(--bs-info);d
-000167e0: 6973 706c 6179 3a62 6c6f 636b 7d75 6c2e  isplay:block}ul.
-000167f0: 6e61 7620 2e6e 6176 2d6c 696e 6b2e 6572  nav .nav-link.er
-00016800: 726f 723e 7370 616e 2e69 6e64 6963 6174  ror>span.indicat
-00016810: 6f72 7b64 6973 706c 6179 3a62 6c6f 636b  or{display:block
-00016820: 7d75 6c2e 6e61 762e 6e61 762d 7069 6c6c  }ul.nav.nav-pill
-00016830: 7320 2e6e 6176 2d6c 696e 6b3a 6e6f 7428  s .nav-link:not(
-00016840: 2e61 6374 6976 6529 7b62 6f72 6465 722d  .active){border-
-00016850: 7374 796c 653a 736f 6c69 643b 626f 7264  style:solid;bord
-00016860: 6572 2d77 6964 7468 3a31 7078 7d62 6f64  er-width:1px}bod
-00016870: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
-00016880: 2d61 646d 696e 2d73 7479 6c65 2920 756c  -admin-style) ul
-00016890: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-000168a0: 656e 642e 6e61 762d 7461 6273 2b64 6976  end.nav-tabs+div
-000168b0: 2e74 6162 2d63 6f6e 7465 6e74 202e 7461  .tab-content .ta
-000168c0: 622d 7061 6e65 7b62 6f72 6465 722d 6c65  b-pane{border-le
-000168d0: 6674 2d73 7479 6c65 3a73 6f6c 6964 3b62  ft-style:solid;b
-000168e0: 6f72 6465 722d 626f 7474 6f6d 2d73 7479  order-bottom-sty
-000168f0: 6c65 3a73 6f6c 6964 3b62 6f72 6465 722d  le:solid;border-
-00016900: 7269 6768 742d 7374 796c 653a 736f 6c69  right-style:soli
-00016910: 643b 626f 7264 6572 2d6c 6566 742d 636f  d;border-left-co
-00016920: 6c6f 723a 7661 7228 2d2d 6861 6972 6c69  lor:var(--hairli
-00016930: 6e65 2d63 6f6c 6f72 293b 626f 7264 6572  ne-color);border
-00016940: 2d62 6f74 746f 6d2d 636f 6c6f 723a 7661  -bottom-color:va
-00016950: 7228 2d2d 6861 6972 6c69 6e65 2d63 6f6c  r(--hairline-col
-00016960: 6f72 293b 626f 7264 6572 2d72 6967 6874  or);border-right
-00016970: 2d63 6f6c 6f72 3a76 6172 282d 2d68 6169  -color:var(--hai
-00016980: 726c 696e 652d 636f 6c6f 7229 3b62 6f72  rline-color);bor
-00016990: 6465 722d 7769 6474 683a 3170 787d 626f  der-width:1px}bo
-000169a0: 6479 3a6e 6f74 282e 646a 616e 676f 636d  dy:not(.djangocm
-000169b0: 732d 6164 6d69 6e2d 7374 796c 6529 2075  s-admin-style) u
-000169c0: 6c2e 646a 616e 676f 636d 732d 6672 6f6e  l.djangocms-fron
-000169d0: 7465 6e64 2e6e 6176 2d74 6162 732b 6469  tend.nav-tabs+di
-000169e0: 762e 7461 622d 636f 6e74 656e 7420 2e74  v.tab-content .t
-000169f0: 6162 2d70 616e 6520 6669 656c 6473 6574  ab-pane fieldset
-00016a00: 3a6c 6173 742d 6368 696c 647b 6d61 7267  :last-child{marg
-00016a10: 696e 2d62 6f74 746f 6d3a 307d 6469 762e  in-bottom:0}div.
-00016a20: 7461 622d 706b 7b2d 6d73 2d66 6c65 782d  tab-pk{-ms-flex-
-00016a30: 6974 656d 2d61 6c69 676e 3a63 656e 7465  item-align:cente
-00016a40: 723b 2d6d 732d 6772 6964 2d72 6f77 2d61  r;-ms-grid-row-a
-00016a50: 6c69 676e 3a63 656e 7465 723b 616c 6967  lign:center;alig
-00016a60: 6e2d 7365 6c66 3a63 656e 7465 723b 636f  n-self:center;co
-00016a70: 6c6f 723a 7661 7228 2d2d 6463 612d 6772  lor:var(--dca-gr
-00016a80: 6179 2d64 6172 6b65 722c 7661 7228 2d2d  ay-darker,var(--
-00016a90: 626f 6479 2d66 672c 2333 3333 2929 3b66  body-fg,#333));f
-00016aa0: 6f6e 742d 7369 7a65 3a38 3025 3b6d 6172  ont-size:80%;mar
-00016ab0: 6769 6e2d 6c65 6674 3a61 7574 6f7d 2e64  gin-left:auto}.d
-00016ac0: 6a61 6e67 6f63 6d73 2d61 646d 696e 2d73  jangocms-admin-s
-00016ad0: 7479 6c65 202e 646a 616e 676f 636d 732d  tyle .djangocms-
-00016ae0: 6672 6f6e 7465 6e64 206c 692e 6e61 762d  frontend li.nav-
-00016af0: 6974 656d 7b62 6f72 6465 722d 746f 703a  item{border-top:
-00016b00: 6e6f 6e65 7d69 6e70 7574 5b74 7970 653d  none}input[type=
-00016b10: 6e75 6d62 6572 5d2e 6175 746f 2d66 6965  number].auto-fie
-00016b20: 6c64 2b73 7061 6e7b 6469 7370 6c61 793a  ld+span{display:
-00016b30: 6e6f 6e65 3b70 6f73 6974 696f 6e3a 6162  none;position:ab
-00016b40: 736f 6c75 7465 3b62 6f74 746f 6d3a 303b  solute;bottom:0;
-00016b50: 7269 6768 743a 303b 7465 7874 2d61 6c69  right:0;text-ali
-00016b60: 676e 3a72 6967 6874 3b6d 6172 6769 6e2d  gn:right;margin-
-00016b70: 7269 6768 743a 3331 7078 3b6d 6172 6769  right:31px;margi
-00016b80: 6e2d 626f 7474 6f6d 3a32 3370 783b 6375  n-bottom:23px;cu
-00016b90: 7273 6f72 3a70 6f69 6e74 6572 7d62 6f64  rsor:pointer}bod
-00016ba0: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
-00016bb0: 2d61 646d 696e 2d73 7479 6c65 2920 696e  -admin-style) in
-00016bc0: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
-00016bd0: 2e61 7574 6f2d 6669 656c 642b 7370 616e  .auto-field+span
-00016be0: 7b6d 6172 6769 6e2d 626f 7474 6f6d 3a32  {margin-bottom:2
-00016bf0: 3370 787d 406d 6564 6961 2028 6d61 782d  3px}@media (max-
-00016c00: 7769 6474 683a 3130 3234 7078 297b 626f  width:1024px){bo
-00016c10: 6479 3a6e 6f74 282e 646a 616e 676f 636d  dy:not(.djangocm
-00016c20: 732d 6164 6d69 6e2d 7374 796c 6529 2069  s-admin-style) i
-00016c30: 6e70 7574 5b74 7970 653d 6e75 6d62 6572  nput[type=number
-00016c40: 5d2e 6175 746f 2d66 6965 6c64 2b73 7061  ].auto-field+spa
-00016c50: 6e7b 6d61 7267 696e 2d62 6f74 746f 6d3a  n{margin-bottom:
-00016c60: 3234 7078 7d7d 696e 7075 745b 7479 7065  24px}}input[type
-00016c70: 3d6e 756d 6265 725d 2e61 7574 6f2d 6669  =number].auto-fi
-00016c80: 656c 642b 7370 616e 3a61 6674 6572 7b63  eld+span:after{c
-00016c90: 6f6e 7465 6e74 3a22 6175 746f 227d 696e  ontent:"auto"}in
-00016ca0: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
-00016cb0: 2e61 7574 6f2d 6669 656c 642e 6175 746f  .auto-field.auto
-00016cc0: 7b63 6f6c 6f72 3a76 6172 282d 2d64 6361  {color:var(--dca
-00016cd0: 2d77 6869 7465 2c76 6172 282d 2d62 6f64  -white,var(--bod
-00016ce0: 792d 6267 2c23 6666 6629 293b 6361 7265  y-bg,#fff));care
-00016cf0: 742d 636f 6c6f 723a 7661 7228 2d2d 6463  t-color:var(--dc
-00016d00: 612d 626c 6163 6b2c 7661 7228 2d2d 626f  a-black,var(--bo
-00016d10: 6479 2d66 672c 2330 3030 2929 7d69 6e70  dy-fg,#000))}inp
-00016d20: 7574 5b74 7970 653d 6e75 6d62 6572 5d2e  ut[type=number].
-00016d30: 6175 746f 2d66 6965 6c64 2e61 7574 6f2b  auto-field.auto+
-00016d40: 7370 616e 7b64 6973 706c 6179 3a62 6c6f  span{display:blo
-00016d50: 636b 7d                                  ck}
+0000a0a0: 696d 706f 7274 616e 743b 2d6d 732d 666c  important;-ms-fl
+0000a0b0: 6578 3a6e 6f6e 653b 666c 6578 3a6e 6f6e  ex:none;flex:non
+0000a0c0: 653b 7061 6464 696e 673a 3135 7078 2031  e;padding:15px 1
+0000a0d0: 3070 783b 6d61 7267 696e 3a30 2169 6d70  0px;margin:0!imp
+0000a0e0: 6f72 7461 6e74 3b62 6f72 6465 722d 626f  ortant;border-bo
+0000a0f0: 7474 6f6d 3a31 7078 2073 6f6c 6964 2023  ttom:1px solid #
+0000a100: 6565 653b 666c 6f61 743a 6c65 6674 2169  eee;float:left!i
+0000a110: 6d70 6f72 7461 6e74 7d2e 646a 616e 676f  mportant}.django
+0000a120: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000a130: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000a140: 2d72 6f77 5f63 6f6c 735f 7873 202e 6669  -row_cols_xs .fi
+0000a150: 656c 642d 626f 7820 696e 7075 742c 2e64  eld-box input,.d
+0000a160: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000a170: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000a180: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000a190: 7320 2e66 6965 6c64 426f 7820 696e 7075  s .fieldBox inpu
+0000a1a0: 747b 7465 7874 2d61 6c69 676e 3a72 6967  t{text-align:rig
+0000a1b0: 6874 3b70 6164 6469 6e67 2d72 6967 6874  ht;padding-right
+0000a1c0: 3a35 7078 2169 6d70 6f72 7461 6e74 3b62  :5px!important;b
+0000a1d0: 6f78 2d73 697a 696e 673a 626f 7264 6572  ox-sizing:border
+0000a1e0: 2d62 6f78 3b77 6964 7468 3a31 3030 257d  -box;width:100%}
+0000a1f0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000a200: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000a210: 772e 6669 656c 642d 726f 775f 636f 6c73  w.field-row_cols
+0000a220: 5f78 7320 2e66 6965 6c64 2d62 6f78 206c  _xs .field-box l
+0000a230: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
+0000a240: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000a250: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
+0000a260: 5f63 6f6c 735f 7873 202e 6669 656c 6442  _cols_xs .fieldB
+0000a270: 6f78 206c 6162 656c 7b66 6f6e 742d 7369  ox label{font-si
+0000a280: 7a65 3a31 3270 7821 696d 706f 7274 616e  ze:12px!importan
+0000a290: 743b 666f 6e74 2d77 6569 6768 743a 3430  t;font-weight:40
+0000a2a0: 3021 696d 706f 7274 616e 743b 636f 6c6f  0!important;colo
+0000a2b0: 723a 2363 6363 2169 6d70 6f72 7461 6e74  r:#ccc!important
+0000a2c0: 3b70 6f73 6974 696f 6e3a 6162 736f 6c75  ;position:absolu
+0000a2d0: 7465 3b6c 6566 743a 3135 7078 3b62 6f74  te;left:15px;bot
+0000a2e0: 746f 6d3a 3137 7078 3b74 6578 742d 7472  tom:17px;text-tr
+0000a2f0: 616e 7366 6f72 6d3a 6c6f 7765 7263 6173  ansform:lowercas
+0000a300: 657d 2e64 6a61 6e67 6f63 6d73 2d66 726f  e}.djangocms-fro
+0000a310: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000a320: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
+0000a330: 6c73 5f78 7320 2e66 6965 6c64 2d62 6f78  ls_xs .field-box
+0000a340: 202e 6469 7361 626c 6564 2c2e 646a 616e   .disabled,.djan
+0000a350: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000a360: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000a370: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
+0000a380: 6669 656c 6442 6f78 202e 6469 7361 626c  fieldBox .disabl
+0000a390: 6564 7b63 6f6c 6f72 3a23 6363 633b 6261  ed{color:#ccc;ba
+0000a3a0: 636b 6772 6f75 6e64 3a23 6565 657d 2e64  ckground:#eee}.d
+0000a3b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000a3c0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000a3d0: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000a3e0: 7320 2e66 6965 6c64 2d62 6f78 3a6c 6173  s .field-box:las
+0000a3f0: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
+0000a400: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000a410: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000a420: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
+0000a430: 6c64 426f 783a 6c61 7374 2d63 6869 6c64  ldBox:last-child
+0000a440: 7b62 6f72 6465 722d 7269 6768 743a 6e6f  {border-right:no
+0000a450: 6e65 7d2e 646a 616e 676f 636d 732d 6672  ne}.djangocms-fr
+0000a460: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000a470: 2d72 6f77 2e66 6965 6c64 2d72 6f77 5f63  -row.field-row_c
+0000a480: 6f6c 735f 7873 202e 6572 726f 7273 7b6d  ols_xs .errors{m
+0000a490: 6172 6769 6e2d 626f 7474 6f6d 3a30 7d2e  argin-bottom:0}.
+0000a4a0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000a4b0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000a4c0: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
+0000a4d0: 7873 202e 6669 656c 642d 626f 782d 6c61  xs .field-box-la
+0000a4e0: 6265 6c7b 6469 7370 6c61 793a 2d6d 732d  bel{display:-ms-
+0000a4f0: 666c 6578 626f 783b 6469 7370 6c61 793a  flexbox;display:
+0000a500: 666c 6578 3b6d 6172 6769 6e2d 746f 703a  flex;margin-top:
+0000a510: 6175 746f 3b63 6f6c 6f72 3a23 3939 397d  auto;color:#999}
+0000a520: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000a530: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000a540: 772e 6669 656c 642d 726f 775f 636f 6c73  w.field-row_cols
+0000a550: 5f78 7320 2e66 6965 6c64 2d62 6f78 2d6c  _xs .field-box-l
+0000a560: 6162 656c 2061 7b77 6964 7468 3a31 3030  abel a{width:100
+0000a570: 253b 6d61 7267 696e 2d74 6f70 3a61 7574  %;margin-top:aut
+0000a580: 6f7d 2e64 6a61 6e67 6f63 6d73 2d66 726f  o}.djangocms-fro
+0000a590: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000a5a0: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
+0000a5b0: 6c73 5f78 7320 2e66 6965 6c64 2d62 6f78  ls_xs .field-box
+0000a5c0: 2d6c 6162 656c 202e 6963 6f6e 7b70 6f73  -label .icon{pos
+0000a5d0: 6974 696f 6e3a 7265 6c61 7469 7665 3b74  ition:relative;t
+0000a5e0: 6f70 3a33 7078 7d2e 646a 616e 676f 636d  op:3px}.djangocm
+0000a5f0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000a600: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000a610: 642d 7873 5f63 6f6c 2c2e 646a 616e 676f  d-xs_col,.django
+0000a620: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000a630: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000a640: 656c 642d 7873 5f6d 652c 2e64 6a61 6e67  eld-xs_me,.djang
+0000a650: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000a660: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000a670: 6965 6c64 2d78 735f 6d73 2c2e 646a 616e  ield-xs_ms,.djan
+0000a680: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000a690: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000a6a0: 6669 656c 642d 7873 5f6f 6666 7365 742c  field-xs_offset,
+0000a6b0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000a6c0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000a6d0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
+0000a6e0: 6465 722c 2e64 6a61 6e67 6f63 6d73 2d66  der,.djangocms-f
+0000a6f0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000a700: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000a710: 6f6c 2c2e 646a 616e 676f 636d 732d 6672  ol,.djangocms-fr
+0000a720: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000a730: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000a740: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000a750: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000a760: 6f77 2e66 6965 6c64 2d78 735f 6d73 2c2e  ow.field-xs_ms,.
+0000a770: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000a780: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000a790: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+0000a7a0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000a7b0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000a7c0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000a7d0: 727b 706f 7369 7469 6f6e 3a72 656c 6174  r{position:relat
+0000a7e0: 6976 653b 6469 7370 6c61 793a 2d6d 732d  ive;display:-ms-
+0000a7f0: 666c 6578 626f 783b 6469 7370 6c61 793a  flexbox;display:
+0000a800: 666c 6578 3b70 6164 6469 6e67 3a30 3b6d  flex;padding:0;m
+0000a810: 696e 2d77 6964 7468 3a38 3030 7078 7d2e  in-width:800px}.
+0000a820: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000a830: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000a840: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000a850: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
+0000a860: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000a870: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000a880: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000a890: 6965 6c64 426f 782c 2e64 6a61 6e67 6f63  ieldBox,.djangoc
+0000a8a0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000a8b0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000a8c0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+0000a8d0: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
+0000a8e0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000a8f0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000a900: 735f 6d65 202e 6669 656c 6442 6f78 2c2e  s_me .fieldBox,.
+0000a910: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000a920: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000a930: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000a940: 2e66 6965 6c64 2d62 6f78 2c2e 646a 616e  .field-box,.djan
+0000a950: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000a960: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000a970: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+0000a980: 6c64 426f 782c 2e64 6a61 6e67 6f63 6d73  ldBox,.djangocms
+0000a990: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000a9a0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000a9b0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000a9c0: 642d 626f 782c 2e64 6a61 6e67 6f63 6d73  d-box,.djangocms
+0000a9d0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000a9e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000a9f0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000aa00: 6442 6f78 2c2e 646a 616e 676f 636d 732d  dBox,.djangocms-
+0000aa10: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000aa20: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000aa30: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000aa40: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
+0000aa50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000aa60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000aa70: 735f 6f72 6465 7220 2e66 6965 6c64 426f  s_order .fieldBo
+0000aa80: 782c 2e64 6a61 6e67 6f63 6d73 2d66 726f  x,.djangocms-fro
+0000aa90: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000aaa0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000aab0: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
+0000aac0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000aad0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000aae0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000aaf0: 6442 6f78 2c2e 646a 616e 676f 636d 732d  dBox,.djangocms-
+0000ab00: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000ab10: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000ab20: 6d65 202e 6669 656c 642d 626f 782c 2e64  me .field-box,.d
+0000ab30: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000ab40: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000ab50: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
+0000ab60: 6c64 426f 782c 2e64 6a61 6e67 6f63 6d73  ldBox,.djangocms
+0000ab70: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000ab80: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000ab90: 5f6d 7320 2e66 6965 6c64 2d62 6f78 2c2e  _ms .field-box,.
+0000aba0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000abb0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000abc0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000abd0: 656c 6442 6f78 2c2e 646a 616e 676f 636d  eldBox,.djangocm
+0000abe0: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000abf0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000ac00: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+0000ac10: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
+0000ac20: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000ac30: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000ac40: 6666 7365 7420 2e66 6965 6c64 426f 782c  ffset .fieldBox,
+0000ac50: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000ac60: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000ac70: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000ac80: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
+0000ac90: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000aca0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000acb0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+0000acc0: 656c 6442 6f78 7b70 6f73 6974 696f 6e3a  eldBox{position:
+0000acd0: 7265 6c61 7469 7665 3b77 6964 7468 3a31  relative;width:1
+0000ace0: 3030 7078 2169 6d70 6f72 7461 6e74 3b2d  00px!important;-
+0000acf0: 6d73 2d66 6c65 783a 6e6f 6e65 3b66 6c65  ms-flex:none;fle
+0000ad00: 783a 6e6f 6e65 3b70 6164 6469 6e67 3a31  x:none;padding:1
+0000ad10: 3570 7820 3130 7078 3b6d 6172 6769 6e3a  5px 10px;margin:
+0000ad20: 3021 696d 706f 7274 616e 743b 626f 7264  0!important;bord
+0000ad30: 6572 2d62 6f74 746f 6d3a 3170 7820 736f  er-bottom:1px so
+0000ad40: 6c69 6420 2365 6565 3b66 6c6f 6174 3a6c  lid #eee;float:l
+0000ad50: 6566 7421 696d 706f 7274 616e 747d 2e64  eft!important}.d
+0000ad60: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000ad70: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000ad80: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000ad90: 2e66 6965 6c64 2d62 6f78 2069 6e70 7574  .field-box input
+0000ada0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000adb0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000adc0: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000add0: 6f6c 202e 6669 656c 6442 6f78 2069 6e70  ol .fieldBox inp
+0000ade0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+0000adf0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000ae00: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000ae10: 5f6d 6520 2e66 6965 6c64 2d62 6f78 2069  _me .field-box i
+0000ae20: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000ae30: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000ae40: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ae50: 7873 5f6d 6520 2e66 6965 6c64 426f 7820  xs_me .fieldBox 
+0000ae60: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+0000ae70: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000ae80: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000ae90: 2d78 735f 6d73 202e 6669 656c 642d 626f  -xs_ms .field-bo
+0000aea0: 7820 696e 7075 742c 2e64 6a61 6e67 6f63  x input,.djangoc
+0000aeb0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000aec0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000aed0: 6c64 2d78 735f 6d73 202e 6669 656c 6442  ld-xs_ms .fieldB
+0000aee0: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
+0000aef0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000af00: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000af10: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
+0000af20: 6965 6c64 2d62 6f78 2069 6e70 7574 2c2e  ield-box input,.
+0000af30: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000af40: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000af50: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+0000af60: 7365 7420 2e66 6965 6c64 426f 7820 696e  set .fieldBox in
+0000af70: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+0000af80: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000af90: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000afa0: 735f 6f72 6465 7220 2e66 6965 6c64 2d62  s_order .field-b
+0000afb0: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
+0000afc0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000afd0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000afe0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+0000aff0: 656c 6442 6f78 2069 6e70 7574 2c2e 646a  eldBox input,.dj
+0000b000: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000b010: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000b020: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+0000b030: 6c64 2d62 6f78 2069 6e70 7574 2c2e 646a  ld-box input,.dj
+0000b040: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000b050: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000b060: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+0000b070: 6c64 426f 7820 696e 7075 742c 2e64 6a61  ldBox input,.dja
+0000b080: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000b090: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000b0a0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000b0b0: 2d62 6f78 2069 6e70 7574 2c2e 646a 616e  -box input,.djan
+0000b0c0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000b0d0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000b0e0: 6c64 2d78 735f 6d65 202e 6669 656c 6442  ld-xs_me .fieldB
+0000b0f0: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
+0000b100: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000b110: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b120: 2d78 735f 6d73 202e 6669 656c 642d 626f  -xs_ms .field-bo
+0000b130: 7820 696e 7075 742c 2e64 6a61 6e67 6f63  x input,.djangoc
+0000b140: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000b150: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000b160: 7873 5f6d 7320 2e66 6965 6c64 426f 7820  xs_ms .fieldBox 
+0000b170: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+0000b180: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000b190: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000b1a0: 5f6f 6666 7365 7420 2e66 6965 6c64 2d62  _offset .field-b
+0000b1b0: 6f78 2069 6e70 7574 2c2e 646a 616e 676f  ox input,.django
+0000b1c0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000b1d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b1e0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000b1f0: 6442 6f78 2069 6e70 7574 2c2e 646a 616e  dBox input,.djan
+0000b200: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000b210: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000b220: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000b230: 6c64 2d62 6f78 2069 6e70 7574 2c2e 646a  ld-box input,.dj
+0000b240: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000b250: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000b260: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+0000b270: 6965 6c64 426f 7820 696e 7075 747b 7465  ieldBox input{te
+0000b280: 7874 2d61 6c69 676e 3a72 6967 6874 3b70  xt-align:right;p
+0000b290: 6164 6469 6e67 2d72 6967 6874 3a35 7078  adding-right:5px
+0000b2a0: 2169 6d70 6f72 7461 6e74 3b62 6f78 2d73  !important;box-s
+0000b2b0: 697a 696e 673a 626f 7264 6572 2d62 6f78  izing:border-box
+0000b2c0: 3b77 6964 7468 3a31 3030 257d 2e64 6a61  ;width:100%}.dja
+0000b2d0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000b2e0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000b2f0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000b300: 6965 6c64 2d62 6f78 206c 6162 656c 2c2e  ield-box label,.
+0000b310: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000b320: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000b330: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000b340: 202e 6669 656c 6442 6f78 206c 6162 656c   .fieldBox label
+0000b350: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000b360: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000b370: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000b380: 6520 2e66 6965 6c64 2d62 6f78 206c 6162  e .field-box lab
+0000b390: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
+0000b3a0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000b3b0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000b3c0: 5f6d 6520 2e66 6965 6c64 426f 7820 6c61  _me .fieldBox la
+0000b3d0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000b3e0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000b3f0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000b400: 735f 6d73 202e 6669 656c 642d 626f 7820  s_ms .field-box 
+0000b410: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000b420: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000b430: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b440: 2d78 735f 6d73 202e 6669 656c 6442 6f78  -xs_ms .fieldBox
+0000b450: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000b460: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000b470: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000b480: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
+0000b490: 6c64 2d62 6f78 206c 6162 656c 2c2e 646a  ld-box label,.dj
+0000b4a0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000b4b0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000b4c0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000b4d0: 7420 2e66 6965 6c64 426f 7820 6c61 6265  t .fieldBox labe
+0000b4e0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000b4f0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000b500: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000b510: 6f72 6465 7220 2e66 6965 6c64 2d62 6f78  order .field-box
+0000b520: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000b530: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000b540: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000b550: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000b560: 6442 6f78 206c 6162 656c 2c2e 646a 616e  dBox label,.djan
+0000b570: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000b580: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000b590: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+0000b5a0: 2d62 6f78 206c 6162 656c 2c2e 646a 616e  -box label,.djan
+0000b5b0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000b5c0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000b5d0: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+0000b5e0: 426f 7820 6c61 6265 6c2c 2e64 6a61 6e67  Box label,.djang
+0000b5f0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000b600: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000b610: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
+0000b620: 6f78 206c 6162 656c 2c2e 646a 616e 676f  ox label,.django
+0000b630: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000b640: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b650: 2d78 735f 6d65 202e 6669 656c 6442 6f78  -xs_me .fieldBox
+0000b660: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000b670: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000b680: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000b690: 735f 6d73 202e 6669 656c 642d 626f 7820  s_ms .field-box 
+0000b6a0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000b6b0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000b6c0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000b6d0: 5f6d 7320 2e66 6965 6c64 426f 7820 6c61  _ms .fieldBox la
+0000b6e0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000b6f0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000b700: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000b710: 6666 7365 7420 2e66 6965 6c64 2d62 6f78  ffset .field-box
+0000b720: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000b730: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000b740: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000b750: 735f 6f66 6673 6574 202e 6669 656c 6442  s_offset .fieldB
+0000b760: 6f78 206c 6162 656c 2c2e 646a 616e 676f  ox label,.django
+0000b770: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000b780: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b790: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+0000b7a0: 2d62 6f78 206c 6162 656c 2c2e 646a 616e  -box label,.djan
+0000b7b0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000b7c0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000b7d0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000b7e0: 6c64 426f 7820 6c61 6265 6c7b 666f 6e74  ldBox label{font
+0000b7f0: 2d73 697a 653a 3132 7078 2169 6d70 6f72  -size:12px!impor
+0000b800: 7461 6e74 3b66 6f6e 742d 7765 6967 6874  tant;font-weight
+0000b810: 3a34 3030 2169 6d70 6f72 7461 6e74 3b63  :400!important;c
+0000b820: 6f6c 6f72 3a23 6363 6321 696d 706f 7274  olor:#ccc!import
+0000b830: 616e 743b 706f 7369 7469 6f6e 3a61 6273  ant;position:abs
+0000b840: 6f6c 7574 653b 6c65 6674 3a31 3570 783b  olute;left:15px;
+0000b850: 626f 7474 6f6d 3a31 3770 783b 7465 7874  bottom:17px;text
+0000b860: 2d74 7261 6e73 666f 726d 3a6c 6f77 6572  -transform:lower
+0000b870: 6361 7365 7d2e 646a 616e 676f 636d 732d  case}.djangocms-
+0000b880: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000b890: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000b8a0: 7873 5f63 6f6c 202e 6669 656c 642d 626f  xs_col .field-bo
+0000b8b0: 7820 2e64 6973 6162 6c65 642c 2e64 6a61  x .disabled,.dja
+0000b8c0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000b8d0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000b8e0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000b8f0: 6965 6c64 426f 7820 2e64 6973 6162 6c65  ieldBox .disable
+0000b900: 642c 2e64 6a61 6e67 6f63 6d73 2d66 726f  d,.djangocms-fro
+0000b910: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000b920: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000b930: 6d65 202e 6669 656c 642d 626f 7820 2e64  me .field-box .d
+0000b940: 6973 6162 6c65 642c 2e64 6a61 6e67 6f63  isabled,.djangoc
+0000b950: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000b960: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000b970: 6c64 2d78 735f 6d65 202e 6669 656c 6442  ld-xs_me .fieldB
+0000b980: 6f78 202e 6469 7361 626c 6564 2c2e 646a  ox .disabled,.dj
+0000b990: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000b9a0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000b9b0: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
+0000b9c0: 6965 6c64 2d62 6f78 202e 6469 7361 626c  ield-box .disabl
+0000b9d0: 6564 2c2e 646a 616e 676f 636d 732d 6672  ed,.djangocms-fr
+0000b9e0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000b9f0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000ba00: 5f6d 7320 2e66 6965 6c64 426f 7820 2e64  _ms .fieldBox .d
+0000ba10: 6973 6162 6c65 642c 2e64 6a61 6e67 6f63  isabled,.djangoc
+0000ba20: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000ba30: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000ba40: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
+0000ba50: 656c 642d 626f 7820 2e64 6973 6162 6c65  eld-box .disable
+0000ba60: 642c 2e64 6a61 6e67 6f63 6d73 2d66 726f  d,.djangocms-fro
+0000ba70: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000ba80: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000ba90: 6f66 6673 6574 202e 6669 656c 6442 6f78  offset .fieldBox
+0000baa0: 202e 6469 7361 626c 6564 2c2e 646a 616e   .disabled,.djan
+0000bab0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000bac0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000bad0: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000bae0: 6669 656c 642d 626f 7820 2e64 6973 6162  field-box .disab
+0000baf0: 6c65 642c 2e64 6a61 6e67 6f63 6d73 2d66  led,.djangocms-f
+0000bb00: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000bb10: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000bb20: 735f 6f72 6465 7220 2e66 6965 6c64 426f  s_order .fieldBo
+0000bb30: 7820 2e64 6973 6162 6c65 642c 2e64 6a61  x .disabled,.dja
+0000bb40: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000bb50: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000bb60: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000bb70: 642d 626f 7820 2e64 6973 6162 6c65 642c  d-box .disabled,
+0000bb80: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000bb90: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000bba0: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+0000bbb0: 6669 656c 6442 6f78 202e 6469 7361 626c  fieldBox .disabl
+0000bbc0: 6564 2c2e 646a 616e 676f 636d 732d 6672  ed,.djangocms-fr
+0000bbd0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000bbe0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000bbf0: 202e 6669 656c 642d 626f 7820 2e64 6973   .field-box .dis
+0000bc00: 6162 6c65 642c 2e64 6a61 6e67 6f63 6d73  abled,.djangocms
+0000bc10: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000bc20: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000bc30: 5f6d 6520 2e66 6965 6c64 426f 7820 2e64  _me .fieldBox .d
+0000bc40: 6973 6162 6c65 642c 2e64 6a61 6e67 6f63  isabled,.djangoc
+0000bc50: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000bc60: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000bc70: 7873 5f6d 7320 2e66 6965 6c64 2d62 6f78  xs_ms .field-box
+0000bc80: 202e 6469 7361 626c 6564 2c2e 646a 616e   .disabled,.djan
+0000bc90: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000bca0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000bcb0: 6c64 2d78 735f 6d73 202e 6669 656c 6442  ld-xs_ms .fieldB
+0000bcc0: 6f78 202e 6469 7361 626c 6564 2c2e 646a  ox .disabled,.dj
+0000bcd0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000bce0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000bcf0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
+0000bd00: 6669 656c 642d 626f 7820 2e64 6973 6162  field-box .disab
+0000bd10: 6c65 642c 2e64 6a61 6e67 6f63 6d73 2d66  led,.djangocms-f
+0000bd20: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000bd30: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000bd40: 6666 7365 7420 2e66 6965 6c64 426f 7820  ffset .fieldBox 
+0000bd50: 2e64 6973 6162 6c65 642c 2e64 6a61 6e67  .disabled,.djang
+0000bd60: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000bd70: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000bd80: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000bd90: 642d 626f 7820 2e64 6973 6162 6c65 642c  d-box .disabled,
+0000bda0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000bdb0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000bdc0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000bdd0: 202e 6669 656c 6442 6f78 202e 6469 7361   .fieldBox .disa
+0000bde0: 626c 6564 7b63 6f6c 6f72 3a23 6363 633b  bled{color:#ccc;
+0000bdf0: 6261 636b 6772 6f75 6e64 3a23 6565 657d  background:#eee}
+0000be00: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000be10: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000be20: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
+0000be30: 6c20 2e66 6965 6c64 2d62 6f78 3a6c 6173  l .field-box:las
+0000be40: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
+0000be50: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000be60: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000be70: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+0000be80: 426f 783a 6c61 7374 2d63 6869 6c64 2c2e  Box:last-child,.
+0000be90: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000bea0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000beb0: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+0000bec0: 2e66 6965 6c64 2d62 6f78 3a6c 6173 742d  .field-box:last-
+0000bed0: 6368 696c 642c 2e64 6a61 6e67 6f63 6d73  child,.djangocms
+0000bee0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000bef0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000bf00: 2d78 735f 6d65 202e 6669 656c 6442 6f78  -xs_me .fieldBox
+0000bf10: 3a6c 6173 742d 6368 696c 642c 2e64 6a61  :last-child,.dja
+0000bf20: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000bf30: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000bf40: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000bf50: 656c 642d 626f 783a 6c61 7374 2d63 6869  eld-box:last-chi
+0000bf60: 6c64 2c2e 646a 616e 676f 636d 732d 6672  ld,.djangocms-fr
+0000bf70: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000bf80: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000bf90: 5f6d 7320 2e66 6965 6c64 426f 783a 6c61  _ms .fieldBox:la
+0000bfa0: 7374 2d63 6869 6c64 2c2e 646a 616e 676f  st-child,.django
+0000bfb0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000bfc0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000bfd0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
+0000bfe0: 6965 6c64 2d62 6f78 3a6c 6173 742d 6368  ield-box:last-ch
+0000bff0: 696c 642c 2e64 6a61 6e67 6f63 6d73 2d66  ild,.djangocms-f
+0000c000: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000c010: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000c020: 735f 6f66 6673 6574 202e 6669 656c 6442  s_offset .fieldB
+0000c030: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
+0000c040: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000c050: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000c060: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000c070: 7220 2e66 6965 6c64 2d62 6f78 3a6c 6173  r .field-box:las
+0000c080: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
+0000c090: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000c0a0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000c0b0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000c0c0: 6c64 426f 783a 6c61 7374 2d63 6869 6c64  ldBox:last-child
+0000c0d0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000c0e0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000c0f0: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000c100: 2e66 6965 6c64 2d62 6f78 3a6c 6173 742d  .field-box:last-
+0000c110: 6368 696c 642c 2e64 6a61 6e67 6f63 6d73  child,.djangocms
+0000c120: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000c130: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000c140: 5f63 6f6c 202e 6669 656c 6442 6f78 3a6c  _col .fieldBox:l
+0000c150: 6173 742d 6368 696c 642c 2e64 6a61 6e67  ast-child,.djang
+0000c160: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000c170: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000c180: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
+0000c190: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
+0000c1a0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000c1b0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000c1c0: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
+0000c1d0: 6c64 426f 783a 6c61 7374 2d63 6869 6c64  ldBox:last-child
+0000c1e0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000c1f0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000c200: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+0000c210: 6669 656c 642d 626f 783a 6c61 7374 2d63  field-box:last-c
+0000c220: 6869 6c64 2c2e 646a 616e 676f 636d 732d  hild,.djangocms-
+0000c230: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000c240: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000c250: 6d73 202e 6669 656c 6442 6f78 3a6c 6173  ms .fieldBox:las
+0000c260: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
+0000c270: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000c280: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000c290: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000c2a0: 2d62 6f78 3a6c 6173 742d 6368 696c 642c  -box:last-child,
+0000c2b0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000c2c0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000c2d0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000c2e0: 7420 2e66 6965 6c64 426f 783a 6c61 7374  t .fieldBox:last
+0000c2f0: 2d63 6869 6c64 2c2e 646a 616e 676f 636d  -child,.djangocm
+0000c300: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000c310: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000c320: 735f 6f72 6465 7220 2e66 6965 6c64 2d62  s_order .field-b
+0000c330: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
+0000c340: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000c350: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000c360: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000c370: 6669 656c 6442 6f78 3a6c 6173 742d 6368  fieldBox:last-ch
+0000c380: 696c 647b 626f 7264 6572 2d72 6967 6874  ild{border-right
+0000c390: 3a6e 6f6e 657d 2e64 6a61 6e67 6f63 6d73  :none}.djangocms
+0000c3a0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000c3b0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000c3c0: 2d78 735f 636f 6c20 2e65 7272 6f72 732c  -xs_col .errors,
+0000c3d0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000c3e0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000c3f0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000c400: 202e 6572 726f 7273 2c2e 646a 616e 676f   .errors,.django
+0000c410: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c420: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000c430: 656c 642d 7873 5f6d 7320 2e65 7272 6f72  eld-xs_ms .error
+0000c440: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000c450: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000c460: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000c470: 6f66 6673 6574 202e 6572 726f 7273 2c2e  offset .errors,.
+0000c480: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000c490: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000c4a0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000c4b0: 6572 202e 6572 726f 7273 2c2e 646a 616e  er .errors,.djan
+0000c4c0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000c4d0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000c4e0: 6c64 2d78 735f 636f 6c20 2e65 7272 6f72  ld-xs_col .error
+0000c4f0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000c500: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000c510: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+0000c520: 2e65 7272 6f72 732c 2e64 6a61 6e67 6f63  .errors,.djangoc
+0000c530: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000c540: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000c550: 7873 5f6d 7320 2e65 7272 6f72 732c 2e64  xs_ms .errors,.d
+0000c560: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000c570: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000c580: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
+0000c590: 2e65 7272 6f72 732c 2e64 6a61 6e67 6f63  .errors,.djangoc
+0000c5a0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000c5b0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000c5c0: 7873 5f6f 7264 6572 202e 6572 726f 7273  xs_order .errors
+0000c5d0: 7b6d 6172 6769 6e2d 626f 7474 6f6d 3a30  {margin-bottom:0
+0000c5e0: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
+0000c5f0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000c600: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000c610: 6f6c 202e 6572 726f 726c 6973 742c 2e64  ol .errorlist,.d
+0000c620: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000c630: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000c640: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+0000c650: 6572 726f 726c 6973 742c 2e64 6a61 6e67  errorlist,.djang
+0000c660: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000c670: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000c680: 6965 6c64 2d78 735f 6d73 202e 6572 726f  ield-xs_ms .erro
+0000c690: 726c 6973 742c 2e64 6a61 6e67 6f63 6d73  rlist,.djangocms
+0000c6a0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000c6b0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000c6c0: 2d78 735f 6f66 6673 6574 202e 6572 726f  -xs_offset .erro
+0000c6d0: 726c 6973 742c 2e64 6a61 6e67 6f63 6d73  rlist,.djangocms
+0000c6e0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000c6f0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000c700: 2d78 735f 6f72 6465 7220 2e65 7272 6f72  -xs_order .error
+0000c710: 6c69 7374 2c2e 646a 616e 676f 636d 732d  list,.djangocms-
+0000c720: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000c730: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000c740: 636f 6c20 2e65 7272 6f72 6c69 7374 2c2e  col .errorlist,.
+0000c750: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000c760: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000c770: 2e66 6965 6c64 2d78 735f 6d65 202e 6572  .field-xs_me .er
+0000c780: 726f 726c 6973 742c 2e64 6a61 6e67 6f63  rorlist,.djangoc
+0000c790: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000c7a0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000c7b0: 7873 5f6d 7320 2e65 7272 6f72 6c69 7374  xs_ms .errorlist
+0000c7c0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000c7d0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000c7e0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000c7f0: 6574 202e 6572 726f 726c 6973 742c 2e64  et .errorlist,.d
+0000c800: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000c810: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000c820: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000c830: 6572 726f 726c 6973 747b 706f 7369 7469  errorlist{positi
+0000c840: 6f6e 3a61 6273 6f6c 7574 6521 696d 706f  on:absolute!impo
+0000c850: 7274 616e 743b 7769 6474 683a 3170 7821  rtant;width:1px!
+0000c860: 696d 706f 7274 616e 743b 6865 6967 6874  important;height
+0000c870: 3a31 7078 2169 6d70 6f72 7461 6e74 3b70  :1px!important;p
+0000c880: 6164 6469 6e67 3a30 2169 6d70 6f72 7461  adding:0!importa
+0000c890: 6e74 3b6d 6172 6769 6e3a 2d31 7078 2169  nt;margin:-1px!i
+0000c8a0: 6d70 6f72 7461 6e74 3b6f 7665 7266 6c6f  mportant;overflo
+0000c8b0: 773a 6869 6464 656e 2169 6d70 6f72 7461  w:hidden!importa
+0000c8c0: 6e74 3b63 6c69 703a 7265 6374 2830 2c30  nt;clip:rect(0,0
+0000c8d0: 2c30 2c30 2921 696d 706f 7274 616e 743b  ,0,0)!important;
+0000c8e0: 7768 6974 652d 7370 6163 653a 6e6f 7772  white-space:nowr
+0000c8f0: 6170 2169 6d70 6f72 7461 6e74 3b62 6f72  ap!important;bor
+0000c900: 6465 723a 3021 696d 706f 7274 616e 747d  der:0!important}
+0000c910: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000c920: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000c930: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
+0000c940: 6c2e 6669 656c 642d 7873 5f6d 6520 2e66  l.field-xs_me .f
+0000c950: 6965 6c64 2d62 6f78 2c2e 646a 616e 676f  ield-box,.django
+0000c960: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c970: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000c980: 656c 642d 7873 5f6d 652e 6669 656c 642d  eld-xs_me.field-
+0000c990: 7873 5f6d 6520 2e66 6965 6c64 2d62 6f78  xs_me .field-box
+0000c9a0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000c9b0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000c9c0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000c9d0: 732e 6669 656c 642d 7873 5f6d 6520 2e66  s.field-xs_me .f
+0000c9e0: 6965 6c64 2d62 6f78 2c2e 646a 616e 676f  ield-box,.django
+0000c9f0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000ca00: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000ca10: 656c 642d 7873 5f6f 6666 7365 742e 6669  eld-xs_offset.fi
+0000ca20: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000ca30: 2d62 6f78 2c2e 646a 616e 676f 636d 732d  -box,.djangocms-
+0000ca40: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000ca50: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ca60: 7873 5f6f 7264 6572 2e66 6965 6c64 2d78  xs_order.field-x
+0000ca70: 735f 6d65 202e 6669 656c 642d 626f 782c  s_me .field-box,
+0000ca80: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000ca90: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000caa0: 772e 6669 656c 642d 7873 5f63 6f6c 2e66  w.field-xs_col.f
+0000cab0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000cac0: 642d 626f 782c 2e64 6a61 6e67 6f63 6d73  d-box,.djangocms
+0000cad0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000cae0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000caf0: 5f6d 652e 6669 656c 642d 7873 5f6d 6520  _me.field-xs_me 
+0000cb00: 2e66 6965 6c64 2d62 6f78 2c2e 646a 616e  .field-box,.djan
+0000cb10: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000cb20: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000cb30: 6c64 2d78 735f 6d73 2e66 6965 6c64 2d78  ld-xs_ms.field-x
+0000cb40: 735f 6d65 202e 6669 656c 642d 626f 782c  s_me .field-box,
+0000cb50: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000cb60: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000cb70: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000cb80: 742e 6669 656c 642d 7873 5f6d 6520 2e66  t.field-xs_me .f
+0000cb90: 6965 6c64 2d62 6f78 2c2e 646a 616e 676f  ield-box,.django
+0000cba0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000cbb0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000cbc0: 2d78 735f 6f72 6465 722e 6669 656c 642d  -xs_order.field-
+0000cbd0: 7873 5f6d 6520 2e66 6965 6c64 2d62 6f78  xs_me .field-box
+0000cbe0: 7b62 6f72 6465 722d 626f 7474 6f6d 3a6e  {border-bottom:n
+0000cbf0: 6f6e 657d 2e64 6a61 6e67 6f63 6d73 2d66  one}.djangocms-f
+0000cc00: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000cc10: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000cc20: 735f 636f 6c20 2e66 6965 6c64 2d62 6f78  s_col .field-box
+0000cc30: 2d6c 6162 656c 2c2e 646a 616e 676f 636d  -label,.djangocm
+0000cc40: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000cc50: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000cc60: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
+0000cc70: 6f78 2d6c 6162 656c 2c2e 646a 616e 676f  ox-label,.django
+0000cc80: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000cc90: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000cca0: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
+0000ccb0: 2d62 6f78 2d6c 6162 656c 2c2e 646a 616e  -box-label,.djan
+0000ccc0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000ccd0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000cce0: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
+0000ccf0: 2e66 6965 6c64 2d62 6f78 2d6c 6162 656c  .field-box-label
+0000cd00: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000cd10: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000cd20: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000cd30: 7264 6572 202e 6669 656c 642d 626f 782d  rder .field-box-
+0000cd40: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000cd50: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000cd60: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000cd70: 5f63 6f6c 202e 6669 656c 642d 626f 782d  _col .field-box-
+0000cd80: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000cd90: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000cda0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000cdb0: 5f6d 6520 2e66 6965 6c64 2d62 6f78 2d6c  _me .field-box-l
+0000cdc0: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
+0000cdd0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000cde0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000cdf0: 6d73 202e 6669 656c 642d 626f 782d 6c61  ms .field-box-la
+0000ce00: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000ce10: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000ce20: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000ce30: 6666 7365 7420 2e66 6965 6c64 2d62 6f78  ffset .field-box
+0000ce40: 2d6c 6162 656c 2c2e 646a 616e 676f 636d  -label,.djangocm
+0000ce50: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000ce60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000ce70: 735f 6f72 6465 7220 2e66 6965 6c64 2d62  s_order .field-b
+0000ce80: 6f78 2d6c 6162 656c 7b64 6973 706c 6179  ox-label{display
+0000ce90: 3a2d 6d73 2d66 6c65 7862 6f78 3b64 6973  :-ms-flexbox;dis
+0000cea0: 706c 6179 3a66 6c65 783b 6d61 7267 696e  play:flex;margin
+0000ceb0: 2d74 6f70 3a61 7574 6f3b 636f 6c6f 723a  -top:auto;color:
+0000cec0: 2339 3939 7d2e 646a 616e 676f 636d 732d  #999}.djangocms-
+0000ced0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000cee0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000cef0: 7873 5f63 6f6c 202e 6669 656c 642d 626f  xs_col .field-bo
+0000cf00: 782d 6c61 6265 6c20 612c 2e64 6a61 6e67  x-label a,.djang
+0000cf10: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000cf20: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000cf30: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000cf40: 642d 626f 782d 6c61 6265 6c20 612c 2e64  d-box-label a,.d
+0000cf50: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000cf60: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000cf70: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+0000cf80: 6669 656c 642d 626f 782d 6c61 6265 6c20  field-box-label 
+0000cf90: 612c 2e64 6a61 6e67 6f63 6d73 2d66 726f  a,.djangocms-fro
+0000cfa0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000cfb0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000cfc0: 6f66 6673 6574 202e 6669 656c 642d 626f  offset .field-bo
+0000cfd0: 782d 6c61 6265 6c20 612c 2e64 6a61 6e67  x-label a,.djang
+0000cfe0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000cff0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d000: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+0000d010: 6965 6c64 2d62 6f78 2d6c 6162 656c 2061  ield-box-label a
+0000d020: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000d030: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000d040: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000d050: 2e66 6965 6c64 2d62 6f78 2d6c 6162 656c  .field-box-label
+0000d060: 2061 2c2e 646a 616e 676f 636d 732d 6672   a,.djangocms-fr
+0000d070: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000d080: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000d090: 202e 6669 656c 642d 626f 782d 6c61 6265   .field-box-labe
+0000d0a0: 6c20 612c 2e64 6a61 6e67 6f63 6d73 2d66  l a,.djangocms-f
+0000d0b0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000d0c0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000d0d0: 7320 2e66 6965 6c64 2d62 6f78 2d6c 6162  s .field-box-lab
+0000d0e0: 656c 2061 2c2e 646a 616e 676f 636d 732d  el a,.djangocms-
+0000d0f0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000d100: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d110: 6f66 6673 6574 202e 6669 656c 642d 626f  offset .field-bo
+0000d120: 782d 6c61 6265 6c20 612c 2e64 6a61 6e67  x-label a,.djang
+0000d130: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000d140: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000d150: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000d160: 642d 626f 782d 6c61 6265 6c20 617b 7769  d-box-label a{wi
+0000d170: 6474 683a 3130 3025 3b6d 6172 6769 6e2d  dth:100%;margin-
+0000d180: 746f 703a 6175 746f 7d2e 646a 616e 676f  top:auto}.django
+0000d190: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000d1a0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000d1b0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000d1c0: 642d 626f 782d 6c61 6265 6c20 2e69 636f  d-box-label .ico
+0000d1d0: 6e2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  n,.djangocms-fro
+0000d1e0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000d1f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d200: 6d65 202e 6669 656c 642d 626f 782d 6c61  me .field-box-la
+0000d210: 6265 6c20 2e69 636f 6e2c 2e64 6a61 6e67  bel .icon,.djang
+0000d220: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000d230: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d240: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
+0000d250: 642d 626f 782d 6c61 6265 6c20 2e69 636f  d-box-label .ico
+0000d260: 6e2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  n,.djangocms-fro
+0000d270: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000d280: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d290: 6f66 6673 6574 202e 6669 656c 642d 626f  offset .field-bo
+0000d2a0: 782d 6c61 6265 6c20 2e69 636f 6e2c 2e64  x-label .icon,.d
+0000d2b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000d2c0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000d2d0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000d2e0: 7220 2e66 6965 6c64 2d62 6f78 2d6c 6162  r .field-box-lab
+0000d2f0: 656c 202e 6963 6f6e 2c2e 646a 616e 676f  el .icon,.django
+0000d300: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000d310: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000d320: 2d78 735f 636f 6c20 2e66 6965 6c64 2d62  -xs_col .field-b
+0000d330: 6f78 2d6c 6162 656c 202e 6963 6f6e 2c2e  ox-label .icon,.
+0000d340: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000d350: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000d360: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+0000d370: 656c 642d 626f 782d 6c61 6265 6c20 2e69  eld-box-label .i
+0000d380: 636f 6e2c 2e64 6a61 6e67 6f63 6d73 2d66  con,.djangocms-f
+0000d390: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000d3a0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000d3b0: 7320 2e66 6965 6c64 2d62 6f78 2d6c 6162  s .field-box-lab
+0000d3c0: 656c 202e 6963 6f6e 2c2e 646a 616e 676f  el .icon,.django
+0000d3d0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000d3e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000d3f0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000d400: 642d 626f 782d 6c61 6265 6c20 2e69 636f  d-box-label .ico
+0000d410: 6e2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  n,.djangocms-fro
+0000d420: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000d430: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000d440: 6572 202e 6669 656c 642d 626f 782d 6c61  er .field-box-la
+0000d450: 6265 6c20 2e69 636f 6e7b 706f 7369 7469  bel .icon{positi
+0000d460: 6f6e 3a72 656c 6174 6976 653b 746f 703a  on:relative;top:
+0000d470: 3370 787d 2e64 6a61 6e67 6f63 6d73 2d66  3px}.djangocms-f
+0000d480: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000d490: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000d4a0: 735f 636f 6c20 2e66 6965 6c64 2d6c 675f  s_col .field-lg_
+0000d4b0: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
+0000d4c0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000d4d0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000d4e0: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
+0000d4f0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000d500: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000d510: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d520: 636f 6c20 2e66 6965 6c64 2d6d 645f 6d65  col .field-md_me
+0000d530: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000d540: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000d550: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000d560: 6f6c 202e 6669 656c 642d 6d64 5f6d 732c  ol .field-md_ms,
+0000d570: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000d580: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000d590: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
+0000d5a0: 6c20 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  l .field-sm_me,.
+0000d5b0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000d5c0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000d5d0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000d5e0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
+0000d5f0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000d600: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000d610: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000d620: 2e66 6965 6c64 2d78 6c5f 6d65 2c2e 646a  .field-xl_me,.dj
+0000d630: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000d640: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000d650: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+0000d660: 6669 656c 642d 786c 5f6d 732c 2e64 6a61  field-xl_ms,.dja
+0000d670: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000d680: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000d690: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000d6a0: 6965 6c64 2d78 735f 6d65 2c2e 646a 616e  ield-xs_me,.djan
+0000d6b0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000d6c0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000d6d0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+0000d6e0: 656c 642d 7873 5f6d 732c 2e64 6a61 6e67  eld-xs_ms,.djang
+0000d6f0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000d700: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d710: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+0000d720: 6c64 2d78 786c 5f6d 652c 2e64 6a61 6e67  ld-xxl_me,.djang
+0000d730: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000d740: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d750: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+0000d760: 6c64 2d78 786c 5f6d 732c 2e64 6a61 6e67  ld-xxl_ms,.djang
+0000d770: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000d780: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d790: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000d7a0: 642d 6c67 5f6d 652c 2e64 6a61 6e67 6f63  d-lg_me,.djangoc
+0000d7b0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000d7c0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000d7d0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+0000d7e0: 6c67 5f6d 732c 2e64 6a61 6e67 6f63 6d73  lg_ms,.djangocms
+0000d7f0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000d800: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000d810: 2d78 735f 6d65 202e 6669 656c 642d 6d64  -xs_me .field-md
+0000d820: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
+0000d830: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000d840: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000d850: 735f 6d65 202e 6669 656c 642d 6d64 5f6d  s_me .field-md_m
+0000d860: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000d870: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000d880: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d890: 6d65 202e 6669 656c 642d 736d 5f6d 652c  me .field-sm_me,
+0000d8a0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000d8b0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000d8c0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000d8d0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
+0000d8e0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000d8f0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000d900: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+0000d910: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
+0000d920: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000d930: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000d940: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+0000d950: 656c 642d 786c 5f6d 732c 2e64 6a61 6e67  eld-xl_ms,.djang
+0000d960: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000d970: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d980: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000d990: 642d 7873 5f6d 652c 2e64 6a61 6e67 6f63  d-xs_me,.djangoc
+0000d9a0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000d9b0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000d9c0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+0000d9d0: 7873 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xs_ms,.djangocms
+0000d9e0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000d9f0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000da00: 2d78 735f 6d65 202e 6669 656c 642d 7878  -xs_me .field-xx
+0000da10: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
+0000da20: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000da30: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000da40: 7873 5f6d 6520 2e66 6965 6c64 2d78 786c  xs_me .field-xxl
+0000da50: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
+0000da60: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000da70: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000da80: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
+0000da90: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
+0000daa0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000dab0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000dac0: 6d73 202e 6669 656c 642d 6c67 5f6d 732c  ms .field-lg_ms,
+0000dad0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000dae0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000daf0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000db00: 202e 6669 656c 642d 6d64 5f6d 652c 2e64   .field-md_me,.d
+0000db10: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000db20: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000db30: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+0000db40: 6669 656c 642d 6d64 5f6d 732c 2e64 6a61  field-md_ms,.dja
+0000db50: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000db60: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000db70: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000db80: 656c 642d 736d 5f6d 652c 2e64 6a61 6e67  eld-sm_me,.djang
+0000db90: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000dba0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000dbb0: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
+0000dbc0: 642d 736d 5f6d 732c 2e64 6a61 6e67 6f63  d-sm_ms,.djangoc
+0000dbd0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000dbe0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000dbf0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000dc00: 786c 5f6d 652c 2e64 6a61 6e67 6f63 6d73  xl_me,.djangocms
+0000dc10: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000dc20: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000dc30: 2d78 735f 6d73 202e 6669 656c 642d 786c  -xs_ms .field-xl
+0000dc40: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
+0000dc50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000dc60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000dc70: 735f 6d73 202e 6669 656c 642d 7873 5f6d  s_ms .field-xs_m
+0000dc80: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
+0000dc90: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000dca0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000dcb0: 6d73 202e 6669 656c 642d 7873 5f6d 732c  ms .field-xs_ms,
+0000dcc0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000dcd0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000dce0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000dcf0: 202e 6669 656c 642d 7878 6c5f 6d65 2c2e   .field-xxl_me,.
+0000dd00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000dd10: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000dd20: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000dd30: 2e66 6965 6c64 2d78 786c 5f6d 732c 2e64  .field-xxl_ms,.d
+0000dd40: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000dd50: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000dd60: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000dd70: 6574 202e 6669 656c 642d 6c67 5f6d 652c  et .field-lg_me,
+0000dd80: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000dd90: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000dda0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
+0000ddb0: 6673 6574 202e 6669 656c 642d 6c67 5f6d  fset .field-lg_m
+0000ddc0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000ddd0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000dde0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000ddf0: 6f66 6673 6574 202e 6669 656c 642d 6d64  offset .field-md
+0000de00: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
+0000de10: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000de20: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000de30: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+0000de40: 6d64 5f6d 732c 2e64 6a61 6e67 6f63 6d73  md_ms,.djangocms
+0000de50: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000de60: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000de70: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000de80: 642d 736d 5f6d 652c 2e64 6a61 6e67 6f63  d-sm_me,.djangoc
+0000de90: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000dea0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000deb0: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
+0000dec0: 656c 642d 736d 5f6d 732c 2e64 6a61 6e67  eld-sm_ms,.djang
+0000ded0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000dee0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000def0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
+0000df00: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
+0000df10: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000df20: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000df30: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+0000df40: 202e 6669 656c 642d 786c 5f6d 732c 2e64   .field-xl_ms,.d
+0000df50: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000df60: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000df70: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000df80: 6574 202e 6669 656c 642d 7873 5f6d 652c  et .field-xs_me,
+0000df90: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000dfa0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000dfb0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
+0000dfc0: 6673 6574 202e 6669 656c 642d 7873 5f6d  fset .field-xs_m
+0000dfd0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000dfe0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000dff0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000e000: 6f66 6673 6574 202e 6669 656c 642d 7878  offset .field-xx
+0000e010: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
+0000e020: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000e030: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000e040: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000e050: 2d78 786c 5f6d 732c 2e64 6a61 6e67 6f63  -xxl_ms,.djangoc
+0000e060: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000e070: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000e080: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000e090: 6c64 2d6c 675f 6d65 2c2e 646a 616e 676f  ld-lg_me,.django
+0000e0a0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000e0b0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000e0c0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+0000e0d0: 656c 642d 6c67 5f6d 732c 2e64 6a61 6e67  eld-lg_ms,.djang
+0000e0e0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000e0f0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000e100: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+0000e110: 6965 6c64 2d6d 645f 6d65 2c2e 646a 616e  ield-md_me,.djan
+0000e120: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000e130: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000e140: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000e150: 6669 656c 642d 6d64 5f6d 732c 2e64 6a61  field-md_ms,.dja
+0000e160: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000e170: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000e180: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
+0000e190: 2e66 6965 6c64 2d73 6d5f 6d65 2c2e 646a  .field-sm_me,.dj
+0000e1a0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000e1b0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000e1c0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000e1d0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
+0000e1e0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e1f0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000e200: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000e210: 7220 2e66 6965 6c64 2d78 6c5f 6d65 2c2e  r .field-xl_me,.
+0000e220: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000e230: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000e240: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000e250: 6572 202e 6669 656c 642d 786c 5f6d 732c  er .field-xl_ms,
+0000e260: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000e270: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000e280: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
+0000e290: 6465 7220 2e66 6965 6c64 2d78 735f 6d65  der .field-xs_me
+0000e2a0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000e2b0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000e2c0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000e2d0: 7264 6572 202e 6669 656c 642d 7873 5f6d  rder .field-xs_m
+0000e2e0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000e2f0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000e300: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000e310: 6f72 6465 7220 2e66 6965 6c64 2d78 786c  order .field-xxl
+0000e320: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
+0000e330: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000e340: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000e350: 735f 6f72 6465 7220 2e66 6965 6c64 2d78  s_order .field-x
+0000e360: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
+0000e370: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000e380: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000e390: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
+0000e3a0: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
+0000e3b0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000e3c0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000e3d0: 202e 6669 656c 642d 6c67 5f6d 732c 2e64   .field-lg_ms,.d
+0000e3e0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e3f0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000e400: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+0000e410: 656c 642d 6d64 5f6d 652c 2e64 6a61 6e67  eld-md_me,.djang
+0000e420: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000e430: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000e440: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+0000e450: 6d64 5f6d 732c 2e64 6a61 6e67 6f63 6d73  md_ms,.djangocms
+0000e460: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000e470: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000e480: 5f63 6f6c 202e 6669 656c 642d 736d 5f6d  _col .field-sm_m
+0000e490: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
+0000e4a0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000e4b0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000e4c0: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
+0000e4d0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e4e0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000e4f0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+0000e500: 656c 642d 786c 5f6d 652c 2e64 6a61 6e67  eld-xl_me,.djang
+0000e510: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000e520: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000e530: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+0000e540: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
+0000e550: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000e560: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000e570: 5f63 6f6c 202e 6669 656c 642d 7873 5f6d  _col .field-xs_m
+0000e580: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
+0000e590: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000e5a0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000e5b0: 202e 6669 656c 642d 7873 5f6d 732c 2e64   .field-xs_ms,.d
+0000e5c0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e5d0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000e5e0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+0000e5f0: 656c 642d 7878 6c5f 6d65 2c2e 646a 616e  eld-xxl_me,.djan
+0000e600: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000e610: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000e620: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+0000e630: 2d78 786c 5f6d 732c 2e64 6a61 6e67 6f63  -xxl_ms,.djangoc
+0000e640: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000e650: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000e660: 7873 5f6d 6520 2e66 6965 6c64 2d6c 675f  xs_me .field-lg_
+0000e670: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
+0000e680: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000e690: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000e6a0: 202e 6669 656c 642d 6c67 5f6d 732c 2e64   .field-lg_ms,.d
+0000e6b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e6c0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000e6d0: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
+0000e6e0: 6c64 2d6d 645f 6d65 2c2e 646a 616e 676f  ld-md_me,.django
+0000e6f0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000e700: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000e710: 2d78 735f 6d65 202e 6669 656c 642d 6d64  -xs_me .field-md
+0000e720: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
+0000e730: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000e740: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000e750: 6520 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  e .field-sm_me,.
+0000e760: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000e770: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000e780: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+0000e790: 656c 642d 736d 5f6d 732c 2e64 6a61 6e67  eld-sm_ms,.djang
+0000e7a0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000e7b0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000e7c0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d78  d-xs_me .field-x
+0000e7d0: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
+0000e7e0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000e7f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000e800: 6d65 202e 6669 656c 642d 786c 5f6d 732c  me .field-xl_ms,
+0000e810: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000e820: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000e830: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
+0000e840: 6965 6c64 2d78 735f 6d65 2c2e 646a 616e  ield-xs_me,.djan
+0000e850: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000e860: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000e870: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+0000e880: 7873 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xs_ms,.djangocms
+0000e890: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000e8a0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000e8b0: 5f6d 6520 2e66 6965 6c64 2d78 786c 5f6d  _me .field-xxl_m
+0000e8c0: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
+0000e8d0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000e8e0: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+0000e8f0: 2e66 6965 6c64 2d78 786c 5f6d 732c 2e64  .field-xxl_ms,.d
+0000e900: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e910: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000e920: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+0000e930: 6c64 2d6c 675f 6d65 2c2e 646a 616e 676f  ld-lg_me,.django
+0000e940: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000e950: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000e960: 2d78 735f 6d73 202e 6669 656c 642d 6c67  -xs_ms .field-lg
+0000e970: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
+0000e980: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000e990: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000e9a0: 7320 2e66 6965 6c64 2d6d 645f 6d65 2c2e  s .field-md_me,.
+0000e9b0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000e9c0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000e9d0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000e9e0: 656c 642d 6d64 5f6d 732c 2e64 6a61 6e67  eld-md_ms,.djang
+0000e9f0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000ea00: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000ea10: 642d 7873 5f6d 7320 2e66 6965 6c64 2d73  d-xs_ms .field-s
+0000ea20: 6d5f 6d65 2c2e 646a 616e 676f 636d 732d  m_me,.djangocms-
+0000ea30: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000ea40: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000ea50: 6d73 202e 6669 656c 642d 736d 5f6d 732c  ms .field-sm_ms,
+0000ea60: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000ea70: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000ea80: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
+0000ea90: 6965 6c64 2d78 6c5f 6d65 2c2e 646a 616e  ield-xl_me,.djan
+0000eaa0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000eab0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000eac0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000ead0: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
+0000eae0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000eaf0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000eb00: 5f6d 7320 2e66 6965 6c64 2d78 735f 6d65  _ms .field-xs_me
+0000eb10: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000eb20: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000eb30: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+0000eb40: 6669 656c 642d 7873 5f6d 732c 2e64 6a61  field-xs_ms,.dja
+0000eb50: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000eb60: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000eb70: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
+0000eb80: 2d78 786c 5f6d 652c 2e64 6a61 6e67 6f63  -xxl_me,.djangoc
+0000eb90: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000eba0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ebb0: 7873 5f6d 7320 2e66 6965 6c64 2d78 786c  xs_ms .field-xxl
+0000ebc0: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
+0000ebd0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000ebe0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000ebf0: 6666 7365 7420 2e66 6965 6c64 2d6c 675f  ffset .field-lg_
+0000ec00: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
+0000ec10: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000ec20: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
+0000ec30: 6673 6574 202e 6669 656c 642d 6c67 5f6d  fset .field-lg_m
+0000ec40: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000ec50: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000ec60: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+0000ec70: 7365 7420 2e66 6965 6c64 2d6d 645f 6d65  set .field-md_me
+0000ec80: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000ec90: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000eca0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000ecb0: 6574 202e 6669 656c 642d 6d64 5f6d 732c  et .field-md_ms,
+0000ecc0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000ecd0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000ece0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000ecf0: 7420 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  t .field-sm_me,.
+0000ed00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000ed10: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000ed20: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+0000ed30: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
+0000ed40: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000ed50: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000ed60: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
+0000ed70: 2e66 6965 6c64 2d78 6c5f 6d65 2c2e 646a  .field-xl_me,.dj
+0000ed80: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000ed90: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000eda0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
+0000edb0: 6669 656c 642d 786c 5f6d 732c 2e64 6a61  field-xl_ms,.dja
+0000edc0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000edd0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000ede0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
+0000edf0: 6965 6c64 2d78 735f 6d65 2c2e 646a 616e  ield-xs_me,.djan
+0000ee00: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000ee10: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000ee20: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
+0000ee30: 656c 642d 7873 5f6d 732c 2e64 6a61 6e67  eld-xs_ms,.djang
+0000ee40: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000ee50: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000ee60: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
+0000ee70: 6c64 2d78 786c 5f6d 652c 2e64 6a61 6e67  ld-xxl_me,.djang
+0000ee80: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000ee90: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000eea0: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
+0000eeb0: 6c64 2d78 786c 5f6d 732c 2e64 6a61 6e67  ld-xxl_ms,.djang
+0000eec0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000eed0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000eee0: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000eef0: 642d 6c67 5f6d 652c 2e64 6a61 6e67 6f63  d-lg_me,.djangoc
+0000ef00: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000ef10: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ef20: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000ef30: 6c67 5f6d 732c 2e64 6a61 6e67 6f63 6d73  lg_ms,.djangocms
+0000ef40: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000ef50: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000ef60: 5f6f 7264 6572 202e 6669 656c 642d 6d64  _order .field-md
+0000ef70: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
+0000ef80: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000ef90: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000efa0: 7264 6572 202e 6669 656c 642d 6d64 5f6d  rder .field-md_m
+0000efb0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
+0000efc0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000efd0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000efe0: 6572 202e 6669 656c 642d 736d 5f6d 652c  er .field-sm_me,
+0000eff0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000f000: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000f010: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000f020: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
+0000f030: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000f040: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000f050: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000f060: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
+0000f070: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000f080: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000f090: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+0000f0a0: 656c 642d 786c 5f6d 732c 2e64 6a61 6e67  eld-xl_ms,.djang
+0000f0b0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000f0c0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000f0d0: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000f0e0: 642d 7873 5f6d 652c 2e64 6a61 6e67 6f63  d-xs_me,.djangoc
+0000f0f0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000f100: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f110: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000f120: 7873 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xs_ms,.djangocms
+0000f130: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000f140: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000f150: 5f6f 7264 6572 202e 6669 656c 642d 7878  _order .field-xx
+0000f160: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
+0000f170: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000f180: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000f190: 6f72 6465 7220 2e66 6965 6c64 2d78 786c  order .field-xxl
+0000f1a0: 5f6d 737b 7465 7874 2d61 6c69 676e 3a6c  _ms{text-align:l
+0000f1b0: 6566 747d 2e64 6a61 6e67 6f63 6d73 2d66  eft}.djangocms-f
+0000f1c0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000f1d0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000f1e0: 735f 636f 6c20 2e66 6965 6c64 2d6c 675f  s_col .field-lg_
+0000f1f0: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
+0000f200: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000f210: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000f220: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000f230: 642d 6c67 5f6d 7320 6c61 6265 6c2c 2e64  d-lg_ms label,.d
+0000f240: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000f250: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000f260: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000f270: 2e66 6965 6c64 2d6d 645f 6d65 206c 6162  .field-md_me lab
+0000f280: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
+0000f290: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000f2a0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000f2b0: 5f63 6f6c 202e 6669 656c 642d 6d64 5f6d  _col .field-md_m
+0000f2c0: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+0000f2d0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000f2e0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000f2f0: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+0000f300: 2d73 6d5f 6d65 206c 6162 656c 2c2e 646a  -sm_me label,.dj
+0000f310: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f320: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000f330: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+0000f340: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
+0000f350: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000f360: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000f370: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000f380: 636f 6c20 2e66 6965 6c64 2d78 6c5f 6d65  col .field-xl_me
+0000f390: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000f3a0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000f3b0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000f3c0: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+0000f3d0: 786c 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xl_ms label,.dja
+0000f3e0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000f3f0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000f400: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000f410: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
+0000f420: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000f430: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000f440: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000f450: 6f6c 202e 6669 656c 642d 7873 5f6d 7320  ol .field-xs_ms 
+0000f460: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000f470: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000f480: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000f490: 2d78 735f 636f 6c20 2e66 6965 6c64 2d78  -xs_col .field-x
+0000f4a0: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
+0000f4b0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000f4c0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000f4d0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000f4e0: 6965 6c64 2d78 786c 5f6d 7320 6c61 6265  ield-xxl_ms labe
+0000f4f0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000f500: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000f510: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000f520: 6d65 202e 6669 656c 642d 6c67 5f6d 6520  me .field-lg_me 
+0000f530: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000f540: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000f550: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000f560: 2d78 735f 6d65 202e 6669 656c 642d 6c67  -xs_me .field-lg
+0000f570: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+0000f580: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000f590: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000f5a0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000f5b0: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
+0000f5c0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000f5d0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000f5e0: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+0000f5f0: 6669 656c 642d 6d64 5f6d 7320 6c61 6265  field-md_ms labe
+0000f600: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000f610: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000f620: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000f630: 6d65 202e 6669 656c 642d 736d 5f6d 6520  me .field-sm_me 
+0000f640: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000f650: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000f660: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000f670: 2d78 735f 6d65 202e 6669 656c 642d 736d  -xs_me .field-sm
+0000f680: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+0000f690: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000f6a0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000f6b0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000f6c0: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
+0000f6d0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000f6e0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000f6f0: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+0000f700: 6669 656c 642d 786c 5f6d 7320 6c61 6265  field-xl_ms labe
+0000f710: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000f720: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000f730: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000f740: 6d65 202e 6669 656c 642d 7873 5f6d 6520  me .field-xs_me 
+0000f750: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000f760: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000f770: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000f780: 2d78 735f 6d65 202e 6669 656c 642d 7873  -xs_me .field-xs
+0000f790: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+0000f7a0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000f7b0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000f7c0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000f7d0: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
+0000f7e0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000f7f0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000f800: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+0000f810: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
+0000f820: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000f830: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000f840: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000f850: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
+0000f860: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
+0000f870: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000f880: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000f890: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000f8a0: 6c67 5f6d 7320 6c61 6265 6c2c 2e64 6a61  lg_ms label,.dja
+0000f8b0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000f8c0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000f8d0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000f8e0: 656c 642d 6d64 5f6d 6520 6c61 6265 6c2c  eld-md_me label,
+0000f8f0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000f900: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000f910: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000f920: 202e 6669 656c 642d 6d64 5f6d 7320 6c61   .field-md_ms la
+0000f930: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000f940: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000f950: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000f960: 735f 6d73 202e 6669 656c 642d 736d 5f6d  s_ms .field-sm_m
+0000f970: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
+0000f980: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000f990: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000f9a0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000f9b0: 736d 5f6d 7320 6c61 6265 6c2c 2e64 6a61  sm_ms label,.dja
+0000f9c0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000f9d0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000f9e0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000f9f0: 656c 642d 786c 5f6d 6520 6c61 6265 6c2c  eld-xl_me label,
+0000fa00: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000fa10: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000fa20: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000fa30: 202e 6669 656c 642d 786c 5f6d 7320 6c61   .field-xl_ms la
+0000fa40: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000fa50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000fa60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000fa70: 735f 6d73 202e 6669 656c 642d 7873 5f6d  s_ms .field-xs_m
+0000fa80: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
+0000fa90: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000faa0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000fab0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000fac0: 7873 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xs_ms label,.dja
+0000fad0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000fae0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000faf0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000fb00: 656c 642d 7878 6c5f 6d65 206c 6162 656c  eld-xxl_me label
+0000fb10: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000fb20: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000fb30: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000fb40: 7320 2e66 6965 6c64 2d78 786c 5f6d 7320  s .field-xxl_ms 
+0000fb50: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000fb60: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000fb70: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000fb80: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000fb90: 642d 6c67 5f6d 6520 6c61 6265 6c2c 2e64  d-lg_me label,.d
+0000fba0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000fbb0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000fbc0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000fbd0: 6574 202e 6669 656c 642d 6c67 5f6d 7320  et .field-lg_ms 
+0000fbe0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000fbf0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000fc00: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000fc10: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000fc20: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
+0000fc30: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000fc40: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000fc50: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000fc60: 6574 202e 6669 656c 642d 6d64 5f6d 7320  et .field-md_ms 
+0000fc70: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000fc80: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000fc90: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000fca0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000fcb0: 642d 736d 5f6d 6520 6c61 6265 6c2c 2e64  d-sm_me label,.d
+0000fcc0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000fcd0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000fce0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000fcf0: 6574 202e 6669 656c 642d 736d 5f6d 7320  et .field-sm_ms 
+0000fd00: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000fd10: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000fd20: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000fd30: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000fd40: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
+0000fd50: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000fd60: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000fd70: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000fd80: 6574 202e 6669 656c 642d 786c 5f6d 7320  et .field-xl_ms 
+0000fd90: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000fda0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000fdb0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000fdc0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000fdd0: 642d 7873 5f6d 6520 6c61 6265 6c2c 2e64  d-xs_me label,.d
+0000fde0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000fdf0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000fe00: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000fe10: 6574 202e 6669 656c 642d 7873 5f6d 7320  et .field-xs_ms 
+0000fe20: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000fe30: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000fe40: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000fe50: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000fe60: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
+0000fe70: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000fe80: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000fe90: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+0000fea0: 7365 7420 2e66 6965 6c64 2d78 786c 5f6d  set .field-xxl_m
+0000feb0: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+0000fec0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000fed0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000fee0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000fef0: 6c64 2d6c 675f 6d65 206c 6162 656c 2c2e  ld-lg_me label,.
+0000ff00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000ff10: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000ff20: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000ff30: 6572 202e 6669 656c 642d 6c67 5f6d 7320  er .field-lg_ms 
+0000ff40: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000ff50: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000ff60: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000ff70: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+0000ff80: 2d6d 645f 6d65 206c 6162 656c 2c2e 646a  -md_me label,.dj
+0000ff90: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000ffa0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000ffb0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000ffc0: 202e 6669 656c 642d 6d64 5f6d 7320 6c61   .field-md_ms la
+0000ffd0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000ffe0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000fff0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00010000: 735f 6f72 6465 7220 2e66 6965 6c64 2d73  s_order .field-s
+00010010: 6d5f 6d65 206c 6162 656c 2c2e 646a 616e  m_me label,.djan
+00010020: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+00010030: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+00010040: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+00010050: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
+00010060: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+00010070: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+00010080: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+00010090: 6f72 6465 7220 2e66 6965 6c64 2d78 6c5f  order .field-xl_
+000100a0: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
+000100b0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+000100c0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+000100d0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+000100e0: 656c 642d 786c 5f6d 7320 6c61 6265 6c2c  eld-xl_ms label,
+000100f0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00010100: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+00010110: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
+00010120: 6465 7220 2e66 6965 6c64 2d78 735f 6d65  der .field-xs_me
+00010130: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+00010140: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+00010150: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+00010160: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+00010170: 642d 7873 5f6d 7320 6c61 6265 6c2c 2e64  d-xs_ms label,.d
+00010180: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00010190: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+000101a0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+000101b0: 7220 2e66 6965 6c64 2d78 786c 5f6d 6520  r .field-xxl_me 
+000101c0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+000101d0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+000101e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+000101f0: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+00010200: 2d78 786c 5f6d 7320 6c61 6265 6c2c 2e64  -xxl_ms label,.d
+00010210: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00010220: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00010230: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+00010240: 656c 642d 6c67 5f6d 6520 6c61 6265 6c2c  eld-lg_me label,
+00010250: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00010260: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00010270: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+00010280: 6669 656c 642d 6c67 5f6d 7320 6c61 6265  field-lg_ms labe
+00010290: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+000102a0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+000102b0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+000102c0: 202e 6669 656c 642d 6d64 5f6d 6520 6c61   .field-md_me la
+000102d0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+000102e0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+000102f0: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+00010300: 6f6c 202e 6669 656c 642d 6d64 5f6d 7320  ol .field-md_ms 
+00010310: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+00010320: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00010330: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00010340: 5f63 6f6c 202e 6669 656c 642d 736d 5f6d  _col .field-sm_m
+00010350: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
+00010360: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+00010370: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00010380: 7873 5f63 6f6c 202e 6669 656c 642d 736d  xs_col .field-sm
+00010390: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+000103a0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+000103b0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+000103c0: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+000103d0: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
+000103e0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+000103f0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00010400: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+00010410: 642d 786c 5f6d 7320 6c61 6265 6c2c 2e64  d-xl_ms label,.d
+00010420: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00010430: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00010440: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+00010450: 656c 642d 7873 5f6d 6520 6c61 6265 6c2c  eld-xs_me label,
+00010460: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00010470: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00010480: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+00010490: 6669 656c 642d 7873 5f6d 7320 6c61 6265  field-xs_ms labe
+000104a0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+000104b0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+000104c0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+000104d0: 202e 6669 656c 642d 7878 6c5f 6d65 206c   .field-xxl_me l
+000104e0: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
+000104f0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+00010500: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+00010510: 636f 6c20 2e66 6965 6c64 2d78 786c 5f6d  col .field-xxl_m
+00010520: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+00010530: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+00010540: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00010550: 7873 5f6d 6520 2e66 6965 6c64 2d6c 675f  xs_me .field-lg_
+00010560: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
+00010570: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+00010580: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+00010590: 2d78 735f 6d65 202e 6669 656c 642d 6c67  -xs_me .field-lg
+000105a0: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+000105b0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+000105c0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+000105d0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d6d  d-xs_me .field-m
+000105e0: 645f 6d65 206c 6162 656c 2c2e 646a 616e  d_me label,.djan
+000105f0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+00010600: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+00010610: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+00010620: 6d64 5f6d 7320 6c61 6265 6c2c 2e64 6a61  md_ms label,.dja
+00010630: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00010640: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00010650: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+00010660: 2d73 6d5f 6d65 206c 6162 656c 2c2e 646a  -sm_me label,.dj
+00010670: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+00010680: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+00010690: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+000106a0: 642d 736d 5f6d 7320 6c61 6265 6c2c 2e64  d-sm_ms label,.d
+000106b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+000106c0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+000106d0: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
+000106e0: 6c64 2d78 6c5f 6d65 206c 6162 656c 2c2e  ld-xl_me label,.
+000106f0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00010700: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+00010710: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+00010720: 656c 642d 786c 5f6d 7320 6c61 6265 6c2c  eld-xl_ms label,
+00010730: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00010740: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00010750: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
+00010760: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
+00010770: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+00010780: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+00010790: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+000107a0: 6669 656c 642d 7873 5f6d 7320 6c61 6265  field-xs_ms labe
+000107b0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+000107c0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+000107d0: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+000107e0: 2e66 6965 6c64 2d78 786c 5f6d 6520 6c61  .field-xxl_me la
+000107f0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+00010800: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00010810: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+00010820: 6520 2e66 6965 6c64 2d78 786c 5f6d 7320  e .field-xxl_ms 
+00010830: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+00010840: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00010850: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00010860: 5f6d 7320 2e66 6965 6c64 2d6c 675f 6d65  _ms .field-lg_me
+00010870: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+00010880: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+00010890: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+000108a0: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
+000108b0: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+000108c0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+000108d0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+000108e0: 7873 5f6d 7320 2e66 6965 6c64 2d6d 645f  xs_ms .field-md_
+000108f0: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
+00010900: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+00010910: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+00010920: 2d78 735f 6d73 202e 6669 656c 642d 6d64  -xs_ms .field-md
+00010930: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+00010940: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+00010950: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+00010960: 642d 7873 5f6d 7320 2e66 6965 6c64 2d73  d-xs_ms .field-s
+00010970: 6d5f 6d65 206c 6162 656c 2c2e 646a 616e  m_me label,.djan
+00010980: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+00010990: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+000109a0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+000109b0: 736d 5f6d 7320 6c61 6265 6c2c 2e64 6a61  sm_ms label,.dja
+000109c0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+000109d0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+000109e0: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
+000109f0: 2d78 6c5f 6d65 206c 6162 656c 2c2e 646a  -xl_me label,.dj
+00010a00: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+00010a10: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+00010a20: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
+00010a30: 642d 786c 5f6d 7320 6c61 6265 6c2c 2e64  d-xl_ms label,.d
+00010a40: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00010a50: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00010a60: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+00010a70: 6c64 2d78 735f 6d65 206c 6162 656c 2c2e  ld-xs_me label,.
+00010a80: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00010a90: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+00010aa0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+00010ab0: 656c 642d 7873 5f6d 7320 6c61 6265 6c2c  eld-xs_ms label,
+00010ac0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00010ad0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00010ae0: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
+00010af0: 6965 6c64 2d78 786c 5f6d 6520 6c61 6265  ield-xxl_me labe
+00010b00: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+00010b10: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00010b20: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+00010b30: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
+00010b40: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+00010b50: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00010b60: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+00010b70: 6666 7365 7420 2e66 6965 6c64 2d6c 675f  ffset .field-lg_
+00010b80: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
+00010b90: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+00010ba0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+00010bb0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+00010bc0: 642d 6c67 5f6d 7320 6c61 6265 6c2c 2e64  d-lg_ms label,.d
+00010bd0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00010be0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00010bf0: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
+00010c00: 2e66 6965 6c64 2d6d 645f 6d65 206c 6162  .field-md_me lab
+00010c10: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
+00010c20: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+00010c30: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
+00010c40: 6673 6574 202e 6669 656c 642d 6d64 5f6d  fset .field-md_m
+00010c50: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+00010c60: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+00010c70: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00010c80: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+00010c90: 2d73 6d5f 6d65 206c 6162 656c 2c2e 646a  -sm_me label,.dj
+00010ca0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+00010cb0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+00010cc0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
+00010cd0: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
+00010ce0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+00010cf0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00010d00: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+00010d10: 7365 7420 2e66 6965 6c64 2d78 6c5f 6d65  set .field-xl_me
+00010d20: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+00010d30: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+00010d40: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00010d50: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+00010d60: 786c 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xl_ms label,.dja
+00010d70: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00010d80: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00010d90: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
+00010da0: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
+00010db0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+00010dc0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+00010dd0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+00010de0: 6574 202e 6669 656c 642d 7873 5f6d 7320  et .field-xs_ms 
+00010df0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+00010e00: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00010e10: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00010e20: 5f6f 6666 7365 7420 2e66 6965 6c64 2d78  _offset .field-x
+00010e30: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
+00010e40: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00010e50: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00010e60: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
+00010e70: 6965 6c64 2d78 786c 5f6d 7320 6c61 6265  ield-xxl_ms labe
+00010e80: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+00010e90: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00010ea0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+00010eb0: 6572 202e 6669 656c 642d 6c67 5f6d 6520  er .field-lg_me 
+00010ec0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+00010ed0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00010ee0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00010ef0: 5f6f 7264 6572 202e 6669 656c 642d 6c67  _order .field-lg
+00010f00: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+00010f10: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+00010f20: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+00010f30: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+00010f40: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
+00010f50: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00010f60: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00010f70: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+00010f80: 6669 656c 642d 6d64 5f6d 7320 6c61 6265  field-md_ms labe
+00010f90: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+00010fa0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00010fb0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+00010fc0: 6572 202e 6669 656c 642d 736d 5f6d 6520  er .field-sm_me 
+00010fd0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+00010fe0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00010ff0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00011000: 5f6f 7264 6572 202e 6669 656c 642d 736d  _order .field-sm
+00011010: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+00011020: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+00011030: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+00011040: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+00011050: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
+00011060: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00011070: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00011080: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+00011090: 6669 656c 642d 786c 5f6d 7320 6c61 6265  field-xl_ms labe
+000110a0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+000110b0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+000110c0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+000110d0: 6572 202e 6669 656c 642d 7873 5f6d 6520  er .field-xs_me 
+000110e0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+000110f0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00011100: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00011110: 5f6f 7264 6572 202e 6669 656c 642d 7873  _order .field-xs
+00011120: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+00011130: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+00011140: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+00011150: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+00011160: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
+00011170: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00011180: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+00011190: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
+000111a0: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
+000111b0: 6265 6c7b 6c65 6674 3a33 3070 783b 626f  bel{left:30px;bo
+000111c0: 7474 6f6d 3a31 3470 787d 2e64 6a61 6e67  ttom:14px}.djang
+000111d0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+000111e0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+000111f0: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+00011200: 6c64 2d6c 675f 6d65 2069 6e70 7574 2c2e  ld-lg_me input,.
+00011210: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00011220: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+00011230: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+00011240: 202e 6669 656c 642d 6c67 5f6d 7320 696e   .field-lg_ms in
+00011250: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00011260: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+00011270: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011280: 735f 636f 6c20 2e66 6965 6c64 2d6d 645f  s_col .field-md_
+00011290: 6d65 2069 6e70 7574 2c2e 646a 616e 676f  me input,.django
+000112a0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+000112b0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+000112c0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+000112d0: 642d 6d64 5f6d 7320 696e 7075 742c 2e64  d-md_ms input,.d
+000112e0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+000112f0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+00011300: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+00011310: 2e66 6965 6c64 2d73 6d5f 6d65 2069 6e70  .field-sm_me inp
+00011320: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+00011330: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+00011340: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00011350: 5f63 6f6c 202e 6669 656c 642d 736d 5f6d  _col .field-sm_m
+00011360: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00011370: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+00011380: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+00011390: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+000113a0: 2d78 6c5f 6d65 2069 6e70 7574 2c2e 646a  -xl_me input,.dj
+000113b0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+000113c0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+000113d0: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+000113e0: 6669 656c 642d 786c 5f6d 7320 696e 7075  field-xl_ms inpu
+000113f0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+00011400: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+00011410: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+00011420: 636f 6c20 2e66 6965 6c64 2d78 735f 6d65  col .field-xs_me
+00011430: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+00011440: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+00011450: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+00011460: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+00011470: 7873 5f6d 7320 696e 7075 742c 2e64 6a61  xs_ms input,.dja
+00011480: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011490: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+000114a0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+000114b0: 6965 6c64 2d78 786c 5f6d 6520 696e 7075  ield-xxl_me inpu
+000114c0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+000114d0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+000114e0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+000114f0: 636f 6c20 2e66 6965 6c64 2d78 786c 5f6d  col .field-xxl_m
+00011500: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00011510: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+00011520: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+00011530: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+00011540: 6c67 5f6d 6520 696e 7075 742c 2e64 6a61  lg_me input,.dja
+00011550: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011560: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011570: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+00011580: 656c 642d 6c67 5f6d 7320 696e 7075 742c  eld-lg_ms input,
+00011590: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+000115a0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+000115b0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+000115c0: 202e 6669 656c 642d 6d64 5f6d 6520 696e   .field-md_me in
+000115d0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+000115e0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+000115f0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011600: 735f 6d65 202e 6669 656c 642d 6d64 5f6d  s_me .field-md_m
+00011610: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00011620: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+00011630: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+00011640: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+00011650: 736d 5f6d 6520 696e 7075 742c 2e64 6a61  sm_me input,.dja
+00011660: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011670: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011680: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+00011690: 656c 642d 736d 5f6d 7320 696e 7075 742c  eld-sm_ms input,
+000116a0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+000116b0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+000116c0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+000116d0: 202e 6669 656c 642d 786c 5f6d 6520 696e   .field-xl_me in
+000116e0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+000116f0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+00011700: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011710: 735f 6d65 202e 6669 656c 642d 786c 5f6d  s_me .field-xl_m
+00011720: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00011730: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+00011740: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+00011750: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+00011760: 7873 5f6d 6520 696e 7075 742c 2e64 6a61  xs_me input,.dja
+00011770: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011780: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011790: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+000117a0: 656c 642d 7873 5f6d 7320 696e 7075 742c  eld-xs_ms input,
+000117b0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+000117c0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+000117d0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+000117e0: 202e 6669 656c 642d 7878 6c5f 6d65 2069   .field-xxl_me i
+000117f0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+00011800: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+00011810: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00011820: 7873 5f6d 6520 2e66 6965 6c64 2d78 786c  xs_me .field-xxl
+00011830: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
+00011840: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+00011850: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+00011860: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
+00011870: 642d 6c67 5f6d 6520 696e 7075 742c 2e64  d-lg_me input,.d
+00011880: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00011890: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+000118a0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+000118b0: 6669 656c 642d 6c67 5f6d 7320 696e 7075  field-lg_ms inpu
+000118c0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+000118d0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+000118e0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+000118f0: 6d73 202e 6669 656c 642d 6d64 5f6d 6520  ms .field-md_me 
+00011900: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+00011910: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+00011920: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+00011930: 2d78 735f 6d73 202e 6669 656c 642d 6d64  -xs_ms .field-md
+00011940: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
+00011950: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+00011960: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+00011970: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
+00011980: 642d 736d 5f6d 6520 696e 7075 742c 2e64  d-sm_me input,.d
+00011990: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+000119a0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+000119b0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+000119c0: 6669 656c 642d 736d 5f6d 7320 696e 7075  field-sm_ms inpu
+000119d0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+000119e0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+000119f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+00011a00: 6d73 202e 6669 656c 642d 786c 5f6d 6520  ms .field-xl_me 
+00011a10: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+00011a20: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+00011a30: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+00011a40: 2d78 735f 6d73 202e 6669 656c 642d 786c  -xs_ms .field-xl
+00011a50: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
+00011a60: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+00011a70: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+00011a80: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
+00011a90: 642d 7873 5f6d 6520 696e 7075 742c 2e64  d-xs_me input,.d
+00011aa0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00011ab0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+00011ac0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+00011ad0: 6669 656c 642d 7873 5f6d 7320 696e 7075  field-xs_ms inpu
+00011ae0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+00011af0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+00011b00: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+00011b10: 6d73 202e 6669 656c 642d 7878 6c5f 6d65  ms .field-xxl_me
+00011b20: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+00011b30: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+00011b40: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+00011b50: 642d 7873 5f6d 7320 2e66 6965 6c64 2d78  d-xs_ms .field-x
+00011b60: 786c 5f6d 7320 696e 7075 742c 2e64 6a61  xl_ms input,.dja
+00011b70: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011b80: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011b90: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+00011ba0: 202e 6669 656c 642d 6c67 5f6d 6520 696e   .field-lg_me in
+00011bb0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00011bc0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+00011bd0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011be0: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+00011bf0: 6c67 5f6d 7320 696e 7075 742c 2e64 6a61  lg_ms input,.dja
+00011c00: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011c10: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011c20: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+00011c30: 202e 6669 656c 642d 6d64 5f6d 6520 696e   .field-md_me in
+00011c40: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00011c50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+00011c60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011c70: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+00011c80: 6d64 5f6d 7320 696e 7075 742c 2e64 6a61  md_ms input,.dja
+00011c90: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011ca0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011cb0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+00011cc0: 202e 6669 656c 642d 736d 5f6d 6520 696e   .field-sm_me in
+00011cd0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00011ce0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+00011cf0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011d00: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+00011d10: 736d 5f6d 7320 696e 7075 742c 2e64 6a61  sm_ms input,.dja
+00011d20: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011d30: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011d40: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+00011d50: 202e 6669 656c 642d 786c 5f6d 6520 696e   .field-xl_me in
+00011d60: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00011d70: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+00011d80: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011d90: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+00011da0: 786c 5f6d 7320 696e 7075 742c 2e64 6a61  xl_ms input,.dja
+00011db0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011dc0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011dd0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+00011de0: 202e 6669 656c 642d 7873 5f6d 6520 696e   .field-xs_me in
+00011df0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00011e00: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+00011e10: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00011e20: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+00011e30: 7873 5f6d 7320 696e 7075 742c 2e64 6a61  xs_ms input,.dja
+00011e40: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011e50: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011e60: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+00011e70: 202e 6669 656c 642d 7878 6c5f 6d65 2069   .field-xxl_me i
+00011e80: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+00011e90: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+00011ea0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00011eb0: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+00011ec0: 2d78 786c 5f6d 7320 696e 7075 742c 2e64  -xxl_ms input,.d
+00011ed0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00011ee0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+00011ef0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+00011f00: 7220 2e66 6965 6c64 2d6c 675f 6d65 2069  r .field-lg_me i
+00011f10: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+00011f20: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+00011f30: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00011f40: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+00011f50: 6c67 5f6d 7320 696e 7075 742c 2e64 6a61  lg_ms input,.dja
+00011f60: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00011f70: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00011f80: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
+00011f90: 2e66 6965 6c64 2d6d 645f 6d65 2069 6e70  .field-md_me inp
+00011fa0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+00011fb0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+00011fc0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00011fd0: 5f6f 7264 6572 202e 6669 656c 642d 6d64  _order .field-md
+00011fe0: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
+00011ff0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+00012000: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+00012010: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+00012020: 6965 6c64 2d73 6d5f 6d65 2069 6e70 7574  ield-sm_me input
+00012030: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+00012040: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+00012050: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+00012060: 7264 6572 202e 6669 656c 642d 736d 5f6d  rder .field-sm_m
+00012070: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00012080: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+00012090: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+000120a0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+000120b0: 6c64 2d78 6c5f 6d65 2069 6e70 7574 2c2e  ld-xl_me input,.
+000120c0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+000120d0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+000120e0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+000120f0: 6572 202e 6669 656c 642d 786c 5f6d 7320  er .field-xl_ms 
+00012100: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+00012110: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+00012120: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+00012130: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+00012140: 2d78 735f 6d65 2069 6e70 7574 2c2e 646a  -xs_me input,.dj
+00012150: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+00012160: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+00012170: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+00012180: 202e 6669 656c 642d 7873 5f6d 7320 696e   .field-xs_ms in
+00012190: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+000121a0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+000121b0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+000121c0: 735f 6f72 6465 7220 2e66 6965 6c64 2d78  s_order .field-x
+000121d0: 786c 5f6d 6520 696e 7075 742c 2e64 6a61  xl_me input,.dja
+000121e0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+000121f0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+00012200: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
+00012210: 2e66 6965 6c64 2d78 786c 5f6d 7320 696e  .field-xxl_ms in
+00012220: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00012230: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00012240: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+00012250: 6f6c 202e 6669 656c 642d 6c67 5f6d 6520  ol .field-lg_me 
+00012260: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+00012270: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00012280: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00012290: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
+000122a0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+000122b0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+000122c0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+000122d0: 7873 5f63 6f6c 202e 6669 656c 642d 6d64  xs_col .field-md
+000122e0: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
+000122f0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+00012300: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+00012310: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+00012320: 6d64 5f6d 7320 696e 7075 742c 2e64 6a61  md_ms input,.dja
+00012330: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00012340: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00012350: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+00012360: 642d 736d 5f6d 6520 696e 7075 742c 2e64  d-sm_me input,.d
+00012370: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00012380: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00012390: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+000123a0: 656c 642d 736d 5f6d 7320 696e 7075 742c  eld-sm_ms input,
+000123b0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+000123c0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+000123d0: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+000123e0: 6669 656c 642d 786c 5f6d 6520 696e 7075  field-xl_me inpu
+000123f0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+00012400: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00012410: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+00012420: 202e 6669 656c 642d 786c 5f6d 7320 696e   .field-xl_ms in
+00012430: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00012440: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00012450: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+00012460: 6f6c 202e 6669 656c 642d 7873 5f6d 6520  ol .field-xs_me 
+00012470: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+00012480: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00012490: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+000124a0: 5f63 6f6c 202e 6669 656c 642d 7873 5f6d  _col .field-xs_m
+000124b0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+000124c0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+000124d0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+000124e0: 7873 5f63 6f6c 202e 6669 656c 642d 7878  xs_col .field-xx
+000124f0: 6c5f 6d65 2069 6e70 7574 2c2e 646a 616e  l_me input,.djan
+00012500: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+00012510: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+00012520: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+00012530: 2d78 786c 5f6d 7320 696e 7075 742c 2e64  -xxl_ms input,.d
+00012540: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00012550: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00012560: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
+00012570: 6c64 2d6c 675f 6d65 2069 6e70 7574 2c2e  ld-lg_me input,.
+00012580: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00012590: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+000125a0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+000125b0: 656c 642d 6c67 5f6d 7320 696e 7075 742c  eld-lg_ms input,
+000125c0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+000125d0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+000125e0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
+000125f0: 6965 6c64 2d6d 645f 6d65 2069 6e70 7574  ield-md_me input
+00012600: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+00012610: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+00012620: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+00012630: 6669 656c 642d 6d64 5f6d 7320 696e 7075  field-md_ms inpu
+00012640: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+00012650: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00012660: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+00012670: 2e66 6965 6c64 2d73 6d5f 6d65 2069 6e70  .field-sm_me inp
+00012680: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+00012690: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+000126a0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+000126b0: 202e 6669 656c 642d 736d 5f6d 7320 696e   .field-sm_ms in
+000126c0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+000126d0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+000126e0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+000126f0: 6520 2e66 6965 6c64 2d78 6c5f 6d65 2069  e .field-xl_me i
+00012700: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+00012710: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+00012720: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+00012730: 6d65 202e 6669 656c 642d 786c 5f6d 7320  me .field-xl_ms 
+00012740: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+00012750: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00012760: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00012770: 5f6d 6520 2e66 6965 6c64 2d78 735f 6d65  _me .field-xs_me
+00012780: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+00012790: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+000127a0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+000127b0: 735f 6d65 202e 6669 656c 642d 7873 5f6d  s_me .field-xs_m
+000127c0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+000127d0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+000127e0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+000127f0: 7873 5f6d 6520 2e66 6965 6c64 2d78 786c  xs_me .field-xxl
+00012800: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
+00012810: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+00012820: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+00012830: 642d 7873 5f6d 6520 2e66 6965 6c64 2d78  d-xs_me .field-x
+00012840: 786c 5f6d 7320 696e 7075 742c 2e64 6a61  xl_ms input,.dja
+00012850: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00012860: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00012870: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
+00012880: 2d6c 675f 6d65 2069 6e70 7574 2c2e 646a  -lg_me input,.dj
+00012890: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+000128a0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+000128b0: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
+000128c0: 642d 6c67 5f6d 7320 696e 7075 742c 2e64  d-lg_ms input,.d
+000128d0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+000128e0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+000128f0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+00012900: 6c64 2d6d 645f 6d65 2069 6e70 7574 2c2e  ld-md_me input,.
+00012910: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00012920: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+00012930: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+00012940: 656c 642d 6d64 5f6d 7320 696e 7075 742c  eld-md_ms input,
+00012950: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00012960: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00012970: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
+00012980: 6965 6c64 2d73 6d5f 6d65 2069 6e70 7574  ield-sm_me input
+00012990: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+000129a0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+000129b0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+000129c0: 6669 656c 642d 736d 5f6d 7320 696e 7075  field-sm_ms inpu
+000129d0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+000129e0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+000129f0: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+00012a00: 2e66 6965 6c64 2d78 6c5f 6d65 2069 6e70  .field-xl_me inp
+00012a10: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+00012a20: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+00012a30: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+00012a40: 202e 6669 656c 642d 786c 5f6d 7320 696e   .field-xl_ms in
+00012a50: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00012a60: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00012a70: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+00012a80: 7320 2e66 6965 6c64 2d78 735f 6d65 2069  s .field-xs_me i
+00012a90: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+00012aa0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+00012ab0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+00012ac0: 6d73 202e 6669 656c 642d 7873 5f6d 7320  ms .field-xs_ms 
+00012ad0: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+00012ae0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+00012af0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+00012b00: 5f6d 7320 2e66 6965 6c64 2d78 786c 5f6d  _ms .field-xxl_m
+00012b10: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
+00012b20: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+00012b30: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00012b40: 7873 5f6d 7320 2e66 6965 6c64 2d78 786c  xs_ms .field-xxl
+00012b50: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
+00012b60: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+00012b70: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+00012b80: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
+00012b90: 6c64 2d6c 675f 6d65 2069 6e70 7574 2c2e  ld-lg_me input,.
+00012ba0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00012bb0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+00012bc0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+00012bd0: 202e 6669 656c 642d 6c67 5f6d 7320 696e   .field-lg_ms in
+00012be0: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00012bf0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00012c00: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+00012c10: 6666 7365 7420 2e66 6965 6c64 2d6d 645f  ffset .field-md_
+00012c20: 6d65 2069 6e70 7574 2c2e 646a 616e 676f  me input,.django
+00012c30: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+00012c40: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+00012c50: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+00012c60: 642d 6d64 5f6d 7320 696e 7075 742c 2e64  d-md_ms input,.d
+00012c70: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00012c80: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+00012c90: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
+00012ca0: 2e66 6965 6c64 2d73 6d5f 6d65 2069 6e70  .field-sm_me inp
+00012cb0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+00012cc0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+00012cd0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
+00012ce0: 6673 6574 202e 6669 656c 642d 736d 5f6d  fset .field-sm_m
+00012cf0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00012d00: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+00012d10: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00012d20: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+00012d30: 2d78 6c5f 6d65 2069 6e70 7574 2c2e 646a  -xl_me input,.dj
+00012d40: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+00012d50: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+00012d60: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
+00012d70: 6669 656c 642d 786c 5f6d 7320 696e 7075  field-xl_ms inpu
+00012d80: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+00012d90: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00012da0: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+00012db0: 7365 7420 2e66 6965 6c64 2d78 735f 6d65  set .field-xs_me
+00012dc0: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+00012dd0: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+00012de0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+00012df0: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+00012e00: 7873 5f6d 7320 696e 7075 742c 2e64 6a61  xs_ms input,.dja
+00012e10: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00012e20: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00012e30: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
+00012e40: 6965 6c64 2d78 786c 5f6d 6520 696e 7075  ield-xxl_me inpu
+00012e50: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+00012e60: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+00012e70: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+00012e80: 7365 7420 2e66 6965 6c64 2d78 786c 5f6d  set .field-xxl_m
+00012e90: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00012ea0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+00012eb0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00012ec0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+00012ed0: 6c67 5f6d 6520 696e 7075 742c 2e64 6a61  lg_me input,.dja
+00012ee0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00012ef0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00012f00: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+00012f10: 656c 642d 6c67 5f6d 7320 696e 7075 742c  eld-lg_ms input,
+00012f20: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00012f30: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00012f40: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+00012f50: 202e 6669 656c 642d 6d64 5f6d 6520 696e   .field-md_me in
+00012f60: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00012f70: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00012f80: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+00012f90: 7264 6572 202e 6669 656c 642d 6d64 5f6d  rder .field-md_m
+00012fa0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+00012fb0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+00012fc0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00012fd0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+00012fe0: 736d 5f6d 6520 696e 7075 742c 2e64 6a61  sm_me input,.dja
+00012ff0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00013000: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00013010: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+00013020: 656c 642d 736d 5f6d 7320 696e 7075 742c  eld-sm_ms input,
+00013030: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00013040: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00013050: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+00013060: 202e 6669 656c 642d 786c 5f6d 6520 696e   .field-xl_me in
+00013070: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+00013080: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+00013090: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+000130a0: 7264 6572 202e 6669 656c 642d 786c 5f6d  rder .field-xl_m
+000130b0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
+000130c0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+000130d0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+000130e0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+000130f0: 7873 5f6d 6520 696e 7075 742c 2e64 6a61  xs_me input,.dja
+00013100: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+00013110: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+00013120: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+00013130: 656c 642d 7873 5f6d 7320 696e 7075 742c  eld-xs_ms input,
+00013140: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00013150: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+00013160: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+00013170: 202e 6669 656c 642d 7878 6c5f 6d65 2069   .field-xxl_me i
+00013180: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+00013190: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+000131a0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+000131b0: 6f72 6465 7220 2e66 6965 6c64 2d78 786c  order .field-xxl
+000131c0: 5f6d 7320 696e 7075 747b 706f 7369 7469  _ms input{positi
+000131d0: 6f6e 3a72 656c 6174 6976 653b 626f 782d  on:relative;box-
+000131e0: 7369 7a69 6e67 3a62 6f72 6465 722d 626f  sizing:border-bo
+000131f0: 783b 746f 703a 2d33 7078 7d2e 646a 616e  x;top:-3px}.djan
+00013200: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+00013210: 6f6c 756d 6e20 2e67 7269 642d 7265 7365  olumn .grid-rese
+00013220: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+00013230: 6e74 656e 642d 726f 7720 2e67 7269 642d  ntend-row .grid-
+00013240: 7265 7365 747b 706f 7369 7469 6f6e 3a61  reset{position:a
+00013250: 6273 6f6c 7574 653b 7269 6768 743a 3570  bsolute;right:5p
+00013260: 783b 746f 703a 307d 2e64 6a61 6e67 6f63  x;top:0}.djangoc
+00013270: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+00013280: 6d6e 202e 6963 6f6e 2d74 6865 6164 2c2e  mn .icon-thead,.
+00013290: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+000132a0: 6e64 2d72 6f77 202e 6963 6f6e 2d74 6865  nd-row .icon-the
+000132b0: 6164 7b74 6578 742d 616c 6967 6e3a 6365  ad{text-align:ce
+000132c0: 6e74 6572 3b6d 6172 6769 6e2d 626f 7474  nter;margin-bott
+000132d0: 6f6d 3a31 3570 787d 2e64 6a61 6e67 6f63  om:15px}.djangoc
+000132e0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+000132f0: 6d6e 202e 6963 6f6e 2d74 6865 6164 202e  mn .icon-thead .
+00013300: 6963 6f6e 2c2e 646a 616e 676f 636d 732d  icon,.djangocms-
+00013310: 6672 6f6e 7465 6e64 2d72 6f77 202e 6963  frontend-row .ic
+00013320: 6f6e 2d74 6865 6164 202e 6963 6f6e 7b66  on-thead .icon{f
+00013330: 6f6e 742d 7369 7a65 3a33 3070 787d 2e64  ont-size:30px}.d
+00013340: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+00013350: 642d 636f 6c75 6d6e 202e 6963 6f6e 2d74  d-column .icon-t
+00013360: 6865 6164 202e 6963 6f6e 2d73 697a 652d  head .icon-size-
+00013370: 736d 2c2e 646a 616e 676f 636d 732d 6672  sm,.djangocms-fr
+00013380: 6f6e 7465 6e64 2d72 6f77 202e 6963 6f6e  ontend-row .icon
+00013390: 2d74 6865 6164 202e 6963 6f6e 2d73 697a  -thead .icon-siz
+000133a0: 652d 736d 7b74 7261 6e73 666f 726d 3a72  e-sm{transform:r
+000133b0: 6f74 6174 6528 3930 6465 6729 7d2e 646a  otate(90deg)}.dj
+000133c0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+000133d0: 2d63 6f6c 756d 6e20 2e69 636f 6e2d 7469  -column .icon-ti
+000133e0: 746c 652c 2e64 6a61 6e67 6f63 6d73 2d66  tle,.djangocms-f
+000133f0: 726f 6e74 656e 642d 726f 7720 2e69 636f  rontend-row .ico
+00013400: 6e2d 7469 746c 657b 6469 7370 6c61 793a  n-title{display:
+00013410: 626c 6f63 6b3b 666f 6e74 2d73 697a 653a  block;font-size:
+00013420: 3132 7078 3b63 6f6c 6f72 3a23 3939 393b  12px;color:#999;
+00013430: 7061 6464 696e 673a 3570 7820 3020 307d  padding:5px 0 0}
+00013440: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+00013450: 656e 642d 7072 6576 6965 777b 706f 7369  end-preview{posi
+00013460: 7469 6f6e 3a66 6978 6564 3b74 6f70 3a30  tion:fixed;top:0
+00013470: 3b72 6967 6874 3a30 3b7a 2d69 6e64 6578  ;right:0;z-index
+00013480: 3a31 303b 7465 7874 2d61 6c69 676e 3a63  :10;text-align:c
+00013490: 656e 7465 723b 626f 7264 6572 2d72 6164  enter;border-rad
+000134a0: 6975 733a 3020 3020 3020 3370 783b 7061  ius:0 0 0 3px;pa
+000134b0: 6464 696e 673a 3130 7078 2032 3070 7820  dding:10px 20px 
+000134c0: 3237 7078 3b62 6f72 6465 723a 3170 7820  27px;border:1px 
+000134d0: 736f 6c69 6420 7661 7228 2d2d 6463 612d  solid var(--dca-
+000134e0: 6772 6179 2c76 6172 282d 2d68 6169 726c  gray,var(--hairl
+000134f0: 696e 652d 636f 6c6f 722c 2363 6363 2929  ine-color,#ccc))
+00013500: 3b62 6f72 6465 722d 746f 703a 6e6f 6e65  ;border-top:none
+00013510: 3b62 6f72 6465 722d 7269 6768 743a 6e6f  ;border-right:no
+00013520: 6e65 3b62 6163 6b67 726f 756e 643a 7661  ne;background:va
+00013530: 7228 2d2d 626f 6479 2d62 672c 2366 6666  r(--body-bg,#fff
+00013540: 297d 406d 6564 6961 2028 7072 6566 6572  )}@media (prefer
+00013550: 732d 636f 6c6f 722d 7363 6865 6d65 3a64  s-color-scheme:d
+00013560: 6172 6b29 7b2e 646a 616e 676f 636d 732d  ark){.djangocms-
+00013570: 6672 6f6e 7465 6e64 2d70 7265 7669 6577  frontend-preview
+00013580: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
+00013590: 2d2d 626f 6479 2d62 672c 2330 3030 297d  --body-bg,#000)}
+000135a0: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
+000135b0: 7465 6e64 2d70 7265 7669 6577 2068 327b  tend-preview h2{
+000135c0: 666f 6e74 2d73 697a 653a 3134 7078 3b6d  font-size:14px;m
+000135d0: 696e 2d77 6964 7468 3a31 3530 7078 3b6d  in-width:150px;m
+000135e0: 6172 6769 6e3a 3020 3020 3132 7078 7d2e  argin:0 0 12px}.
+000135f0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+00013600: 6e64 2d70 7265 7669 6577 202e 6234 2d70  nd-preview .b4-p
+00013610: 7265 7669 6577 7b6d 6172 6769 6e3a 3020  review{margin:0 
+00013620: 3020 2d31 3570 787d 2e64 6a61 6e67 6f63  0 -15px}.djangoc
+00013630: 6d73 2d66 726f 6e74 656e 642d 7072 6576  ms-frontend-prev
+00013640: 6965 7720 2e62 342d 636c 6f73 657b 706f  iew .b4-close{po
+00013650: 7369 7469 6f6e 3a61 6273 6f6c 7574 653b  sition:absolute;
+00013660: 7269 6768 743a 3130 7078 3b74 6f70 3a38  right:10px;top:8
+00013670: 7078 3b7a 2d69 6e64 6578 3a31 3030 3b64  px;z-index:100;d
+00013680: 6973 706c 6179 3a62 6c6f 636b 3b63 6f6c  isplay:block;col
+00013690: 6f72 3a23 3565 3565 3565 3b66 6f6e 742d  or:#5e5e5e;font-
+000136a0: 7369 7a65 3a31 3270 783b 6c69 6e65 2d68  size:12px;line-h
+000136b0: 6569 6768 743a 3230 7078 3b66 6f6e 742d  eight:20px;font-
+000136c0: 7765 6967 6874 3a37 3030 3b74 6578 742d  weight:700;text-
+000136d0: 7472 616e 7366 6f72 6d3a 7570 7065 7263  transform:upperc
+000136e0: 6173 653b 7769 6474 683a 3230 7078 3b68  ase;width:20px;h
+000136f0: 6569 6768 743a 3230 7078 3b62 6f72 6465  eight:20px;borde
+00013700: 722d 7261 6469 7573 3a33 7078 3b62 6163  r-radius:3px;bac
+00013710: 6b67 726f 756e 643a 2364 6464 7d2e 646a  kground:#ddd}.dj
+00013720: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+00013730: 2d70 7265 7669 6577 202e 6234 2d63 6c6f  -preview .b4-clo
+00013740: 7365 3a68 6f76 6572 7b63 6f6c 6f72 3a23  se:hover{color:#
+00013750: 6666 6621 696d 706f 7274 616e 743b 7465  fff!important;te
+00013760: 7874 2d64 6563 6f72 6174 696f 6e3a 6e6f  xt-decoration:no
+00013770: 6e65 3b62 6163 6b67 726f 756e 643a 2330  ne;background:#0
+00013780: 6266 7d2e 646a 616e 676f 636d 732d 6672  bf}.djangocms-fr
+00013790: 6f6e 7465 6e64 2d70 7265 7669 6577 202e  ontend-preview .
+000137a0: 6274 6e3e 7370 616e 7b76 6572 7469 6361  btn>span{vertica
+000137b0: 6c2d 616c 6967 6e3a 6d69 6464 6c65 7d2e  l-align:middle}.
+000137c0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+000137d0: 6e64 2d70 7265 7669 6577 202e 6274 6e3e  nd-preview .btn>
+000137e0: 7370 616e 3e2e 6963 6f6e 7b76 6572 7469  span>.icon{verti
+000137f0: 6361 6c2d 616c 6967 6e3a 6d69 6464 6c65  cal-align:middle
+00013800: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
+00013810: 7465 6e64 2d70 7265 7669 6577 202e 6274  tend-preview .bt
+00013820: 6e3e 7370 616e 2073 7667 2c2e 646a 616e  n>span svg,.djan
+00013830: 676f 636d 732d 6672 6f6e 7465 6e64 2d70  gocms-frontend-p
+00013840: 7265 7669 6577 202e 6274 6e3e 7370 616e  review .btn>span
+00013850: 2075 7365 7b66 696c 6c3a 6375 7272 656e   use{fill:curren
+00013860: 7443 6f6c 6f72 7d2e 646a 616e 676f 636d  tColor}.djangocm
+00013870: 732d 6672 6f6e 7465 6e64 2d62 6c6f 636b  s-frontend-block
+00013880: 7175 6f74 6520 7465 7874 6172 6561 7b68  quote textarea{h
+00013890: 6569 6768 743a 3131 3070 787d 2369 645f  eight:110px}#id_
+000138a0: 6c69 6e6b 5f74 7970 657b 7061 6464 696e  link_type{paddin
+000138b0: 673a 303b 6d61 7267 696e 3a30 3b62 6f72  g:0;margin:0;bor
+000138c0: 6465 723a 6e6f 6e65 7d23 6964 5f6c 696e  der:none}#id_lin
+000138d0: 6b5f 7479 7065 206c 697b 7061 6464 696e  k_type li{paddin
+000138e0: 673a 303b 6d61 7267 696e 3a30 2031 3570  g:0;margin:0 15p
+000138f0: 7820 3570 7820 303b 626f 7264 6572 3a6e  x 5px 0;border:n
+00013900: 6f6e 657d 2369 645f 6c69 6e6b 5f74 7970  one}#id_link_typ
+00013910: 6520 6c61 6265 6c20 696e 7075 747b 706f  e label input{po
+00013920: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
+00013930: 746f 703a 2d34 7078 7d61 5b64 6174 612d  top:-4px}a[data-
+00013940: 706b 5d7b 706f 7369 7469 6f6e 3a72 656c  pk]{position:rel
+00013950: 6174 6976 657d 615b 6461 7461 2d70 6b5d  ative}a[data-pk]
+00013960: 3a61 6674 6572 7b63 6f6e 7465 6e74 3a61  :after{content:a
+00013970: 7474 7228 6461 7461 2d70 6b29 3b76 6973  ttr(data-pk);vis
+00013980: 6962 696c 6974 793a 6869 6464 656e 3b77  ibility:hidden;w
+00013990: 6964 7468 3a61 7574 6f3b 666f 6e74 2d77  idth:auto;font-w
+000139a0: 6569 6768 743a 3430 303b 666f 6e74 2d73  eight:400;font-s
+000139b0: 697a 653a 3830 253b 6261 636b 6772 6f75  ize:80%;backgrou
+000139c0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d64  nd-color:var(--d
+000139d0: 6361 2d77 6869 7465 2c76 6172 282d 2d62  ca-white,var(--b
+000139e0: 6f64 792d 6267 2c23 6666 6629 293b 636f  ody-bg,#fff));co
+000139f0: 6c6f 723a 7661 7228 2d2d 6463 612d 6772  lor:var(--dca-gr
+00013a00: 6179 2c76 6172 282d 2d62 6f64 792d 6667  ay,var(--body-fg
+00013a10: 2c23 3333 3329 293b 626f 7264 6572 3a73  ,#333));border:s
+00013a20: 6f6c 6964 2031 7078 2076 6172 282d 2d64  olid 1px var(--d
+00013a30: 6361 2d67 7261 792c 7661 7228 2d2d 626f  ca-gray,var(--bo
+00013a40: 6479 2d66 672c 2333 3333 2929 3b74 6578  dy-fg,#333));tex
+00013a50: 742d 616c 6967 6e3a 6365 6e74 6572 3b70  t-align:center;p
+00013a60: 6164 6469 6e67 3a35 7078 2031 3070 783b  adding:5px 10px;
+00013a70: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
+00013a80: 653b 7a2d 696e 6465 783a 313b 746f 703a  e;z-index:1;top:
+00013a90: 3131 3025 3b6c 6566 743a 3530 253b 6d61  110%;left:50%;ma
+00013aa0: 7267 696e 2d6c 6566 743a 2d35 3025 7d61  rgin-left:-50%}a
+00013ab0: 5b64 6174 612d 706b 5d3a 686f 7665 723a  [data-pk]:hover:
+00013ac0: 6166 7465 727b 7669 7369 6269 6c69 7479  after{visibility
+00013ad0: 3a76 6973 6962 6c65 7d2e 646a 616e 676f  :visible}.django
+00013ae0: 636d 732d 6164 6d69 6e2d 7374 796c 6520  cms-admin-style 
+00013af0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+00013b00: 706c 7567 696e 5f74 6974 6c65 2069 6e70  plugin_title inp
+00013b10: 7574 5b6e 616d 653d 706c 7567 696e 5f74  ut[name=plugin_t
+00013b20: 6974 6c65 5f30 5d7b 6d61 7267 696e 2d62  itle_0]{margin-b
+00013b30: 6f74 746f 6d3a 2e35 656d 2169 6d70 6f72  ottom:.5em!impor
+00013b40: 7461 6e74 7d2e 646a 616e 676f 636d 732d  tant}.djangocms-
+00013b50: 6164 6d69 6e2d 7374 796c 6520 2e66 6f72  admin-style .for
+00013b60: 6d2d 726f 772e 6669 656c 642d 706c 7567  m-row.field-plug
+00013b70: 696e 5f74 6974 6c65 2069 6e70 7574 5b6e  in_title input[n
+00013b80: 616d 653d 706c 7567 696e 5f74 6974 6c65  ame=plugin_title
+00013b90: 5f31 5d7b 7769 6474 683a 6361 6c63 2831  _1]{width:calc(1
+00013ba0: 3030 2520 2d20 3265 6d29 2169 6d70 6f72  00% - 2em)!impor
+00013bb0: 7461 6e74 7d62 6f64 793a 6e6f 7428 2e64  tant}body:not(.d
+00013bc0: 6a61 6e67 6f63 6d73 2d61 646d 696e 2d73  jangocms-admin-s
+00013bd0: 7479 6c65 2920 2e66 6f72 6d2d 726f 772e  tyle) .form-row.
+00013be0: 6669 656c 642d 706c 7567 696e 5f74 6974  field-plugin_tit
+00013bf0: 6c65 2069 6e70 7574 5b6e 616d 653d 706c  le input[name=pl
+00013c00: 7567 696e 5f74 6974 6c65 5f31 5d7b 7769  ugin_title_1]{wi
+00013c10: 6474 683a 6361 6c63 2831 3030 2520 2d20  dth:calc(100% - 
+00013c20: 3230 3070 7820 2d20 3165 6d29 2169 6d70  200px - 1em)!imp
+00013c30: 6f72 7461 6e74 3b6d 6172 6769 6e2d 6c65  ortant;margin-le
+00013c40: 6674 3a31 656d 7d2e 6672 6f6e 7465 6e64  ft:1em}.frontend
+00013c50: 2d69 636f 6e2d 7069 636b 6572 7b74 6578  -icon-picker{tex
+00013c60: 742d 616c 6967 6e3a 6365 6e74 6572 3b64  t-align:center;d
+00013c70: 6973 706c 6179 3a69 6e6c 696e 652d 626c  isplay:inline-bl
+00013c80: 6f63 6b7d 2e66 726f 6e74 656e 642d 6963  ock}.frontend-ic
+00013c90: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
+00013ca0: 636f 6e74 6169 6e65 727b 706f 7369 7469  container{positi
+00013cb0: 6f6e 3a72 656c 6174 6976 653b 6d61 7267  on:relative;marg
+00013cc0: 696e 2d62 6f74 746f 6d3a 2e35 656d 3b6d  in-bottom:.5em;m
+00013cd0: 6172 6769 6e2d 6c65 6674 3a61 7574 6f3b  argin-left:auto;
+00013ce0: 6d61 7267 696e 2d72 6967 6874 3a61 7574  margin-right:aut
+00013cf0: 6f3b 7769 6474 683a 3765 6d3b 6865 6967  o;width:7em;heig
+00013d00: 6874 3a37 656d 3b62 6f72 6465 723a 3170  ht:7em;border:1p
+00013d10: 7820 7661 7228 2d2d 6463 612d 6772 6179  x var(--dca-gray
+00013d20: 2d6c 6967 6874 2c76 6172 282d 2d62 6f72  -light,var(--bor
+00013d30: 6465 722d 636f 6c6f 722c 2364 3364 3364  der-color,#d3d3d
+00013d40: 3329 2920 736f 6c69 643b 7472 616e 7369  3)) solid;transi
+00013d50: 7469 6f6e 3a62 6163 6b67 726f 756e 642d  tion:background-
+00013d60: 636f 6c6f 7220 2e31 3573 2c63 6f6c 6f72  color .15s,color
+00013d70: 202e 3135 737d 2e66 726f 6e74 656e 642d   .15s}.frontend-
+00013d80: 6963 6f6e 2d70 6963 6b65 7220 2e69 636f  icon-picker .ico
+00013d90: 6e2d 636f 6e74 6169 6e65 7220 2e69 636f  n-container .ico
+00013da0: 6e2d 7072 6576 6965 777b 7769 6474 683a  n-preview{width:
+00013db0: 3765 6d3b 6865 6967 6874 3a37 656d 3b64  7em;height:7em;d
+00013dc0: 6973 706c 6179 3a2d 6d73 2d66 6c65 7862  isplay:-ms-flexb
+00013dd0: 6f78 3b64 6973 706c 6179 3a66 6c65 783b  ox;display:flex;
+00013de0: 2d6d 732d 666c 6578 2d64 6972 6563 7469  -ms-flex-directi
+00013df0: 6f6e 3a63 6f6c 756d 6e3b 666c 6578 2d64  on:column;flex-d
+00013e00: 6972 6563 7469 6f6e 3a63 6f6c 756d 6e3b  irection:column;
+00013e10: 2d6d 732d 666c 6578 2d70 6163 6b3a 6365  -ms-flex-pack:ce
+00013e20: 6e74 6572 3b6a 7573 7469 6679 2d63 6f6e  nter;justify-con
+00013e30: 7465 6e74 3a63 656e 7465 727d 2e66 726f  tent:center}.fro
+00013e40: 6e74 656e 642d 6963 6f6e 2d70 6963 6b65  ntend-icon-picke
+00013e50: 7220 2e69 636f 6e2d 636f 6e74 6169 6e65  r .icon-containe
+00013e60: 7220 2e69 636f 6e2d 7072 6576 6965 7720  r .icon-preview 
+00013e70: 2e69 636f 6e2d 626f 787b 666f 6e74 2d73  .icon-box{font-s
+00013e80: 697a 653a 3530 3025 3b6c 696e 652d 6865  ize:500%;line-he
+00013e90: 6967 6874 3a31 2e33 3b6d 6172 6769 6e3a  ight:1.3;margin:
+00013ea0: 303b 7465 7874 2d61 6c69 676e 3a63 656e  0;text-align:cen
+00013eb0: 7465 727d 2e66 726f 6e74 656e 642d 6963  ter}.frontend-ic
+00013ec0: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
+00013ed0: 636f 6e74 6169 6e65 7220 2e69 636f 6e2d  container .icon-
+00013ee0: 7072 6576 6965 7720 2e69 636f 6e2d 626f  preview .icon-bo
+00013ef0: 7820 692c 2e66 726f 6e74 656e 642d 6963  x i,.frontend-ic
+00013f00: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
+00013f10: 636f 6e74 6169 6e65 7220 2e69 636f 6e2d  container .icon-
+00013f20: 7072 6576 6965 7720 2e69 636f 6e2d 626f  preview .icon-bo
+00013f30: 7820 7370 616e 7b66 6f6e 742d 7369 7a65  x span{font-size
+00013f40: 3a75 6e73 6574 7d2e 6672 6f6e 7465 6e64  :unset}.frontend
+00013f50: 2d69 636f 6e2d 7069 636b 6572 202e 6963  -icon-picker .ic
+00013f60: 6f6e 2d63 6f6e 7461 696e 6572 202e 6963  on-container .ic
+00013f70: 6f6e 2d70 7265 7669 6577 202e 656d 7074  on-preview .empt
+00013f80: 792d 626f 787b 7465 7874 2d61 6c69 676e  y-box{text-align
+00013f90: 3a63 656e 7465 723b 6f76 6572 666c 6f77  :center;overflow
+00013fa0: 3a68 6964 6465 6e3b 7465 7874 2d6f 7665  :hidden;text-ove
+00013fb0: 7266 6c6f 773a 656c 6c69 7073 6973 3b6c  rflow:ellipsis;l
+00013fc0: 696e 652d 6865 6967 6874 3a31 3b66 6f6e  ine-height:1;fon
+00013fd0: 742d 7369 7a65 3a31 3030 257d 2e66 726f  t-size:100%}.fro
+00013fe0: 6e74 656e 642d 6963 6f6e 2d70 6963 6b65  ntend-icon-picke
+00013ff0: 7220 2e69 636f 6e2d 636f 6e74 6169 6e65  r .icon-containe
+00014000: 7220 2e69 636f 6e2d 7072 6576 6965 7720  r .icon-preview 
+00014010: 2e65 6d70 7479 2d62 6f78 2e68 6964 6465  .empty-box.hidde
+00014020: 6e7b 6469 7370 6c61 793a 6e6f 6e65 7d2e  n{display:none}.
+00014030: 6672 6f6e 7465 6e64 2d69 636f 6e2d 7069  frontend-icon-pi
+00014040: 636b 6572 202e 6963 6f6e 2d63 6f6e 7461  cker .icon-conta
+00014050: 696e 6572 202e 6963 6f6e 2d70 7265 7669  iner .icon-previ
+00014060: 6577 3a68 6f76 6572 7b62 6163 6b67 726f  ew:hover{backgro
+00014070: 756e 643a 7661 7228 2d2d 6463 612d 6772  und:var(--dca-gr
+00014080: 6179 2d6c 6967 6874 2c76 6172 282d 2d62  ay-light,var(--b
+00014090: 6f72 6465 722d 636f 6c6f 722c 2364 3364  order-color,#d3d
+000140a0: 3364 3329 293b 6375 7273 6f72 3a70 6f69  3d3));cursor:poi
+000140b0: 6e74 6572 7d2e 6672 6f6e 7465 6e64 2d69  nter}.frontend-i
+000140c0: 636f 6e2d 7069 636b 6572 202e 6963 6f6e  con-picker .icon
+000140d0: 2d63 6f6e 7461 696e 6572 202e 6963 6f6e  -container .icon
+000140e0: 2d63 6c6f 7365 2d69 6e64 6963 6174 6f72  -close-indicator
+000140f0: 7b64 6973 706c 6179 3a62 6c6f 636b 3b62  {display:block;b
+00014100: 6f72 6465 722d 7261 6469 7573 3a35 3025  order-radius:50%
+00014110: 3b63 6f6c 6f72 3a76 6172 282d 2d64 6361  ;color:var(--dca
+00014120: 2d62 6c61 636b 2c76 6172 282d 2d62 6f64  -black,var(--bod
+00014130: 792d 6667 2c23 3030 3029 293b 6261 636b  y-fg,#000));back
+00014140: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+00014150: 282d 2d64 6361 2d77 6869 7465 2c76 6172  (--dca-white,var
+00014160: 282d 2d62 6f64 792d 6267 2c23 6666 6629  (--body-bg,#fff)
+00014170: 293b 7061 6464 696e 673a 2e35 7265 6d3b  );padding:.5rem;
+00014180: 626f 7264 6572 3a31 7078 2073 6f6c 6964  border:1px solid
+00014190: 2076 6172 282d 2d64 6361 2d62 6c61 636b   var(--dca-black
+000141a0: 2c76 6172 282d 2d62 6f64 792d 6667 2c23  ,var(--body-fg,#
+000141b0: 3030 3029 293b 7472 616e 7366 6f72 6d3a  000));transform:
+000141c0: 7472 616e 736c 6174 6528 2d35 3025 2c2d  translate(-50%,-
+000141d0: 3530 2529 3b74 6f70 3a30 3b6c 6566 743a  50%);top:0;left:
+000141e0: 3130 3025 3b77 6964 7468 3a2e 3665 6d3b  100%;width:.6em;
+000141f0: 6865 6967 6874 3a2e 3665 6d3b 6c69 6e65  height:.6em;line
+00014200: 2d68 6569 6768 743a 2e35 656d 3b70 6f73  -height:.5em;pos
+00014210: 6974 696f 6e3a 6162 736f 6c75 7465 3b74  ition:absolute;t
+00014220: 7261 6e73 6974 696f 6e3a 6261 636b 6772  ransition:backgr
+00014230: 6f75 6e64 2d63 6f6c 6f72 202e 3135 737d  ound-color .15s}
+00014240: 2e66 726f 6e74 656e 642d 6963 6f6e 2d70  .frontend-icon-p
+00014250: 6963 6b65 7220 2e69 636f 6e2d 636f 6e74  icker .icon-cont
+00014260: 6169 6e65 7220 2e69 636f 6e2d 636c 6f73  ainer .icon-clos
+00014270: 652d 696e 6469 6361 746f 723a 6265 666f  e-indicator:befo
+00014280: 7265 7b63 6f6e 7465 6e74 3a22 c397 227d  re{content:".."}
+00014290: 2e66 726f 6e74 656e 642d 6963 6f6e 2d70  .frontend-icon-p
+000142a0: 6963 6b65 7220 2e69 636f 6e2d 636f 6e74  icker .icon-cont
+000142b0: 6169 6e65 7220 2e69 636f 6e2d 636c 6f73  ainer .icon-clos
+000142c0: 652d 696e 6469 6361 746f 723a 686f 7665  e-indicator:hove
+000142d0: 727b 6261 636b 6772 6f75 6e64 3a76 6172  r{background:var
+000142e0: 282d 2d64 656c 6574 652d 6275 7474 6f6e  (--delete-button
+000142f0: 2d62 672c 7265 6429 3b63 6f6c 6f72 3a76  -bg,red);color:v
+00014300: 6172 282d 2d64 656c 6574 652d 6275 7474  ar(--delete-butt
+00014310: 6f6e 2d66 672c 2366 6666 293b 6375 7273  on-fg,#fff);curs
+00014320: 6f72 3a70 6f69 6e74 6572 7d2e 7569 702d  or:pointer}.uip-
+00014330: 6d6f 6461 6c7b 706f 7369 7469 6f6e 3a66  modal{position:f
+00014340: 6978 6564 3b68 6569 6768 743a 3130 3025  ixed;height:100%
+00014350: 3b77 6964 7468 3a31 3030 253b 626f 7474  ;width:100%;bott
+00014360: 6f6d 3a30 3b6c 6566 743a 303b 6261 636b  om:0;left:0;back
+00014370: 6772 6f75 6e64 2d63 6f6c 6f72 3a72 6762  ground-color:rgb
+00014380: 6128 302c 302c 302c 2e38 293b 7a2d 696e  a(0,0,0,.8);z-in
+00014390: 6465 783a 3939 3939 3b2d 7765 626b 6974  dex:9999;-webkit
+000143a0: 2d75 7365 722d 7365 6c65 6374 3a6e 6f6e  -user-select:non
+000143b0: 653b 2d6d 732d 7573 6572 2d73 656c 6563  e;-ms-user-selec
+000143c0: 743a 6e6f 6e65 3b75 7365 722d 7365 6c65  t:none;user-sele
+000143d0: 6374 3a6e 6f6e 653b 6469 7370 6c61 793a  ct:none;display:
+000143e0: 2d6d 732d 666c 6578 626f 783b 6469 7370  -ms-flexbox;disp
+000143f0: 6c61 793a 666c 6578 3b2d 6d73 2d66 6c65  lay:flex;-ms-fle
+00014400: 782d 616c 6967 6e3a 6365 6e74 6572 3b61  x-align:center;a
+00014410: 6c69 676e 2d69 7465 6d73 3a63 656e 7465  lign-items:cente
+00014420: 727d 2e75 6970 2d6d 6f64 616c 202a 2c2e  r}.uip-modal *,.
+00014430: 7569 702d 6d6f 6461 6c20 3a61 6674 6572  uip-modal :after
+00014440: 2c2e 7569 702d 6d6f 6461 6c20 3a62 6566  ,.uip-modal :bef
+00014450: 6f72 657b 626f 782d 7369 7a69 6e67 3a62  ore{box-sizing:b
+00014460: 6f72 6465 722d 626f 787d 2e75 6970 2d6d  order-box}.uip-m
+00014470: 6f64 616c 2e75 6970 2d63 6c6f 7365 7b6f  odal.uip-close{o
+00014480: 7061 6369 7479 3a30 3b76 6973 6962 696c  pacity:0;visibil
+00014490: 6974 793a 6869 6464 656e 3b74 7261 6e73  ity:hidden;trans
+000144a0: 6974 696f 6e3a 616c 6c20 2e34 7320 6561  ition:all .4s ea
+000144b0: 7365 2d69 6e2d 6f75 747d 2e75 6970 2d6d  se-in-out}.uip-m
+000144c0: 6f64 616c 2e75 6970 2d6f 7065 6e7b 6f70  odal.uip-open{op
+000144d0: 6163 6974 793a 313b 7669 7369 6269 6c69  acity:1;visibili
+000144e0: 7479 3a76 6973 6962 6c65 3b74 7261 6e73  ty:visible;trans
+000144f0: 6974 696f 6e3a 616c 6c20 2e34 7320 6561  ition:all .4s ea
+00014500: 7365 2d69 6e2d 6f75 747d 2e75 6970 2d6d  se-in-out}.uip-m
+00014510: 6f64 616c 202e 7569 702d 6d6f 6461 6c2d  odal .uip-modal-
+00014520: 2d63 6f6e 7465 6e74 7b70 6f73 6974 696f  -content{positio
+00014530: 6e3a 6162 736f 6c75 7465 3b62 6f72 6465  n:absolute;borde
+00014540: 722d 7261 6469 7573 3a33 7078 3b62 6f78  r-radius:3px;box
+00014550: 2d73 6861 646f 773a 3270 7820 3870 7820  -shadow:2px 8px 
+00014560: 3233 7078 2033 7078 2072 6762 6128 302c  23px 3px rgba(0,
+00014570: 302c 302c 2e32 293b 6f76 6572 666c 6f77  0,0,.2);overflow
+00014580: 3a68 6964 6465 6e3b 666f 6e74 2d66 616d  :hidden;font-fam
+00014590: 696c 793a 526f 626f 746f 2c41 7269 616c  ily:Roboto,Arial
+000145a0: 2c48 656c 7665 7469 6361 2c56 6572 6461  ,Helvetica,Verda
+000145b0: 6e61 2c73 616e 732d 7365 7269 663b 6261  na,sans-serif;ba
+000145c0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+000145d0: 6172 282d 2d64 6361 2d67 7261 792d 6c69  ar(--dca-gray-li
+000145e0: 6768 7465 7374 2c76 6172 282d 2d64 6172  ghtest,var(--dar
+000145f0: 6b65 6e65 642d 6267 2c23 6638 6638 6638  kened-bg,#f8f8f8
+00014600: 2929 3b77 6964 7468 3a31 3030 253b 6d61  ));width:100%;ma
+00014610: 7267 696e 3a61 7574 6f3b 6c65 6674 3a30  rgin:auto;left:0
+00014620: 3b72 6967 6874 3a30 3b6d 6172 6769 6e2d  ;right:0;margin-
+00014630: 626f 7474 6f6d 3a32 656d 7d2e 7569 702d  bottom:2em}.uip-
+00014640: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
+00014650: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
+00014660: 6f64 616c 2d2d 6865 6164 6572 7b70 6164  odal--header{pad
+00014670: 6469 6e67 3a31 3570 7820 3135 7078 3b62  ding:15px 15px;b
+00014680: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00014690: 7661 7228 2d2d 6463 612d 7768 6974 652c  var(--dca-white,
+000146a0: 7661 7228 2d2d 6267 2d63 6f6c 6f72 2c23  var(--bg-color,#
+000146b0: 6666 6629 293b 626f 782d 7368 6164 6f77  fff));box-shadow
+000146c0: 3a30 2030 2038 7078 2072 6762 6128 302c  :0 0 8px rgba(0,
+000146d0: 302c 302c 2e31 293b 706f 7369 7469 6f6e  0,0,.1);position
+000146e0: 3a72 656c 6174 6976 653b 7a2d 696e 6465  :relative;z-inde
+000146f0: 783a 313b 666f 6e74 2d73 697a 653a 3135  x:1;font-size:15
+00014700: 7078 3b63 6f6c 6f72 3a76 6172 282d 2d64  px;color:var(--d
+00014710: 6361 2d67 7261 792c 7661 7228 2d2d 626f  ca-gray,var(--bo
+00014720: 6479 2d71 7569 6574 2d63 6f6c 6f72 2c23  dy-quiet-color,#
+00014730: 3636 3629 293b 666f 6e74 2d77 6569 6768  666));font-weigh
+00014740: 743a 3530 303b 6469 7370 6c61 793a 2d6d  t:500;display:-m
+00014750: 732d 666c 6578 626f 783b 6469 7370 6c61  s-flexbox;displa
+00014760: 793a 666c 6578 3b2d 6d73 2d66 6c65 782d  y:flex;-ms-flex-
+00014770: 616c 6967 6e3a 6365 6e74 6572 3b61 6c69  align:center;ali
+00014780: 676e 2d69 7465 6d73 3a63 656e 7465 723b  gn-items:center;
+00014790: 2d6d 732d 666c 6578 2d70 6163 6b3a 6a75  -ms-flex-pack:ju
+000147a0: 7374 6966 793b 6a75 7374 6966 792d 636f  stify;justify-co
+000147b0: 6e74 656e 743a 7370 6163 652d 6265 7477  ntent:space-betw
+000147c0: 6565 6e7d 2e75 6970 2d6d 6f64 616c 202e  een}.uip-modal .
+000147d0: 7569 702d 6d6f 6461 6c2d 2d63 6f6e 7465  uip-modal--conte
+000147e0: 6e74 202e 7569 702d 6d6f 6461 6c2d 2d68  nt .uip-modal--h
+000147f0: 6561 6465 7220 2e75 6970 2d6d 6f64 616c  eader .uip-modal
+00014800: 2d2d 6865 6164 6572 2d6c 6f67 6f2d 7469  --header-logo-ti
+00014810: 746c 657b 7061 6464 696e 672d 746f 703a  tle{padding-top:
+00014820: 3270 783b 6c69 6e65 2d68 6569 6768 743a  2px;line-height:
+00014830: 313b 7465 7874 2d74 7261 6e73 666f 726d  1;text-transform
+00014840: 3a75 7070 6572 6361 7365 3b66 6f6e 742d  :uppercase;font-
+00014850: 7765 6967 6874 3a37 3030 3b63 7572 736f  weight:700;curso
+00014860: 723a 706f 696e 7465 727d 2e75 6970 2d6d  r:pointer}.uip-m
+00014870: 6f64 616c 202e 7569 702d 6d6f 6461 6c2d  odal .uip-modal-
+00014880: 2d63 6f6e 7465 6e74 202e 7569 702d 6d6f  -content .uip-mo
+00014890: 6461 6c2d 2d68 6561 6465 7220 2e75 6970  dal--header .uip
+000148a0: 2d6d 6f64 616c 2d2d 6865 6164 6572 2d63  -modal--header-c
+000148b0: 6c6f 7365 2d62 746e 7b63 7572 736f 723a  lose-btn{cursor:
+000148c0: 706f 696e 7465 727d 2e75 6970 2d6d 6f64  pointer}.uip-mod
+000148d0: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
+000148e0: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
+000148f0: 6c2d 2d62 6f64 797b 666f 6e74 2d73 697a  l--body{font-siz
+00014900: 653a 3132 7078 3b6c 696e 652d 6865 6967  e:12px;line-heig
+00014910: 6874 3a31 2e35 3b62 6f78 2d73 697a 696e  ht:1.5;box-sizin
+00014920: 673a 626f 7264 6572 2d62 6f78 3b70 6164  g:border-box;pad
+00014930: 6469 6e67 3a30 3b68 6569 6768 743a 3730  ding:0;height:70
+00014940: 7668 3b64 6973 706c 6179 3a2d 6d73 2d66  vh;display:-ms-f
+00014950: 6c65 7862 6f78 3b64 6973 706c 6179 3a66  lexbox;display:f
+00014960: 6c65 783b 6d69 6e2d 6865 6967 6874 3a35  lex;min-height:5
+00014970: 3070 783b 6d61 782d 6865 6967 6874 3a38  0px;max-height:8
+00014980: 3576 683b 6f76 6572 666c 6f77 3a61 7574  5vh;overflow:aut
+00014990: 6f7d 2e75 6970 2d6d 6f64 616c 202e 7569  o}.uip-modal .ui
+000149a0: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
+000149b0: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
+000149c0: 7920 2e75 6970 2d6d 6f64 616c 2d2d 7369  y .uip-modal--si
+000149d0: 6465 6261 727b 2d6d 732d 666c 6578 2d6e  debar{-ms-flex-n
+000149e0: 6567 6174 6976 653a 303b 666c 6578 2d73  egative:0;flex-s
+000149f0: 6872 696e 6b3a 303b 6d61 782d 7769 6474  hrink:0;max-widt
+00014a00: 683a 3235 257d 2e75 6970 2d6d 6f64 616c  h:25%}.uip-modal
+00014a10: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
+00014a20: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
+00014a30: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
+00014a40: 2d2d 7369 6465 6261 7220 2e75 6970 2d6d  --sidebar .uip-m
+00014a50: 6f64 616c 2d2d 7369 6465 6261 722d 7461  odal--sidebar-ta
+00014a60: 6273 7b6d 6172 6769 6e2d 746f 703a 3330  bs{margin-top:30
+00014a70: 7078 7d2e 7569 702d 6d6f 6461 6c20 2e75  px}.uip-modal .u
+00014a80: 6970 2d6d 6f64 616c 2d2d 636f 6e74 656e  ip-modal--conten
+00014a90: 7420 2e75 6970 2d6d 6f64 616c 2d2d 626f  t .uip-modal--bo
+00014aa0: 6479 202e 7569 702d 6d6f 6461 6c2d 2d73  dy .uip-modal--s
+00014ab0: 6964 6562 6172 202e 7569 702d 6d6f 6461  idebar .uip-moda
+00014ac0: 6c2d 2d73 6964 6562 6172 2d74 6162 7320  l--sidebar-tabs 
+00014ad0: 2e75 6970 2d6d 6f64 616c 2d2d 7369 6465  .uip-modal--side
+00014ae0: 6261 722d 7461 622d 6974 656d 7b70 6164  bar-tab-item{pad
+00014af0: 6469 6e67 3a31 3570 783b 666f 6e74 2d73  ding:15px;font-s
+00014b00: 697a 653a 3134 7078 3b63 6f6c 6f72 3a76  ize:14px;color:v
+00014b10: 6172 282d 2d64 6361 2d67 7261 792c 7661  ar(--dca-gray,va
+00014b20: 7228 2d2d 626f 6479 2d71 7569 6574 2d63  r(--body-quiet-c
+00014b30: 6f6c 6f72 2c23 3636 3629 293b 7465 7874  olor,#666));text
+00014b40: 2d61 6c69 676e 3a6c 6566 743b 6375 7273  -align:left;curs
+00014b50: 6f72 3a70 6f69 6e74 6572 3b70 6f73 6974  or:pointer;posit
+00014b60: 696f 6e3a 7265 6c61 7469 7665 3b64 6973  ion:relative;dis
+00014b70: 706c 6179 3a2d 6d73 2d66 6c65 7862 6f78  play:-ms-flexbox
+00014b80: 3b64 6973 706c 6179 3a66 6c65 783b 2d6d  ;display:flex;-m
+00014b90: 732d 666c 6578 2d61 6c69 676e 3a63 656e  s-flex-align:cen
+00014ba0: 7465 723b 616c 6967 6e2d 6974 656d 733a  ter;align-items:
+00014bb0: 6365 6e74 6572 3b74 6578 742d 7472 616e  center;text-tran
+00014bc0: 7366 6f72 6d3a 6361 7069 7461 6c69 7a65  sform:capitalize
+00014bd0: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
+00014be0: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
+00014bf0: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
+00014c00: 202e 7569 702d 6d6f 6461 6c2d 2d73 6964   .uip-modal--sid
+00014c10: 6562 6172 202e 7569 702d 6d6f 6461 6c2d  ebar .uip-modal-
+00014c20: 2d73 6964 6562 6172 2d74 6162 7320 2e75  -sidebar-tabs .u
+00014c30: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
+00014c40: 722d 7461 622d 6974 656d 2069 7b66 6f6e  r-tab-item i{fon
+00014c50: 742d 7369 7a65 3a32 3070 783b 7061 6464  t-size:20px;padd
+00014c60: 696e 672d 7269 6768 743a 3135 7078 3b63  ing-right:15px;c
+00014c70: 6f6c 6f72 3a76 6172 282d 2d64 6361 2d67  olor:var(--dca-g
+00014c80: 7261 792d 6c69 6768 7465 722c 7661 7228  ray-lighter,var(
+00014c90: 2d2d 626f 7264 6572 2d63 6f6c 6f72 2c23  --border-color,#
+00014ca0: 6363 6329 297d 2e75 6970 2d6d 6f64 616c  ccc))}.uip-modal
+00014cb0: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
+00014cc0: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
+00014cd0: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
+00014ce0: 2d2d 7369 6465 6261 7220 2e75 6970 2d6d  --sidebar .uip-m
+00014cf0: 6f64 616c 2d2d 7369 6465 6261 722d 7461  odal--sidebar-ta
+00014d00: 6273 202e 7569 702d 6d6f 6461 6c2d 2d73  bs .uip-modal--s
+00014d10: 6964 6562 6172 2d74 6162 2d69 7465 6d20  idebar-tab-item 
+00014d20: 696d 677b 7061 6464 696e 672d 7269 6768  img{padding-righ
+00014d30: 743a 3135 7078 7d2e 7569 702d 6d6f 6461  t:15px}.uip-moda
+00014d40: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
+00014d50: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
+00014d60: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
+00014d70: 6c2d 2d73 6964 6562 6172 202e 7569 702d  l--sidebar .uip-
+00014d80: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
+00014d90: 6162 7320 2e75 6970 2d6d 6f64 616c 2d2d  abs .uip-modal--
+00014da0: 7369 6465 6261 722d 7461 622d 6974 656d  sidebar-tab-item
+00014db0: 2e75 6e69 7665 7273 616c 2d61 6374 6976  .universal-activ
+00014dc0: 657b 6261 636b 6772 6f75 6e64 2d63 6f6c  e{background-col
+00014dd0: 6f72 3a76 6172 282d 2d64 6361 2d77 6869  or:var(--dca-whi
+00014de0: 7465 2c76 6172 282d 2d62 672d 636f 6c6f  te,var(--bg-colo
+00014df0: 722c 2366 6666 2929 3b62 6f78 2d73 6861  r,#fff));box-sha
+00014e00: 646f 773a 3020 3670 7820 3230 7078 2030  dow:0 6px 20px 0
+00014e10: 2072 6762 6128 302c 302c 302c 2e31 297d   rgba(0,0,0,.1)}
+00014e20: 2e75 6970 2d6d 6f64 616c 202e 7569 702d  .uip-modal .uip-
+00014e30: 6d6f 6461 6c2d 2d63 6f6e 7465 6e74 202e  modal--content .
+00014e40: 7569 702d 6d6f 6461 6c2d 2d62 6f64 7920  uip-modal--body 
+00014e50: 2e75 6970 2d6d 6f64 616c 2d2d 7369 6465  .uip-modal--side
+00014e60: 6261 7220 2e75 6970 2d6d 6f64 616c 2d2d  bar .uip-modal--
+00014e70: 7369 6465 6261 722d 7461 6273 202e 7569  sidebar-tabs .ui
+00014e80: 702d 6d6f 6461 6c2d 2d73 6964 6562 6172  p-modal--sidebar
+00014e90: 2d74 6162 2d69 7465 6d2e 756e 6976 6572  -tab-item.univer
+00014ea0: 7361 6c2d 6163 7469 7665 3a61 6674 6572  sal-active:after
+00014eb0: 7b63 6f6e 7465 6e74 3a22 223b 706f 7369  {content:"";posi
+00014ec0: 7469 6f6e 3a61 6273 6f6c 7574 653b 6865  tion:absolute;he
+00014ed0: 6967 6874 3a31 3030 253b 7769 6474 683a  ight:100%;width:
+00014ee0: 3570 783b 746f 703a 303b 6c65 6674 3a30  5px;top:0;left:0
+00014ef0: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
+00014f00: 723a 2330 6266 7d2e 7569 702d 6d6f 6461  r:#0bf}.uip-moda
+00014f10: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
+00014f20: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
+00014f30: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
+00014f40: 6c2d 2d73 6964 6562 6172 202e 7569 702d  l--sidebar .uip-
+00014f50: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
+00014f60: 6162 7320 2e75 6970 2d6d 6f64 616c 2d2d  abs .uip-modal--
+00014f70: 7369 6465 6261 722d 7461 622d 6974 656d  sidebar-tab-item
+00014f80: 2e75 6e69 7665 7273 616c 2d61 6374 6976  .universal-activ
+00014f90: 6520 697b 636f 6c6f 723a 2330 6266 7d2e  e i{color:#0bf}.
+00014fa0: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
+00014fb0: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
+00014fc0: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
+00014fd0: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
+00014fe0: 6172 202e 7569 702d 6d6f 6461 6c2d 2d73  ar .uip-modal--s
+00014ff0: 6964 6562 6172 2d74 6162 7320 2e75 6970  idebar-tabs .uip
+00015000: 2d6d 6f64 616c 2d2d 7369 6465 6261 722d  -modal--sidebar-
+00015010: 7461 622d 6974 656d 3a6f 6e6c 792d 6368  tab-item:only-ch
+00015020: 696c 647b 6469 7370 6c61 793a 6e6f 6e65  ild{display:none
+00015030: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
+00015040: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
+00015050: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
+00015060: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
+00015070: 6e2d 7072 6576 6965 772d 7772 6170 7b64  n-preview-wrap{d
+00015080: 6973 706c 6179 3a2d 6d73 2d66 6c65 7862  isplay:-ms-flexb
+00015090: 6f78 3b64 6973 706c 6179 3a66 6c65 783b  ox;display:flex;
+000150a0: 2d6d 732d 666c 6578 2d64 6972 6563 7469  -ms-flex-directi
+000150b0: 6f6e 3a63 6f6c 756d 6e3b 666c 6578 2d64  on:column;flex-d
+000150c0: 6972 6563 7469 6f6e 3a63 6f6c 756d 6e3b  irection:column;
+000150d0: 7061 6464 696e 673a 3330 7078 2038 3070  padding:30px 80p
+000150e0: 7820 303b 7769 6474 683a 3130 3025 7d2e  x 0;width:100%}.
+000150f0: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
+00015100: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
+00015110: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
+00015120: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
+00015130: 7072 6576 6965 772d 7772 6170 202e 7569  preview-wrap .ui
+00015140: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7072  p-modal--icon-pr
+00015150: 6576 6965 772d 696e 6e65 727b 6f76 6572  eview-inner{over
+00015160: 666c 6f77 3a61 7574 6f3b 6d61 7267 696e  flow:auto;margin
+00015170: 3a32 3570 7820 2d31 3570 7820 303b 7061  :25px -15px 0;pa
+00015180: 6464 696e 673a 3020 3135 7078 2031 3570  dding:0 15px 15p
+00015190: 787d 2e75 6970 2d6d 6f64 616c 202e 7569  x}.uip-modal .ui
+000151a0: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
+000151b0: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
+000151c0: 7920 2e75 6970 2d6d 6f64 616c 2d2d 6963  y .uip-modal--ic
+000151d0: 6f6e 2d70 7265 7669 6577 2d77 7261 7020  on-preview-wrap 
+000151e0: 2e75 6970 2d6d 6f64 616c 2d2d 6963 6f6e  .uip-modal--icon
+000151f0: 2d70 7265 7669 6577 2d69 6e6e 6572 202e  -preview-inner .
+00015200: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
+00015210: 7072 6576 6965 777b 6469 7370 6c61 793a  preview{display:
+00015220: 2d6d 732d 6772 6964 3b64 6973 706c 6179  -ms-grid;display
+00015230: 3a67 7269 643b 6772 6964 2d67 6170 3a32  :grid;grid-gap:2
+00015240: 3070 783b 6d61 7267 696e 3a32 3070 7820  0px;margin:20px 
+00015250: 307d 2e75 6970 2d6d 6f64 616c 202e 7569  0}.uip-modal .ui
+00015260: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
+00015270: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
+00015280: 7920 2e75 6970 2d6d 6f64 616c 2d2d 6963  y .uip-modal--ic
+00015290: 6f6e 2d70 7265 7669 6577 2d77 7261 7020  on-preview-wrap 
+000152a0: 2e75 6970 2d6d 6f64 616c 2d2d 6963 6f6e  .uip-modal--icon
+000152b0: 2d70 7265 7669 6577 2d69 6e6e 6572 202e  -preview-inner .
+000152c0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
+000152d0: 7072 6576 6965 7720 2e75 6970 2d69 636f  preview .uip-ico
+000152e0: 6e2d 6974 656d 7b70 6f73 6974 696f 6e3a  n-item{position:
+000152f0: 7265 6c61 7469 7665 3b70 6164 6469 6e67  relative;padding
+00015300: 3a31 3070 783b 6261 636b 6772 6f75 6e64  :10px;background
+00015310: 2d63 6f6c 6f72 3a76 6172 282d 2d64 6361  -color:var(--dca
+00015320: 2d77 6869 7465 2c76 6172 282d 2d62 672d  -white,var(--bg-
+00015330: 636f 6c6f 722c 2366 6666 2929 3b62 6f78  color,#fff));box
+00015340: 2d73 6861 646f 773a 3020 3170 7820 3132  -shadow:0 1px 12
+00015350: 7078 2072 6762 6128 302c 302c 302c 2e30  px rgba(0,0,0,.0
+00015360: 3529 3b62 6f72 6465 722d 7261 6469 7573  5);border-radius
+00015370: 3a33 7078 3b63 7572 736f 723a 706f 696e  :3px;cursor:poin
+00015380: 7465 723b 7472 616e 7369 7469 6f6e 3a61  ter;transition:a
+00015390: 6c6c 202e 3373 3b6f 7665 7266 6c6f 773a  ll .3s;overflow:
+000153a0: 6869 6464 656e 7d2e 7569 702d 6d6f 6461  hidden}.uip-moda
+000153b0: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
+000153c0: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
+000153d0: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
+000153e0: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
+000153f0: 7772 6170 202e 7569 702d 6d6f 6461 6c2d  wrap .uip-modal-
+00015400: 2d69 636f 6e2d 7072 6576 6965 772d 696e  -icon-preview-in
+00015410: 6e65 7220 2e75 6970 2d6d 6f64 616c 2d2d  ner .uip-modal--
+00015420: 6963 6f6e 2d70 7265 7669 6577 202e 7569  icon-preview .ui
+00015430: 702d 6963 6f6e 2d69 7465 6d3a 686f 7665  p-icon-item:hove
+00015440: 727b 626f 782d 7368 6164 6f77 3a30 2031  r{box-shadow:0 1
+00015450: 7078 2031 3470 7820 7267 6261 2830 2c30  px 14px rgba(0,0
+00015460: 2c30 2c2e 3136 297d 2e75 6970 2d6d 6f64  ,0,.16)}.uip-mod
+00015470: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
+00015480: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
+00015490: 6c2d 2d62 6f64 7920 2e75 6970 2d6d 6f64  l--body .uip-mod
+000154a0: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
+000154b0: 2d77 7261 7020 2e75 6970 2d6d 6f64 616c  -wrap .uip-modal
+000154c0: 2d2d 6963 6f6e 2d70 7265 7669 6577 2d69  --icon-preview-i
+000154d0: 6e6e 6572 202e 7569 702d 6d6f 6461 6c2d  nner .uip-modal-
+000154e0: 2d69 636f 6e2d 7072 6576 6965 7720 2e75  -icon-preview .u
+000154f0: 6970 2d69 636f 6e2d 6974 656d 2e75 6e69  ip-icon-item.uni
+00015500: 7665 7273 616c 2d73 656c 6563 7465 647b  versal-selected{
+00015510: 626f 782d 7368 6164 6f77 3a30 2031 7078  box-shadow:0 1px
+00015520: 2031 3270 7820 7267 6261 2830 2c30 2c30   12px rgba(0,0,0
+00015530: 2c2e 3035 292c 3020 3020 3020 3370 7820  ,.05),0 0 0 3px 
+00015540: 2330 6266 7d2e 7569 702d 6d6f 6461 6c20  #0bf}.uip-modal 
+00015550: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
+00015560: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
+00015570: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
+00015580: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
+00015590: 6170 202e 7569 702d 6d6f 6461 6c2d 2d69  ap .uip-modal--i
+000155a0: 636f 6e2d 7072 6576 6965 772d 696e 6e65  con-preview-inne
+000155b0: 7220 2e75 6970 2d6d 6f64 616c 2d2d 6963  r .uip-modal--ic
+000155c0: 6f6e 2d70 7265 7669 6577 202e 7569 702d  on-preview .uip-
+000155d0: 6963 6f6e 2d69 7465 6d20 2e75 6970 2d69  icon-item .uip-i
+000155e0: 636f 6e2d 6974 656d 2d69 6e6e 6572 7b64  con-item-inner{d
+000155f0: 6973 706c 6179 3a2d 6d73 2d66 6c65 7862  isplay:-ms-flexb
+00015600: 6f78 3b64 6973 706c 6179 3a66 6c65 783b  ox;display:flex;
+00015610: 2d6d 732d 666c 6578 2d64 6972 6563 7469  -ms-flex-directi
+00015620: 6f6e 3a63 6f6c 756d 6e3b 666c 6578 2d64  on:column;flex-d
+00015630: 6972 6563 7469 6f6e 3a63 6f6c 756d 6e3b  irection:column;
+00015640: 2d6d 732d 666c 6578 2d61 6c69 676e 3a63  -ms-flex-align:c
+00015650: 656e 7465 723b 616c 6967 6e2d 6974 656d  enter;align-item
+00015660: 733a 6365 6e74 6572 3b70 6164 6469 6e67  s:center;padding
+00015670: 3a31 7078 7d2e 7569 702d 6d6f 6461 6c20  :1px}.uip-modal 
+00015680: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
+00015690: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
+000156a0: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
+000156b0: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
+000156c0: 6170 202e 7569 702d 6d6f 6461 6c2d 2d69  ap .uip-modal--i
+000156d0: 636f 6e2d 7072 6576 6965 772d 696e 6e65  con-preview-inne
+000156e0: 7220 2e75 6970 2d6d 6f64 616c 2d2d 6963  r .uip-modal--ic
+000156f0: 6f6e 2d70 7265 7669 6577 202e 7569 702d  on-preview .uip-
+00015700: 6963 6f6e 2d69 7465 6d20 2e75 6970 2d69  icon-item .uip-i
+00015710: 636f 6e2d 6974 656d 2d69 6e6e 6572 202e  con-item-inner .
+00015720: 7569 702d 6963 6f6e 2d69 7465 6d5f 5f69  uip-icon-item__i
+00015730: 636f 6e2c 2e75 6970 2d6d 6f64 616c 202e  con,.uip-modal .
+00015740: 7569 702d 6d6f 6461 6c2d 2d63 6f6e 7465  uip-modal--conte
+00015750: 6e74 202e 7569 702d 6d6f 6461 6c2d 2d62  nt .uip-modal--b
+00015760: 6f64 7920 2e75 6970 2d6d 6f64 616c 2d2d  ody .uip-modal--
+00015770: 6963 6f6e 2d70 7265 7669 6577 2d77 7261  icon-preview-wra
+00015780: 7020 2e75 6970 2d6d 6f64 616c 2d2d 6963  p .uip-modal--ic
+00015790: 6f6e 2d70 7265 7669 6577 2d69 6e6e 6572  on-preview-inner
+000157a0: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
+000157b0: 6e2d 7072 6576 6965 7720 2e75 6970 2d69  n-preview .uip-i
+000157c0: 636f 6e2d 6974 656d 202e 7569 702d 6963  con-item .uip-ic
+000157d0: 6f6e 2d69 7465 6d2d 696e 6e65 7220 697b  on-item-inner i{
+000157e0: 666f 6e74 2d73 697a 653a 3235 7078 3b63  font-size:25px;c
+000157f0: 6f6c 6f72 3a76 6172 282d 2d64 6361 2d67  olor:var(--dca-g
+00015800: 7261 792d 6461 726b 6573 742c 7661 7228  ray-darkest,var(
+00015810: 2d2d 626f 6479 2d66 672c 2333 3333 2929  --body-fg,#333))
+00015820: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
+00015830: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
+00015840: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
+00015850: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
+00015860: 6e2d 7072 6576 6965 772d 7772 6170 202e  n-preview-wrap .
+00015870: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
+00015880: 7072 6576 6965 772d 696e 6e65 7220 2e75  preview-inner .u
+00015890: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
+000158a0: 7265 7669 6577 202e 7569 702d 6963 6f6e  review .uip-icon
+000158b0: 2d69 7465 6d20 2e75 6970 2d69 636f 6e2d  -item .uip-icon-
+000158c0: 6974 656d 2d69 6e6e 6572 202e 7569 702d  item-inner .uip-
+000158d0: 6963 6f6e 2d69 7465 6d2d 6e61 6d65 7b63  icon-item-name{c
+000158e0: 6f6c 6f72 3a76 6172 282d 2d64 6361 2d67  olor:var(--dca-g
+000158f0: 7261 792c 7661 7228 2d2d 626f 6479 2d71  ray,var(--body-q
+00015900: 7569 6574 2d63 6f6c 6f72 2c23 3636 3629  uiet-color,#666)
+00015910: 293b 666f 6e74 2d73 697a 653a 3131 7078  );font-size:11px
+00015920: 3b70 6164 6469 6e67 3a31 3370 7820 3020  ;padding:13px 0 
+00015930: 303b 6d61 782d 7769 6474 683a 3130 3025  0;max-width:100%
+00015940: 3b77 6869 7465 2d73 7061 6365 3a6e 6f77  ;white-space:now
+00015950: 7261 703b 7465 7874 2d6f 7665 7266 6c6f  rap;text-overflo
+00015960: 773a 656c 6c69 7073 6973 3b6f 7665 7266  w:ellipsis;overf
+00015970: 6c6f 773a 6869 6464 656e 3b74 6578 742d  low:hidden;text-
+00015980: 7472 616e 7366 6f72 6d3a 6361 7069 7461  transform:capita
+00015990: 6c69 7a65 7d2e 7569 702d 6d6f 6461 6c20  lize}.uip-modal 
+000159a0: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
+000159b0: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
+000159c0: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
+000159d0: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
+000159e0: 6170 202e 7569 702d 6d6f 6461 6c2d 2d69  ap .uip-modal--i
+000159f0: 636f 6e2d 7365 6172 6368 7b70 6f73 6974  con-search{posit
+00015a00: 696f 6e3a 7265 6c61 7469 7665 7d2e 7569  ion:relative}.ui
+00015a10: 702d 6d6f 6461 6c20 2e75 6970 2d6d 6f64  p-modal .uip-mod
+00015a20: 616c 2d2d 636f 6e74 656e 7420 2e75 6970  al--content .uip
+00015a30: 2d6d 6f64 616c 2d2d 626f 6479 202e 7569  -modal--body .ui
+00015a40: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7072  p-modal--icon-pr
+00015a50: 6576 6965 772d 7772 6170 202e 7569 702d  eview-wrap .uip-
+00015a60: 6d6f 6461 6c2d 2d69 636f 6e2d 7365 6172  modal--icon-sear
+00015a70: 6368 2069 6e70 7574 7b77 6964 7468 3a31  ch input{width:1
+00015a80: 3030 253b 7061 6464 696e 673a 3870 7820  00%;padding:8px 
+00015a90: 3135 7078 3b62 6163 6b67 726f 756e 642d  15px;background-
+00015aa0: 636f 6c6f 723a 7661 7228 2d2d 6463 612d  color:var(--dca-
+00015ab0: 7768 6974 652c 7661 7228 2d2d 6267 2d63  white,var(--bg-c
+00015ac0: 6f6c 6f72 2c23 6666 6629 293b 626f 7264  olor,#fff));bord
+00015ad0: 6572 3a6e 6f6e 657d 2e75 6970 2d6d 6f64  er:none}.uip-mod
+00015ae0: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
+00015af0: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
+00015b00: 6c2d 2d62 6f64 7920 2e75 6970 2d6d 6f64  l--body .uip-mod
+00015b10: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
+00015b20: 2d77 7261 7020 2e75 6970 2d6d 6f64 616c  -wrap .uip-modal
+00015b30: 2d2d 6963 6f6e 2d73 6561 7263 6820 696e  --icon-search in
+00015b40: 7075 743a 2d6d 732d 696e 7075 742d 706c  put:-ms-input-pl
+00015b50: 6163 6568 6f6c 6465 727b 666f 6e74 2d73  aceholder{font-s
+00015b60: 7479 6c65 3a69 7461 6c69 637d 2e75 6970  tyle:italic}.uip
+00015b70: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00015b80: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
+00015b90: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
+00015ba0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+00015bb0: 7669 6577 2d77 7261 7020 2e75 6970 2d6d  view-wrap .uip-m
+00015bc0: 6f64 616c 2d2d 6963 6f6e 2d73 6561 7263  odal--icon-searc
+00015bd0: 6820 696e 7075 743a 3a70 6c61 6365 686f  h input::placeho
+00015be0: 6c64 6572 7b66 6f6e 742d 7374 796c 653a  lder{font-style:
+00015bf0: 6974 616c 6963 7d2e 7569 702d 6d6f 6461  italic}.uip-moda
+00015c00: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
+00015c10: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
+00015c20: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
+00015c30: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
+00015c40: 7772 6170 202e 7569 702d 6d6f 6461 6c2d  wrap .uip-modal-
+00015c50: 2d69 636f 6e2d 7365 6172 6368 2069 6d67  -icon-search img
+00015c60: 7b70 6f73 6974 696f 6e3a 6162 736f 6c75  {position:absolu
+00015c70: 7465 3b74 6f70 3a35 3025 3b74 7261 6e73  te;top:50%;trans
+00015c80: 666f 726d 3a74 7261 6e73 6c61 7465 5928  form:translateY(
+00015c90: 2d35 3025 293b 7269 6768 743a 3130 7078  -50%);right:10px
+00015ca0: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
+00015cb0: 2d6d 6f64 616c 2d2d 666f 6f74 6572 7b62  -modal--footer{b
+00015cc0: 6f72 6465 722d 746f 703a 3170 7820 736f  order-top:1px so
+00015cd0: 6c69 6420 7661 7228 2d2d 6463 612d 6772  lid var(--dca-gr
+00015ce0: 6179 2d6c 6967 6874 6572 2c76 6172 282d  ay-lighter,var(-
+00015cf0: 2d62 6f72 6465 722d 636f 6c6f 722c 2363  -border-color,#c
+00015d00: 6363 2929 3b74 6578 742d 616c 6967 6e3a  cc));text-align:
+00015d10: 6365 6e74 6572 3b62 6163 6b67 726f 756e  center;backgroun
+00015d20: 642d 636f 6c6f 723a 7661 7228 2d2d 6463  d-color:var(--dc
+00015d30: 612d 7768 6974 652c 7661 7228 2d2d 6267  a-white,var(--bg
+00015d40: 2d63 6f6c 6f72 2c23 6666 6629 293b 626f  -color,#fff));bo
+00015d50: 7264 6572 3a6e 6f6e 653b 6469 7370 6c61  rder:none;displa
+00015d60: 793a 6e6f 6e65 3b2d 6d73 2d66 6c65 782d  y:none;-ms-flex-
+00015d70: 7061 636b 3a65 6e64 3b6a 7573 7469 6679  pack:end;justify
+00015d80: 2d63 6f6e 7465 6e74 3a66 6c65 782d 656e  -content:flex-en
+00015d90: 643b 7061 6464 696e 673a 3570 783b 626f  d;padding:5px;bo
+00015da0: 782d 7368 6164 6f77 3a30 2030 2038 7078  x-shadow:0 0 8px
+00015db0: 2072 6762 6128 302c 302c 302c 2e31 293b   rgba(0,0,0,.1);
+00015dc0: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+00015dd0: 653b 6469 7370 6c61 793a 2d6d 732d 666c  e;display:-ms-fl
+00015de0: 6578 626f 783b 6469 7370 6c61 793a 666c  exbox;display:fl
+00015df0: 6578 7d2e 7569 702d 6d6f 6461 6c20 2e75  ex}.uip-modal .u
+00015e00: 6970 2d6d 6f64 616c 2d2d 666f 6f74 6572  ip-modal--footer
+00015e10: 2062 7574 746f 6e2e 7569 702d 696e 7365   button.uip-inse
+00015e20: 7274 2d69 636f 6e2d 6275 7474 6f6e 7b70  rt-icon-button{p
+00015e30: 6164 6469 6e67 3a31 3070 7820 3335 7078  adding:10px 35px
+00015e40: 2169 6d70 6f72 7461 6e74 3b63 6f6c 6f72  !important;color
+00015e50: 3a76 6172 282d 2d64 6361 2d77 6869 7465  :var(--dca-white
+00015e60: 2c76 6172 282d 2d62 672d 636f 6c6f 722c  ,var(--bg-color,
+00015e70: 2366 6666 2929 2169 6d70 6f72 7461 6e74  #fff))!important
+00015e80: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
+00015e90: 723a 2330 6266 2169 6d70 6f72 7461 6e74  r:#0bf!important
+00015ea0: 3b62 6f72 6465 723a 6e6f 6e65 3b63 7572  ;border:none;cur
+00015eb0: 736f 723a 706f 696e 7465 723b 6f75 746c  sor:pointer;outl
+00015ec0: 696e 653a 307d 2e75 6970 2d6d 6f64 616c  ine:0}.uip-modal
+00015ed0: 202e 7569 702d 6d6f 6461 6c2d 2d66 6f6f   .uip-modal--foo
+00015ee0: 7465 7220 2e75 6e69 7665 7273 616c 2d62  ter .universal-b
+00015ef0: 7574 746f 6e7b 6865 6967 6874 3a34 3070  utton{height:40p
+00015f00: 783b 6d61 7267 696e 2d6c 6566 743a 3570  x;margin-left:5p
+00015f10: 787d 2e75 6970 2d6d 6f64 616c 202e 7569  x}.uip-modal .ui
+00015f20: 702d 6d6f 6461 6c2d 2d66 6f6f 7465 7220  p-modal--footer 
+00015f30: 2e75 6e69 7665 7273 616c 2d62 7574 746f  .universal-butto
+00015f40: 6e2d 7375 6363 6573 737b 7061 6464 696e  n-success{paddin
+00015f50: 673a 3132 7078 2033 3670 783b 636f 6c6f  g:12px 36px;colo
+00015f60: 723a 7661 7228 2d2d 6463 612d 7768 6974  r:var(--dca-whit
+00015f70: 652c 7661 7228 2d2d 6267 2d63 6f6c 6f72  e,var(--bg-color
+00015f80: 2c23 6666 6629 293b 7769 6474 683a 696e  ,#fff));width:in
+00015f90: 6974 6961 6c7d 2e75 6970 2d6d 6f64 616c  itial}.uip-modal
+00015fa0: 202e 7569 702d 6d6f 6461 6c2d 2d66 6f6f   .uip-modal--foo
+00015fb0: 7465 7220 2e75 6e69 7665 7273 616c 2d62  ter .universal-b
+00015fc0: 7574 746f 6e2d 7375 6363 6573 733a 686f  utton-success:ho
+00015fd0: 7665 727b 6261 636b 6772 6f75 6e64 2d63  ver{background-c
+00015fe0: 6f6c 6f72 3a23 3062 667d 406d 6564 6961  olor:#0bf}@media
+00015ff0: 2028 6d69 6e2d 7769 6474 683a 3134 3430   (min-width:1440
+00016000: 7078 297b 626f 6479 3a6e 6f74 282e 636d  px){body:not(.cm
+00016010: 732d 6164 6d69 6e2d 6d6f 6461 6c29 202e  s-admin-modal) .
+00016020: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
+00016030: 6f64 616c 2d2d 636f 6e74 656e 747b 6d61  odal--content{ma
+00016040: 782d 7769 6474 683a 3132 3030 7078 7d7d  x-width:1200px}}
+00016050: 406d 6564 6961 2028 6d61 782d 7769 6474  @media (max-widt
+00016060: 683a 3134 3339 7078 297b 626f 6479 3a6e  h:1439px){body:n
+00016070: 6f74 282e 636d 732d 6164 6d69 6e2d 6d6f  ot(.cms-admin-mo
+00016080: 6461 6c29 202e 7569 702d 6d6f 6461 6c20  dal) .uip-modal 
+00016090: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
+000160a0: 656e 747b 6d61 782d 7769 6474 683a 3939  ent{max-width:99
+000160b0: 3070 787d 2e75 6970 2d6d 6f64 616c 2d2d  0px}.uip-modal--
+000160c0: 6963 6f6e 2d70 7265 7669 6577 2d77 7261  icon-preview-wra
+000160d0: 707b 7061 6464 696e 673a 3330 7078 2035  p{padding:30px 5
+000160e0: 3070 7820 307d 7d40 6d65 6469 6120 286d  0px 0}}@media (m
+000160f0: 6178 2d77 6964 7468 3a31 3032 3370 7829  ax-width:1023px)
+00016100: 7b62 6f64 793a 6e6f 7428 2e63 6d73 2d61  {body:not(.cms-a
+00016110: 646d 696e 2d6d 6f64 616c 2920 2e75 6970  dmin-modal) .uip
+00016120: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00016130: 6c2d 2d63 6f6e 7465 6e74 7b6d 6178 2d77  l--content{max-w
+00016140: 6964 7468 3a37 3430 7078 7d7d 406d 6564  idth:740px}}@med
+00016150: 6961 2028 6d61 782d 7769 6474 683a 3736  ia (max-width:76
+00016160: 3770 7829 7b2e 7569 702d 6d6f 6461 6c2d  7px){.uip-modal-
+00016170: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
+00016180: 6170 7b70 6164 6469 6e67 3a31 3570 7821  ap{padding:15px!
+00016190: 696d 706f 7274 616e 747d 2e75 6970 2d6d  important}.uip-m
+000161a0: 6f64 616c 2d2d 7369 6465 6261 727b 6469  odal--sidebar{di
+000161b0: 7370 6c61 793a 6e6f 6e65 7d7d 406d 6564  splay:none}}@med
+000161c0: 6961 2028 6d69 6e2d 7769 6474 683a 3134  ia (min-width:14
+000161d0: 3430 7078 297b 2e75 6970 2d6d 6f64 616c  40px){.uip-modal
+000161e0: 2d2d 6963 6f6e 2d70 7265 7669 6577 7b2d  --icon-preview{-
+000161f0: 6d73 2d67 7269 642d 636f 6c75 6d6e 733a  ms-grid-columns:
+00016200: 2831 6672 295b 375d 3b67 7269 642d 7465  (1fr)[7];grid-te
+00016210: 6d70 6c61 7465 2d63 6f6c 756d 6e73 3a72  mplate-columns:r
+00016220: 6570 6561 7428 372c 3166 7229 7d7d 406d  epeat(7,1fr)}}@m
+00016230: 6564 6961 2028 6d61 782d 7769 6474 683a  edia (max-width:
+00016240: 3134 3339 7078 297b 2e75 6970 2d6d 6f64  1439px){.uip-mod
+00016250: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
+00016260: 7b2d 6d73 2d67 7269 642d 636f 6c75 6d6e  {-ms-grid-column
+00016270: 733a 2831 6672 295b 365d 3b67 7269 642d  s:(1fr)[6];grid-
+00016280: 7465 6d70 6c61 7465 2d63 6f6c 756d 6e73  template-columns
+00016290: 3a72 6570 6561 7428 362c 3166 7229 7d7d  :repeat(6,1fr)}}
+000162a0: 406d 6564 6961 2028 6d61 782d 7769 6474  @media (max-widt
+000162b0: 683a 3130 3234 7078 297b 2e75 6970 2d6d  h:1024px){.uip-m
+000162c0: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
+000162d0: 6577 7b2d 6d73 2d67 7269 642d 636f 6c75  ew{-ms-grid-colu
+000162e0: 6d6e 733a 2831 6672 295b 355d 3b67 7269  mns:(1fr)[5];gri
+000162f0: 642d 7465 6d70 6c61 7465 2d63 6f6c 756d  d-template-colum
+00016300: 6e73 3a72 6570 6561 7428 352c 3166 7229  ns:repeat(5,1fr)
+00016310: 7d7d 406d 6564 6961 2028 6d61 782d 7769  }}@media (max-wi
+00016320: 6474 683a 3736 3770 7829 7b2e 7569 702d  dth:767px){.uip-
+00016330: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
+00016340: 6965 777b 2d6d 732d 6772 6964 2d63 6f6c  iew{-ms-grid-col
+00016350: 756d 6e73 3a28 3166 7229 5b34 5d3b 6772  umns:(1fr)[4];gr
+00016360: 6964 2d74 656d 706c 6174 652d 636f 6c75  id-template-colu
+00016370: 6d6e 733a 7265 7065 6174 2834 2c31 6672  mns:repeat(4,1fr
+00016380: 297d 7d40 6d65 6469 6120 286d 6178 2d77  )}}@media (max-w
+00016390: 6964 7468 3a34 3739 7078 297b 2e75 6970  idth:479px){.uip
+000163a0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+000163b0: 7669 6577 7b2d 6d73 2d67 7269 642d 636f  view{-ms-grid-co
+000163c0: 6c75 6d6e 733a 2831 6672 295b 335d 3b67  lumns:(1fr)[3];g
+000163d0: 7269 642d 7465 6d70 6c61 7465 2d63 6f6c  rid-template-col
+000163e0: 756d 6e73 3a72 6570 6561 7428 332c 3166  umns:repeat(3,1f
+000163f0: 7229 7d7d 406d 6564 6961 2028 6d61 782d  r)}}@media (max-
+00016400: 7769 6474 683a 3134 3339 7078 297b 2e75  width:1439px){.u
+00016410: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
+00016420: 722d 7461 622d 6974 656d 7b70 6164 6469  r-tab-item{paddi
+00016430: 6e67 3a31 3570 7820 3135 7078 2031 3570  ng:15px 15px 15p
+00016440: 7820 3235 7078 3b66 6f6e 742d 7369 7a65  x 25px;font-size
+00016450: 3a31 3170 787d 2e75 6970 2d6d 6f64 616c  :11px}.uip-modal
+00016460: 2d2d 7369 6465 6261 722d 7461 622d 6974  --sidebar-tab-it
+00016470: 656d 2069 7b66 6f6e 742d 7369 7a65 3a31  em i{font-size:1
+00016480: 3570 787d 7d40 6d65 6469 6120 286d 6178  5px}}@media (max
+00016490: 2d77 6964 7468 3a31 3032 3470 7829 7b2e  -width:1024px){.
+000164a0: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
+000164b0: 6172 2d74 6162 2d69 7465 6d20 692c 2e75  ar-tab-item i,.u
+000164c0: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
+000164d0: 722d 7461 622d 6974 656d 2069 6d67 7b64  r-tab-item img{d
+000164e0: 6973 706c 6179 3a6e 6f6e 657d 7d2e 7372  isplay:none}}.sr
+000164f0: 2d6f 6e6c 797b 706f 7369 7469 6f6e 3a61  -only{position:a
+00016500: 6273 6f6c 7574 6521 696d 706f 7274 616e  bsolute!importan
+00016510: 743b 7769 6474 683a 3170 7821 696d 706f  t;width:1px!impo
+00016520: 7274 616e 743b 6865 6967 6874 3a31 7078  rtant;height:1px
+00016530: 2169 6d70 6f72 7461 6e74 3b70 6164 6469  !important;paddi
+00016540: 6e67 3a30 2169 6d70 6f72 7461 6e74 3b6d  ng:0!important;m
+00016550: 6172 6769 6e3a 2d31 7078 2169 6d70 6f72  argin:-1px!impor
+00016560: 7461 6e74 3b6f 7665 7266 6c6f 773a 6869  tant;overflow:hi
+00016570: 6464 656e 2169 6d70 6f72 7461 6e74 3b63  dden!important;c
+00016580: 6c69 703a 7265 6374 2830 2c30 2c30 2c30  lip:rect(0,0,0,0
+00016590: 2921 696d 706f 7274 616e 743b 7768 6974  )!important;whit
+000165a0: 652d 7370 6163 653a 6e6f 7772 6170 2169  e-space:nowrap!i
+000165b0: 6d70 6f72 7461 6e74 3b62 6f72 6465 723a  mportant;border:
+000165c0: 3021 696d 706f 7274 616e 747d 756c 2e6e  0!important}ul.n
+000165d0: 6176 7b6d 6172 6769 6e2d 626f 7474 6f6d  av{margin-bottom
+000165e0: 3a31 656d 7d75 6c2e 6e61 763e 6c69 2e6e  :1em}ul.nav>li.n
+000165f0: 6176 2d69 7465 6d7b 6c69 7374 2d73 7479  av-item{list-sty
+00016600: 6c65 2d74 7970 653a 6e6f 6e65 3b70 6164  le-type:none;pad
+00016610: 6469 6e67 3a69 6e68 6572 6974 7d2e 636f  ding:inherit}.co
+00016620: 6c4d 2075 6c3a 6e6f 7428 2e6f 626a 6563  lM ul:not(.objec
+00016630: 742d 746f 6f6c 7329 2e6e 6176 7b6d 6172  t-tools).nav{mar
+00016640: 6769 6e2d 746f 703a 303b 6d61 7267 696e  gin-top:0;margin
+00016650: 2d62 6f74 746f 6d3a 3230 7078 7d75 6c2e  -bottom:20px}ul.
+00016660: 6e61 7620 2e6e 6176 2d69 7465 6d7b 6d61  nav .nav-item{ma
+00016670: 7267 696e 2d72 6967 6874 3a31 7265 6d7d  rgin-right:1rem}
+00016680: 756c 2e6e 6176 202e 6e61 762d 6c69 6e6b  ul.nav .nav-link
+00016690: 7b70 6f73 6974 696f 6e3a 7265 6c61 7469  {position:relati
+000166a0: 7665 3b74 6578 742d 6465 636f 7261 7469  ve;text-decorati
+000166b0: 6f6e 3a6e 6f6e 657d 756c 2e6e 6176 202e  on:none}ul.nav .
+000166c0: 6e61 762d 6c69 6e6b 2073 7061 6e2e 696e  nav-link span.in
+000166d0: 6469 6361 746f 727b 6469 7370 6c61 793a  dicator{display:
+000166e0: 6e6f 6e65 3b62 6f72 6465 722d 7261 6469  none;border-radi
+000166f0: 7573 3a35 3025 3b70 6164 6469 6e67 3a2e  us:50%;padding:.
+00016700: 3572 656d 3b62 6f72 6465 723a 3170 7820  5rem;border:1px 
+00016710: 736f 6c69 6420 7661 7228 2d2d 6463 612d  solid var(--dca-
+00016720: 7768 6974 652c 7661 7228 2d2d 626f 6479  white,var(--body
+00016730: 2d62 672c 2366 6666 2929 3b74 7261 6e73  -bg,#fff));trans
+00016740: 666f 726d 3a74 7261 6e73 6c61 7465 282d  form:translate(-
+00016750: 3530 252c 2d35 3025 293b 746f 703a 303b  50%,-50%);top:0;
+00016760: 6c65 6674 3a31 3030 253b 706f 7369 7469  left:100%;positi
+00016770: 6f6e 3a61 6273 6f6c 7574 657d 756c 2e6e  on:absolute}ul.n
+00016780: 6176 202e 6e61 762d 6c69 6e6b 2073 7061  av .nav-link spa
+00016790: 6e2e 696e 6469 6361 746f 722e 6572 726f  n.indicator.erro
+000167a0: 727b 6261 636b 6772 6f75 6e64 2d63 6f6c  r{background-col
+000167b0: 6f72 3a76 6172 282d 2d62 732d 6461 6e67  or:var(--bs-dang
+000167c0: 6572 297d 756c 2e6e 6176 202e 6e61 762d  er)}ul.nav .nav-
+000167d0: 6c69 6e6b 2073 7061 6e2e 696e 6469 6361  link span.indica
+000167e0: 746f 722e 6174 7472 6962 7574 6573 7b62  tor.attributes{b
+000167f0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00016800: 7661 7228 2d2d 6273 2d69 6e66 6f29 3b64  var(--bs-info);d
+00016810: 6973 706c 6179 3a62 6c6f 636b 7d75 6c2e  isplay:block}ul.
+00016820: 6e61 7620 2e6e 6176 2d6c 696e 6b2e 6572  nav .nav-link.er
+00016830: 726f 723e 7370 616e 2e69 6e64 6963 6174  ror>span.indicat
+00016840: 6f72 7b64 6973 706c 6179 3a62 6c6f 636b  or{display:block
+00016850: 7d75 6c2e 6e61 762e 6e61 762d 7069 6c6c  }ul.nav.nav-pill
+00016860: 7320 2e6e 6176 2d6c 696e 6b3a 6e6f 7428  s .nav-link:not(
+00016870: 2e61 6374 6976 6529 7b62 6f72 6465 722d  .active){border-
+00016880: 7374 796c 653a 736f 6c69 643b 626f 7264  style:solid;bord
+00016890: 6572 2d77 6964 7468 3a31 7078 7d62 6f64  er-width:1px}bod
+000168a0: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
+000168b0: 2d61 646d 696e 2d73 7479 6c65 2920 756c  -admin-style) ul
+000168c0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+000168d0: 656e 642e 6e61 762d 7461 6273 2b64 6976  end.nav-tabs+div
+000168e0: 2e74 6162 2d63 6f6e 7465 6e74 202e 7461  .tab-content .ta
+000168f0: 622d 7061 6e65 7b62 6f72 6465 722d 6c65  b-pane{border-le
+00016900: 6674 2d73 7479 6c65 3a73 6f6c 6964 3b62  ft-style:solid;b
+00016910: 6f72 6465 722d 626f 7474 6f6d 2d73 7479  order-bottom-sty
+00016920: 6c65 3a73 6f6c 6964 3b62 6f72 6465 722d  le:solid;border-
+00016930: 7269 6768 742d 7374 796c 653a 736f 6c69  right-style:soli
+00016940: 643b 626f 7264 6572 2d6c 6566 742d 636f  d;border-left-co
+00016950: 6c6f 723a 7661 7228 2d2d 6861 6972 6c69  lor:var(--hairli
+00016960: 6e65 2d63 6f6c 6f72 293b 626f 7264 6572  ne-color);border
+00016970: 2d62 6f74 746f 6d2d 636f 6c6f 723a 7661  -bottom-color:va
+00016980: 7228 2d2d 6861 6972 6c69 6e65 2d63 6f6c  r(--hairline-col
+00016990: 6f72 293b 626f 7264 6572 2d72 6967 6874  or);border-right
+000169a0: 2d63 6f6c 6f72 3a76 6172 282d 2d68 6169  -color:var(--hai
+000169b0: 726c 696e 652d 636f 6c6f 7229 3b62 6f72  rline-color);bor
+000169c0: 6465 722d 7769 6474 683a 3170 787d 626f  der-width:1px}bo
+000169d0: 6479 3a6e 6f74 282e 646a 616e 676f 636d  dy:not(.djangocm
+000169e0: 732d 6164 6d69 6e2d 7374 796c 6529 2075  s-admin-style) u
+000169f0: 6c2e 646a 616e 676f 636d 732d 6672 6f6e  l.djangocms-fron
+00016a00: 7465 6e64 2e6e 6176 2d74 6162 732b 6469  tend.nav-tabs+di
+00016a10: 762e 7461 622d 636f 6e74 656e 7420 2e74  v.tab-content .t
+00016a20: 6162 2d70 616e 6520 6669 656c 6473 6574  ab-pane fieldset
+00016a30: 3a6c 6173 742d 6368 696c 647b 6d61 7267  :last-child{marg
+00016a40: 696e 2d62 6f74 746f 6d3a 307d 6469 762e  in-bottom:0}div.
+00016a50: 7461 622d 706b 7b2d 6d73 2d66 6c65 782d  tab-pk{-ms-flex-
+00016a60: 6974 656d 2d61 6c69 676e 3a63 656e 7465  item-align:cente
+00016a70: 723b 2d6d 732d 6772 6964 2d72 6f77 2d61  r;-ms-grid-row-a
+00016a80: 6c69 676e 3a63 656e 7465 723b 616c 6967  lign:center;alig
+00016a90: 6e2d 7365 6c66 3a63 656e 7465 723b 636f  n-self:center;co
+00016aa0: 6c6f 723a 7661 7228 2d2d 6463 612d 6772  lor:var(--dca-gr
+00016ab0: 6179 2d64 6172 6b65 722c 7661 7228 2d2d  ay-darker,var(--
+00016ac0: 626f 6479 2d66 672c 2333 3333 2929 3b66  body-fg,#333));f
+00016ad0: 6f6e 742d 7369 7a65 3a38 3025 3b6d 6172  ont-size:80%;mar
+00016ae0: 6769 6e2d 6c65 6674 3a61 7574 6f7d 2e64  gin-left:auto}.d
+00016af0: 6a61 6e67 6f63 6d73 2d61 646d 696e 2d73  jangocms-admin-s
+00016b00: 7479 6c65 202e 646a 616e 676f 636d 732d  tyle .djangocms-
+00016b10: 6672 6f6e 7465 6e64 206c 692e 6e61 762d  frontend li.nav-
+00016b20: 6974 656d 7b62 6f72 6465 722d 746f 703a  item{border-top:
+00016b30: 6e6f 6e65 7d69 6e70 7574 5b74 7970 653d  none}input[type=
+00016b40: 6e75 6d62 6572 5d2e 6175 746f 2d66 6965  number].auto-fie
+00016b50: 6c64 2b73 7061 6e7b 6469 7370 6c61 793a  ld+span{display:
+00016b60: 6e6f 6e65 3b70 6f73 6974 696f 6e3a 6162  none;position:ab
+00016b70: 736f 6c75 7465 3b62 6f74 746f 6d3a 303b  solute;bottom:0;
+00016b80: 7269 6768 743a 303b 7465 7874 2d61 6c69  right:0;text-ali
+00016b90: 676e 3a72 6967 6874 3b6d 6172 6769 6e2d  gn:right;margin-
+00016ba0: 7269 6768 743a 3331 7078 3b6d 6172 6769  right:31px;margi
+00016bb0: 6e2d 626f 7474 6f6d 3a32 3370 783b 6375  n-bottom:23px;cu
+00016bc0: 7273 6f72 3a70 6f69 6e74 6572 7d62 6f64  rsor:pointer}bod
+00016bd0: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
+00016be0: 2d61 646d 696e 2d73 7479 6c65 2920 696e  -admin-style) in
+00016bf0: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
+00016c00: 2e61 7574 6f2d 6669 656c 642b 7370 616e  .auto-field+span
+00016c10: 7b6d 6172 6769 6e2d 626f 7474 6f6d 3a32  {margin-bottom:2
+00016c20: 3370 787d 406d 6564 6961 2028 6d61 782d  3px}@media (max-
+00016c30: 7769 6474 683a 3130 3234 7078 297b 626f  width:1024px){bo
+00016c40: 6479 3a6e 6f74 282e 646a 616e 676f 636d  dy:not(.djangocm
+00016c50: 732d 6164 6d69 6e2d 7374 796c 6529 2069  s-admin-style) i
+00016c60: 6e70 7574 5b74 7970 653d 6e75 6d62 6572  nput[type=number
+00016c70: 5d2e 6175 746f 2d66 6965 6c64 2b73 7061  ].auto-field+spa
+00016c80: 6e7b 6d61 7267 696e 2d62 6f74 746f 6d3a  n{margin-bottom:
+00016c90: 3234 7078 7d7d 696e 7075 745b 7479 7065  24px}}input[type
+00016ca0: 3d6e 756d 6265 725d 2e61 7574 6f2d 6669  =number].auto-fi
+00016cb0: 656c 642b 7370 616e 3a61 6674 6572 7b63  eld+span:after{c
+00016cc0: 6f6e 7465 6e74 3a22 6175 746f 227d 696e  ontent:"auto"}in
+00016cd0: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
+00016ce0: 2e61 7574 6f2d 6669 656c 642e 6175 746f  .auto-field.auto
+00016cf0: 7b63 6f6c 6f72 3a76 6172 282d 2d64 6361  {color:var(--dca
+00016d00: 2d77 6869 7465 2c76 6172 282d 2d62 6f64  -white,var(--bod
+00016d10: 792d 6267 2c23 6666 6629 293b 6361 7265  y-bg,#fff));care
+00016d20: 742d 636f 6c6f 723a 7661 7228 2d2d 6463  t-color:var(--dc
+00016d30: 612d 626c 6163 6b2c 7661 7228 2d2d 626f  a-black,var(--bo
+00016d40: 6479 2d66 672c 2330 3030 2929 7d69 6e70  dy-fg,#000))}inp
+00016d50: 7574 5b74 7970 653d 6e75 6d62 6572 5d2e  ut[type=number].
+00016d60: 6175 746f 2d66 6965 6c64 2e61 7574 6f2b  auto-field.auto+
+00016d70: 7370 616e 7b64 6973 706c 6179 3a62 6c6f  span{display:blo
+00016d80: 636b 7d                                  ck}
```

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css.map` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/base.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/select2.css` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/select2.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/auto_input.js` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/auto_input.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/django_select2.js` & `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/django_select2.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/base.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/menu.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend.html` & `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend/templatetags/frontend.py` & `djangocms-frontend-1.1.3/djangocms_frontend/templatetags/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend.egg-info/PKG-INFO` & `djangocms-frontend-1.1.3/djangocms_frontend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.2
+Version: 1.1.3
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.2/djangocms_frontend.egg-info/SOURCES.txt` & `djangocms-frontend-1.1.3/djangocms_frontend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/pyproject.toml` & `djangocms-frontend-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/setup.py` & `djangocms-frontend-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/accordion/test_models.py` & `djangocms-frontend-1.1.3/tests/accordion/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/accordion/test_plugins.py` & `djangocms-frontend-1.1.3/tests/accordion/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/alert/test_plugins.py` & `djangocms-frontend-1.1.3/tests/alert/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/badge/test_plugins.py` & `djangocms-frontend-1.1.3/tests/badge/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/card/test_models.py` & `djangocms-frontend-1.1.3/tests/card/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/card/test_plugins.py` & `djangocms-frontend-1.1.3/tests/card/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/carousel/test_models.py` & `djangocms-frontend-1.1.3/tests/carousel/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/carousel/test_plugins.py` & `djangocms-frontend-1.1.3/tests/carousel/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/collapse/test_models.py` & `djangocms-frontend-1.1.3/tests/collapse/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/collapse/test_plugins.py` & `djangocms-frontend-1.1.3/tests/collapse/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/content/test_models.py` & `djangocms-frontend-1.1.3/tests/content/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/content/test_plugins.py` & `djangocms-frontend-1.1.3/tests/content/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/fixtures.py` & `djangocms-frontend-1.1.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/grid/test_models.py` & `djangocms-frontend-1.1.3/tests/grid/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/grid/test_plugins.py` & `djangocms-frontend-1.1.3/tests/grid/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/helpers.py` & `djangocms-frontend-1.1.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/icon/test_models.py` & `djangocms-frontend-1.1.3/tests/icon/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/icon/test_plugins.py` & `djangocms-frontend-1.1.3/tests/icon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/image/test_plugins.py` & `djangocms-frontend-1.1.3/tests/image/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/jumbotron/test_plugins.py` & `djangocms-frontend-1.1.3/tests/jumbotron/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/link/test_plugins.py` & `djangocms-frontend-1.1.3/tests/link/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/listgroup/test_models.py` & `djangocms-frontend-1.1.3/tests/listgroup/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/listgroup/test_plugins.py` & `djangocms-frontend-1.1.3/tests/listgroup/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/media/test_models.py` & `djangocms-frontend-1.1.3/tests/media/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/media/test_plugins.py` & `djangocms-frontend-1.1.3/tests/media/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/navigation/test_models.py` & `djangocms-frontend-1.1.3/tests/navigation/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/navigation/test_plugins.py` & `djangocms-frontend-1.1.3/tests/navigation/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/tabs/test_models.py` & `djangocms-frontend-1.1.3/tests/tabs/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/tabs/test_plugins.py` & `djangocms-frontend-1.1.3/tests/tabs/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/test_constants.py` & `djangocms-frontend-1.1.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/test_fields.py` & `djangocms-frontend-1.1.3/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/test_helpers.py` & `djangocms-frontend-1.1.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/test_migrations.py` & `djangocms-frontend-1.1.3/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/test_settings.py` & `djangocms-frontend-1.1.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/utilities/test_models.py` & `djangocms-frontend-1.1.3/tests/utilities/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.2/tests/utilities/test_plugins.py` & `djangocms-frontend-1.1.3/tests/utilities/test_plugins.py`

 * *Files identical despite different names*


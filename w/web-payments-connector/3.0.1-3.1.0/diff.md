# Comparing `tmp/web-payments-connector-3.0.1.tar.gz` & `tmp/web_payments_connector-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/web-payments-connector-3.0.1.tar", last modified: Wed May  2 12:35:08 2018, max compression
+gzip compressed data, was "web_payments_connector-3.1.0.tar", max compression
```

## Comparing `web-payments-connector-3.0.1.tar` & `web_payments_connector-3.1.0.tar`

### file list

```diff
@@ -1,103 +1,49 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/docs/
--rw-r--r--   0 alex      (1000) alex      (1000)      936 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/Makefile
--rw-r--r--   0 alex      (1000) alex      (1000)     1476 2018-04-26 22:10:54.000000 web-payments-connector-3.0.1/docs/backends.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     5458 2018-04-26 22:42:46.000000 web-payments-connector-3.0.1/docs/conf.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3218 2018-04-26 22:10:54.000000 web-payments-connector-3.0.1/docs/django.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      585 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/index.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     3675 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/install.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      128 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/modules.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     1629 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/preauth.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      551 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/refund.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     2854 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/usage.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      888 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/web_payments.django.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     1176 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/docs/web_payments.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      376 2018-04-26 22:10:54.000000 web-payments-connector-3.0.1/docs/web_payments_dummy.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      442 2018-04-26 22:10:54.000000 web-payments-connector-3.0.1/docs/web_payments_externalpayments.rst
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)    10195 2018-05-02 12:25:40.000000 web-payments-connector-3.0.1/tests/test_core.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3901 2018-05-02 12:24:53.000000 web-payments-connector-3.0.1/tests/test_django.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5331 2018-05-02 12:25:04.000000 web-payments-connector-3.0.1/tests/test_dummy.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2911 2018-05-02 12:25:15.000000 web-payments-connector-3.0.1/tests/test_externalpayments.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/django/
--rw-r--r--   0 alex      (1000) alex      (1000)     2130 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/django/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      319 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/django/apps.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4162 2018-05-01 09:54:00.000000 web-payments-connector-3.0.1/web_payments/django/models.py
--rw-r--r--   0 alex      (1000) alex      (1000)      221 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/django/signals.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3538 2018-05-01 10:08:44.000000 web-payments-connector-3.0.1/web_payments/django/urls.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/locale/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/locale/de/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/locale/de/LC_MESSAGES/
--rw-r--r--   0 alex      (1000) alex      (1000)     1816 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/locale/de/LC_MESSAGES/web_payments.mo
--rw-r--r--   0 alex      (1000) alex      (1000)     2574 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/locale/de/LC_MESSAGES/web_payments.po
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/locale/it/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/locale/it/LC_MESSAGES/
--rw-r--r--   0 alex      (1000) alex      (1000)     1797 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/locale/it/LC_MESSAGES/web_payments.mo
--rw-r--r--   0 alex      (1000) alex      (1000)     2602 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/locale/it/LC_MESSAGES/web_payments.po
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/locale/ru/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments/locale/ru/LC_MESSAGES/
--rw-r--r--   0 alex      (1000) alex      (1000)     2092 2018-05-01 20:03:25.000000 web-payments-connector-3.0.1/web_payments/locale/ru/LC_MESSAGES/web_payments.mo
--rw-r--r--   0 alex      (1000) alex      (1000)     2850 2018-05-01 20:00:08.000000 web-payments-connector-3.0.1/web_payments/locale/ru/LC_MESSAGES/web_payments.po
--rw-r--r--   0 alex      (1000) alex      (1000)     2031 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/locale/web_payments.pot
--rw-r--r--   0 alex      (1000) alex      (1000)     1726 2018-05-01 09:54:00.000000 web-payments-connector-3.0.1/web_payments/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      437 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/_exceptions.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4558 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/forms.py
--rw-r--r--   0 alex      (1000) alex      (1000)    13495 2018-05-02 06:10:02.000000 web-payments-connector-3.0.1/web_payments/logic.py
--rw-r--r--   0 alex      (1000) alex      (1000)      901 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/status.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3243 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/testcommon.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4338 2018-04-26 22:42:46.000000 web-payments-connector-3.0.1/web_payments/translation.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2801 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments/utils.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_connector.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     1052 2018-05-02 12:35:07.000000 web-payments-connector-3.0.1/web_payments_connector.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     2594 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_connector.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2018-05-02 12:35:07.000000 web-payments-connector-3.0.1/web_payments_connector.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2018-03-24 14:03:19.000000 web-payments-connector-3.0.1/web_payments_connector.egg-info/not-zip-safe
--rw-r--r--   0 alex      (1000) alex      (1000)       91 2018-05-02 12:35:07.000000 web-payments-connector-3.0.1/web_payments_connector.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       62 2018-05-02 12:35:07.000000 web-payments-connector-3.0.1/web_payments_connector.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_dummy/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/migrations/
--rw-r--r--   0 alex      (1000) alex      (1000)     3856 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/migrations/0001_initial.py
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/migrations/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/settings/
--rw-r--r--   0 alex      (1000) alex      (1000)       36 2018-04-26 22:42:46.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/settings/.gitignore
--rw-r--r--   0 alex      (1000) alex      (1000)     3981 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/settings/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      461 2018-04-26 22:42:46.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/settings/test.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/static/
--rw-r--r--   0 alex      (1000) alex      (1000)    23293 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/static/w3.css
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/templates/
--rw-r--r--   0 alex      (1000) alex      (1000)     1361 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/templates/base.html
--rw-r--r--   0 alex      (1000) alex      (1000)     1771 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/templates/form.html
--rw-r--r--   0 alex      (1000) alex      (1000)     1372 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/templates/payob.html
--rw-r--r--   0 alex      (1000) alex      (1000)       80 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      151 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/apps.py
--rwxr-xr-x   0 alex      (1000) alex      (1000)      755 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/manage.py
--rw-r--r--   0 alex      (1000) alex      (1000)      582 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/models.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1277 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/urls.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8045 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/views.py
--rw-r--r--   0 alex      (1000) alex      (1000)      621 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/django_dummy/wsgi.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3100 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1085 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_dummy/forms.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_externalpayments/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_externalpayments/locale/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_externalpayments/locale/de/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/web_payments_externalpayments/locale/de/LC_MESSAGES/
--rw-r--r--   0 alex      (1000) alex      (1000)      456 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_externalpayments/locale/de/LC_MESSAGES/web_payments.mo
--rw-r--r--   0 alex      (1000) alex      (1000)      742 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_externalpayments/locale/de/LC_MESSAGES/web_payments.po
--rw-r--r--   0 alex      (1000) alex      (1000)      716 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_externalpayments/locale/web_payments.pot
--rw-r--r--   0 alex      (1000) alex      (1000)     4341 2018-04-26 22:10:54.000000 web-payments-connector-3.0.1/web_payments_externalpayments/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      665 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_externalpayments/forms.py
--rw-r--r--   0 alex      (1000) alex      (1000)      243 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/web_payments_externalpayments/translation.py
--rw-r--r--   0 alex      (1000) alex      (1000)      225 2018-05-02 12:21:58.000000 web-payments-connector-3.0.1/.coveragerc
--rw-r--r--   0 alex      (1000) alex      (1000)     1205 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/.gitignore
--rw-r--r--   0 alex      (1000) alex      (1000)      471 2018-03-23 09:32:45.000000 web-payments-connector-3.0.1/.travis.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1265 2018-03-23 09:32:45.000000 web-payments-connector-3.0.1/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)     1467 2018-03-23 09:32:45.000000 web-payments-connector-3.0.1/LICENSE.mirumee.md
--rw-r--r--   0 alex      (1000) alex      (1000)       96 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)      894 2018-04-20 16:04:15.000000 web-payments-connector-3.0.1/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)      791 2018-04-26 22:42:46.000000 web-payments-connector-3.0.1/doc_settings.py
--rw-r--r--   0 alex      (1000) alex      (1000)       79 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/setup.cfg
--rwxr-xr-x   0 alex      (1000) alex      (1000)     2797 2018-04-26 22:42:46.000000 web-payments-connector-3.0.1/setup.py
--rw-r--r--   0 alex      (1000) alex      (1000)      577 2018-05-02 12:22:51.000000 web-payments-connector-3.0.1/tox.ini
--rw-r--r--   0 alex      (1000) alex      (1000)     1052 2018-05-02 12:35:08.000000 web-payments-connector-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1269 2023-05-26 07:40:07.631298 web_payments_connector-3.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1467 2023-05-26 06:56:14.533665 web_payments_connector-3.1.0/LICENSE.mirumee.md
+-rw-r--r--   0        0        0      894 2023-05-26 06:56:14.533665 web_payments_connector-3.1.0/README.md
+-rw-r--r--   0        0        0     1497 2023-05-26 08:39:05.230952 web_payments_connector-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1640 2023-05-26 08:30:00.073521 web_payments_connector-3.1.0/web_payments/__init__.py
+-rw-r--r--   0        0        0      442 2023-05-26 08:30:08.286798 web_payments_connector-3.1.0/web_payments/_exceptions.py
+-rw-r--r--   0        0        0     2130 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/django/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/django/apps.py
+-rw-r--r--   0        0        0     4282 2023-05-26 08:29:51.223582 web_payments_connector-3.1.0/web_payments/django/models.py
+-rw-r--r--   0        0        0      221 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/django/signals.py
+-rw-r--r--   0        0        0     3688 2023-05-26 08:27:11.764930 web_payments_connector-3.1.0/web_payments/django/urls.py
+-rw-r--r--   0        0        0     4917 2023-05-26 08:31:23.386327 web_payments_connector-3.1.0/web_payments/forms.py
+-rw-r--r--   0        0        0     1816 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/locale/de/LC_MESSAGES/web_payments.mo
+-rw-r--r--   0        0        0     2574 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/locale/de/LC_MESSAGES/web_payments.po
+-rw-r--r--   0        0        0     1797 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/locale/it/LC_MESSAGES/web_payments.mo
+-rw-r--r--   0        0        0     2602 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/locale/it/LC_MESSAGES/web_payments.po
+-rw-r--r--   0        0        0     2092 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/locale/ru/LC_MESSAGES/web_payments.mo
+-rw-r--r--   0        0        0     2850 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/locale/ru/LC_MESSAGES/web_payments.po
+-rw-r--r--   0        0        0     2031 2023-05-26 06:56:14.536998 web_payments_connector-3.1.0/web_payments/locale/web_payments.pot
+-rw-r--r--   0        0        0    13576 2023-05-26 08:30:32.119974 web_payments_connector-3.1.0/web_payments/logic.py
+-rw-r--r--   0        0        0      921 2023-05-26 08:30:40.996585 web_payments_connector-3.1.0/web_payments/status.py
+-rw-r--r--   0        0        0     3657 2023-05-26 08:30:45.469890 web_payments_connector-3.1.0/web_payments/testcommon.py
+-rw-r--r--   0        0        0     4693 2023-05-26 08:30:47.959874 web_payments_connector-3.1.0/web_payments/translation.py
+-rw-r--r--   0        0        0     2889 2023-05-26 08:30:51.196521 web_payments_connector-3.1.0/web_payments/utils.py
+-rw-r--r--   0        0        0     3100 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/__init__.py
+-rw-r--r--   0        0        0       80 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-26 08:36:05.254975 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/apps.py
+-rwxr-xr-x   0        0        0      755 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/manage.py
+-rw-r--r--   0        0        0     3856 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/migrations/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-26 08:31:41.446223 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/models.py
+-rw-r--r--   0        0        0       36 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/settings/.gitignore
+-rw-r--r--   0        0        0     3981 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/settings/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/settings/test.py
+-rw-r--r--   0        0        0    23293 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/static/w3.css
+-rw-r--r--   0        0        0     1361 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/templates/base.html
+-rw-r--r--   0        0        0     1771 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/templates/form.html
+-rw-r--r--   0        0        0     1372 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/templates/payob.html
+-rw-r--r--   0        0        0     1188 2023-05-26 08:26:39.928605 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/urls.py
+-rw-r--r--   0        0        0     8045 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/views.py
+-rw-r--r--   0        0        0      621 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/django_dummy/wsgi.py
+-rw-r--r--   0        0        0     1085 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_dummy/forms.py
+-rw-r--r--   0        0        0     4341 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_externalpayments/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_externalpayments/forms.py
+-rw-r--r--   0        0        0      456 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_externalpayments/locale/de/LC_MESSAGES/web_payments.mo
+-rw-r--r--   0        0        0      742 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_externalpayments/locale/de/LC_MESSAGES/web_payments.po
+-rw-r--r--   0        0        0      716 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_externalpayments/locale/web_payments.pot
+-rw-r--r--   0        0        0      243 2023-05-26 06:56:14.540331 web_payments_connector-3.1.0/web_payments_externalpayments/translation.py
+-rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 web_payments_connector-3.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `web-payments-connector-3.0.1/web_payments/django/__init__.py` & `web_payments_connector-3.1.0/web_payments/django/__init__.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/django/models.py` & `web_payments_connector-3.1.0/web_payments/django/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,103 @@
-
 from decimal import Decimal
 from urllib.parse import urlencode, urljoin
 
 from django.db import models
 from django.conf import settings
 
-try:
-    from django.urls import reverse
-except ImportError:
-    from django.core.urlresolvers import reverse
+from django.urls import reverse
 
 from .. import FraudStatus, PaymentStatus, ProviderVariant
 from ..logic import BasicPayment
 from ..utils import getter_prefixed_address
 from .signals import status_changed
 from . import get_base_url
 
 __all__ = ["BasePayment", "BasePaymentWithAddress"]
 
 
 class BasePayment(models.Model, BasicPayment):
-    '''
+    """
     Represents a single transaction. Each instance has one or more PaymentItem.
-    '''
+    """
+
     # overwrite variant to remove field
     #: select payment provider
     variant = models.CharField(max_length=255)
     #: Transaction status
     status = models.CharField(
-        max_length=10, choices=PaymentStatus.CHOICES,
-        default=PaymentStatus.WAITING)
+        max_length=10,
+        choices=PaymentStatus.CHOICES,
+        default=PaymentStatus.WAITING,
+    )
     #: Transaction status message
-    message = models.TextField(blank=True, default='')
+    message = models.TextField(blank=True, default="")
 
     #: fraud status
     fraud_status = models.CharField(
-        max_length=10, choices=FraudStatus.CHOICES,
-        default=FraudStatus.UNKNOWN)
+        max_length=10, choices=FraudStatus.CHOICES, default=FraudStatus.UNKNOWN
+    )
     #: fraud message
-    fraud_message = models.TextField(blank=True, default='')
+    fraud_message = models.TextField(blank=True, default="")
 
     #: for attrs pseudo dict
-    extra_data = models.TextField(blank=True, default='')
+    extra_data = models.TextField(blank=True, default="")
     #: secret token (for get_process_url)
-    token = models.CharField(max_length=36, blank=True, default='')
+    token = models.CharField(max_length=36, blank=True, default="")
     #: Transaction ID (if applicable)
     transaction_id = models.CharField(max_length=255, blank=True)
 
     #: Currency code (may be provider-specific)
     currency = models.CharField(max_length=10)
     #: Total amount (gross)
-    total = models.DecimalField(max_digits=20, decimal_places=8, default=Decimal('0.0'))
+    total = models.DecimalField(
+        max_digits=20, decimal_places=8, default=Decimal("0.0")
+    )
     #: captured = current captured amount
     captured_amount = models.DecimalField(
-        max_digits=20, decimal_places=8, default=Decimal('0.0'))
+        max_digits=20, decimal_places=8, default=Decimal("0.0")
+    )
 
     #: recommended for audit:
-    #created = models.DateTimeField(auto_now_add=True)
-    #modified = models.DateTimeField(auto_now=True)
+    # created = models.DateTimeField(auto_now_add=True)
+    # modified = models.DateTimeField(auto_now=True)
 
     class Meta:
         abstract = True
 
     def signal_status_change(self):
         status_changed.send(sender=type(self), instance=self)
 
     def get_process_url(self, extra_data=None):
-        url = reverse('process_payment', kwargs={'token': self.token})
+        url = reverse("process_payment", kwargs={"token": self.token})
         url = urljoin(get_base_url(self.provider), url)
         if extra_data:
             qs = urlencode(extra_data)
-            return url + '?' + qs
+            return url + "?" + qs
         return url
 
     @classmethod
     def list_providers(cls, **kwargs):
-        """ returns an iterable with ProviderVariants """
+        """returns an iterable with ProviderVariants"""
+
         def _helper(item):
             t = {"name": item[0]}
             t.update(item[1][2])
             return ProviderVariant(item[1][0], item[1][1], t)
+
         if "name" in kwargs:
             if kwargs["name"] in settings.PAYMENT_VARIANTS_API:
-                return [_helper((kwargs["name"], settings.PAYMENT_VARIANTS_API[kwargs["name"]]))]
+                return [
+                    _helper(
+                        (
+                            kwargs["name"],
+                            settings.PAYMENT_VARIANTS_API[kwargs["name"]],
+                        )
+                    )
+                ]
             else:
                 return []
         else:
             return map(_helper, settings.PAYMENT_VARIANTS_API.items())
 
     @classmethod
     def check_token_exists(cls, token):
@@ -94,15 +105,16 @@
 
     def save(self, **kwargs):
         self.create_token()
         return models.Model.save(self, **kwargs)
 
 
 class BasePaymentWithAddress(BasePayment):
-    """ Has real billing address + shippingaddress alias on billing address """
+    """Has real billing address + shippingaddress alias on billing address"""
+
     get_billing_address = getter_prefixed_address("billing")
     get_shipping_address = get_billing_address
 
     billing_first_name = models.CharField(max_length=256, blank=True)
     billing_last_name = models.CharField(max_length=256, blank=True)
     billing_address_1 = models.CharField(max_length=256, blank=True)
     billing_address_2 = models.CharField(max_length=256, blank=True)
```

### Comparing `web-payments-connector-3.0.1/web_payments/django/urls.py` & `web_payments_connector-3.1.0/web_payments/django/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,67 @@
-'''
+"""
 This module is responsible for automatic processing of provider callback
 data (asynchronous transaction updates).
-'''
+"""
 import logging
 
 import simplejson as json
 import xmltodict
 
-from django.http import Http404, HttpResponseRedirect, HttpResponseServerError, HttpResponse
+from django.http import (
+    Http404,
+    HttpResponseRedirect,
+    HttpResponseServerError,
+    HttpResponse,
+)
 from django.shortcuts import get_object_or_404
 from django.views.decorators.csrf import csrf_exempt
 from django.db.transaction import atomic
-try:
-    from django.urls import re_path as url
-except ImportError:
-    from django.conf.urls import url
+
+from django.urls import re_path
 
 from . import get_payment_model
-from .. import HttpRequest, RedirectNeeded, provider_factory
+from .. import HttpRequest, RedirectNeeded
 
 
 def _process_data(request, payment, provider):
     try:
         # request should have some abstraction
         # redefine django request as namedtuple
         # parse most used content types correct
         if request.method == "GET":
             content = None
-        elif request.content_type in ("application/json", "application/hal+json"):
+        elif request.content_type in (
+            "application/json",
+            "application/hal+json",
+        ):
             content = json.loads(request.body, use_decimal=True)
         elif request.content_type == "application/x-www-form-urlencoded":
             content = request.POST
-        elif request.content_type in ('application/xml', 'application/hal+xml', 'text/xml'):
+        elif request.content_type in (
+            "application/xml",
+            "application/hal+xml",
+            "text/xml",
+        ):
             # I cannot allow people to handle xml themselves
             # You need good security know-how to handle it
             content = xmltodict.parse(request.body)
         else:
             content = request.body
-        reqparsed = HttpRequest(request.method, request.GET, content, request.content_type)
+        reqparsed = HttpRequest(
+            request.method, request.GET, content, request.content_type
+        )
         ret = provider.process_data(payment, reqparsed)
         if ret in (True, False, None):
             status = 200
             if ret is None:
-                logging.error("process_data returned None, reached end of function without returning")
+                logging.error(
+                    "process_data returned None, "
+                    "reached end of function without returning"
+                )
                 status = 500
             elif not ret:
                 status = 404
             return HttpResponse(status=status)
         else:
             content, type = ret
             return HttpResponse(content, type)
@@ -56,46 +71,54 @@
         # for some providers this faces to the banking solution
         # log here for beeing visible
         logging.exception(exc)
         # could contain sensitive data so don't return any information
         # just log
         return HttpResponseServerError()
 
+
 @csrf_exempt
 @atomic
 def process_data(request, token, provider=None):
-    '''
+    """
     Calls process_data of an appropriate provider.
 
     Raises Http404 if variant does not exist.
-    '''
+    """
     Payment = get_payment_model()
     payment = get_object_or_404(Payment, token=token)
     if not provider:
         try:
             provider = payment.provider
         except ValueError:
-            raise Http404('No such provider')
+            raise Http404("No such provider")
     return _process_data(request, payment, provider)
 
+
 @csrf_exempt
 @atomic
 def static_callback(request, variant):
     Payment = get_payment_model()
     try:
         provider = Payment.get_provider(name=variant)
     except ValueError:
-        raise Http404('No such provider')
+        raise Http404("No such provider")
 
     token = provider.get_token_from_request(request=request)
     if not token:
-        raise Http404('Invalid response')
+        raise Http404("Invalid response")
     return process_data(request, token, provider)
 
 
 urlpatterns = [
-    url(r'^process/(?P<token>[0-9a-z]{8}-[0-9a-z]{4}-'
-        '[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12})/$', process_data,
-        name='process_payment'),
-    url(r'^process/(?P<variant>[a-z-]+)/$', static_callback,
-        name='static_process_payment')
-    ]
+    re_path(
+        r"^process/(?P<token>[0-9a-z]{8}-[0-9a-z]{4}-"
+        r"[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12})/$",
+        process_data,
+        name="process_payment",
+    ),
+    re_path(
+        r"^process/(?P<variant>[a-z-]+)/$",
+        static_callback,
+        name="static_process_payment",
+    ),
+]
```

### Comparing `web-payments-connector-3.0.1/web_payments/locale/de/LC_MESSAGES/web_payments.mo` & `web_payments_connector-3.1.0/web_payments/locale/de/LC_MESSAGES/web_payments.mo`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/locale/de/LC_MESSAGES/web_payments.po` & `web_payments_connector-3.1.0/web_payments/locale/de/LC_MESSAGES/web_payments.po`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/locale/it/LC_MESSAGES/web_payments.mo` & `web_payments_connector-3.1.0/web_payments/locale/it/LC_MESSAGES/web_payments.mo`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/locale/it/LC_MESSAGES/web_payments.po` & `web_payments_connector-3.1.0/web_payments/locale/it/LC_MESSAGES/web_payments.po`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/locale/ru/LC_MESSAGES/web_payments.mo` & `web_payments_connector-3.1.0/web_payments/locale/ru/LC_MESSAGES/web_payments.mo`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/locale/ru/LC_MESSAGES/web_payments.po` & `web_payments_connector-3.1.0/web_payments/locale/ru/LC_MESSAGES/web_payments.po`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/locale/web_payments.pot` & `web_payments_connector-3.1.0/web_payments/locale/web_payments.pot`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments/forms.py` & `web_payments_connector-3.1.0/web_payments/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,120 +1,159 @@
-
+__all__ = [
+    "DateValidator",
+    "CreditCardNumberValidator",
+    "PaymentForm",
+    "CreditCardPaymentForm",
+    "CreditCardPaymentFormWithName",
+]
 import datetime
 
 from wtforms import Form, validators, ValidationError
 from wtforms import StringField, DateField
 from wtforms.utils import WebobInputWrapper
 
 from .translation import translation
-_ = translation.gettext_lazy
 
 from .utils import get_credit_card_issuer, DictInputWrapper
 
-__all__ = ["DateValidator", "CreditCardNumberValidator", "PaymentForm", "CreditCardPaymentForm", "CreditCardPaymentFormWithName"]
+_ = translation.gettext_lazy
+
 
 class DateValidator(object):
     def __init__(self, message=None):
         if not message:
-            message = _('Please enter a valid date.')
+            message = _("Please enter a valid date.")
         self.message = message
+
     def __call__(self, form, field):
         data = field.data
         if isinstance(data, str):
-            data = datetime.datetime.strptime(data, '%Y-%m').date()
+            data = datetime.datetime.strptime(data, "%Y-%m").date()
         if not data or data < datetime.date.today():
             raise ValidationError(self.message)
 
+
 class CreditCardNumberValidator(object):
     def __init__(self, message=None):
         if not message:
-            message = _('Please enter a valid card number.')
+            message = _("Please enter a valid card number.")
         self.message = message
 
     def __call__(self, form, field):
         if not self.cart_number_checksum_validation(field.data):
             raise ValidationError(self.message)
 
     @staticmethod
     def cart_number_checksum_validation(number):
         digits = []
         even = False
         if not number.isdigit():
             return False
         for digit in reversed(number):
-            digit = ord(digit) - ord('0')
+            digit = ord(digit) - ord("0")
             if even:
                 digit *= 2
                 if digit >= 10:
                     digit = digit % 10 + digit // 10
             digits.append(digit)
             even = not even
         return sum(digits) % 10 == 0 if digits else False
 
+
 class PaymentForm(Form):
-    '''
+    """
     Payment form
 
     When displaying the form remember to use *action* and *method*.
     use always formdata except for defaults.
     formdata of is different to Wtforms as it supports dicts
-    '''
-    method = 'post'
-    action = ''
+    """
+
+    method = "post"
+    action = ""
     provider = None
     payment = None
 
     class Meta:
         def wrap_formdata(self, form, formdata):
-            """ work around wtform implementation """
-            if formdata is not None and not hasattr(formdata, 'getlist'):
-                if hasattr(formdata, 'getall'):
+            """work around wtform implementation"""
+            if formdata is not None and not hasattr(formdata, "getlist"):
+                if hasattr(formdata, "getall"):
                     return WebobInputWrapper(formdata)
-                elif hasattr(formdata, '__getitem__'): # wtform lacks this
+                elif hasattr(formdata, "__getitem__"):  # wtform lacks this
                     return DictInputWrapper(formdata)
                 else:
-                    raise TypeError("formdata should be a (multi)dict-type wrapper that supports the 'getlist' method")
+                    raise TypeError(
+                        "formdata should be a (multi)dict-type wrapper"
+                        "that supports the 'getlist' method"
+                    )
             return formdata
 
     def __init__(self, *, provider=None, payment=None, **kwargs):
         kwargs["obj"] = payment
         super().__init__(**kwargs)
         self.provider = provider
         self.payment = payment
         if provider and payment:
             self.action = provider.get_action(payment)
 
+
 class CreditCardPaymentForm(PaymentForm):
     # which credit card types are accepted?
     VALID_TYPES = None
 
-    number = StringField(label=_('Credit Card Number'),
-        validators=[validators.InputRequired(), validators.Length(max=32),
-                    CreditCardNumberValidator()],
-        render_kw={'autocomplete': 'cc-number'})
-
-    expiration = DateField(label=_('Expiration date (MM/YYYY):'),
-        validators=[validators.InputRequired(_('Enter a valid expiration date.')), DateValidator()],
-        format='%m/%Y',
-        render_kw={'autocomplete': 'cc-exp', 'pattern': '[0-9]{2}/[0-9]{4}'})
+    number = StringField(
+        label=_("Credit Card Number"),
+        validators=[
+            validators.InputRequired(),
+            validators.Length(max=32),
+            CreditCardNumberValidator(),
+        ],
+        render_kw={"autocomplete": "cc-number"},
+    )
+
+    expiration = DateField(
+        label=_("Expiration date (MM/YYYY):"),
+        validators=[
+            validators.InputRequired(_("Enter a valid expiration date.")),
+            DateValidator(),
+        ],
+        format="%m/%Y",
+        render_kw={"autocomplete": "cc-exp", "pattern": "[0-9]{2}/[0-9]{4}"},
+    )
 
     cvv2 = StringField(
-        label=_('CVV2 Security Number'), validators=[validators.InputRequired(_('Enter a valid security number.')), validators.Regexp('^[0-9]{3,4}$', message=_('Enter a valid security number.'))],
+        label=_("CVV2 Security Number"),
+        validators=[
+            validators.InputRequired(_("Enter a valid security number.")),
+            validators.Regexp(
+                "^[0-9]{3,4}$", message=_("Enter a valid security number.")
+            ),
+        ],
         description=_(
-            'Last three digits located on the back of your card.'
-            ' For American Express the four digits found on the front side.'),
-        render_kw={'autocomplete': 'cc-csc'})
+            "Last three digits located on the back of your card."
+            " For American Express the four digits found on the front side."
+        ),
+        render_kw={"autocomplete": "cc-csc"},
+    )
 
     def __init__(self, *, valid_types=None, **kwargs):
         self.VALID_TYPES = valid_types
         super().__init__(**kwargs)
 
     def validate_number(self, field):
-        if self.VALID_TYPES and get_credit_card_issuer(field.data)[0] not in self.VALID_TYPES:
+        if (
+            self.VALID_TYPES
+            and get_credit_card_issuer(field.data)[0] not in self.VALID_TYPES
+        ):
             raise ValidationError(
-                _('We accept only %(valid_types)s') % {"valid_types": ", ".join(self.VALID_TYPES)})
+                _("We accept only %(valid_types)s")
+                % {"valid_types": ", ".join(self.VALID_TYPES)}
+            )
 
 
 class CreditCardPaymentFormWithName(CreditCardPaymentForm):
-    name = StringField(label=_('Name on Credit Card'),
+    name = StringField(
+        label=_("Name on Credit Card"),
         validators=[validators.Length(max=128)],
-        render_kw={'autocomplete': 'cc-name'})
+        render_kw={"autocomplete": "cc-name"},
+    )
```

### Comparing `web-payments-connector-3.0.1/web_payments/logic.py` & `web_payments_connector-3.1.0/web_payments/logic.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,75 +2,88 @@
 from decimal import Decimal
 import threading
 import logging
 import datetime
 
 import simplejson as json
 
-from . import NotSupported, FraudStatus, PaymentStatus, ProviderVariant, provider_factory, PROVIDER_CACHE
+from . import (
+    NotSupported,
+    FraudStatus,
+    PaymentStatus,
+    provider_factory,
+    PROVIDER_CACHE,
+)
 
 __all__ = ["BasicPayment", "BasicProvider"]
 
+
 class TokenCache(object):
     """
-        threadsafe token cache
-        Should not be accessed by other functions than token
+    threadsafe token cache
+    Should not be accessed by other functions than token
     """
+
     expires = None
     token = None
     lock = None
+
     def __init__(self):
         self.lock = threading.Lock()
 
 
 class PaymentAttributeProxy(object):
     """
-        Access payment extra attributes like an object
+    Access payment extra attributes like an object
     """
+
     _payment = None
 
     def __init__(self, payment=None):
         super().__init__()
         self._payment = payment
 
     def __get__(self, pay_inst, _payment_cls):
         if self._payment or pay_inst is None:
             return self
         if not hasattr(pay_inst, "_payment_attribute_proxy_instance"):
-            pay_inst._payment_attribute_proxy_instance = PaymentAttributeProxy(pay_inst)
+            pay_inst._payment_attribute_proxy_instance = PaymentAttributeProxy(
+                pay_inst
+            )
         return pay_inst._payment_attribute_proxy_instance
 
     @staticmethod
     def __set__(pay_inst, value):
-        """ can assign dict to attrs; updates extra_data """
+        """can assign dict to attrs; updates extra_data"""
         # instance is always a payment object
         # don't use _payment as it could be not initialized yet
         pay_inst.extra_data = json.dumps(value, use_decimal=True)
 
     def __getattr__(self, item):
-        data = json.loads(self._payment.extra_data or '{}')
+        data = json.loads(self._payment.extra_data or "{}")
         try:
             return data[item]
         except KeyError as e:
             raise AttributeError(*e.args)
 
     def __setattr__(self, key, value):
-        if key == '_payment':
+        if key == "_payment":
             return super().__setattr__(key, value)
         try:
             data = json.loads(self._payment.extra_data, use_decimal=True)
         except ValueError:
             data = {}
         data[key] = value
         self.__set__(self._payment, data)
 
+
 class BasicPayment(object):
-    '''
-        Logic of a Payment object, basis for implementations
-    '''
+    """
+    Logic of a Payment object, basis for implementations
+    """
 
     #: select payment provider
     variant = NotImplemented
     #: Transaction status
     status = NotImplemented
     #: Transaction status message
     message = NotImplemented
@@ -90,208 +103,214 @@
     #: Currency code (may be provider-specific)
     currency = NotImplemented
     #: Total amount (gross)
     total = NotImplemented
     #: captured = current captured amount
     captured_amount = NotImplemented
 
-    def change_status(self, status, message=''):
-        '''
-            Updates the Payment status and sends the status_changed signal.
-        '''
+    def change_status(self, status, message=""):
+        """
+        Updates the Payment status and sends the status_changed signal.
+        """
         self.status = status
         self.message = message
         self.save()
         self.signal_status_change()
 
     def signal_status_change(self):
-        '''
-            Called on status change. Should send signal (see django.models for example).
-            must to be overwritten to be useful
-        '''
+        """
+        Called on status change. Should send signal (see django.models for example).
+        must to be overwritten to be useful
+        """
         pass
 
-    def change_fraud_status(self, status, message='', commit=True):
+    def change_fraud_status(self, status, message="", commit=True):
         available_statuses = [choice[0] for choice in FraudStatus.CHOICES]
         if status not in available_statuses:
             raise ValueError(
-                'Wrong status "%s", it should be one of: %s' % (
-                    status, ', '.join(available_statuses)))
+                'Wrong status "%s", it should be one of: %s'
+                % (status, ", ".join(available_statuses))
+            )
         self.fraud_status = status
         self.fraud_message = message
         if commit:
             self.save()
 
     def get_form(self, data=None, **kwargs):
         return self.provider.get_form(self, data=data, **kwargs)
 
     def get_purchased_items(self):
         return []
 
     def get_failure_url(self):
-        '''
-            url where customer should be redirected if payment had an error
-        '''
+        """
+        url where customer should be redirected if payment had an error
+        """
         raise NotImplementedError()
 
     def get_success_url(self):
-        '''
-            url where customer should be redirected if payment was successful
-        '''
+        """
+        url where customer should be redirected if payment was successful
+        """
         raise NotImplementedError()
 
     def get_process_url(self, extra_data=None):
-        '''
-            returns a communication url, should kept secret
-            except if provider communication is with customer
-        '''
+        """
+        returns a communication url, should kept secret
+        except if provider communication is with customer
+        """
         raise NotImplementedError()
 
     @classmethod
     def list_providers(cls, **_kwargs):
-        '''
-            returns an iterable with ProviderVariants
-            possible keywords:
-            name=<variantname>: extract variant, return list with one provider or [], required for static_callback
-        '''
+        """
+        returns an iterable with ProviderVariants
+        possible keywords:
+        name=<variantname>: extract variant, return list with one provider or [], required for static_callback
+        """
         raise NotImplementedError()
 
     @classmethod
     def get_provider(cls, name):
-        '''
-            returns provider object with internal name or None, defaults to cls.list_providers(name=name)
-        '''
+        """
+        returns provider object with internal name or None, defaults to cls.list_providers(name=name)
+        """
         if name in PROVIDER_CACHE:
             return PROVIDER_CACHE[name]
         ret = cls.list_providers(name=name)
         if not ret or not len(ret) == 1:
-            raise ValueError("Invalid provider name/or incorrect implementation")
+            raise ValueError(
+                "Invalid provider name/or incorrect implementation"
+            )
         return provider_factory(ret[0])
 
     @property
     def provider(self):
-        ''' returns provider object '''
+        """returns provider object"""
         return self.get_provider(self.variant)
 
     @classmethod
     def load_providers(cls):
-        '''
-            Load all providers in cache
-            Also useful method to check if all providers are valid
-        '''
+        """
+        Load all providers in cache
+        Also useful method to check if all providers are valid
+        """
         for i in cls.list_providers():
             provider_factory(i)
 
     def get_payment_extra(self):
-        '''
-            extra costs like delivery or tax (required, Decimal), defaults to zero
-            Payment message, minimumage,... (not required, provider SHOULD not depend on it)
-            Overwrite or extend to add functionality
-            universal types:
-            type: what type is the transaction (official, physical, ...), VALID value can be provider dependent
-            message: message for customer
-            minimumage: minimum age for customer
-        '''
-        return {
-            "tax": Decimal("0"),
-            "delivery": Decimal("0")
-        }
+        """
+        extra costs like delivery or tax (required, Decimal), defaults to zero
+        Payment message, minimumage,... (not required, provider SHOULD not depend on it)
+        Overwrite or extend to add functionality
+        universal types:
+        type: what type is the transaction (official, physical, ...), VALID value can be provider dependent
+        message: message for customer
+        minimumage: minimum age for customer
+        """
+        return {"tax": Decimal("0"), "delivery": Decimal("0")}
 
     # needs to be implemented, see BasePaymentWithAddress for an example
     def get_shipping_address(self):
-        ''' return shipping address '''
+        """return shipping address"""
         raise NotImplementedError()
 
     # needs to be implemented, see BasePaymentWithAddress for an example
     def get_billing_address(self):
-        ''' return billing address '''
+        """return billing address"""
         raise NotImplementedError()
 
     def capture(self, amount=None, final=True):
-        '''
-            Capture a fraction of the total amount of a payment.
-            Return amount captured or None
-        '''
+        """
+        Capture a fraction of the total amount of a payment.
+        Return amount captured or None
+        """
         if self.status != PaymentStatus.PREAUTH:
-            raise ValueError(
-                'Only pre-authorized payments can be captured.')
+            raise ValueError("Only pre-authorized payments can be captured.")
         amount = self.provider.capture(self, amount, final)
         if amount is not None:
             self.captured_amount += amount
             if final:
                 self.change_status(PaymentStatus.CONFIRMED)
             else:
                 self.save()
         return amount
 
     def release(self):
-        ''' Annilates captured payment '''
+        """Annilates captured payment"""
         if self.status != PaymentStatus.PREAUTH:
-            raise ValueError(
-                'Only pre-authorized payments can be released.')
+            raise ValueError("Only pre-authorized payments can be released.")
         self.provider.release(self)
         self.captured_amount = Decimal("0")
         self.change_status(PaymentStatus.REFUNDED)
 
     def refund(self, amount=None):
-        ''' Refund payment, return amount which was refunded '''
-        if self.status not in (PaymentStatus.CONFIRMED, PaymentStatus.REFUNDED) or self.captured_amount == 0:
-            raise ValueError(
-                'Only charged payments can be refunded.')
+        """Refund payment, return amount which was refunded"""
+        if (
+            self.status
+            not in (PaymentStatus.CONFIRMED, PaymentStatus.REFUNDED)
+            or self.captured_amount == 0
+        ):
+            raise ValueError("Only charged payments can be refunded.")
         if amount is not None:
             if amount > self.captured_amount:
                 raise ValueError(
-                    'Refund amount can not be greater than captured amount')
+                    "Refund amount can not be greater than captured amount"
+                )
         amount = self.provider.refund(self, amount)
         if amount is not None:
             if amount > self.captured_amount:
                 raise ValueError(
-                    'Provider returned refund amount can not be greater than captured amount')
+                    "Provider returned refund amount can not be greater than captured amount"
+                )
             self.captured_amount -= amount
             if self.status != PaymentStatus.REFUNDED:
                 self.change_status(PaymentStatus.REFUNDED)
             else:
                 self.save()
         return amount
 
     @classmethod
     def check_token_exists(cls, token):
-        ''' create token for process_url '''
+        """create token for process_url"""
         return False
 
     def create_token(self):
         if not self.token:
             tries = set()  # Stores a set of tried values
             while True:
                 token = str(uuid4())
-                if token in tries and len(tries) >= 100:  # After 100 tries we are impliying an infinite loop
-                    raise SystemExit('A possible infinite loop was detected')
+                if (
+                    token in tries and len(tries) >= 100
+                ):  # After 100 tries we are impliying an infinite loop
+                    raise SystemExit("A possible infinite loop was detected")
                 else:
                     if not self.check_token_exists(token):
                         self.token = token
                         break
                 tries.add(token)
 
     # auto initializes, see PaymentAttributeProxy
     attrs = PaymentAttributeProxy()
 
     def save(self, **kwargs):
-        ''' save model implementation dependent '''
+        """save model implementation dependent"""
         raise NotImplementedError()
 
 
 BasePaymentLogic = BasicPayment
 
 
 class BasicProvider(object):
-    '''
-        This class defines the backend provider API. It should not be instantiated directly. Use BasicPayment methods instead.
+    """
+    This class defines the backend provider API. It should not be instantiated directly. Use BasicPayment methods instead.
+
+    :param bool capture: automatic capture of payments, False not supported by all backends
+    """
 
-        :param bool capture: automatic capture of payments, False not supported by all backends
-    '''
     form_class = None
 
     # Replace by dict to provide default arguments, like name for Provider
     # see extra documentation for variant
     extra = None
 
     # class used for token_cache, will be initialized with instance copy in __init__
@@ -301,100 +320,109 @@
     def __init__(self, capture=True):
         self._capture = capture
         if self.token_cache:
             self.token_cache = self.token_cache()
 
     @property
     def token(self):
-        '''
-            Access to authentication token
-        '''
+        """
+        Access to authentication token
+        """
         now = datetime.datetime.now(tz=datetime.timezone.utc)
         if not self.token_cache:
             return self.get_auth_token(now)[0]
         with self.token_cache.lock:
             if not self.token_cache.expires or self.token_cache.expires <= now:
                 self.token_cache.token, expires = self.get_auth_token(now)
                 if not isinstance(expires, datetime.datetime):
-                    raise TypeError("Invalid expire type (requires datetime):  %s, %s", type(expires), expires)
+                    raise TypeError(
+                        "Invalid expire type (requires datetime):  %s, %s",
+                        type(expires),
+                        expires,
+                    )
                 self.token_cache.expires = expires
                 if self.token_cache.expires < now:
-                    logging.warning("now > expire, new expire date is in the past: %s", self.token_cache.expires)
+                    logging.warning(
+                        "now > expire, new expire date is in the past: %s",
+                        self.token_cache.expires,
+                    )
             _token = self.token_cache.token
         return _token
 
     def get_auth_token(self, now):
-        '''
-            Return authentication token, expire date of token for datetime object
+        """
+        Return authentication token, expire date of token for datetime object
 
-            :param datetime now: datetime.now(tz=timezone.UTC) object
-        '''
+        :param datetime now: datetime.now(tz=timezone.UTC) object
+        """
         return NotImplemented, now
 
     def clear_token_cache(self):
-        ''' clear token cache '''
+        """clear token cache"""
         if self.token_cache:
             with self.token_cache.lock:
                 self.token_cache.expires = None
                 self.token_cache.token = None
 
     def get_action(self, payment):
         return ""
 
     def get_form(self, payment, data=None, **kwargs):
-        '''
-            Converts *payment* into a form
+        """
+        Converts *payment* into a form
 
-            :param Payment payment: Payment object
-            :param dict data: data from e.g. Get dictionary
-        '''
+        :param Payment payment: Payment object
+        :param dict data: data from e.g. Get dictionary
+        """
         if not self.form_class:
             raise NotSupported("No form class specified")
-        return self.form_class(formdata=data, provider=self, payment=payment, **kwargs)
+        return self.form_class(
+            formdata=data, provider=self, payment=payment, **kwargs
+        )
 
     def process_data(self, payment, request):
-        '''
-            Process callback request from a payment provider.
-            Default: return 404 if somebody tries it
-
-            :param Payment payment: Payment object
-            :param HttpRequest request: abstracted Http Request
-        '''
+        """
+        Process callback request from a payment provider.
+        Default: return 404 if somebody tries it
+
+        :param Payment payment: Payment object
+        :param HttpRequest request: abstracted Http Request
+        """
         return False
 
     def get_token_from_request(self, request):
-        '''
-            Return payment token from provider request.
+        """
+        Return payment token from provider request.
 
-            :param Payment payment: Payment object
-            :param HttpRequest request: abstracted Http Request
-        '''
+        :param Payment payment: Payment object
+        :param HttpRequest request: abstracted Http Request
+        """
         raise NotImplementedError()
 
     def capture(self, payment, amount=None, final=True):
-        '''
-            Capture a fraction of the total amount of a payment.
-            Return amount captured or None
-
-            :param Payment payment: Payment object
-            :param Decimal amount: amount which should be captured or None for remaining
-            :param bool final: final capturement
-        '''
+        """
+        Capture a fraction of the total amount of a payment.
+        Return amount captured or None
+
+        :param Payment payment: Payment object
+        :param Decimal amount: amount which should be captured or None for remaining
+        :param bool final: final capturement
+        """
         raise NotImplementedError()
 
     def release(self, payment):
-        '''
-            Annilates captured payment
+        """
+        Annilates captured payment
 
-            :param Payment payment: Payment object
-        '''
+        :param Payment payment: Payment object
+        """
         raise NotImplementedError()
 
     def refund(self, payment, amount=None):
-        '''
-            Refund payment, return amount which was refunded
+        """
+        Refund payment, return amount which was refunded
 
-            :param Payment payment: Payment object
-            :param Decimal amount: amount which should be refunded or None for all
-            :param bool final: final capturement
-        '''
+        :param Payment payment: Payment object
+        :param Decimal amount: amount which should be refunded or None for all
+        :param bool final: final capturement
+        """
         raise NotImplementedError()
```

### Comparing `web-payments-connector-3.0.1/web_payments/status.py` & `web_payments_connector-3.1.0/web_payments/status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from .translation import translation
+
 _ = translation.gettext_lazy
 
-#may better include from web_payments
+# may better include from web_payments
 __all__ = []
 
+
 class PaymentStatus:
-    WAITING = 'waiting'
-    PREAUTH = 'preauth'
-    CONFIRMED = 'confirmed'
-    REJECTED = 'rejected' # end status
-    REFUNDED = 'refunded' # end status
-    ERROR = 'error' # end status
-    INPUT = 'input'
+    WAITING = "waiting"
+    PREAUTH = "preauth"
+    CONFIRMED = "confirmed"
+    REJECTED = "rejected"  # end status
+    REFUNDED = "refunded"  # end status
+    ERROR = "error"  # end status
+    INPUT = "input"
 
     CHOICES = [
-        (WAITING, _('Waiting for confirmation')),
-        (PREAUTH, _('Pre-authorized')),
-        (CONFIRMED, _('Confirmed')),
-        (REJECTED, _('Rejected')),
-        (REFUNDED, _('Refunded')),
-        (ERROR, _('Error')),
-        (INPUT, _('Input'))]
+        (WAITING, _("Waiting for confirmation")),
+        (PREAUTH, _("Pre-authorized")),
+        (CONFIRMED, _("Confirmed")),
+        (REJECTED, _("Rejected")),
+        (REFUNDED, _("Refunded")),
+        (ERROR, _("Error")),
+        (INPUT, _("Input")),
+    ]
 
 
 class FraudStatus:
-    UNKNOWN = 'unknown'
-    ACCEPT = 'accept' # end status
-    REJECT = 'reject' # end status
-    REVIEW = 'review'
+    UNKNOWN = "unknown"
+    ACCEPT = "accept"  # end status
+    REJECT = "reject"  # end status
+    REVIEW = "review"
 
     CHOICES = [
-        (UNKNOWN, _('Unknown')),
-        (ACCEPT, _('Passed')),
-        (REJECT, _('Rejected')),
-        (REVIEW, _('Review'))]
+        (UNKNOWN, _("Unknown")),
+        (ACCEPT, _("Passed")),
+        (REJECT, _("Rejected")),
+        (REVIEW, _("Review")),
+    ]
```

### Comparing `web-payments-connector-3.0.1/web_payments/testcommon.py` & `web_payments_connector-3.1.0/web_payments/testcommon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-
 from decimal import Decimal
 from .logic import BasicPayment
 from . import PaymentStatus, PurchasedItem, ProviderVariant
 from .utils import getter_prefixed_address
 
 __all__ = ["create_test_payment"]
 
 PAYMENT_VARIANTS_API = {
-    'default': ('web_payments_dummy.DummyProvider', {}, {}),
-    'DummyProvider': ('web_payments_dummy.DummyProvider', {}, {"test_var": "test"}),
-    'DirectPaymentProvider': ('web_payments_externalpayments.DirectPaymentProvider', {}, {}),
-    'iban': ('web_payments_externalpayments.BankTransferProvider', {
-        "iban": "GL5604449876543210",
-        "bic": "DABAIE2D"}, {"localized_name": "iban"}
-        ),
-    }
-
-def create_test_payment(PAYMENT_VARIANTS_API=PAYMENT_VARIANTS_API, **attributes):
+    "default": ("web_payments_dummy.DummyProvider", {}, {}),
+    "DummyProvider": (
+        "web_payments_dummy.DummyProvider",
+        {},
+        {"test_var": "test"},
+    ),
+    "DirectPaymentProvider": (
+        "web_payments_externalpayments.DirectPaymentProvider",
+        {},
+        {},
+    ),
+    "iban": (
+        "web_payments_externalpayments.BankTransferProvider",
+        {"iban": "GL5604449876543210", "bic": "DABAIE2D"},
+        {"localized_name": "iban"},
+    ),
+}
+
+
+def create_test_payment(
+    PAYMENT_VARIANTS_API=PAYMENT_VARIANTS_API, **attributes
+):
     class TestPayment(BasicPayment):
         id = 523
         pk = id
-        description = 'payment'
-        currency = 'USD'
+        description = "payment"
+        currency = "USD"
         status = PaymentStatus.WAITING
         message = ""
         token = "354338723"
         total = Decimal(100)
         captured_amount = Decimal("0.0")
         extra_data = ""
         variant = "undefined"
@@ -47,46 +58,63 @@
         def __init__(self, **kwargs):
             for key, val in kwargs.items():
                 setattr(self, key, val)
 
         def get_purchased_items(self):
             return [
                 PurchasedItem(
-                    name='foo', quantity=10, price=Decimal('20'),
-                    currency='USD', sku='bar')]
+                    name="foo",
+                    quantity=10,
+                    price=Decimal("20"),
+                    currency="USD",
+                    sku="bar",
+                )
+            ]
 
         @staticmethod
         def _list_providers_helper(item):
             _ndict = {"name": item[0]}
             _ndict.update(item[1][2])
             return ProviderVariant(item[1][0], item[1][1], _ndict)
 
         @classmethod
         def list_providers(cls, **kwargs):
-            """ returns an iterable with ProviderVariants """
+            """returns an iterable with ProviderVariants"""
             if "name" in kwargs:
                 if kwargs["name"] in PAYMENT_VARIANTS_API:
-                    return [cls._list_providers_helper((kwargs["name"], PAYMENT_VARIANTS_API[kwargs["name"]]))]
+                    return [
+                        cls._list_providers_helper(
+                            (
+                                kwargs["name"],
+                                PAYMENT_VARIANTS_API[kwargs["name"]],
+                            )
+                        )
+                    ]
                 return []
-            return map(cls._list_providers_helper, PAYMENT_VARIANTS_API.items())
+            return map(
+                cls._list_providers_helper, PAYMENT_VARIANTS_API.items()
+            )
 
         def get_provider_variant(self):
             variant_tup = PAYMENT_VARIANTS_API[self.variant]
-            variant = ProviderVariant(variant_tup[0], variant_tup[1], {"name": self.variant})
+            variant = ProviderVariant(
+                variant_tup[0], variant_tup[1], {"name": self.variant}
+            )
             variant.extra.update(variant_tup[2])
             return variant
 
         def get_failure_url(self):
-            return 'http://cancel.com'
+            return "http://cancel.com"
 
         def get_process_url(self, extra_data=None):
-            return 'http://example.com/token'
+            return "http://example.com/token"
 
         def get_success_url(self):
-            return 'http://success.com'
+            return "http://success.com"
 
         def save(self, **kwargs):
             pass
+
     # workaround limitation in python
     for key, val in attributes.items():
         setattr(TestPayment, key, val)
     return TestPayment
```

### Comparing `web-payments-connector-3.0.1/web_payments/translation.py` & `web_payments_connector-3.1.0/web_payments/translation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,158 @@
 import os
 import gettext
 import functools
 import threading
 
 
-__all__ = ["web_payments_translation_path", "set_language", "get_language", "Translation", "translation"]
+__all__ = [
+    "web_payments_translation_path",
+    "set_language",
+    "get_language",
+    "Translation",
+    "translation",
+]
+
+web_payments_translation_path = os.path.join(
+    os.path.dirname(__file__), "locale"
+)
 
-web_payments_translation_path = os.path.join(os.path.dirname(__file__), "locale")
 
 class _TLocal(threading.local):
     def __init__(self, **kwargs):
         super().__init__()
         for key, val in kwargs.items():
             setattr(self, key, val)
 
+
 _tlocal = _TLocal(current_language="en")
 
+
 def set_language(language):
-    '''
-        Set language.
-        Default implementation can be overwritten.
-        Note: if get_language is overwritten this method should be also overwritten
-        or not used
-        Note: loading with django overwrites this method if not initialized
+    """
+    Set language.
+    Default implementation can be overwritten.
+    Note: if get_language is overwritten this method should be also overwritten
+    or not used
+    Note: loading with django overwrites this method if not initialized
 
-        :param str language: language to set to
-    '''
+    :param str language: language to set to
+    """
     _tlocal.current_language = language
 
+
 def get_language():
-    '''
-        Get language. For translations.
-        Default implementation can be overwritten.
-        Note: if set_language is overwritten this method should be also overwritten
-        Note: loading with django overwrites this method if not initialized
-    '''
+    """
+    Get language. For translations.
+    Default implementation can be overwritten.
+    Note: if set_language is overwritten this method should be also overwritten
+    Note: loading with django overwrites this method if not initialized
+    """
     return _tlocal.current_language
 
+
 class _lazy_constant(object):
     def __init__(self, func, *args, **kwargs):
         if not callable(func):
             instance_path, func_name = func
             module_path, instance_path = instance_path.rsplit(".", 1)
             module = __import__(
-                str(module_path), globals(), locals(), [str(instance_path)])
+                str(module_path), globals(), locals(), [str(instance_path)]
+            )
             instance_ = getattr(module, instance_path)
             func = getattr(instance_, func_name)
 
         self.func = functools.partial(func, *args, **kwargs)
         # skip partial, provide func
         functools.update_wrapper(self, func)
 
     def deconstruct(self):
-        selfname = ".".join([_lazy_constant.__module__, _lazy_constant.__qualname__])
-        args = [(self.func.func.__self__.instance_path, self.func.func.__qualname__.split(".", 1)[1])]
+        selfname = ".".join(
+            [_lazy_constant.__module__, _lazy_constant.__qualname__]
+        )
+        args = [
+            (
+                self.func.func.__self__.instance_path,
+                self.func.func.__qualname__.split(".", 1)[1],
+            )
+        ]
         # python 3.4 compatibility
         for arg in self.func.args:
             args.append(arg)
         return (selfname, args, self.func.keywords)
 
     def __getattribute__(self, item):
         if item in ("func", "__dict__", "__init__", "deconstruct"):
             return super().__getattribute__(item)
         return self.func().__getattribute__(item)
 
-    def __eq__(self, obj): return self.func().__eq__(obj)
-    def __ne__(self, obj): return self.func().__ne__(obj)
-    def __lt__(self, obj): return self.func().__lt__(obj)
-    def __le__(self, obj): return self.func().__le__(obj)
-    def __gt__(self, obj): return self.func().__gt__(obj)
-    def __ge__(self, obj): return self.func().__ge__(obj)
-    def __iter__(self): return self.func().__iter__()
-    def __len__(self): return self.func().__len__()
-    def __str__(self): return self.func()
-    def __repr__(self): return "'%s'" % self.func()
+    def __eq__(self, obj):
+        return self.func().__eq__(obj)
+
+    def __ne__(self, obj):
+        return self.func().__ne__(obj)
+
+    def __lt__(self, obj):
+        return self.func().__lt__(obj)
+
+    def __le__(self, obj):
+        return self.func().__le__(obj)
+
+    def __gt__(self, obj):
+        return self.func().__gt__(obj)
+
+    def __ge__(self, obj):
+        return self.func().__ge__(obj)
+
+    def __iter__(self):
+        return self.func().__iter__()
+
+    def __len__(self):
+        return self.func().__len__()
+
+    def __str__(self):
+        return self.func()
+
+    def __repr__(self):
+        return "'%s'" % self.func()
+
 
 class Translation(object):
     fallback = None
     domain = None
     instance_path = None
     translation_path = None
-    def __init__(self, instance_path, translation_path, domain="web_payments", fallback=None):
+
+    def __init__(
+        self,
+        instance_path,
+        translation_path,
+        domain="web_payments",
+        fallback=None,
+    ):
         self.translation_path = translation_path
         self.instance_path = instance_path
         self.domain = domain
         if fallback:
             self.fallback = fallback
         else:
             self.fallback = []
 
     @functools.lru_cache(typed=True)
     def _trans(self, lang):
         if lang:
-            return gettext.translation("web_payments", self.translation_path, [lang]+self.fallback, fallback=True)
-        return gettext.translation("web_payments", self.translation_path, self.fallback, fallback=True)
+            return gettext.translation(
+                "web_payments",
+                self.translation_path,
+                [lang] + self.fallback,
+                fallback=True,
+            )
+        return gettext.translation(
+            "web_payments", self.translation_path, self.fallback, fallback=True
+        )
 
     def trans(self, cur_lang=None):
         if not cur_lang:
             cur_lang = get_language()
         return self._trans(cur_lang)
 
     def gettext(self, msg, cur_lang=None):
@@ -108,8 +163,13 @@
 
     def gettext_lazy(self, msg, cur_lang=None):
         return _lazy_constant(self.gettext, msg, cur_lang)
 
     def ngettext_lazy(self, msg, msgplural, n, cur_lang=None):
         return _lazy_constant(self.ngettext, msg, msgplural, n, cur_lang)
 
-translation = Translation("web_payments.translation.translation", web_payments_translation_path, domain="web_payments")
+
+translation = Translation(
+    "web_payments.translation.translation",
+    web_payments_translation_path,
+    domain="web_payments",
+)
```

### Comparing `web-payments-connector-3.0.1/web_payments/utils.py` & `web_payments_connector-3.1.0/web_payments/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,75 @@
 import re
 
-__all__ = ["split_streetnr", "getter_prefixed_address", "CARD_TYPES", "get_credit_card_issuer"]
+__all__ = [
+    "split_streetnr",
+    "getter_prefixed_address",
+    "CARD_TYPES",
+    "get_credit_card_issuer",
+]
 
 _extract_streetnr = re.compile(r"([0-9]+)$")
+
+
 def split_streetnr(address, fallback=None):
     address = address.strip()
     # to prevent regex attacks, limit to 15 chars
     ret = _extract_streetnr.search(address[-15:])
     if ret:
         # use rstrip because left side is stripped already
-        return address[:(ret.start()-15)].rstrip(), ret.group(0)
+        return address[: (ret.start() - 15)].rstrip(), ret.group(0)
     else:
         return address, fallback
 
+
 def getter_prefixed_address(prefix):
-    """ create getter for prefixed address format """
+    """create getter for prefixed address format"""
     email = "{}_email".format(prefix)
     first_name = "{}_first_name".format(prefix)
     last_name = "{}_last_name".format(prefix)
     address_1 = "{}_address_1".format(prefix)
     address_2 = "{}_address_2".format(prefix)
     city = "{}_city".format(prefix)
     postcode = "{}_postcode".format(prefix)
     country_code = "{}_country_code".format(prefix)
     country_area = "{}_country_area".format(prefix)
+
     def _get_address(self):
         return {
             "email": getattr(self, email, None),
             "first_name": getattr(self, first_name, None),
             "last_name": getattr(self, last_name, None),
             "address_1": getattr(self, address_1, None),
             "address_2": getattr(self, address_2, None),
             "city": getattr(self, city, None),
             "postcode": getattr(self, postcode, None),
             "country_code": getattr(self, country_code, None),
-            "country_area": getattr(self, country_area, None)
+            "country_area": getattr(self, country_area, None),
         }
+
     return _get_address
 
 
 CARD_TYPES = [
-    (re.compile(r'^4[0-9]{12}(?:[0-9]{3})?$'), 'visa', 'VISA'),
-    (re.compile(r'^5[1-5][0-9]{14}$'), 'mastercard', 'MasterCard'),
-    (re.compile(r'^6(?:011|5[0-9]{2})[0-9]{12}$'), 'discover', 'Discover'),
-    (re.compile(r'^3[47][0-9]{13}$'), 'amex', 'American Express'),
-    (re.compile(r'^(?:(?:2131|1800|35\d{3})\d{11})$'), 'jcb', 'JCB'),
-    (re.compile(r'^(?:3(?:0[0-5]|[68][0-9])[0-9]{11})$'), 'diners', 'Diners Club'),
-    (re.compile(r'^(?:5[0678]\d\d|6304|6390|67\d\d)\d{8,15}$'), 'maestro', 'Maestro')]
+    (re.compile(r"^4[0-9]{12}(?:[0-9]{3})?$"), "visa", "VISA"),
+    (re.compile(r"^5[1-5][0-9]{14}$"), "mastercard", "MasterCard"),
+    (re.compile(r"^6(?:011|5[0-9]{2})[0-9]{12}$"), "discover", "Discover"),
+    (re.compile(r"^3[47][0-9]{13}$"), "amex", "American Express"),
+    (re.compile(r"^(?:(?:2131|1800|35\d{3})\d{11})$"), "jcb", "JCB"),
+    (
+        re.compile(r"^(?:3(?:0[0-5]|[68][0-9])[0-9]{11})$"),
+        "diners",
+        "Diners Club",
+    ),
+    (
+        re.compile(r"^(?:5[0678]\d\d|6304|6390|67\d\d)\d{8,15}$"),
+        "maestro",
+        "Maestro",
+    ),
+]
 
 
 def get_credit_card_issuer(number):
     for reg, card_type, name in CARD_TYPES:
         if reg.match(number):
             return card_type, name
     return None, None
@@ -67,14 +86,14 @@
     def __iter__(self):
         return iter(self._wrapped)
 
     def __len__(self):
         return len(self._wrapped)
 
     def __contains__(self, name):
-        return (name in self._wrapped)
+        return name in self._wrapped
 
     def getlist(self, name, default=None):
         if name in self._wrapped:
             return [self._wrapped[name]]
         else:
             return default
```

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/migrations/0001_initial.py` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/settings/__init__.py` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/static/w3.css` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/static/w3.css`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/templates/base.html` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/templates/base.html`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/templates/form.html` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/templates/form.html`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/templates/payob.html` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/templates/payob.html`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/manage.py` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/manage.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/models.py` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 from django.urls import reverse
 from django.db import models
 
 from web_payments.django import get_base_url
 from web_payments.django.models import BasePaymentWithAddress
 
+
 class QPayment(BasePaymentWithAddress):
     class Meta:
-        ordering = ['-id']
+        ordering = ["-id"]
+
     created = models.DateTimeField(auto_now_add=True)
     modified = models.DateTimeField(auto_now=True)
 
     def get_success_url(self):
         return urljoin(get_base_url(), reverse("select-form"))
 
     def get_failure_url(self):
```

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/urls.py` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,23 @@
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.contrib import admin
-try:
-    from django.urls import include
-    from django.urls import path_re as url
-except ImportError:
-    from django.conf.urls import url
-    from django.conf.urls import include
+from django.urls import include
+from django.urls import path, re_path
 
 from web_payments.django import urls as web_payment_urls
 from .views import PaymentView, PayObView, SelectView
 
 
 urlpatterns = [
-    url('^admin/', admin.site.urls),
-    url('^payment/', include(web_payment_urls)),
-    url('^payob/(?P<id>[0-9]+)/$', PayObView.as_view(), name="paymentob"),
-    url('^form/(?P<id>[0-9]+)/$', PaymentView.as_view(), name="payment-form"),
-    url('', SelectView.as_view(), name="select-form"),
+    path("admin/", admin.site.urls),
+    path("payment/", include(web_payment_urls)),
+    re_path("^payob/(?P<id>[0-9]+)/$", PayObView.as_view(), name="paymentob"),
+    re_path(
+        "^form/(?P<id>[0-9]+)/$", PaymentView.as_view(), name="payment-form"
+    ),
+    path("", SelectView.as_view(), name="select-form"),
 ]
```

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/views.py` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/views.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/django_dummy/wsgi.py` & `web_payments_connector-3.1.0/web_payments_dummy/django_dummy/wsgi.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/__init__.py` & `web_payments_connector-3.1.0/web_payments_dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_dummy/forms.py` & `web_payments_connector-3.1.0/web_payments_dummy/forms.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_externalpayments/locale/de/LC_MESSAGES/web_payments.po` & `web_payments_connector-3.1.0/web_payments_externalpayments/locale/de/LC_MESSAGES/web_payments.po`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_externalpayments/locale/web_payments.pot` & `web_payments_connector-3.1.0/web_payments_externalpayments/locale/web_payments.pot`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_externalpayments/__init__.py` & `web_payments_connector-3.1.0/web_payments_externalpayments/__init__.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/web_payments_externalpayments/forms.py` & `web_payments_connector-3.1.0/web_payments_externalpayments/forms.py`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/LICENSE.md` & `web_payments_connector-3.1.0/LICENSE.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Copyright (c) 2018, Alexander Kaftan
+Copyright (c) 2018-2023, Alexander Kaftan
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright
    notice, this list of conditions and the following disclaimer in the
    documentation and/or other materials provided with the distribution.
 
-
 THIS SOFTWARE IS PROVIDED BY MIRUMEE SOFTWARE ''AS IS'' AND ANY
 EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL MIRUMEE SOFTWARE BE LIABLE FOR ANY
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
```

### Comparing `web-payments-connector-3.0.1/LICENSE.mirumee.md` & `web_payments_connector-3.1.0/LICENSE.mirumee.md`

 * *Files identical despite different names*

### Comparing `web-payments-connector-3.0.1/README.md` & `web_payments_connector-3.1.0/README.md`

 * *Files identical despite different names*


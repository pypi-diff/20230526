# Comparing `tmp/django-adminactions-2.0.0.tar.gz` & `tmp/django-adminactions-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-adminactions-2.0.0.tar", last modified: Sun Jun 26 16:34:05 2022, max compression
+gzip compressed data, was "django-adminactions-2.1.0.tar", last modified: Fri May 26 13:32:37 2023, max compression
```

## Comparing `django-adminactions-2.0.0.tar` & `django-adminactions-2.1.0.tar`

### file list

```diff
@@ -1,190 +1,218 @@
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.113650 django-adminactions-2.0.0/
--rw-r--r--   0 sax        (501) staff       (20)     1304 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/AUTHORS.rst
--rw-r--r--   0 sax        (501) staff       (20)     7965 2022-06-26 16:06:34.000000 django-adminactions-2.0.0/CHANGES
--rw-r--r--   0 sax        (501) staff       (20)     1220 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/LICENSE
--rw-r--r--   0 sax        (501) staff       (20)      588 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/MANIFEST.in
--rw-r--r--   0 sax        (501) staff       (20)     1429 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/Makefile
--rw-r--r--   0 sax        (501) staff       (20)     2200 2022-06-26 16:34:05.113817 django-adminactions-2.0.0/PKG-INFO
--rw-r--r--   0 sax        (501) staff       (20)     1276 2022-06-26 14:34:53.000000 django-adminactions-2.0.0/README.md
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.991012 django-adminactions-2.0.0/docs/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.014237 django-adminactions-2.0.0/docs/source/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.017395 django-adminactions-2.0.0/docs/source/_ext/
--rw-r--r--   0 sax        (501) staff       (20)     7192 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/docs/source/_ext/djangodocs.py
--rw-r--r--   0 sax        (501) staff       (20)     5338 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/docs/source/_ext/github.py
--rw-r--r--   0 sax        (501) staff       (20)     2350 2017-05-30 13:47:59.000000 django-adminactions-2.0.0/docs/source/_ext/version.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.026689 django-adminactions-2.0.0/docs/source/_static/
--rw-r--r--   0 sax        (501) staff       (20)   109338 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/_static/export_as_csv.png
--rw-r--r--   0 sax        (501) staff       (20)    15635 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/_static/export_as_fixture.png
--rw-r--r--   0 sax        (501) staff       (20)    21663 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/_static/graph_bar.png
--rw-r--r--   0 sax        (501) staff       (20)    41344 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/_static/graph_pie.png
--rw-r--r--   0 sax        (501) staff       (20)    32269 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/_static/mass_update.png
--rw-r--r--   0 sax        (501) staff       (20)    47396 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/_static/merge_1.png
--rw-r--r--   0 sax        (501) staff       (20)    26901 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/_static/merge_2.png
--rw-r--r--   0 sax        (501) staff       (20)    11434 2022-06-26 16:02:30.000000 django-adminactions-2.0.0/docs/source/actions.rst
--rw-r--r--   0 sax        (501) staff       (20)     4474 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/docs/source/api.rst
--rw-r--r--   0 sax        (501) staff       (20)       31 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/docs/source/authors.rst
--rw-r--r--   0 sax        (501) staff       (20)      202 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/changes.rst
--rw-r--r--   0 sax        (501) staff       (20)     8723 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/docs/source/conf.py
--rw-r--r--   0 sax        (501) staff       (20)     3192 2017-06-12 19:48:51.000000 django-adminactions-2.0.0/docs/source/contributing.rst
--rw-r--r--   0 sax        (501) staff       (20)      176 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/docs/source/exceptions.rst
--rw-r--r--   0 sax        (501) staff       (20)     2151 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/faq.rst
--rw-r--r--   0 sax        (501) staff       (20)      340 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/docs/source/globals.rst
--rw-r--r--   0 sax        (501) staff       (20)     2022 2021-06-26 05:51:23.000000 django-adminactions-2.0.0/docs/source/howto.rst
--rw-r--r--   0 sax        (501) staff       (20)     1193 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/docs/source/index.rst
--rw-r--r--   0 sax        (501) staff       (20)     1912 2021-08-12 16:42:17.000000 django-adminactions-2.0.0/docs/source/install.rst
--rw-r--r--   0 sax        (501) staff       (20)      523 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/docs/source/permissions.rst
--rw-r--r--   0 sax        (501) staff       (20)     2801 2017-05-30 13:47:34.000000 django-adminactions-2.0.0/docs/source/signals.rst
--rw-r--r--   0 sax        (501) staff       (20)      488 2022-06-26 16:34:05.114579 django-adminactions-2.0.0/setup.cfg
--rwxr-xr-x   0 sax        (501) staff       (20)     1956 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/setup.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.995511 django-adminactions-2.0.0/src/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.039170 django-adminactions-2.0.0/src/adminactions/
--rw-r--r--   0 sax        (501) staff       (20)      109 2022-06-26 16:07:54.000000 django-adminactions-2.0.0/src/adminactions/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     1190 2022-06-26 14:34:53.000000 django-adminactions-2.0.0/src/adminactions/actions.py
--rw-r--r--   0 sax        (501) staff       (20)    18962 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/api.py
--rw-r--r--   0 sax        (501) staff       (20)      402 2022-06-11 05:52:34.000000 django-adminactions-2.0.0/src/adminactions/apps.py
--rw-r--r--   0 sax        (501) staff       (20)     4360 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/src/adminactions/byrows_update.py
--rw-r--r--   0 sax        (501) staff       (20)      995 2022-06-11 11:25:44.000000 django-adminactions-2.0.0/src/adminactions/checks.py
--rw-r--r--   0 sax        (501) staff       (20)      403 2022-06-11 11:25:37.000000 django-adminactions-2.0.0/src/adminactions/compat.py
--rw-r--r--   0 sax        (501) staff       (20)      244 2022-06-11 05:52:34.000000 django-adminactions-2.0.0/src/adminactions/config.py
--rw-r--r--   0 sax        (501) staff       (20)      311 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/src/adminactions/consts.py
--rw-r--r--   0 sax        (501) staff       (20)     5301 2022-06-26 14:34:53.000000 django-adminactions-2.0.0/src/adminactions/duplicates.py
--rw-r--r--   0 sax        (501) staff       (20)      230 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/adminactions/exceptions.py
--rw-r--r--   0 sax        (501) staff       (20)    17240 2022-06-26 16:02:30.000000 django-adminactions-2.0.0/src/adminactions/export.py
--rw-r--r--   0 sax        (501) staff       (20)     4202 2022-06-26 16:02:30.000000 django-adminactions-2.0.0/src/adminactions/forms.py
--rw-r--r--   0 sax        (501) staff       (20)     7716 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/graph.py
--rw-r--r--   0 sax        (501) staff       (20)     2839 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/src/adminactions/helpers.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.993258 django-adminactions-2.0.0/src/adminactions/locale/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.991910 django-adminactions-2.0.0/src/adminactions/locale/en/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.039864 django-adminactions-2.0.0/src/adminactions/locale/en/LC_MESSAGES/
--rw-r--r--   0 sax        (501) staff       (20)    15925 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.992198 django-adminactions-2.0.0/src/adminactions/locale/es/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.040918 django-adminactions-2.0.0/src/adminactions/locale/es/LC_MESSAGES/
--rw-r--r--   0 sax        (501) staff       (20)    17327 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.992466 django-adminactions-2.0.0/src/adminactions/locale/fr/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.042243 django-adminactions-2.0.0/src/adminactions/locale/fr/LC_MESSAGES/
--rw-r--r--   0 sax        (501) staff       (20)    17313 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.992686 django-adminactions-2.0.0/src/adminactions/locale/it/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.043331 django-adminactions-2.0.0/src/adminactions/locale/it/LC_MESSAGES/
--rw-r--r--   0 sax        (501) staff       (20)    17026 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.993014 django-adminactions-2.0.0/src/adminactions/locale/pl/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.044289 django-adminactions-2.0.0/src/adminactions/locale/pl/LC_MESSAGES/
--rw-r--r--   0 sax        (501) staff       (20)    17263 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.993360 django-adminactions-2.0.0/src/adminactions/locale/pt_BR/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.045524 django-adminactions-2.0.0/src/adminactions/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 sax        (501) staff       (20)    20169 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.046563 django-adminactions-2.0.0/src/adminactions/management/
--rw-r--r--   0 sax        (501) staff       (20)        0 2021-06-26 08:44:42.000000 django-adminactions-2.0.0/src/adminactions/management/__init__.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.047295 django-adminactions-2.0.0/src/adminactions/management/commands/
--rw-r--r--   0 sax        (501) staff       (20)        0 2021-06-26 08:44:42.000000 django-adminactions-2.0.0/src/adminactions/management/commands/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      216 2021-06-26 08:44:42.000000 django-adminactions-2.0.0/src/adminactions/management/commands/create_extra_permissions.py
--rw-r--r--   0 sax        (501) staff       (20)    20290 2022-06-11 11:27:18.000000 django-adminactions-2.0.0/src/adminactions/mass_update.py
--rw-r--r--   0 sax        (501) staff       (20)     8405 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/merge.py
--rw-r--r--   0 sax        (501) staff       (20)      526 2022-06-11 06:35:59.000000 django-adminactions-2.0.0/src/adminactions/models.py
--rw-r--r--   0 sax        (501) staff       (20)     1659 2022-06-11 11:25:44.000000 django-adminactions-2.0.0/src/adminactions/perms.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.049082 django-adminactions-2.0.0/src/adminactions/requirements/
--rw-r--r--   0 sax        (501) staff       (20)       93 2018-11-30 21:35:12.000000 django-adminactions-2.0.0/src/adminactions/requirements/develop.pip
--rw-r--r--   0 sax        (501) staff       (20)        0 2018-11-30 21:35:12.000000 django-adminactions-2.0.0/src/adminactions/requirements/install.py2.pip
--rw-r--r--   0 sax        (501) staff       (20)        0 2018-11-30 21:35:12.000000 django-adminactions-2.0.0/src/adminactions/requirements/install.py3.pip
--rw-r--r--   0 sax        (501) staff       (20)      161 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/adminactions/signals.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.994041 django-adminactions-2.0.0/src/adminactions/static/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:04.994282 django-adminactions-2.0.0/src/adminactions/static/adminactions/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.049826 django-adminactions-2.0.0/src/adminactions/static/adminactions/css/
--rw-r--r--   0 sax        (501) staff       (20)      746 2022-06-26 16:02:30.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/css/adminactions.css
--rw-r--r--   0 sax        (501) staff       (20)      269 2022-06-10 19:20:37.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/css/massupdate.css
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.054564 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/
--rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/export.js
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.059614 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/
--rw-r--r--   0 sax        (501) staff       (20)     1082 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/MIT-LICENSE.txt
--rw-r--r--   0 sax        (501) staff       (20)     3175 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/README.txt
--rw-r--r--   0 sax        (501) staff       (20)     5624 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.css
--rw-r--r--   0 sax        (501) staff       (20)     3522 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.css
--rw-r--r--   0 sax        (501) staff       (20)   172372 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.js
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.067525 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/
--rw-r--r--   0 sax        (501) staff       (20)    34731 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.js
--rw-r--r--   0 sax        (501) staff       (20)    13314 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.min.js
--rw-r--r--   0 sax        (501) staff       (20)    28563 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.js
--rw-r--r--   0 sax        (501) staff       (20)     9669 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.min.js
--rw-r--r--   0 sax        (501) staff       (20)    35545 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.js
--rw-r--r--   0 sax        (501) staff       (20)    13537 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.min.js
--rw-r--r--   0 sax        (501) staff       (20)     2132 2022-06-10 11:11:52.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/massupdate.js
--rw-r--r--   0 sax        (501) staff       (20)     1487 2022-06-10 11:11:52.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/massupdate.min.js
--rw-r--r--   0 sax        (501) staff       (20)     3689 2022-06-10 18:52:29.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/merge.js
--rw-r--r--   0 sax        (501) staff       (20)     2448 2022-06-10 18:52:29.000000 django-adminactions-2.0.0/src/adminactions/static/adminactions/js/merge.min.js
--rw-r--r--   0 sax        (501) staff       (20)      526 2022-06-11 06:49:41.000000 django-adminactions-2.0.0/src/adminactions/tasks.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.068468 django-adminactions-2.0.0/src/adminactions/templates/
--rw-r--r--   0 sax        (501) staff       (20)      177 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/src/adminactions/templates/500.html
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.075427 django-adminactions-2.0.0/src/adminactions/templates/adminactions/
--rw-r--r--   0 sax        (501) staff       (20)     3445 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/any_model.html
--rw-r--r--   0 sax        (501) staff       (20)     2807 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/byrows_update.html
--rw-r--r--   0 sax        (501) staff       (20)     1991 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/charts.html
--rw-r--r--   0 sax        (501) staff       (20)     1418 2022-06-26 14:34:53.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/duplicates.html
--rw-r--r--   0 sax        (501) staff       (20)    12888 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/export_csv.html
--rw-r--r--   0 sax        (501) staff       (20)      994 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/export_fixture.html
--rw-r--r--   0 sax        (501) staff       (20)     1436 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/export_xls.html
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.076364 django-adminactions-2.0.0/src/adminactions/templates/adminactions/helpers/
--rw-r--r--   0 sax        (501) staff       (20)      872 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/helpers/import_fixture.html
--rw-r--r--   0 sax        (501) staff       (20)     3098 2022-06-10 19:25:02.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/mass_update.html
--rw-r--r--   0 sax        (501) staff       (20)     3459 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/merge.html
--rw-r--r--   0 sax        (501) staff       (20)     1658 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templates/adminactions/merge_preview.html
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.079538 django-adminactions-2.0.0/src/adminactions/templatetags/
--rw-r--r--   0 sax        (501) staff       (20)        0 2018-01-30 09:22:13.000000 django-adminactions-2.0.0/src/adminactions/templatetags/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      185 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/src/adminactions/templatetags/aa_compat.py
--rw-r--r--   0 sax        (501) staff       (20)      567 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/adminactions/templatetags/actions.py
--rw-r--r--   0 sax        (501) staff       (20)     2898 2022-06-11 11:27:18.000000 django-adminactions-2.0.0/src/adminactions/templatetags/massupdate.py
--rw-r--r--   0 sax        (501) staff       (20)     1206 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/adminactions/templatetags/merge.py
--rw-r--r--   0 sax        (501) staff       (20)      163 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/adminactions/urls.py
--rw-r--r--   0 sax        (501) staff       (20)     9228 2022-06-26 14:34:53.000000 django-adminactions-2.0.0/src/adminactions/utils.py
--rw-r--r--   0 sax        (501) staff       (20)      229 2021-07-05 06:32:27.000000 django-adminactions-2.0.0/src/adminactions/views.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.084375 django-adminactions-2.0.0/src/django_adminactions.egg-info/
--rw-r--r--   0 sax        (501) staff       (20)     2200 2022-06-26 16:34:04.000000 django-adminactions-2.0.0/src/django_adminactions.egg-info/PKG-INFO
--rw-r--r--   0 sax        (501) staff       (20)     5330 2022-06-26 16:34:04.000000 django-adminactions-2.0.0/src/django_adminactions.egg-info/SOURCES.txt
--rw-r--r--   0 sax        (501) staff       (20)        1 2022-06-26 16:34:04.000000 django-adminactions-2.0.0/src/django_adminactions.egg-info/dependency_links.txt
--rw-r--r--   0 sax        (501) staff       (20)        1 2022-02-24 06:03:49.000000 django-adminactions-2.0.0/src/django_adminactions.egg-info/not-zip-safe
--rw-r--r--   0 sax        (501) staff       (20)      752 2022-06-26 16:34:04.000000 django-adminactions-2.0.0/src/django_adminactions.egg-info/requires.txt
--rw-r--r--   0 sax        (501) staff       (20)       13 2022-06-26 16:34:04.000000 django-adminactions-2.0.0/src/django_adminactions.egg-info/top_level.txt
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.086406 django-adminactions-2.0.0/src/requirements/
--rw-r--r--   0 sax        (501) staff       (20)       47 2021-07-05 06:32:27.000000 django-adminactions-2.0.0/src/requirements/develop.pip
--rw-r--r--   0 sax        (501) staff       (20)       22 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/src/requirements/install.pip
--rw-r--r--   0 sax        (501) staff       (20)       31 2022-02-24 06:52:56.000000 django-adminactions-2.0.0/src/requirements/rtd.pip
--rw-r--r--   0 sax        (501) staff       (20)      297 2022-06-11 06:29:42.000000 django-adminactions-2.0.0/src/requirements/testing.pip
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.098925 django-adminactions-2.0.0/tests/
--rw-r--r--   0 sax        (501) staff       (20)      687 2017-06-12 19:48:51.000000 django-adminactions-2.0.0/tests/.coveragerc
--rw-r--r--   0 sax        (501) staff       (20)     4041 2022-06-08 18:10:37.000000 django-adminactions-2.0.0/tests/conftest.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.105233 django-adminactions-2.0.0/tests/demo/
--rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/tests/demo/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      160 2022-06-09 06:49:14.000000 django-adminactions-2.0.0/tests/demo/apps.py
--rw-r--r--   0 sax        (501) staff       (20)      449 2022-06-11 11:25:48.000000 django-adminactions-2.0.0/tests/demo/celery.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.107316 django-adminactions-2.0.0/tests/demo/fixtures/
--rw-r--r--   0 sax        (501) staff       (20)     6629 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/tests/demo/fixtures/adminactions.json
--rw-r--r--   0 sax        (501) staff       (20)     2435 2021-06-26 08:44:42.000000 django-adminactions-2.0.0/tests/demo/fixtures/demoproject.json
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.108608 django-adminactions-2.0.0/tests/demo/media/
--rw-r--r--   0 sax        (501) staff       (20)        0 2017-06-12 19:48:51.000000 django-adminactions-2.0.0/tests/demo/media/first.png
--rw-r--r--   0 sax        (501) staff       (20)        0 2017-06-12 19:48:51.000000 django-adminactions-2.0.0/tests/demo/media/second.png
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.109694 django-adminactions-2.0.0/tests/demo/migrations/
--rw-r--r--   0 sax        (501) staff       (20)     2826 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/demo/migrations/0001_initial.py
--rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/tests/demo/migrations/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     2675 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/demo/models.py
--rw-r--r--   0 sax        (501) staff       (20)     5597 2022-06-11 11:25:48.000000 django-adminactions-2.0.0/tests/demo/settings.py
--rw-r--r--   0 sax        (501) staff       (20)     7080 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/demo/storage.py
--rw-r--r--   0 sax        (501) staff       (20)      308 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/tests/demo/urls.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2022-06-26 16:34:05.112746 django-adminactions-2.0.0/tests/selenium_tests/
--rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.0.0/tests/selenium_tests/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     1724 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/selenium_tests/conftest.py
--rw-r--r--   0 sax        (501) staff       (20)     1955 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/selenium_tests/test_export_csv.py
--rw-r--r--   0 sax        (501) staff       (20)      545 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/tests/selenium_tests/test_export_xls.py
--rw-r--r--   0 sax        (501) staff       (20)     1180 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/tests/selenium_tests/test_mass_update.py
--rw-r--r--   0 sax        (501) staff       (20)     6390 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/test_api.py
--rw-r--r--   0 sax        (501) staff       (20)     4596 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/test_byrows_update.py
--rw-r--r--   0 sax        (501) staff       (20)     4474 2022-06-26 14:34:53.000000 django-adminactions-2.0.0/tests/test_duplicates.py
--rw-r--r--   0 sax        (501) staff       (20)    18340 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/test_exports.py
--rw-r--r--   0 sax        (501) staff       (20)     2188 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/tests/test_graph.py
--rw-r--r--   0 sax        (501) staff       (20)     4499 2022-06-11 11:26:08.000000 django-adminactions-2.0.0/tests/test_mass_update.py
--rw-r--r--   0 sax        (501) staff       (20)    17330 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/test_merge.py
--rw-r--r--   0 sax        (501) staff       (20)     2370 2022-06-26 14:34:53.000000 django-adminactions-2.0.0/tests/test_permissions.py
--rw-r--r--   0 sax        (501) staff       (20)      676 2021-06-26 05:44:50.000000 django-adminactions-2.0.0/tests/test_templatetags.py
--rw-r--r--   0 sax        (501) staff       (20)     2313 2022-06-10 18:46:35.000000 django-adminactions-2.0.0/tests/test_transaction.py
--rw-r--r--   0 sax        (501) staff       (20)      991 2022-02-24 06:51:10.000000 django-adminactions-2.0.0/tests/test_utils.py
--rw-r--r--   0 sax        (501) staff       (20)      529 2021-07-15 08:51:27.000000 django-adminactions-2.0.0/tests/test_views.py
--rw-r--r--   0 sax        (501) staff       (20)    11076 2022-06-11 11:26:08.000000 django-adminactions-2.0.0/tests/utils.py
--rw-r--r--   0 sax        (501) staff       (20)     1734 2022-06-11 06:42:55.000000 django-adminactions-2.0.0/tox.ini
--rwxr-xr-x   0 sax        (501) staff       (20)     2104 2021-07-15 07:58:56.000000 django-adminactions-2.0.0/~setup.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.620591 django-adminactions-2.1.0/
+-rw-r--r--   0 sax        (501) staff       (20)     1273 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/AUTHORS.rst
+-rw-r--r--   0 sax        (501) staff       (20)     8655 2023-05-26 11:07:59.000000 django-adminactions-2.1.0/CHANGES
+-rw-r--r--   0 sax        (501) staff       (20)     1220 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/LICENSE
+-rw-r--r--   0 sax        (501) staff       (20)      588 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/MANIFEST.in
+-rw-r--r--   0 sax        (501) staff       (20)     1747 2023-05-26 11:23:15.000000 django-adminactions-2.1.0/Makefile
+-rw-r--r--   0 sax        (501) staff       (20)     2212 2023-05-26 13:32:37.620814 django-adminactions-2.1.0/PKG-INFO
+-rw-r--r--   0 sax        (501) staff       (20)     1290 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/README.md
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.491837 django-adminactions-2.1.0/docs/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.519357 django-adminactions-2.1.0/docs/source/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.521977 django-adminactions-2.1.0/docs/source/_ext/
+-rw-r--r--   0 sax        (501) staff       (20)     7192 2022-06-26 16:35:57.000000 django-adminactions-2.1.0/docs/source/_ext/djangodocs.py
+-rw-r--r--   0 sax        (501) staff       (20)     5338 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/docs/source/_ext/github.py
+-rw-r--r--   0 sax        (501) staff       (20)     2350 2017-05-30 13:47:59.000000 django-adminactions-2.1.0/docs/source/_ext/version.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.535751 django-adminactions-2.1.0/docs/source/_static/
+-rw-r--r--   0 sax        (501) staff       (20)   151544 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/docs/source/_static/bulk_update.png
+-rw-r--r--   0 sax        (501) staff       (20)   186636 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/docs/source/_static/byrows_update.png
+-rw-r--r--   0 sax        (501) staff       (20)   109338 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/_static/export_as_csv.png
+-rw-r--r--   0 sax        (501) staff       (20)    15635 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/_static/export_as_fixture.png
+-rw-r--r--   0 sax        (501) staff       (20)   132535 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/docs/source/_static/find_duplicates.png
+-rw-r--r--   0 sax        (501) staff       (20)    21663 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/_static/graph_bar.png
+-rw-r--r--   0 sax        (501) staff       (20)    41344 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/_static/graph_pie.png
+-rw-r--r--   0 sax        (501) staff       (20)    32269 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/_static/mass_update.png
+-rw-r--r--   0 sax        (501) staff       (20)    47396 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/_static/merge_1.png
+-rw-r--r--   0 sax        (501) staff       (20)    26901 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/_static/merge_2.png
+-rw-r--r--   0 sax        (501) staff       (20)    12387 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/docs/source/actions.rst
+-rw-r--r--   0 sax        (501) staff       (20)     4474 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/docs/source/api.rst
+-rw-r--r--   0 sax        (501) staff       (20)       31 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/docs/source/authors.rst
+-rw-r--r--   0 sax        (501) staff       (20)      202 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/changes.rst
+-rw-r--r--   0 sax        (501) staff       (20)     8723 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/docs/source/conf.py
+-rw-r--r--   0 sax        (501) staff       (20)     3192 2017-06-12 19:48:51.000000 django-adminactions-2.1.0/docs/source/contributing.rst
+-rw-r--r--   0 sax        (501) staff       (20)      176 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/docs/source/exceptions.rst
+-rw-r--r--   0 sax        (501) staff       (20)     2151 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/faq.rst
+-rw-r--r--   0 sax        (501) staff       (20)      340 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/docs/source/globals.rst
+-rw-r--r--   0 sax        (501) staff       (20)     2022 2021-06-26 05:51:23.000000 django-adminactions-2.1.0/docs/source/howto.rst
+-rw-r--r--   0 sax        (501) staff       (20)     1193 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/docs/source/index.rst
+-rw-r--r--   0 sax        (501) staff       (20)     1912 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/docs/source/install.rst
+-rw-r--r--   0 sax        (501) staff       (20)      523 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/docs/source/permissions.rst
+-rw-r--r--   0 sax        (501) staff       (20)     2801 2017-05-30 13:47:34.000000 django-adminactions-2.1.0/docs/source/signals.rst
+-rw-r--r--   0 sax        (501) staff       (20)      488 2023-05-26 13:32:37.621366 django-adminactions-2.1.0/setup.cfg
+-rwxr-xr-x   0 sax        (501) staff       (20)     1956 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/setup.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.498749 django-adminactions-2.1.0/src/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.553303 django-adminactions-2.1.0/src/adminactions/
+-rw-r--r--   0 sax        (501) staff       (20)      109 2023-05-26 11:40:55.000000 django-adminactions-2.1.0/src/adminactions/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     1171 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/actions.py
+-rw-r--r--   0 sax        (501) staff       (20)    19212 2023-05-26 11:31:10.000000 django-adminactions-2.1.0/src/adminactions/api.py
+-rw-r--r--   0 sax        (501) staff       (20)      522 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/apps.py
+-rw-r--r--   0 sax        (501) staff       (20)    11744 2023-05-26 11:31:10.000000 django-adminactions-2.1.0/src/adminactions/bulk_update.py
+-rw-r--r--   0 sax        (501) staff       (20)     4448 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/byrows_update.py
+-rw-r--r--   0 sax        (501) staff       (20)     1245 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/checks.py
+-rw-r--r--   0 sax        (501) staff       (20)      403 2023-05-25 17:28:14.000000 django-adminactions-2.1.0/src/adminactions/compat.py
+-rw-r--r--   0 sax        (501) staff       (20)      250 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/config.py
+-rw-r--r--   0 sax        (501) staff       (20)      262 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/consts.py
+-rw-r--r--   0 sax        (501) staff       (20)     5049 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/duplicates.py
+-rw-r--r--   0 sax        (501) staff       (20)      230 2021-06-26 05:44:50.000000 django-adminactions-2.1.0/src/adminactions/exceptions.py
+-rw-r--r--   0 sax        (501) staff       (20)    16818 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/export.py
+-rw-r--r--   0 sax        (501) staff       (20)     5189 2023-05-26 11:31:10.000000 django-adminactions-2.1.0/src/adminactions/forms.py
+-rw-r--r--   0 sax        (501) staff       (20)     7958 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/graph.py
+-rw-r--r--   0 sax        (501) staff       (20)     2932 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/helpers.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.495794 django-adminactions-2.1.0/src/adminactions/locale/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.493800 django-adminactions-2.1.0/src/adminactions/locale/en/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.553946 django-adminactions-2.1.0/src/adminactions/locale/en/LC_MESSAGES/
+-rw-r--r--   0 sax        (501) staff       (20)    15925 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.494274 django-adminactions-2.1.0/src/adminactions/locale/es/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.554747 django-adminactions-2.1.0/src/adminactions/locale/es/LC_MESSAGES/
+-rw-r--r--   0 sax        (501) staff       (20)    17327 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.494615 django-adminactions-2.1.0/src/adminactions/locale/fr/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.555639 django-adminactions-2.1.0/src/adminactions/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 sax        (501) staff       (20)    17313 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.495040 django-adminactions-2.1.0/src/adminactions/locale/it/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.556254 django-adminactions-2.1.0/src/adminactions/locale/it/LC_MESSAGES/
+-rw-r--r--   0 sax        (501) staff       (20)    17026 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.495551 django-adminactions-2.1.0/src/adminactions/locale/pl/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.556759 django-adminactions-2.1.0/src/adminactions/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 sax        (501) staff       (20)    17263 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.495943 django-adminactions-2.1.0/src/adminactions/locale/pt_BR/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.557851 django-adminactions-2.1.0/src/adminactions/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 sax        (501) staff       (20)    20169 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.558981 django-adminactions-2.1.0/src/adminactions/management/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2021-06-26 08:44:42.000000 django-adminactions-2.1.0/src/adminactions/management/__init__.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.559525 django-adminactions-2.1.0/src/adminactions/management/commands/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2021-06-26 08:44:42.000000 django-adminactions-2.1.0/src/adminactions/management/commands/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      217 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/management/commands/create_extra_permissions.py
+-rw-r--r--   0 sax        (501) staff       (20)    22114 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/mass_update.py
+-rw-r--r--   0 sax        (501) staff       (20)     9537 2023-05-26 11:31:10.000000 django-adminactions-2.1.0/src/adminactions/merge.py
+-rw-r--r--   0 sax        (501) staff       (20)      516 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/models.py
+-rw-r--r--   0 sax        (501) staff       (20)     1838 2023-05-26 09:17:30.000000 django-adminactions-2.1.0/src/adminactions/perms.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.561104 django-adminactions-2.1.0/src/adminactions/requirements/
+-rw-r--r--   0 sax        (501) staff       (20)       93 2018-11-30 21:35:12.000000 django-adminactions-2.1.0/src/adminactions/requirements/develop.pip
+-rw-r--r--   0 sax        (501) staff       (20)        0 2018-11-30 21:35:12.000000 django-adminactions-2.1.0/src/adminactions/requirements/install.py2.pip
+-rw-r--r--   0 sax        (501) staff       (20)        0 2018-11-30 21:35:12.000000 django-adminactions-2.1.0/src/adminactions/requirements/install.py3.pip
+-rw-r--r--   0 sax        (501) staff       (20)      161 2021-06-26 05:44:50.000000 django-adminactions-2.1.0/src/adminactions/signals.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.496935 django-adminactions-2.1.0/src/adminactions/static/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.497277 django-adminactions-2.1.0/src/adminactions/static/adminactions/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.562211 django-adminactions-2.1.0/src/adminactions/static/adminactions/css/
+-rw-r--r--   0 sax        (501) staff       (20)      746 2022-06-26 16:36:26.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/css/adminactions.css
+-rw-r--r--   0 sax        (501) staff       (20)      269 2022-06-26 16:36:26.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/css/massupdate.css
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.565652 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/
+-rw-r--r--   0 sax        (501) staff       (20)     1293 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/bulkupdate.js
+-rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/export.js
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.569196 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/
+-rw-r--r--   0 sax        (501) staff       (20)     1082 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/MIT-LICENSE.txt
+-rw-r--r--   0 sax        (501) staff       (20)     3175 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/README.txt
+-rw-r--r--   0 sax        (501) staff       (20)     5624 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.css
+-rw-r--r--   0 sax        (501) staff       (20)     3522 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.css
+-rw-r--r--   0 sax        (501) staff       (20)   172372 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.js
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.575634 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/
+-rw-r--r--   0 sax        (501) staff       (20)    34732 2023-05-26 09:13:03.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.js
+-rw-r--r--   0 sax        (501) staff       (20)    13314 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.min.js
+-rw-r--r--   0 sax        (501) staff       (20)    28563 2023-05-26 09:13:03.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.js
+-rw-r--r--   0 sax        (501) staff       (20)     9669 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.min.js
+-rw-r--r--   0 sax        (501) staff       (20)    35546 2023-05-26 09:13:03.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.js
+-rw-r--r--   0 sax        (501) staff       (20)    13537 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.min.js
+-rw-r--r--   0 sax        (501) staff       (20)     2136 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/massupdate.js
+-rw-r--r--   0 sax        (501) staff       (20)     1487 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/massupdate.min.js
+-rw-r--r--   0 sax        (501) staff       (20)     3689 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/merge.js
+-rw-r--r--   0 sax        (501) staff       (20)     2448 2022-06-10 18:52:29.000000 django-adminactions-2.1.0/src/adminactions/static/adminactions/js/merge.min.js
+-rw-r--r--   0 sax        (501) staff       (20)      527 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/tasks.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.576296 django-adminactions-2.1.0/src/adminactions/templates/
+-rw-r--r--   0 sax        (501) staff       (20)      177 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/src/adminactions/templates/500.html
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.581112 django-adminactions-2.1.0/src/adminactions/templates/adminactions/
+-rw-r--r--   0 sax        (501) staff       (20)     3445 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/any_model.html
+-rw-r--r--   0 sax        (501) staff       (20)     3173 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/bulk_update.html
+-rw-r--r--   0 sax        (501) staff       (20)     2824 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/byrows_update.html
+-rw-r--r--   0 sax        (501) staff       (20)     2008 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/charts.html
+-rw-r--r--   0 sax        (501) staff       (20)     1418 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/duplicates.html
+-rw-r--r--   0 sax        (501) staff       (20)    12905 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/export_csv.html
+-rw-r--r--   0 sax        (501) staff       (20)     1011 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/export_fixture.html
+-rw-r--r--   0 sax        (501) staff       (20)     1453 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/export_xls.html
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.581720 django-adminactions-2.1.0/src/adminactions/templates/adminactions/helpers/
+-rw-r--r--   0 sax        (501) staff       (20)      872 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/helpers/import_fixture.html
+-rw-r--r--   0 sax        (501) staff       (20)     3158 2023-05-26 10:29:18.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/mass_update.html
+-rw-r--r--   0 sax        (501) staff       (20)     3475 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/merge.html
+-rw-r--r--   0 sax        (501) staff       (20)     1674 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templates/adminactions/merge_preview.html
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.583846 django-adminactions-2.1.0/src/adminactions/templatetags/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2018-01-30 09:22:13.000000 django-adminactions-2.1.0/src/adminactions/templatetags/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      186 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templatetags/aa_compat.py
+-rw-r--r--   0 sax        (501) staff       (20)      555 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templatetags/actions.py
+-rw-r--r--   0 sax        (501) staff       (20)     2817 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/templatetags/massupdate.py
+-rw-r--r--   0 sax        (501) staff       (20)     1206 2021-06-26 05:44:50.000000 django-adminactions-2.1.0/src/adminactions/templatetags/merge.py
+-rw-r--r--   0 sax        (501) staff       (20)      163 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/adminactions/urls.py
+-rw-r--r--   0 sax        (501) staff       (20)     9195 2023-05-26 11:31:10.000000 django-adminactions-2.1.0/src/adminactions/utils.py
+-rw-r--r--   0 sax        (501) staff       (20)      229 2023-05-26 11:31:06.000000 django-adminactions-2.1.0/src/adminactions/views.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.586835 django-adminactions-2.1.0/src/django_adminactions.egg-info/
+-rw-r--r--   0 sax        (501) staff       (20)     2212 2023-05-26 13:32:37.000000 django-adminactions-2.1.0/src/django_adminactions.egg-info/PKG-INFO
+-rw-r--r--   0 sax        (501) staff       (20)     6296 2023-05-26 13:32:37.000000 django-adminactions-2.1.0/src/django_adminactions.egg-info/SOURCES.txt
+-rw-r--r--   0 sax        (501) staff       (20)        1 2023-05-26 13:32:37.000000 django-adminactions-2.1.0/src/django_adminactions.egg-info/dependency_links.txt
+-rw-r--r--   0 sax        (501) staff       (20)        1 2022-02-24 06:03:49.000000 django-adminactions-2.1.0/src/django_adminactions.egg-info/not-zip-safe
+-rw-r--r--   0 sax        (501) staff       (20)      771 2023-05-26 13:32:37.000000 django-adminactions-2.1.0/src/django_adminactions.egg-info/requires.txt
+-rw-r--r--   0 sax        (501) staff       (20)       13 2023-05-26 13:32:37.000000 django-adminactions-2.1.0/src/django_adminactions.egg-info/top_level.txt
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.588173 django-adminactions-2.1.0/src/requirements/
+-rw-r--r--   0 sax        (501) staff       (20)       62 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/requirements/develop.pip
+-rw-r--r--   0 sax        (501) staff       (20)       22 2021-06-26 05:44:50.000000 django-adminactions-2.1.0/src/requirements/install.pip
+-rw-r--r--   0 sax        (501) staff       (20)       31 2022-06-26 16:36:09.000000 django-adminactions-2.1.0/src/requirements/rtd.pip
+-rw-r--r--   0 sax        (501) staff       (20)      299 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/src/requirements/testing.pip
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.598475 django-adminactions-2.1.0/tests/
+-rw-r--r--   0 sax        (501) staff       (20)      687 2017-06-12 19:48:51.000000 django-adminactions-2.1.0/tests/.coveragerc
+-rw-r--r--   0 sax        (501) staff       (20)       45 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/bulk_update.csv
+-rw-r--r--   0 sax        (501) staff       (20)     3968 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/conftest.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.601891 django-adminactions-2.1.0/tests/demo/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/tests/demo/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      222 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/demo/apps.py
+-rw-r--r--   0 sax        (501) staff       (20)      575 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/demo/backends.py
+-rw-r--r--   0 sax        (501) staff       (20)      552 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/demo/celery.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.603218 django-adminactions-2.1.0/tests/demo/fixtures/
+-rw-r--r--   0 sax        (501) staff       (20)     6629 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/tests/demo/fixtures/adminactions.json
+-rw-r--r--   0 sax        (501) staff       (20)     2435 2021-06-26 08:44:42.000000 django-adminactions-2.1.0/tests/demo/fixtures/demoproject.json
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.617571 django-adminactions-2.1.0/tests/demo/media/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2017-06-12 19:48:51.000000 django-adminactions-2.1.0/tests/demo/media/first.png
+-rw-r--r--   0 sax        (501) staff       (20)        0 2017-06-12 19:48:51.000000 django-adminactions-2.1.0/tests/demo/media/second.png
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:26:32.000000 django-adminactions-2.1.0/tests/demo/media/test.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:28:09.000000 django-adminactions-2.1.0/tests/demo/media/test_9gUcdqc.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:27:42.000000 django-adminactions-2.1.0/tests/demo/media/test_9qyuDfv.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:29:02.000000 django-adminactions-2.1.0/tests/demo/media/test_I3DMvoi.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:28:09.000000 django-adminactions-2.1.0/tests/demo/media/test_JsO7xeM.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:29:02.000000 django-adminactions-2.1.0/tests/demo/media/test_M6mqKom.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:27:10.000000 django-adminactions-2.1.0/tests/demo/media/test_OTXH5S5.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:27:10.000000 django-adminactions-2.1.0/tests/demo/media/test_S3U5A2n.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:28:35.000000 django-adminactions-2.1.0/tests/demo/media/test_SnwP8Qj.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:27:10.000000 django-adminactions-2.1.0/tests/demo/media/test_Tj4qRIO.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:29:02.000000 django-adminactions-2.1.0/tests/demo/media/test_eTNypv4.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:26:32.000000 django-adminactions-2.1.0/tests/demo/media/test_lPNAXvh.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:28:09.000000 django-adminactions-2.1.0/tests/demo/media/test_mlG9HTK.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:26:32.000000 django-adminactions-2.1.0/tests/demo/media/test_q0gyVTr.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:28:35.000000 django-adminactions-2.1.0/tests/demo/media/test_u224GIR.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:27:42.000000 django-adminactions-2.1.0/tests/demo/media/test_vrXhmUq.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:27:42.000000 django-adminactions-2.1.0/tests/demo/media/test_wT3a4sy.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 13:28:35.000000 django-adminactions-2.1.0/tests/demo/media/test_zY9mZJC.jpeg
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.618559 django-adminactions-2.1.0/tests/demo/migrations/
+-rw-r--r--   0 sax        (501) staff       (20)     3958 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/demo/migrations/0001_initial.py
+-rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/tests/demo/migrations/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     2686 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/demo/models.py
+-rw-r--r--   0 sax        (501) staff       (20)     5918 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/demo/settings.py
+-rw-r--r--   0 sax        (501) staff       (20)     7058 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/demo/storage.py
+-rw-r--r--   0 sax        (501) staff       (20)      346 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/demo/urls.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-26 13:32:37.620293 django-adminactions-2.1.0/tests/selenium_tests/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2017-05-30 13:50:17.000000 django-adminactions-2.1.0/tests/selenium_tests/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     1707 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/selenium_tests/conftest.py
+-rw-r--r--   0 sax        (501) staff       (20)     1983 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/selenium_tests/test_export_csv.py
+-rw-r--r--   0 sax        (501) staff       (20)      559 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/selenium_tests/test_export_xls.py
+-rw-r--r--   0 sax        (501) staff       (20)     1194 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/selenium_tests/test_mass_update.py
+-rw-r--r--   0 sax        (501) staff       (20)     8896 2023-05-26 10:22:40.000000 django-adminactions-2.1.0/tests/test.jpeg
+-rw-r--r--   0 sax        (501) staff       (20)     6523 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_api.py
+-rw-r--r--   0 sax        (501) staff       (20)     7880 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_bulk_update.py
+-rw-r--r--   0 sax        (501) staff       (20)     4753 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/test_byrows_update.py
+-rw-r--r--   0 sax        (501) staff       (20)     4498 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/test_duplicates.py
+-rw-r--r--   0 sax        (501) staff       (20)    18691 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_exports.py
+-rw-r--r--   0 sax        (501) staff       (20)     2290 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/test_graph.py
+-rw-r--r--   0 sax        (501) staff       (20)     5977 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_mass_update.py
+-rw-r--r--   0 sax        (501) staff       (20)    18942 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_merge.py
+-rw-r--r--   0 sax        (501) staff       (20)     2249 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_permissions.py
+-rw-r--r--   0 sax        (501) staff       (20)      561 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_templatetags.py
+-rw-r--r--   0 sax        (501) staff       (20)     2397 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/test_transaction.py
+-rw-r--r--   0 sax        (501) staff       (20)     1118 2023-05-26 05:23:58.000000 django-adminactions-2.1.0/tests/test_utils.py
+-rw-r--r--   0 sax        (501) staff       (20)      530 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/test_views.py
+-rw-r--r--   0 sax        (501) staff       (20)    10862 2023-05-26 11:31:52.000000 django-adminactions-2.1.0/tests/utils.py
+-rw-r--r--   0 sax        (501) staff       (20)     1827 2023-05-26 11:45:24.000000 django-adminactions-2.1.0/tox.ini
+-rwxr-xr-x   0 sax        (501) staff       (20)     2104 2021-07-15 07:58:56.000000 django-adminactions-2.1.0/~setup.py
```

### Comparing `django-adminactions-2.0.0/AUTHORS.rst` & `django-adminactions-2.1.0/AUTHORS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 * ipmb (`@ipmb`_)
 * Peter Baumgartner (`@ipmb`_)
 * BoscoMW  (`@Mbosco`_)
 * Bertrand Bordage  (`@BertrandBordage`_)
 * jht001 (`@jht001`_)
 * Cesar Abel (`@xangmuve`_)
 * Viator (`@viatoriche`_)
-* Serhiy Zahoriya (`@int-ua`_)
 * Pavel Savchenko (`@asfaltboy`_)
 * Petr Kůdela (`@PetrKudy`_)
 * Bastien Vallet (`@Djailla`_)
 
 .. _`@PetrKudy`: https://github.com/PetrKudy
 .. _`@tdruez`: https://github.com/tdruez
 .. _`@jht001`: https://github.com/jht001
```

### Comparing `django-adminactions-2.0.0/CHANGES` & `django-adminactions-2.1.0/CHANGES`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Release 2.1
+===========
+* new action "Bulk Update"
+* add support for ImageField / FileField
+* add Django 4.1 support
+* add Python 3.11 support
+* Use Black for code formatting
+* Merged #212 - Inspect the MRO (in reversed order) - https://github.com/saxix/django-adminactions/pull/212
+* Merged #215 - Merge action support signals  - https://github.com/saxix/django-adminactions/pull/212
+* Merged #207 - work with any collection to ignore fields - https://github.com/saxix/django-adminactions/pull/207
+* Merged #206 - docs: Fix a few typos - https://github.com/saxix/django-adminactions/pull/206
+* Merged #200 - Very lame fix for #199 - https://github.com/saxix/django-adminactions/pull/200
+
+
 Release 2.0
 ===========
 * new action "Find Duplicates"
 * allows customization of exportable columns (`get_exportable_columns(request)`)
 * allows customization od ExportForm (`get_export_form(request, export_type)`)
 * Add Admin logging support (LogEntry)
 * add Celery support
```

### Comparing `django-adminactions-2.0.0/LICENSE` & `django-adminactions-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/MANIFEST.in` & `django-adminactions-2.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/PKG-INFO` & `django-adminactions-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-adminactions
-Version: 2.0.0
+Version: 2.1.0
 Summary: Collections of useful actions to use with django.contrib.admin.ModelAdmin
 Home-page: https://github.com/saxix/django-adminactions
+Download-URL: https://github.com/saxix/django-adminactions
 Author: sax
 Author-email: s.apostolico@gmail.com
 License: MIT
-Download-URL: https://github.com/saxix/django-adminactions
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -45,18 +45,17 @@
 * Export as Excel
 * Export as fixture
 * Export delete tree
 * Mass update records
 * Graph queryset
 * Merge records
 * Find Duplicates
+* Bulk Update
 
 
 #### Project Links
 
 
 - Code: https://github.com/saxix/django-adminactions
 - Documentation: https://django-adminactions.readthedocs.org/en/latest/
 - Issue Tracker: https://github.com/saxix/django-adminactions/issues?sort
 - Download Package: https://pypi.org/project/django-adminactions/
-
-
```

### Comparing `django-adminactions-2.0.0/README.md` & `django-adminactions-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 * Export as Excel
 * Export as fixture
 * Export delete tree
 * Mass update records
 * Graph queryset
 * Merge records
 * Find Duplicates
+* Bulk Update
 
 
 #### Project Links
 
 
 - Code: https://github.com/saxix/django-adminactions
 - Documentation: https://django-adminactions.readthedocs.org/en/latest/
```

### Comparing `django-adminactions-2.0.0/docs/source/_ext/djangodocs.py` & `django-adminactions-2.1.0/docs/source/_ext/djangodocs.py`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_ext/github.py` & `django-adminactions-2.1.0/docs/source/_ext/github.py`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_ext/version.py` & `django-adminactions-2.1.0/docs/source/_ext/version.py`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_static/export_as_csv.png` & `django-adminactions-2.1.0/docs/source/_static/export_as_csv.png`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_static/export_as_fixture.png` & `django-adminactions-2.1.0/docs/source/_static/export_as_fixture.png`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_static/graph_bar.png` & `django-adminactions-2.1.0/docs/source/_static/graph_bar.png`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_static/graph_pie.png` & `django-adminactions-2.1.0/docs/source/_static/graph_pie.png`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_static/mass_update.png` & `django-adminactions-2.1.0/docs/source/_static/mass_update.png`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_static/merge_1.png` & `django-adminactions-2.1.0/docs/source/_static/merge_1.png`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/_static/merge_2.png` & `django-adminactions-2.1.0/docs/source/_static/merge_2.png`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/actions.rst` & `django-adminactions-2.1.0/docs/source/actions.rst`

 * *Files 7% similar despite different names*

```diff
@@ -346,18 +346,63 @@
 
 **Limitations/TODO**
 
 - merge doesn't work for models related with ``on_delete=Protect`` (see :ghissue:`85`)
 
 
 ``Ignore Fields``
-------------------------
+-----------------
 .. versionadded:: 1.9
 
 It is possible to prevent some fields to be displayed to avoid merge.
 To filter out some fields you need to set `MERGE_ACTION_IGNORED_FIELDS` settings parameter as follow::
 
     MERGE_ACTION_IGNORED_FIELDS = {
         'app_name': {
                 'user': ['is_staff', 'is_superuser'],
         },
     }
+
+``By Rows Update``
+=================
+
+.. versionadded:: 2.0
+
+Dynamycally enable changelist editing
+
+**Screenshots**
+
+.. figure:: _static/byrows_update.png
+
+
+
+``Find Duplicates``
+==================
+
+.. versionadded:: 2.0
+
+Find duplicated records.
+
+Note: This can be used to count records based on simple grouping
+
+
+======================= ===========================================================================================
+**min**                 only reports duplicates more than <value>
+**max**                 only reports duplicates less than <value>
+**fields**              selection of fields to be used to detect duplicates
+======================= ===========================================================================================
+
+**Screenshots**
+
+.. figure:: _static/find_duplicates.png
+
+
+
+``Bulk Update``
+==================
+
+.. versionadded:: 1.1
+
+Updates queryset using csv file
+
+**Screenshots**
+.. figure:: _static/bulk_update.png
```

### Comparing `django-adminactions-2.0.0/docs/source/api.rst` & `django-adminactions-2.1.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/conf.py` & `django-adminactions-2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/contributing.rst` & `django-adminactions-2.1.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/faq.rst` & `django-adminactions-2.1.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/howto.rst` & `django-adminactions-2.1.0/docs/source/howto.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/index.rst` & `django-adminactions-2.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/install.rst` & `django-adminactions-2.1.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/permissions.rst` & `django-adminactions-2.1.0/docs/source/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/docs/source/signals.rst` & `django-adminactions-2.1.0/docs/source/signals.rst`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/setup.py` & `django-adminactions-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/actions.py` & `django-adminactions-2.1.0/src/adminactions/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+from .bulk_update import bulk_update
 from .byrows_update import byrows_update
 from .duplicates import find_duplicates_action
-from .export import (export_as_csv, export_as_fixture,
-                     export_as_xls, export_delete_tree,)
+from .export import export_as_csv, export_as_fixture, export_as_xls, export_delete_tree
 from .graph import graph_queryset
 from .mass_update import mass_update
 from .merge import merge
 
-actions = [export_as_fixture,
-           export_as_csv,
-           export_as_xls,
-           export_delete_tree,
-           find_duplicates_action,
-           merge,
-           mass_update,
-           graph_queryset,
-           byrows_update]
+actions = [
+    export_as_fixture,
+    export_as_csv,
+    export_as_xls,
+    export_delete_tree,
+    find_duplicates_action,
+    merge,
+    mass_update,
+    graph_queryset,
+    bulk_update,
+    byrows_update,
+]
 
 
 def add_to_site(site, exclude=None, include=None):
     """
     Register all the adminactions into passed site
 
     :param site: AdminSite instance
```

### Comparing `django-adminactions-2.0.0/src/adminactions/api.py` & `django-adminactions-2.1.0/src/adminactions/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import collections
 import csv
 import datetime
 import itertools
+from io import BytesIO
+
 import xlwt
 from django.conf import settings
 from django.core.exceptions import FieldDoesNotExist, ObjectDoesNotExist
 from django.db.models import FileField
 from django.db.models.fields.related import ManyToManyField, OneToOneField
 from django.db.transaction import atomic
 from django.http import HttpResponse, StreamingHttpResponse
 from django.utils import dateformat
 from django.utils.encoding import force_str, smart_str
 from django.utils.timezone import get_default_timezone
-from io import BytesIO
 
 from adminactions import utils
 
-from .utils import (clone_instance, get_field_by_path,
-                    get_field_value, get_ignored_fields,)
-
-csv_options_default = {'date_format': 'd/m/Y',
-                       'datetime_format': 'N j, Y, P',
-                       'time_format': 'P',
-                       'header': False,
-                       'quotechar': '"',
-                       'quoting': csv.QUOTE_ALL,
-                       'delimiter': ';',
-                       'escapechar': '\\', }
+from .utils import (
+    clone_instance,
+    get_field_by_path,
+    get_field_value,
+    get_ignored_fields,
+)
+
+csv_options_default = {
+    "date_format": "d/m/Y",
+    "datetime_format": "N j, Y, P",
+    "time_format": "P",
+    "header": False,
+    "quotechar": '"',
+    "quoting": csv.QUOTE_ALL,
+    "delimiter": ";",
+    "escapechar": "\\",
+}
 
 delimiters = ",;|:"
 quotes = "'\"`"
 escapechars = " \\"
 ALL_FIELDS = -999
 
 
@@ -52,30 +59,31 @@
 
     fields = fields or []
 
     all_m2m = {}
     all_related = {}
 
     if related == ALL_FIELDS:
-        related = [rel.get_accessor_name()
-                   for rel in utils.get_all_related_objects(master)]
+        related = [
+            rel.get_accessor_name() for rel in utils.get_all_related_objects(master)
+        ]
 
     if m2m == ALL_FIELDS:
         m2m = set()
         for field in master._meta.get_fields():
-            if getattr(field, 'many_to_many', None):
+            if getattr(field, "many_to_many", None):
                 if isinstance(field, ManyToManyField):
                     if not field.remote_field.through._meta.auto_created:
                         continue
                     m2m.add(field.name)
                 else:
                     # reverse relation
                     m2m.add(field.get_accessor_name())
     if m2m and not commit:
-        raise ValueError('Cannot save related with `commit=False`')
+        raise ValueError("Cannot save related with `commit=False`")
     with atomic():
         result = clone_instance(master)
         for fieldname in fields:
             f = get_field_by_path(master, fieldname)
             if isinstance(f, FileField) or f and not f.primary_key:
                 setattr(result, fieldname, getattr(other, fieldname))
 
@@ -94,27 +102,33 @@
                         accessor = getattr(other, name)
                         all_related[name] = [(related_object.field.name, accessor)]
                     except ObjectDoesNotExist:
                         pass
                 else:
                     accessor = getattr(other, name, None)
                     if accessor:
-                        rel_fieldname = list(accessor.core_filters.keys())[0].split('__')[0]
+                        rel_fieldname = list(accessor.core_filters.keys())[0].split(
+                            "__"
+                        )[0]
                         for r in accessor.all():
                             all_related[name].append((rel_fieldname, r))
 
         if commit:
             for name, elements in list(all_related.items()):
                 for rel_fieldname, element in elements:
                     setattr(element, rel_fieldname, master)
                     element.save()
             other.delete()
-            ignored_fields = get_ignored_fields(result._meta.model, 'MERGE_ACTION_IGNORED_FIELDS')
+            ignored_fields = get_ignored_fields(
+                result._meta.model, "MERGE_ACTION_IGNORED_FIELDS"
+            )
             for ig_field in ignored_fields:
-                setattr(result, ig_field, result._meta.get_field(ig_field).get_default())
+                setattr(
+                    result, ig_field, result._meta.get_field(ig_field).get_default()
+                )
             result.save()
             for fieldname, elements in list(all_m2m.items()):
                 dest_m2m = getattr(result, fieldname)
                 for element in elements:
                     dest_m2m.add(element)
     return result
 
@@ -125,129 +139,145 @@
     """
 
     def write(self, value):
         """Write the value by returning it, instead of storing in a buffer."""
         return value
 
 
-def export_as_csv(queryset, fields=None, header=None,  # noqa
-                  filename=None, options=None, out=None):
+def export_as_csv(  # noqa: max-complexity: 20
+    queryset, fields=None, header=None, filename=None, options=None, out=None
+):  # noqa
     """
         Exports a queryset as csv from a queryset with the given fields.
 
     :param queryset: queryset to export
     :param fields: list of fields names to export. None for all fields
     :param header: if True, the exported file will have the first row as column names
     :param filename: name of the filename
     :param options: CSVOptions() instance or none
     :param: out: object that implements File protocol. HttpResponse if None.
 
     :return: HttpResponse instance
     """
-    streaming_enabled = (
-        getattr(settings, 'ADMINACTIONS_STREAM_CSV', False)
-    )
+    streaming_enabled = getattr(settings, "ADMINACTIONS_STREAM_CSV", False)
     if out is None:
         if streaming_enabled:
             response_class = StreamingHttpResponse
         else:
             response_class = HttpResponse
 
         if filename is None:
-            filename = filename or "%s.csv" % queryset.model._meta.verbose_name_plural.lower().replace(" ", "_")
-        response = response_class(content_type='text/csv')
-        response['Content-Disposition'] = ('attachment;filename="%s"' % filename).encode('us-ascii', 'replace')
+            filename = (
+                "%s.csv"
+                % queryset.model._meta.verbose_name_plural.lower().replace(" ", "_")
+            )
+
+        response = response_class(content_type="text/csv")
+        response["Content-Disposition"] = (
+            'attachment;filename="%s"' % filename
+        ).encode("us-ascii", "replace")
     else:
         response = out
 
     if options is None:
         config = csv_options_default
     else:
         config = csv_options_default.copy()
         config.update(options)
-
     if fields is None:
-        fields = [f.name for f in queryset.model._meta.fields + queryset.model._meta.many_to_many]
+        fields = [
+            f.name
+            for f in queryset.model._meta.fields + queryset.model._meta.many_to_many
+        ]
 
     if streaming_enabled:
         buffer_object = Echo()
     else:
         buffer_object = response
 
-    dialect = config.get('dialect', None)
+    dialect = config.get("dialect", None)
     if dialect is not None:
         writer = csv.writer(buffer_object, dialect=dialect)
     else:
-        writer = csv.writer(buffer_object,
-                            escapechar=str(config['escapechar']),
-                            delimiter=str(config['delimiter']),
-                            quotechar=str(config['quotechar']),
-                            quoting=int(config['quoting']))
+        writer = csv.writer(
+            buffer_object,
+            escapechar=config["escapechar"],
+            delimiter=str(config["delimiter"]),
+            quotechar=str(config["quotechar"]),
+            quoting=int(config["quoting"]),
+        )
 
     settingstime_zone = get_default_timezone()
 
     def yield_header():
         if bool(header):
             if isinstance(header, (list, tuple)):
                 yield writer.writerow(header)
             else:
                 yield writer.writerow([f for f in fields])
-        yield ''
+        yield ""
 
     def yield_rows():
         for obj in queryset:
             row = []
             for fieldname in fields:
                 value = get_field_value(obj, fieldname)
                 if isinstance(value, datetime.datetime):
                     try:
-                        value = dateformat.format(value.astimezone(settingstime_zone), config['datetime_format'])
+                        value = dateformat.format(
+                            value.astimezone(settingstime_zone),
+                            config["datetime_format"],
+                        )
                     except ValueError:
                         # astimezone() cannot be applied to a naive datetime
-                        value = dateformat.format(value, config['datetime_format'])
+                        value = dateformat.format(value, config["datetime_format"])
                 elif isinstance(value, datetime.date):
-                    value = dateformat.format(value, config['date_format'])
+                    value = dateformat.format(value, config["date_format"])
                 elif isinstance(value, datetime.time):
-                    value = dateformat.format(value, config['time_format'])
+                    value = dateformat.format(value, config["time_format"])
                 row.append(smart_str(value))
             yield writer.writerow(row)
 
     if streaming_enabled:
-        content_attr = 'content' if (
-            StreamingHttpResponse is HttpResponse) else 'streaming_content'
-        setattr(response, content_attr,
-                itertools.chain(yield_header(), yield_rows()))
+        content_attr = (
+            "content"
+            if (StreamingHttpResponse is HttpResponse)
+            else "streaming_content"
+        )
+        setattr(response, content_attr, itertools.chain(yield_header(), yield_rows()))
     else:
-        collections.deque(itertools.chain(
-            yield_header(), yield_rows()), maxlen=0)
+        collections.deque(itertools.chain(yield_header(), yield_rows()), maxlen=0)
 
     return response
 
 
-xls_options_default = {'date_format': 'd/m/Y',
-                       'datetime_format': 'N j, Y, P',
-                       'time_format': 'P',
-                       'sheet_name': 'Sheet1',
-                       'DateField': 'DD MMM-YY',
-                       'DateTimeField': 'DD MMD YY hh:mm',
-                       'TimeField': 'hh:mm',
-                       'IntegerField': '#,##',
-                       'PositiveIntegerField': '#,##',
-                       'PositiveSmallIntegerField': '#,##',
-                       'BigIntegerField': '#,##',
-                       'DecimalField': '#,##0.00',
-                       'BooleanField': 'boolean',
-                       'NullBooleanField': 'boolean',
-                       'EmailField': lambda value: 'HYPERLINK("mailto:%s","%s")' % (value, value),
-                       'URLField': lambda value: 'HYPERLINK("%s","%s")' % (value, value),
-                       'CurrencyColumn': '"$"#,##0.00);[Red]("$"#,##0.00)', }
-
-
-def export_as_xls2(queryset, fields=None, header=None,  # noqa
-                   filename=None, options=None, out=None):
+xls_options_default = {
+    "date_format": "d/m/Y",
+    "datetime_format": "N j, Y, P",
+    "time_format": "P",
+    "sheet_name": "Sheet1",
+    "DateField": "DD MMM-YY",
+    "DateTimeField": "DD MMD YY hh:mm",
+    "TimeField": "hh:mm",
+    "IntegerField": "#,##",
+    "PositiveIntegerField": "#,##",
+    "PositiveSmallIntegerField": "#,##",
+    "BigIntegerField": "#,##",
+    "DecimalField": "#,##0.00",
+    "BooleanField": "boolean",
+    "NullBooleanField": "boolean",
+    "EmailField": lambda value: 'HYPERLINK("mailto:%s","%s")' % (value, value),
+    "URLField": lambda value: 'HYPERLINK("%s","%s")' % (value, value),
+    "CurrencyColumn": '"$"#,##0.00);[Red]("$"#,##0.00)',
+}
+
+
+def export_as_xls2(  # noqa: max-complexity: 24
+    queryset, fields=None, header=None, filename=None, options=None, out=None  # noqa
+):
     # sheet_name=None,  header_alt=None,
     # formatting=None, out=None):
     """
     Exports a queryset as xls from a queryset with the given fields.
 
     :param queryset: queryset to export (can also be list of namedtuples)
     :param fields: list of fields names to export. None for all fields
@@ -256,118 +286,147 @@
     :param header_alt: if is not None, and header is True, the first row will be as header_alt (same nr columns)
     :param formatting: if is None will use formatting_default
     :return: HttpResponse instance if out not supplied, otherwise out
     """
 
     def _get_qs_formats(queryset):
         formats = {}
-        if hasattr(queryset, 'model'):
+        if hasattr(queryset, "model"):
             for i, fieldname in enumerate(fields):
                 try:
-                    f, __, __, __, = utils.get_field_by_name(queryset.model, fieldname)
-                    fmt = xls_options_default.get(f.name, xls_options_default.get(f.__class__.__name__, 'general'))
+                    (
+                        f,
+                        __,
+                        __,
+                        __,
+                    ) = utils.get_field_by_name(queryset.model, fieldname)
+                    fmt = xls_options_default.get(
+                        f.name, xls_options_default.get(f.__class__.__name__, "general")
+                    )
                     formats[i] = fmt
                 except FieldDoesNotExist:
                     pass
 
         return formats
 
     if out is None:
         if filename is None:
-            filename = filename or "%s.xls" % queryset.model._meta.verbose_name_plural.lower().replace(" ", "_")
-        response = HttpResponse(content_type='application/vnd.ms-excel')
-        response['Content-Disposition'] = ('attachment;filename="%s"' % filename).encode('us-ascii', 'replace')
+            filename = (
+                "%s.xls"
+                % queryset.model._meta.verbose_name_plural.lower().replace(" ", "_")
+            )
+
+        response = HttpResponse(content_type="application/vnd.ms-excel")
+        response["Content-Disposition"] = (
+            'attachment;filename="%s"' % filename
+        ).encode("us-ascii", "replace")
     else:
         response = out
 
     config = xls_options_default.copy()
     if options:
         config.update(options)
 
     if fields is None:
-        fields = [f.name for f in queryset.model._meta.fields + queryset.model._meta.many_to_many]
+        fields = [
+            f.name
+            for f in queryset.model._meta.fields + queryset.model._meta.many_to_many
+        ]
 
     book = xlwt.Workbook(encoding="utf-8", style_compression=2)
-    sheet_name = config.pop('sheet_name')
-    use_display = config.get('use_display', False)
+    sheet_name = config.pop("sheet_name")
+    use_display = config.get("use_display", False)
 
     sheet = book.add_sheet(sheet_name)
     style = xlwt.XFStyle()
     row = 0
-    heading_xf = xlwt.easyxf('font:height 200; font: bold on; align: wrap on, vert centre, horiz center')
-    sheet.write(row, 0, u'#', style)
+    heading_xf = xlwt.easyxf(
+        "font:height 200; font: bold on; align: wrap on, vert centre, horiz center"
+    )
+    sheet.write(row, 0, "#", style)
     if header:
         if not isinstance(header, (list, tuple)):
-            header = [force_str(f.verbose_name) for f in
-                      queryset.model._meta.fields + queryset.model._meta.many_to_many if f.name in fields]
+            header = [
+                force_str(f.verbose_name)
+                for f in queryset.model._meta.fields + queryset.model._meta.many_to_many
+                if f.name in fields
+            ]
 
         for col, fieldname in enumerate(header, start=1):
             sheet.write(row, col, fieldname, heading_xf)
             sheet.col(col).width = 5000
 
     sheet.row(row).height = 500
     formats = _get_qs_formats(queryset)
 
     _styles = {}
 
     for rownum, row in enumerate(queryset):
         sheet.write(rownum + 1, 0, rownum + 1)
         for col_idx, fieldname in enumerate(fields):
-            fmt = formats.get(col_idx, 'general')
+            fmt = formats.get(col_idx, "general")
             try:
-                value = get_field_value(row,
-                                        fieldname,
-                                        usedisplay=use_display,
-                                        raw_callable=False)
+                value = get_field_value(
+                    row, fieldname, usedisplay=use_display, raw_callable=False
+                )
                 if callable(fmt):
                     value = xlwt.Formula(fmt(value))
                 if hash(fmt) not in _styles:
                     if callable(fmt):
-                        _styles[hash(fmt)] = xlwt.easyxf(num_format_str='formula')
+                        _styles[hash(fmt)] = xlwt.easyxf(num_format_str="formula")
                     elif isinstance(value, datetime.datetime):
-                        _styles[hash(fmt)] = xlwt.easyxf(num_format_str=config['datetime_format'])
+                        _styles[hash(fmt)] = xlwt.easyxf(
+                            num_format_str=config["datetime_format"]
+                        )
                     elif isinstance(value, datetime.date):
-                        _styles[hash(fmt)] = xlwt.easyxf(num_format_str=config['date_format'])
+                        _styles[hash(fmt)] = xlwt.easyxf(
+                            num_format_str=config["date_format"]
+                        )
                     elif isinstance(value, datetime.datetime):
-                        _styles[hash(fmt)] = xlwt.easyxf(num_format_str=config['time_format'])
+                        _styles[hash(fmt)] = xlwt.easyxf(
+                            num_format_str=config["time_format"]
+                        )
                     else:
                         _styles[hash(fmt)] = xlwt.easyxf(num_format_str=fmt)
 
                 if isinstance(value, (list, tuple)):
                     value = "".join(value)
 
                 sheet.write(rownum + 1, col_idx + 1, value, _styles[hash(fmt)])
             except Exception as e:
                 sheet.write(rownum + 1, col_idx + 1, smart_str(e), _styles[hash(fmt)])
 
     book.save(response)
     return response
 
 
-xlsxwriter_options = {'date_format': 'd/m/Y',
-                      'datetime_format': 'N j, Y, P',
-                      'time_format': 'P',
-                      'sheet_name': 'Sheet1',
-                      'DateField': 'DD MMM-YY',
-                      'DateTimeField': 'DD MMD YY hh:mm',
-                      'TimeField': 'hh:mm',
-                      'IntegerField': '#,##',
-                      'PositiveIntegerField': '#,##',
-                      'PositiveSmallIntegerField': '#,##',
-                      'BigIntegerField': '#,##',
-                      'DecimalField': '#,##0.00',
-                      'BooleanField': 'boolean',
-                      'NullBooleanField': 'boolean',
-                      # 'EmailField': lambda value: 'HYPERLINK("mailto:%s","%s")' % (value, value),
-                      # 'URLField': lambda value: 'HYPERLINK("%s","%s")' % (value, value),
-                      'CurrencyColumn': '"$"#,##0.00);[Red]("$"#,##0.00)', }
-
-
-def export_as_xls3(queryset, fields=None, header=None,  # noqa
-                   filename=None, options=None, out=None):  # pragma: no cover
+xlsxwriter_options = {
+    "date_format": "d/m/Y",
+    "datetime_format": "N j, Y, P",
+    "time_format": "P",
+    "sheet_name": "Sheet1",
+    "DateField": "DD MMM-YY",
+    "DateTimeField": "DD MMD YY hh:mm",
+    "TimeField": "hh:mm",
+    "IntegerField": "#,##",
+    "PositiveIntegerField": "#,##",
+    "PositiveSmallIntegerField": "#,##",
+    "BigIntegerField": "#,##",
+    "DecimalField": "#,##0.00",
+    "BooleanField": "boolean",
+    "NullBooleanField": "boolean",
+    # 'EmailField': lambda value: 'HYPERLINK("mailto:%s","%s")' % (value, value),
+    # 'URLField': lambda value: 'HYPERLINK("%s","%s")' % (value, value),
+    "CurrencyColumn": '"$"#,##0.00);[Red]("$"#,##0.00)',
+}
+
+
+def export_as_xls3(  # noqa: max-complexity: 23
+    queryset, fields=None, header=None, filename=None, options=None, out=None  # noqa
+):  # pragma: no cover
     # sheet_name=None,  header_alt=None,
     # formatting=None, out=None):
     """
     Exports a queryset as xls from a queryset with the given fields.
 
     :param queryset: queryset to export (can also be list of namedtuples)
     :param fields: list of fields names to export. None for all fields
@@ -376,89 +435,109 @@
     :param header_alt: if is not None, and header is True, the first row will be as header_alt (same nr columns)
     :param formatting: if is None will use formatting_default
     :return: HttpResponse instance if out not supplied, otherwise out
     """
     import xlsxwriter
 
     def _get_qs_formats(queryset):
-        formats = {'_general_': book.add_format()}
-        if hasattr(queryset, 'model'):
+        formats = {"_general_": book.add_format()}
+        if hasattr(queryset, "model"):
             for i, fieldname in enumerate(fields):
                 try:
-                    f, __, __, __, = queryset.model._meta.get_field_by_name(fieldname)
-                    pattern = xlsxwriter_options.get(f.name, xlsxwriter_options.get(f.__class__.__name__, 'general'))
-                    fmt = book.add_format({'num_format': pattern})
+                    (
+                        f,
+                        __,
+                        __,
+                        __,
+                    ) = queryset.model._meta.get_field_by_name(fieldname)
+                    pattern = xlsxwriter_options.get(
+                        f.name, xlsxwriter_options.get(f.__class__.__name__, "general")
+                    )
+                    fmt = book.add_format({"num_format": pattern})
                     formats[fieldname] = fmt
                 except FieldDoesNotExist:
                     pass
         return formats
 
     http_response = out is None
     if out is None:
         out = BytesIO()
 
     config = xlsxwriter_options.copy()
     if options:
         config.update(options)
 
     if fields is None:
-        fields = [f.name for f in queryset.model._meta.fields + queryset.model._meta.many_to_many]
-
-    book = xlsxwriter.Workbook(out, {'in_memory': True})
-    sheet_name = config.pop('sheet_name')
-    use_display = config.get('use_display', False)
+        fields = [
+            f.name
+            for f in queryset.model._meta.fields + queryset.model._meta.many_to_many
+        ]
+
+    book = xlsxwriter.Workbook(out, {"in_memory": True})
+    sheet_name = config.pop("sheet_name")
+    use_display = config.get("use_display", False)
     sheet = book.add_worksheet(sheet_name)
     book.close()
     formats = _get_qs_formats(queryset)
 
     row = 0
-    sheet.write(row, 0, force_str('#'), formats['_general_'])
+    sheet.write(row, 0, force_str("#"), formats["_general_"])
     if header:
         if not isinstance(header, (list, tuple)):
-            header = [force_str(f.verbose_name) for f in
-                      queryset.model._meta.fields + queryset.model._meta.many_to_many if f.name in fields]
+            header = [
+                force_str(f.verbose_name)
+                for f in queryset.model._meta.fields + queryset.model._meta.many_to_many
+                if f.name in fields
+            ]
 
         for col, fieldname in enumerate(header, start=1):
-            sheet.write(row, col, force_str(fieldname), formats['_general_'])
+            sheet.write(row, col, force_str(fieldname), formats["_general_"])
 
     settingstime_zone = get_default_timezone()
 
     for rownum, row in enumerate(queryset):
         sheet.write(rownum + 1, 0, rownum + 1)
         for idx, fieldname in enumerate(fields):
-            fmt = formats.get(fieldname, formats['_general_'])
+            fmt = formats.get(fieldname, formats["_general_"])
             try:
-                value = get_field_value(row,
-                                        fieldname,
-                                        usedisplay=use_display,
-                                        raw_callable=False)
+                value = get_field_value(
+                    row, fieldname, usedisplay=use_display, raw_callable=False
+                )
                 if callable(fmt):
                     value = fmt(value)
                 if isinstance(value, (list, tuple)):
-                    value = smart_str(u"".join(value))
+                    value = smart_str("".join(value))
 
                 if isinstance(value, datetime.datetime):
                     try:
-                        value = dateformat.format(value.astimezone(settingstime_zone), config['datetime_format'])
+                        value = dateformat.format(
+                            value.astimezone(settingstime_zone),
+                            config["datetime_format"],
+                        )
                     except ValueError:
-                        value = dateformat.format(value, config['datetime_format'])
+                        value = dateformat.format(value, config["datetime_format"])
 
                 value = str(value)
 
                 sheet.write(rownum + 1, idx + 1, smart_str(value), fmt)
             except BaseException:
                 raise
 
     book.close()
     out.seek(0)
     if http_response:
         if filename is None:
-            filename = filename or "%s.xls" % queryset.model._meta.verbose_name_plural.lower().replace(" ", "_")
-        response = HttpResponse(out.read(),
-                                content_type="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet")
+            filename = (
+                "%s.xls"
+                % queryset.model._meta.verbose_name_plural.lower().replace(" ", "_")
+            )
+        response = HttpResponse(
+            out.read(),
+            content_type="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
+        )
         # content_type='application/vnd.ms-excel')
-        response['Content-Disposition'] = 'attachment;filename="%s"' % filename
+        response["Content-Disposition"] = 'attachment;filename="%s"' % filename
         return response
     return out
 
 
 export_as_xls = export_as_xls2
```

### Comparing `django-adminactions-2.0.0/src/adminactions/byrows_update.py` & `django-adminactions-2.1.0/src/adminactions/byrows_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,102 +9,126 @@
 from .forms import GenericActionForm
 from .perms import get_permission_codename
 from .utils import get_ignored_fields
 
 
 def byrows_update(modeladmin, request, queryset):  # noqa
     """
-        by rows update queryset
+    by rows update queryset
 
-        :type modeladmin: ModelAdmin
-        :type request: HttpRequest
-        :type queryset: QuerySet
+    :type modeladmin: ModelAdmin
+    :type request: HttpRequest
+    :type queryset: QuerySet
     """
 
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label.lower(),
-                            get_permission_codename(byrows_update.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label.lower(),
+        get_permission_codename(byrows_update.base_permission, opts),
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
 
     class modelform(modeladmin.form):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             if self.instance:
-                readonly_fields = (modeladmin.model._meta.pk.name,) + tuple(modeladmin.get_readonly_fields(request))
+                readonly_fields = (modeladmin.model._meta.pk.name,) + tuple(
+                    modeladmin.get_readonly_fields(request)
+                )
                 for fname in readonly_fields:
                     if fname in self.fields:
-                        self.fields[fname].widget.attrs['readonly'] = 'readonly'
-                        self.fields[fname].widget.attrs['class'] = 'readonly'
+                        self.fields[fname].widget.attrs["readonly"] = "readonly"
+                        self.fields[fname].widget.attrs["class"] = "readonly"
 
     fields = byrows_update_get_fields(modeladmin)
 
     def formfield_callback(field, **kwargs):
         return modeladmin.formfield_for_dbfield(field, request=request, **kwargs)
 
     ActionForm = modelform_factory(
         modeladmin.model,
         form=GenericActionForm,
         fields=fields,
-        formfield_callback=formfield_callback)
+        formfield_callback=formfield_callback,
+    )
 
-    MFormSet = modelformset_factory(modeladmin.model, form=modelform,
-                                    fields=fields, extra=0,
-                                    formfield_callback=formfield_callback)
+    MFormSet = modelformset_factory(
+        modeladmin.model,
+        form=modelform,
+        fields=fields,
+        extra=0,
+        formfield_callback=formfield_callback,
+    )
 
-    if 'apply' in request.POST:
+    if "apply" in request.POST:
         actionform = ActionForm(request.POST)
         formset = MFormSet(request.POST)
         if formset.is_valid():
             formset.save()
             messages.info(request, _("Updated record(s)"))
             return HttpResponseRedirect(request.get_full_path())
     else:
-        action_form_initial = {'_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-                               'select_across': request.POST.get('select_across') == '1',
-                               'action': 'byrows_update'}
+        action_form_initial = {
+            "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+            "select_across": request.POST.get("select_across") == "1",
+            "action": "byrows_update",
+        }
         actionform = ActionForm(initial=action_form_initial, instance=None)
         formset = MFormSet(queryset=queryset)
 
     adminform = helpers.AdminForm(
-        actionform,
-        modeladmin.get_fieldsets(request),
-        {},
-        [],
-        model_admin=modeladmin)
+        actionform, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin
+    )
 
-    tpl = 'adminactions/byrows_update.html'
+    tpl = "adminactions/byrows_update.html"
     ctx = {
-        'adminform': adminform,
-        'actionform': actionform,
-        'action_short_description': byrows_update.short_description,
-        'title': u"%s (%s)" % (
+        "adminform": adminform,
+        "actionform": actionform,
+        "action_short_description": byrows_update.short_description,
+        "title": "%s (%s)"
+        % (
             byrows_update.short_description.capitalize(),
             smart_str(modeladmin.opts.verbose_name_plural),
         ),
-        'formset': formset,
-        'opts': modeladmin.model._meta,
-        'app_label': modeladmin.model._meta.app_label,
+        "formset": formset,
+        "opts": modeladmin.model._meta,
+        "app_label": modeladmin.model._meta.app_label,
     }
     ctx.update(modeladmin.admin_site.each_context(request))
     return render(request, tpl, ctx)
 
 
 byrows_update.short_description = _("By rows update")
-byrows_update.base_permission = 'adminactions_byrowsupdate'
+byrows_update.base_permission = "adminactions_byrowsupdate"
 
 
 def byrows_update_get_fields(modeladmin):
     """
-        Get fields names to be shown of the model rows formset considering the
-        admin option:
-        - adminactions_byrows_update_fields
-        - adminactions_byrows_update_exclude
+    Get fields names to be shown of the model rows formset considering the
+    admin option:
+    - adminactions_byrows_update_fields
+    - adminactions_byrows_update_exclude
     """
-    ignored_fields = get_ignored_fields(modeladmin.model, "UPDATE_ACTION_IGNORED_FIELDS")
-    out = getattr(modeladmin, 'adminactions_byrows_update_fields',
-                  [f.name for f in modeladmin.model._meta.fields if f.editable and f.name not in ignored_fields])
-    if hasattr(modeladmin, 'adminactions_byrows_update_exclude'):
+    ignored_fields = get_ignored_fields(
+        modeladmin.model, "UPDATE_ACTION_IGNORED_FIELDS"
+    )
+    out = getattr(
+        modeladmin,
+        "adminactions_byrows_update_fields",
+        [
+            f.name
+            for f in modeladmin.model._meta.fields
+            if f.editable and f.name not in ignored_fields
+        ],
+    )
+    if hasattr(modeladmin, "adminactions_byrows_update_exclude"):
         fields = modeladmin.adminactions_byrows_update_exclude
-        out = [fname for fname in fields if fname not in modeladmin.adminactions_byrows_update_exclude]
+        out = [
+            fname
+            for fname in fields
+            if fname not in modeladmin.adminactions_byrows_update_exclude
+        ]
     return out
```

### Comparing `django-adminactions-2.0.0/src/adminactions/duplicates.py` & `django-adminactions-2.1.0/src/adminactions/duplicates.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,52 +4,58 @@
 from django.core.exceptions import ValidationError
 from django.db.models import Count
 from django.shortcuts import render
 from django.utils.translation import gettext as _
 
 from adminactions.exceptions import ActionInterrupted
 from adminactions.perms import get_permission_codename
-from adminactions.signals import (adminaction_end, adminaction_requested,
-                                  adminaction_start,)
+from adminactions.signals import (
+    adminaction_end,
+    adminaction_requested,
+    adminaction_start,
+)
 from adminactions.utils import get_common_context
 
 
 class DuplicatesForm(forms.Form):
     _selected_action = forms.CharField(widget=forms.MultipleHiddenInput)
-    select_across = forms.BooleanField(label='', required=False, initial=0,
-                                       widget=forms.HiddenInput({'class': 'select-across'}))
-    action = forms.CharField(label='', required=True, initial='', widget=forms.HiddenInput())
+    select_across = forms.BooleanField(
+        label="",
+        required=False,
+        initial=0,
+        widget=forms.HiddenInput({"class": "select-across"}),
+    )
+    action = forms.CharField(
+        label="", required=True, initial="", widget=forms.HiddenInput()
+    )
     min = forms.IntegerField(required=True, initial=2)
     max = forms.IntegerField(required=False)
 
     def __init__(self, *args, **kwargs):
-        self.model = kwargs.pop('model')
+        self.model = kwargs.pop("model")
         self.field_names = []
         super().__init__(*args, **kwargs)
         for field in self.model._meta.concrete_fields:
             label = field.verbose_name
             if field.db_index:
                 label = f"{label} **"
             self.field_names.append(field.name)
-            self.fields[field.name] = forms.BooleanField(label=label,
-                                                         required=False)
+            self.fields[field.name] = forms.BooleanField(label=label, required=False)
 
     def clean(self):
         checked = [fname for fname in self.field_names if self.cleaned_data[fname]]
         if not checked:
             raise ValidationError("Select at least one field")
         return self.cleaned_data
 
     @property
     def media(self):
         return super().media + forms.Media(
             css={
-                'screen': (
-                    'adminactions/css/adminactions.css',
-                ),
+                "screen": ("adminactions/css/adminactions.css",),
             },
         )
 
 
 def find_duplicates(qs, fields, min_dupe=1, max_dupe=None):
     qs = qs.order_by()
     qs = qs.values(*fields)
@@ -58,68 +64,85 @@
     if max_dupe:
         qs = qs.filter(count_id__lte=max_dupe)
     return qs
 
 
 def find_duplicates_action(modeladmin, request, queryset):
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label,
-                            get_permission_codename(find_duplicates_action.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label,
+        get_permission_codename(find_duplicates_action.base_permission, opts),
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
-    ctx = get_common_context(modeladmin,
-                             action_short_description=find_duplicates_action.short_description,
-                             selection=queryset)
-    tpl = 'adminactions/duplicates.html'
-    initial = {'_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-               'select_across': request.POST.get('select_across') == '1',
-               'action': 'find_duplicates_action'}
+    ctx = get_common_context(
+        modeladmin,
+        action_short_description=find_duplicates_action.short_description,
+        selection=queryset,
+    )
+    tpl = "adminactions/duplicates.html"
+    initial = {
+        "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+        "select_across": request.POST.get("select_across") == "1",
+        "action": "find_duplicates_action",
+    }
     try:
-        adminaction_requested.send(sender=modeladmin.model,
-                                   action='find_duplicates_action',
-                                   request=request,
-                                   queryset=queryset,
-                                   modeladmin=modeladmin)
+        adminaction_requested.send(
+            sender=modeladmin.model,
+            action="find_duplicates_action",
+            request=request,
+            queryset=queryset,
+            modeladmin=modeladmin,
+        )
     except ActionInterrupted as e:
         messages.error(request, str(e))
         return
-    if 'apply' in request.POST:
+    if "apply" in request.POST:
         form = DuplicatesForm(request.POST, request.FILES, model=modeladmin.model)
         if form.is_valid():
             try:
-                adminaction_start.send(sender=queryset.model,
-                                       action='find_duplicates_action',
-                                       request=request,
-                                       queryset=queryset,
-                                       modeladmin=modeladmin)
+                adminaction_start.send(
+                    sender=queryset.model,
+                    action="find_duplicates_action",
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                )
             except ActionInterrupted as e:
                 messages.error(request, str(e))
                 return
 
-            min_dupe = form.cleaned_data['min']
-            max_dupe = form.cleaned_data.get('max', None)
+            min_dupe = form.cleaned_data["min"]
+            max_dupe = form.cleaned_data.get("max", None)
             checked = [fname for fname in form.field_names if form.cleaned_data[fname]]
-            qs = find_duplicates(modeladmin.get_queryset(request),
-                                 checked,
-                                 min_dupe=min_dupe,
-                                 max_dupe=max_dupe
-                                 )
-            ctx['results'] = qs.all()
-            if not ctx['results']:
-                modeladmin.message_user(request, _("No duplicated rows found"), messages.WARNING)
-            ctx['checked'] = checked
-            ctx['sql'] = str(qs.query)
-            adminaction_end.send(sender=queryset.model,
-                                 action='find_duplicates_action',
-                                 request=request,
-                                 queryset=queryset)
+            qs = find_duplicates(
+                modeladmin.get_queryset(request),
+                checked,
+                min_dupe=min_dupe,
+                max_dupe=max_dupe,
+            )
+            ctx["results"] = qs.all()
+            if not ctx["results"]:
+                modeladmin.message_user(
+                    request, _("No duplicated rows found"), messages.WARNING
+                )
+            ctx["checked"] = checked
+            ctx["sql"] = str(qs.query)
+            adminaction_end.send(
+                sender=queryset.model,
+                action="find_duplicates_action",
+                request=request,
+                queryset=queryset,
+            )
         else:
             pass
     else:
         form = DuplicatesForm(model=modeladmin.model, initial=initial)
-    ctx['form'] = form
+    ctx["form"] = form
     return render(request, tpl, context=ctx)
 
 
 find_duplicates_action.short_description = _("Find Duplicates")
-find_duplicates_action.base_permission = 'adminactions_find_duplicates'
+find_duplicates_action.base_permission = "adminactions_find_duplicates"
```

### Comparing `django-adminactions-2.0.0/src/adminactions/export.py` & `django-adminactions-2.1.0/src/adminactions/export.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,214 @@
+import logging
+from itertools import chain
+
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.admin import helpers
 from django.core import serializers as ser
 from django.db import router
 from django.db.models import ForeignKey, ManyToManyField
 from django.db.models.deletion import Collector
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import render
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
-from itertools import chain
 
-from .api import (export_as_csv as _export_as_csv,
-                  export_as_xls as _export_as_xls,)
+from .api import export_as_csv as _export_as_csv
+from .api import export_as_xls as _export_as_xls
 from .exceptions import ActionInterrupted
 from .forms import CSVOptions, FixtureOptions, XLSOptions
 from .perms import get_permission_codename
 from .signals import adminaction_end, adminaction_requested, adminaction_start
 
+logger = logging.getLogger(__name__)
+
 
 def get_action(request):
     try:
-        action_index = int(request.POST.get('index', 0))
+        action_index = int(request.POST.get("index", 0))
     except ValueError:
         action_index = 0
-    return request.POST.getlist('action')[action_index]
+    return request.POST.getlist("action")[action_index]
 
 
-def base_export(modeladmin, request, queryset, title, impl,  # noqa
-                name, action_short_description, template, form_class):
+def base_export(
+    modeladmin,
+    request,
+    queryset,
+    title,
+    impl,  # noqa
+    name,
+    action_short_description,
+    template,
+    form_class,
+):
     """
-        export a queryset to csv file
+    export a queryset to csv file
     """
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label,
-                            get_permission_codename(base_export.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label, get_permission_codename(base_export.base_permission, opts)
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
 
     try:
-        adminaction_requested.send(sender=modeladmin.model,
-                                   action=name,
-                                   request=request,
-                                   queryset=queryset,
-                                   modeladmin=modeladmin)
+        adminaction_requested.send(
+            sender=modeladmin.model,
+            action=name,
+            request=request,
+            queryset=queryset,
+            modeladmin=modeladmin,
+        )
     except ActionInterrupted as e:
         messages.error(request, str(e))
         return
-    if hasattr(modeladmin, 'get_exportable_columns'):
+    if hasattr(modeladmin, "get_exportable_columns"):
         cols = modeladmin.get_exportable_columns(request, form_class)
     else:
-        cols = [(f.name, f.verbose_name) for f in queryset.model._meta.fields + queryset.model._meta.many_to_many]
-    initial = {'_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-               'select_across': request.POST.get('select_across') == '1',
-               'action': get_action(request),
-               'columns': [x for x, v in cols]}
+        cols = [
+            (f.name, f.verbose_name)
+            for f in queryset.model._meta.fields + queryset.model._meta.many_to_many
+        ]
+    initial = {
+        "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+        "select_across": request.POST.get("select_across") == "1",
+        "action": get_action(request),
+        "columns": [x for x, v in cols],
+    }
     if initial["action"] == "export_as_csv":
-        initial.update(getattr(
-            settings, "ADMINACTIONS_CSV_OPTIONS_DEFAULT", {}))
+        initial.update(getattr(settings, "ADMINACTIONS_CSV_OPTIONS_DEFAULT", {}))
 
-    if 'apply' in request.POST:
+    if "apply" in request.POST:
         form = form_class(request.POST)
-        form.fields['columns'].choices = cols
+        form.fields["columns"].choices = cols
         if form.is_valid():
             try:
-                adminaction_start.send(sender=modeladmin.model,
-                                       action=name,
-                                       request=request,
-                                       queryset=queryset,
-                                       modeladmin=modeladmin,
-                                       form=form)
+                adminaction_start.send(
+                    sender=modeladmin.model,
+                    action=name,
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
             except ActionInterrupted as e:
                 messages.error(request, str(e))
                 return
 
-            if hasattr(modeladmin, 'get_%s_filename' % name):
+            if hasattr(modeladmin, "get_%s_filename" % name):
                 filename = modeladmin.get_export_as_csv_filename(request, queryset)
             else:
                 filename = None
             try:
-                response = impl(queryset,
-                                fields=form.cleaned_data['columns'],
-                                header=form.cleaned_data.get('header', False),
-                                filename=filename,
-                                options=form.cleaned_data)
+                response = impl(
+                    queryset,
+                    fields=form.cleaned_data["columns"],
+                    header=form.cleaned_data.get("header", False),
+                    filename=filename,
+                    options=form.cleaned_data,
+                )
             except Exception as e:
+                logger.exception(e)
                 messages.error(request, "Error: (%s)" % str(e))
             else:
-                adminaction_end.send(sender=modeladmin.model,
-                                     action=name,
-                                     request=request,
-                                     queryset=queryset,
-                                     modeladmin=modeladmin,
-                                     form=form)
+                adminaction_end.send(
+                    sender=modeladmin.model,
+                    action=name,
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
                 return response
     else:
         form = form_class(initial=initial)
-        form.fields['columns'].choices = cols
+        form.fields["columns"].choices = cols
 
-    adminForm = helpers.AdminForm(form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin)
+    adminForm = helpers.AdminForm(
+        form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin
+    )
     media = modeladmin.media + adminForm.media
     # tpl = 'adminactions/export_csv.html'
-    ctx = {'adminform': adminForm,
-           'change': True,
-           'action_short_description': action_short_description,
-           'title': title,
-           'is_popup': False,
-           'save_as': False,
-           'has_delete_permission': False,
-           'has_add_permission': False,
-           'has_change_permission': True,
-           'queryset': queryset,
-           'opts': queryset.model._meta,
-           'app_label': queryset.model._meta.app_label,
-           'media': mark_safe(media)}
+    ctx = {
+        "adminform": adminForm,
+        "change": True,
+        "action_short_description": action_short_description,
+        "title": title,
+        "is_popup": False,
+        "save_as": False,
+        "has_delete_permission": False,
+        "has_add_permission": False,
+        "has_change_permission": True,
+        "queryset": queryset,
+        "opts": queryset.model._meta,
+        "app_label": queryset.model._meta.app_label,
+        "media": mark_safe(media),
+    }
     ctx.update(modeladmin.admin_site.each_context(request))
     return render(request, template, ctx)
 
 
-base_export.base_permission = 'adminactions_export'
+base_export.base_permission = "adminactions_export"
 
 
 def export_as_csv(modeladmin, request, queryset):
-    if hasattr(modeladmin, 'get_export_form'):
-        form_class = modeladmin.get_export_form(request, 'csv') or CSVOptions
+    if hasattr(modeladmin, "get_export_form"):
+        form_class = modeladmin.get_export_form(request, "csv") or CSVOptions
     else:
         form_class = CSVOptions
-    return base_export(modeladmin, request, queryset,
-                       impl=_export_as_csv,
-                       name='export_as_csv',
-                       action_short_description=export_as_csv.short_description,
-                       title=u"%s (%s)" % (
-                           export_as_csv.short_description.capitalize(),
-                           modeladmin.opts.verbose_name_plural,
-                       ),
-                       template='adminactions/export_csv.html',
-                       form_class=form_class)
+    return base_export(
+        modeladmin,
+        request,
+        queryset,
+        impl=_export_as_csv,
+        name="export_as_csv",
+        action_short_description=export_as_csv.short_description,
+        title="%s (%s)"
+        % (
+            export_as_csv.short_description.capitalize(),
+            modeladmin.opts.verbose_name_plural,
+        ),
+        template="adminactions/export_csv.html",
+        form_class=form_class,
+    )
 
 
 export_as_csv.short_description = _("Export as CSV")
-export_as_csv.base_permission = 'adminactions_export'
+export_as_csv.base_permission = "adminactions_export"
 
 
 def export_as_xls(modeladmin, request, queryset):
-    if hasattr(modeladmin, 'get_export_form'):
-        form_class = modeladmin.get_export_form(request, 'xls') or XLSOptions
+    if hasattr(modeladmin, "get_export_form"):
+        form_class = modeladmin.get_export_form(request, "xls") or XLSOptions
     else:
         form_class = XLSOptions
-    return base_export(modeladmin, request, queryset,
-                       impl=_export_as_xls,
-                       name='export_as_xls',
-                       action_short_description=export_as_xls.short_description,
-                       title=u"%s (%s)" % (
-                           export_as_xls.short_description.capitalize(),
-                           modeladmin.opts.verbose_name_plural,
-                       ),
-                       template='adminactions/export_xls.html',
-                       form_class=form_class)
+    return base_export(
+        modeladmin,
+        request,
+        queryset,
+        impl=_export_as_xls,
+        name="export_as_xls",
+        action_short_description=export_as_xls.short_description,
+        title="%s (%s)"
+        % (
+            export_as_xls.short_description.capitalize(),
+            modeladmin.opts.verbose_name_plural,
+        ),
+        template="adminactions/export_xls.html",
+        form_class=form_class,
+    )
 
 
 export_as_xls.short_description = _("Export as XLS")
-export_as_xls.base_permission = 'adminactions_export'
+export_as_xls.base_permission = "adminactions_export"
 
 
 class FlatCollector:
     def __init__(self, using):
         self._visited = []
         super().__init__()
 
@@ -204,209 +247,256 @@
         self.models = set([o.__class__ for o in self.data])
 
     def __str__(self):
         return mark_safe(self.data)
 
 
 def _dump_qs(form, queryset, data, filename):
-    fmt = form.cleaned_data.get('serializer')
+    fmt = form.cleaned_data.get("serializer")
 
     json = ser.get_serializer(fmt)()
-    ret = json.serialize(data,
-                         use_natural_foreign_keys=form.cleaned_data.get('use_natural_fk', False),
-                         use_natural_primary_keys=form.cleaned_data.get('use_natural_pk', False),
-                         indent=form.cleaned_data.get('indent'))
-
-    response = HttpResponse(content_type='application/json')
-    if not form.cleaned_data.get('on_screen', False):
-        filename = filename or "%s.%s" % (queryset.model._meta.verbose_name_plural.lower().replace(" ", "_"), fmt)
-        response['Content-Disposition'] = ('attachment;filename="%s"' % filename).encode('us-ascii', 'replace')
+    ret = json.serialize(
+        data,
+        use_natural_foreign_keys=form.cleaned_data.get("use_natural_fk", False),
+        use_natural_primary_keys=form.cleaned_data.get("use_natural_pk", False),
+        indent=form.cleaned_data.get("indent"),
+    )
+
+    response = HttpResponse(content_type="application/json")
+    if not form.cleaned_data.get("on_screen", False):
+        filename = filename or "%s.%s" % (
+            queryset.model._meta.verbose_name_plural.lower().replace(" ", "_"),
+            fmt,
+        )
+        response["Content-Disposition"] = (
+            'attachment;filename="%s"' % filename
+        ).encode("us-ascii", "replace")
     response.content = ret
     return response
 
 
 def export_as_fixture(modeladmin, request, queryset):
-    initial = {'_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-               'select_across': request.POST.get('select_across') == '1',
-               'action': get_action(request),
-               'serializer': 'json',
-               'indent': 4}
+    initial = {
+        "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+        "select_across": request.POST.get("select_across") == "1",
+        "action": get_action(request),
+        "serializer": "json",
+        "indent": 4,
+    }
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label,
-                            get_permission_codename(export_as_fixture.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label, get_permission_codename(export_as_fixture.base_permission, opts)
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
 
     try:
-        adminaction_requested.send(sender=modeladmin.model,
-                                   action='export_as_fixture',
-                                   request=request,
-                                   queryset=queryset,
-                                   modeladmin=modeladmin)
+        adminaction_requested.send(
+            sender=modeladmin.model,
+            action="export_as_fixture",
+            request=request,
+            queryset=queryset,
+            modeladmin=modeladmin,
+        )
     except ActionInterrupted as e:
         messages.error(request, str(e))
         return
-    if hasattr(modeladmin, 'get_export_form'):
-        form_class = modeladmin.get_export_form(request, 'fixture') or FixtureOptions
+    if hasattr(modeladmin, "get_export_form"):
+        form_class = modeladmin.get_export_form(request, "fixture") or FixtureOptions
     else:
         form_class = FixtureOptions
 
-    if 'apply' in request.POST:
+    if "apply" in request.POST:
         form = form_class(request.POST)
         if form.is_valid():
             try:
-                adminaction_start.send(sender=modeladmin.model,
-                                       action='export_as_fixture',
-                                       request=request,
-                                       queryset=queryset,
-                                       modeladmin=modeladmin,
-                                       form=form)
+                adminaction_start.send(
+                    sender=modeladmin.model,
+                    action="export_as_fixture",
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
             except ActionInterrupted as e:
                 messages.error(request, str(e))
                 return
             try:
-                _collector = ForeignKeysCollector if form.cleaned_data.get('add_foreign_keys') else FlatCollector
+                _collector = (
+                    ForeignKeysCollector
+                    if form.cleaned_data.get("add_foreign_keys")
+                    else FlatCollector
+                )
                 c = _collector(None)
                 c.collect(queryset)
-                adminaction_end.send(sender=modeladmin.model,
-                                     action='export_as_fixture',
-                                     request=request,
-                                     queryset=queryset,
-                                     modeladmin=modeladmin,
-                                     form=form)
-
-                if hasattr(modeladmin, 'get_export_as_fixture_filename'):
-                    filename = modeladmin.get_export_as_fixture_filename(request, queryset)
+                adminaction_end.send(
+                    sender=modeladmin.model,
+                    action="export_as_fixture",
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
+
+                if hasattr(modeladmin, "get_export_as_fixture_filename"):
+                    filename = modeladmin.get_export_as_fixture_filename(
+                        request, queryset
+                    )
                 else:
                     filename = None
                 return _dump_qs(form, queryset, c.data, filename)
             except AttributeError as e:
                 messages.error(request, str(e))
                 return HttpResponseRedirect(request.path)
     else:
         form = form_class(initial=initial)
 
-    adminForm = helpers.AdminForm(form, modeladmin.get_fieldsets(request), {}, model_admin=modeladmin)
+    adminForm = helpers.AdminForm(
+        form, modeladmin.get_fieldsets(request), {}, model_admin=modeladmin
+    )
     media = modeladmin.media + adminForm.media
-    tpl = 'adminactions/export_fixture.html'
-    ctx = {'adminform': adminForm,
-           'change': True,
-           'action_short_description': export_as_fixture.short_description,
-           'title': "%s (%s)" % (
-               export_as_fixture.short_description.capitalize(),
-               modeladmin.opts.verbose_name_plural,
-           ),
-           'is_popup': False,
-           'save_as': False,
-           'has_delete_permission': False,
-           'has_add_permission': False,
-           'has_change_permission': True,
-           'queryset': queryset,
-           'opts': queryset.model._meta,
-           'app_label': queryset.model._meta.app_label,
-           'media': mark_safe(media)}
+    tpl = "adminactions/export_fixture.html"
+    ctx = {
+        "adminform": adminForm,
+        "change": True,
+        "action_short_description": export_as_fixture.short_description,
+        "title": "%s (%s)"
+        % (
+            export_as_fixture.short_description.capitalize(),
+            modeladmin.opts.verbose_name_plural,
+        ),
+        "is_popup": False,
+        "save_as": False,
+        "has_delete_permission": False,
+        "has_add_permission": False,
+        "has_change_permission": True,
+        "queryset": queryset,
+        "opts": queryset.model._meta,
+        "app_label": queryset.model._meta.app_label,
+        "media": mark_safe(media),
+    }
     ctx.update(modeladmin.admin_site.each_context(request))
     return render(request, tpl, ctx)
 
 
 export_as_fixture.short_description = _("Export as fixture")
-export_as_fixture.base_permission = 'adminactions_export'
+export_as_fixture.base_permission = "adminactions_export"
 
 
 def export_delete_tree(modeladmin, request, queryset):  # noqa
     """
     Export as fixture selected queryset and all the records that belong to.
     That mean that dump what will be deleted if the queryset was deleted
     """
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label,
-                            get_permission_codename(export_delete_tree.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label,
+        get_permission_codename(export_delete_tree.base_permission, opts),
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
     try:
-        adminaction_requested.send(sender=modeladmin.model,
-                                   action='export_delete_tree',
-                                   request=request,
-                                   queryset=queryset,
-                                   modeladmin=modeladmin)
+        adminaction_requested.send(
+            sender=modeladmin.model,
+            action="export_delete_tree",
+            request=request,
+            queryset=queryset,
+            modeladmin=modeladmin,
+        )
     except ActionInterrupted as e:
         messages.error(request, str(e))
         return
 
-    initial = {'_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-               'select_across': request.POST.get('select_across') == '1',
-               'action': get_action(request),
-
-               'serializer': 'json',
-               'indent': 4}
+    initial = {
+        "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+        "select_across": request.POST.get("select_across") == "1",
+        "action": get_action(request),
+        "serializer": "json",
+        "indent": 4,
+    }
 
-    if hasattr(modeladmin, 'get_export_form'):
-        form_class = modeladmin.get_export_form(request, 'delete') or FixtureOptions
+    if hasattr(modeladmin, "get_export_form"):
+        form_class = modeladmin.get_export_form(request, "delete") or FixtureOptions
     else:
         form_class = FixtureOptions
 
-    if 'apply' in request.POST:
+    if "apply" in request.POST:
         form = form_class(request.POST)
         if form.is_valid():
             try:
-                adminaction_start.send(sender=modeladmin.model,
-                                       action='export_delete_tree',
-                                       request=request,
-                                       queryset=queryset,
-                                       modeladmin=modeladmin,
-                                       form=form)
+                adminaction_start.send(
+                    sender=modeladmin.model,
+                    action="export_delete_tree",
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
             except ActionInterrupted as e:
                 messages.error(request, str(e))
                 return
             try:
-                collect_related = form.cleaned_data.get('add_foreign_keys')
+                collect_related = form.cleaned_data.get("add_foreign_keys")
                 using = router.db_for_write(modeladmin.model)
 
                 c = Collector(using)
                 c.collect(queryset, collect_related=collect_related)
                 data = []
                 for model, instances in list(c.data.items()):
                     data.extend(instances)
-                adminaction_end.send(sender=modeladmin.model,
-                                     action='export_delete_tree',
-                                     request=request,
-                                     queryset=queryset,
-                                     modeladmin=modeladmin,
-                                     form=form)
-                if hasattr(modeladmin, 'get_export_delete_tree_filename'):
-                    filename = modeladmin.get_export_delete_tree_filename(request, queryset)
+                adminaction_end.send(
+                    sender=modeladmin.model,
+                    action="export_delete_tree",
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
+                if hasattr(modeladmin, "get_export_delete_tree_filename"):
+                    filename = modeladmin.get_export_delete_tree_filename(
+                        request, queryset
+                    )
                 else:
                     filename = None
                 return _dump_qs(form, queryset, data, filename)
             except AttributeError as e:
                 messages.error(request, str(e))
                 return HttpResponseRedirect(request.path)
     else:
         form = form_class(initial=initial)
 
-    adminForm = helpers.AdminForm(form, modeladmin.get_fieldsets(request), {}, model_admin=modeladmin)
+    adminForm = helpers.AdminForm(
+        form, modeladmin.get_fieldsets(request), {}, model_admin=modeladmin
+    )
     media = modeladmin.media + adminForm.media
-    tpl = 'adminactions/export_fixture.html'
-    ctx = {'adminform': adminForm,
-           'change': True,
-           'action_short_description': export_delete_tree.short_description,
-           'title': u"%s (%s)" % (
-               export_delete_tree.short_description.capitalize(),
-               modeladmin.opts.verbose_name_plural,
-           ),
-           'is_popup': False,
-           'save_as': False,
-           'has_delete_permission': False,
-           'has_add_permission': False,
-           'has_change_permission': True,
-           'queryset': queryset,
-           'opts': queryset.model._meta,
-           'app_label': queryset.model._meta.app_label,
-           'media': mark_safe(media)}
+    tpl = "adminactions/export_fixture.html"
+    ctx = {
+        "adminform": adminForm,
+        "change": True,
+        "action_short_description": export_delete_tree.short_description,
+        "title": "%s (%s)"
+        % (
+            export_delete_tree.short_description.capitalize(),
+            modeladmin.opts.verbose_name_plural,
+        ),
+        "is_popup": False,
+        "save_as": False,
+        "has_delete_permission": False,
+        "has_add_permission": False,
+        "has_change_permission": True,
+        "queryset": queryset,
+        "opts": queryset.model._meta,
+        "app_label": queryset.model._meta.app_label,
+        "media": mark_safe(media),
+    }
     ctx.update(modeladmin.admin_site.each_context(request))
     return render(request, tpl, ctx)
 
 
 export_delete_tree.short_description = _("Export delete tree")
-export_delete_tree.base_permission = 'adminactions_export'
+export_delete_tree.base_permission = "adminactions_export"
```

### Comparing `django-adminactions-2.0.0/src/adminactions/graph.py` & `django-adminactions-2.1.0/src/adminactions/graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+
 from django.contrib import messages
 from django.contrib.admin import helpers
 from django.db.models.aggregates import Count
 from django.db.models.fields.related import ForeignKey
 from django.forms.fields import BooleanField, CharField, ChoiceField
 from django.forms.forms import DeclarativeFieldsMetaclass, Form
 from django.forms.widgets import HiddenInput, MultipleHiddenInput
@@ -16,141 +17,182 @@
 from .utils import get_field_by_name
 
 
 def graph_form_factory(model):
     app_name = model._meta.app_label
     model_name = model.__name__
 
-    model_fields = [(str(f.name), str(f.verbose_name)) for f in model._meta.fields if not f.primary_key]
-    graphs = [('PieChart', 'PieChart'), ('BarChart', 'BarChart')]
-    model_fields.insert(0, ('', 'N/A'))
+    model_fields = [
+        (str(f.name), str(f.verbose_name))
+        for f in model._meta.fields
+        if not f.primary_key
+    ]
+    graphs = [("PieChart", "PieChart"), ("BarChart", "BarChart")]
+    model_fields.insert(0, ("", "N/A"))
     class_name = "%s%sGraphForm" % (app_name, model_name)
-    attrs = {'initial': {'app': app_name, 'model': model_name},
-             '_selected_action': CharField(widget=MultipleHiddenInput),
-             'select_across': BooleanField(initial='0', widget=HiddenInput, required=False),
-             'app': CharField(initial=app_name, widget=HiddenInput),
-             'model': CharField(initial=model_name, widget=HiddenInput),
-             'graph_type': ChoiceField(label=_("Graph type"), choices=graphs, required=True),
-             'axes_x': ChoiceField(label=_("Group by and count by"), choices=model_fields, required=True)}
+    attrs = {
+        "initial": {"app": app_name, "model": model_name},
+        "_selected_action": CharField(widget=MultipleHiddenInput),
+        "select_across": BooleanField(initial="0", widget=HiddenInput, required=False),
+        "app": CharField(initial=app_name, widget=HiddenInput),
+        "model": CharField(initial=model_name, widget=HiddenInput),
+        "graph_type": ChoiceField(label=_("Graph type"), choices=graphs, required=True),
+        "axes_x": ChoiceField(
+            label=_("Group by and count by"), choices=model_fields, required=True
+        ),
+    }
 
     return DeclarativeFieldsMetaclass(str(class_name), (Form,), attrs)
 
 
 def graph_queryset(modeladmin, request, queryset):  # noqa
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label.lower(),
-                            get_permission_codename(graph_queryset.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label.lower(),
+        get_permission_codename(graph_queryset.base_permission, opts),
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
 
     MForm = graph_form_factory(modeladmin.model)
 
     graph_type = table = None
-    extra = '{}'
+    extra = "{}"
     try:
-        adminaction_requested.send(sender=modeladmin.model,
-                                   action='graph_queryset',
-                                   request=request,
-                                   queryset=queryset,
-                                   modeladmin=modeladmin)
+        adminaction_requested.send(
+            sender=modeladmin.model,
+            action="graph_queryset",
+            request=request,
+            queryset=queryset,
+            modeladmin=modeladmin,
+        )
     except ActionInterrupted as e:
         messages.error(request, str(e))
         return
 
-    if 'apply' in request.POST:
+    if "apply" in request.POST:
         form = MForm(request.POST)
         if form.is_valid():
             try:
-                adminaction_start.send(sender=modeladmin.model,
-                                       action='graph_queryset',
-                                       request=request,
-                                       queryset=queryset,
-                                       modeladmin=modeladmin,
-                                       form=form)
+                adminaction_start.send(
+                    sender=modeladmin.model,
+                    action="graph_queryset",
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
             except ActionInterrupted as e:
                 messages.error(request, str(e))
                 return
             try:
-                x = form.cleaned_data['axes_x']
+                x = form.cleaned_data["axes_x"]
                 # y = form.cleaned_data['axes_y']
-                graph_type = form.cleaned_data['graph_type']
+                graph_type = form.cleaned_data["graph_type"]
 
                 field, model, direct, m2m = get_field_by_name(modeladmin.model, x)
                 cc = queryset.values_list(x).annotate(Count(x)).order_by()
                 if isinstance(field, ForeignKey):
                     data_labels = []
                     for value, cnt in cc:
                         data_labels.append(str(field.rel.to.objects.get(pk=value)))
                 elif isinstance(field, BooleanField):
                     data_labels = [str(label) for label, v in cc]
-                elif hasattr(modeladmin.model, 'get_%s_display' % field.name):
+                elif hasattr(modeladmin.model, "get_%s_display" % field.name):
                     data_labels = []
                     for value, cnt in cc:
-                        data_labels.append(smart_str(dict(field.flatchoices).get(value, value), strings_only=True))
+                        data_labels.append(
+                            smart_str(
+                                dict(field.flatchoices).get(value, value),
+                                strings_only=True,
+                            )
+                        )
                 else:
                     data_labels = [str(label) for label, v in cc]
                 data = [str(v) for label, v in cc]
 
-                if graph_type == 'BarChart':
+                if graph_type == "BarChart":
                     table = [data]
                     extra = """{seriesDefaults:{renderer:$.jqplot.BarRenderer,
                                                 rendererOptions: {fillToZero: true,
                                                                   barDirection: 'horizontal'},
                                                 shadowAngle: -135,
                                                },
                                 series:[%s],
                                 axes: {yaxis: {renderer: $.jqplot.CategoryAxisRenderer,
                                                 ticks: %s},
                                        xaxis: {pad: 1.05,
                                                tickOptions: {formatString: '%%d'}}
                                       }
-                                }""" % (json.dumps(data_labels), json.dumps(data_labels))
-                elif graph_type == 'PieChart':
-                    table = [list(zip(list(map(str, data_labels)), list(map(str, data))))]
+                                }""" % (
+                        json.dumps(data_labels),
+                        json.dumps(data_labels),
+                    )
+                elif graph_type == "PieChart":
+                    table = [
+                        list(zip(list(map(str, data_labels)), list(map(str, data))))
+                    ]
                     extra = """{seriesDefaults: {renderer: jQuery.jqplot.PieRenderer,
                                                 rendererOptions: {fill: true,
                                                                     showDataLabels: true,
                                                                     sliceMargin: 4,
                                                                     lineWidth: 5}},
                              legend: {show: true, location: 'e'}}"""
 
             except Exception as e:
-                messages.error(request, 'Unable to produce valid data: %s' % str(e))
+                messages.error(request, "Unable to produce valid data: %s" % str(e))
             else:
-                adminaction_end.send(sender=modeladmin.model,
-                                     action='graph_queryset',
-                                     request=request,
-                                     queryset=queryset,
-                                     modeladmin=modeladmin,
-                                     form=form)
-    elif request.method == 'POST':
-        initial = {helpers.ACTION_CHECKBOX_NAME: request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-                   'select_across': request.POST.get('select_across', 0)}
+                adminaction_end.send(
+                    sender=modeladmin.model,
+                    action="graph_queryset",
+                    request=request,
+                    queryset=queryset,
+                    modeladmin=modeladmin,
+                    form=form,
+                )
+    elif request.method == "POST":
+        initial = {
+            helpers.ACTION_CHECKBOX_NAME: request.POST.getlist(
+                helpers.ACTION_CHECKBOX_NAME
+            ),
+            "select_across": request.POST.get("select_across", 0),
+        }
         form = MForm(initial=initial)
     else:
-        initial = {helpers.ACTION_CHECKBOX_NAME: request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-                   'select_across': request.POST.get('select_across', 0)}
+        initial = {
+            helpers.ACTION_CHECKBOX_NAME: request.POST.getlist(
+                helpers.ACTION_CHECKBOX_NAME
+            ),
+            "select_across": request.POST.get("select_across", 0),
+        }
         form = MForm(initial=initial)
 
-    adminForm = helpers.AdminForm(form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin)
+    adminForm = helpers.AdminForm(
+        form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin
+    )
     media = modeladmin.media + adminForm.media
 
-    ctx = {'adminform': adminForm,
-           'action': 'graph_queryset',
-           'opts': modeladmin.model._meta,
-           'action_short_description': graph_queryset.short_description,
-           'title': u"%s (%s)" % (
-               graph_queryset.short_description.capitalize(),
-               smart_str(modeladmin.opts.verbose_name_plural),
-           ),
-           'app_label': queryset.model._meta.app_label,
-           'media': media,
-           'extra': extra,
-           'as_json': json.dumps(table),
-           'graph_type': graph_type}
+    ctx = {
+        "adminform": adminForm,
+        "action": "graph_queryset",
+        "opts": modeladmin.model._meta,
+        "action_short_description": graph_queryset.short_description,
+        "title": "%s (%s)"
+        % (
+            graph_queryset.short_description.capitalize(),
+            smart_str(modeladmin.opts.verbose_name_plural),
+        ),
+        "app_label": queryset.model._meta.app_label,
+        "media": media,
+        "extra": extra,
+        "as_json": json.dumps(table),
+        "graph_type": graph_type,
+    }
     ctx.update(modeladmin.admin_site.each_context(request))
-    return render(request, 'adminactions/charts.html', ctx)
+    return render(request, "adminactions/charts.html", ctx)
 
 
 graph_queryset.short_description = _("Graph selected records")
-graph_queryset.base_permission = 'adminactions_chart'
+graph_queryset.base_permission = "adminactions_chart"
```

### Comparing `django-adminactions-2.0.0/src/adminactions/helpers.py` & `django-adminactions-2.1.0/src/adminactions/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,59 +11,71 @@
     fixture_file = forms.FileField(required=False)
     fixture_content = forms.CharField(widget=forms.Textarea, required=False)
 
     use_natural_foreign_keys = forms.BooleanField(required=False)
     use_natural_primary_keys = forms.BooleanField(required=False)
 
     def clean(self):
-        if not (self.cleaned_data['fixture_file'] or self.cleaned_data['fixture_content']):
-            raise ValidationError('You must provide file or content')
+        if not (
+            self.cleaned_data["fixture_file"] or self.cleaned_data["fixture_content"]
+        ):
+            raise ValidationError("You must provide file or content")
 
 
 def import_fixture(modeladmin, request):
     context = modeladmin.get_common_context(request)
-    if request.method == 'POST':
+    if request.method == "POST":
         form = ImportFixtureForm(data=request.POST)
         if form.is_valid():
-            use_natural_fk = form.cleaned_data['use_natural_foreign_keys']
-            use_natural_pk = form.cleaned_data['use_natural_primary_keys']
-            ser_fmt = 'json'
+            use_natural_fk = form.cleaned_data["use_natural_foreign_keys"]
+            use_natural_pk = form.cleaned_data["use_natural_primary_keys"]
+            ser_fmt = "json"
             try:
-                if form.cleaned_data['fixture_content']:
-                    fixture_data = form.cleaned_data['fixture_content']
+                if form.cleaned_data["fixture_content"]:
+                    fixture_data = form.cleaned_data["fixture_content"]
                 else:
-                    fixture_data = request.FILES['fixture_file'].read()
+                    fixture_data = request.FILES["fixture_file"].read()
 
-                ser_fmt = 'json'
-                objects = serializers.deserialize(ser_fmt, fixture_data,
-                                                  use_natural_foreign_keys=use_natural_fk,
-                                                  use_natural_primary_keys=use_natural_pk)
+                ser_fmt = "json"
+                objects = serializers.deserialize(
+                    ser_fmt,
+                    fixture_data,
+                    use_natural_foreign_keys=use_natural_fk,
+                    use_natural_primary_keys=use_natural_pk,
+                )
                 imported = 0
                 for obj in objects:
                     obj.save()
                     imported += 1
 
                 modeladmin.message_user(request, imported, messages.SUCCESS)
             except Exception as e:
-                modeladmin.message_user(request, f'{e.__class__.__name__}: {e}', messages.ERROR)
+                modeladmin.message_user(
+                    request, f"{e.__class__.__name__}: {e}", messages.ERROR
+                )
 
     else:
         form = ImportFixtureForm()
-    context['form'] = form
-    context['action'] = 'Import fixture'
-    return TemplateResponse(request, "adminactions/helpers/import_fixture.html", context)
+    context["form"] = form
+    context["action"] = "Import fixture"
+    return TemplateResponse(
+        request, "adminactions/helpers/import_fixture.html", context
+    )
 
 
 class AdminActionPermMixin:
     def _filter_actions_by_permissions(self, request, actions):
         opts = self.model._meta
         filtered_actions = []
         actions = super()._filter_actions_by_permissions(request, actions)
         from .actions import actions as aa
+
         for action in actions:
             if action[0] in aa:
-                perm = "{0}.{1}".format(opts.app_label,
-                                        get_permission_codename(action[0].base_permission, opts))
+                perm = "{0}.{1}".format(
+                    opts.app_label,
+                    get_permission_codename(action[0].base_permission, opts),
+                )
                 if not request.user.has_perm(perm):
                     continue
             filtered_actions.append(action)
         return filtered_actions
```

### Comparing `django-adminactions-2.0.0/src/adminactions/locale/en/LC_MESSAGES/django.po` & `django-adminactions-2.1.0/src/adminactions/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/locale/es/LC_MESSAGES/django.po` & `django-adminactions-2.1.0/src/adminactions/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/locale/fr/LC_MESSAGES/django.po` & `django-adminactions-2.1.0/src/adminactions/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/locale/it/LC_MESSAGES/django.po` & `django-adminactions-2.1.0/src/adminactions/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/locale/pl/LC_MESSAGES/django.po` & `django-adminactions-2.1.0/src/adminactions/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/locale/pt_BR/LC_MESSAGES/django.po` & `django-adminactions-2.1.0/src/adminactions/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/mass_update.py` & `django-adminactions-2.1.0/src/adminactions/mass_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,55 @@
+import logging
 import re
-from collections import OrderedDict as SortedDict, defaultdict
+from collections import OrderedDict as SortedDict
+from collections import defaultdict
+
 from django import forms
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.admin import helpers
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
-from django.db.models import ForeignKey, fields as df
+from django.core.files import File
+from django.db.models import FileField, ForeignKey
+from django.db.models import fields as df
 from django.db.transaction import atomic
 from django.forms import fields as ff
-from django.forms.models import (InlineForeignKeyField,
-                                 ModelMultipleChoiceField, construct_instance,
-                                 modelform_factory,)
+from django.forms.models import (
+    InlineForeignKeyField,
+    ModelMultipleChoiceField,
+    construct_instance,
+    modelform_factory,
+)
 from django.http import HttpResponseRedirect
 from django.shortcuts import render
 from django.utils.encoding import smart_str
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 
 from . import config
 from .compat import celery_present
 from .exceptions import ActionInterrupted
 from .forms import GenericActionForm
 from .perms import get_permission_codename
 from .signals import adminaction_end, adminaction_requested, adminaction_start
 from .utils import curry, get_field_by_name
 
-DO_NOT_MASS_UPDATE = 'do_NOT_mass_UPDATE'
+logger = logging.getLogger(__name__)
+
+DO_NOT_MASS_UPDATE = "do_NOT_mass_UPDATE"
 
 add = lambda arg, value: value + arg
 sub = lambda arg, value: value - arg
 add_percent = lambda arg, value: value + (value * arg / 100)
 sub_percent = lambda arg, value: value - (value * arg / 100)
 negate = lambda value: not value
 trim = lambda arg, value: value.strip(arg)
 
-change_domain = lambda arg, value: re.sub('@.*', arg, value)
-change_protocol = lambda arg, value: re.sub('^[a-z]*://', "%s://" % arg, value)
+change_domain = lambda arg, value: re.sub("@.*", arg, value)
+change_protocol = lambda arg, value: re.sub("^[a-z]*://", "%s://" % arg, value)
 
 disable_if_not_nullable = lambda field: field.null
 disable_if_unique = lambda field: not field.unique
 
 
 class OperationManager:
     """
@@ -54,270 +64,343 @@
     enabler: boolean or callable that receive the specific Model field as argument
             and should returns True/False to indicate the `function` can be used with this
             specific field. i.e. disable 'set null` if the field cannot be null, or disable `set` if
             the field is unique
     description: string description of the operator
     """
 
-    COMMON = [('set', (None, True, disable_if_unique, "")),
-              ('set null', (lambda old_value: None, False, disable_if_not_nullable, ""))]
+    COMMON = [
+        ("set", (None, True, disable_if_unique, "")),
+        ("set null", (lambda old_value: None, False, disable_if_not_nullable, "")),
+    ]
 
     def __init__(self, _dict):
-        self._dict = dict()
+        self._dict = defaultdict(SortedDict)
         self.operations = dict()
-        for field_class, args in list(_dict.items()):
-            self._dict[field_class] = SortedDict(self.COMMON + args)
-            for label, (func, param, enabler, help) in args:
-                self.operations[label] = func
+        self.register_operations(df.Field, self.COMMON)
+        for field_class, args in _dict.items():
+            self.register_operations(field_class, args)
+
+    def register_operations(self, field_class, operations):
+        for label, operation in operations:
+            self._dict[field_class][label] = operation
+            if operation:
+                self.operations[label] = operation[0]
 
     def get_function(self, name):
         return self.operations.get(name, None)
 
-    def get(self, field_class, d=None):
-        return self._dict.get(field_class, SortedDict(self.COMMON))
+    def get(self, field_class: type):
+        data = SortedDict()
+        # reversed to make the most specific overrule the more general ones
+        for typ in reversed(field_class.__mro__):
+            data |= self._dict.get(typ, ())
+        return data
+
+    def operation_enabled(self, field, operation):
+        if operation:
+            enabler = operation[2]
+            return enabler is True or (callable(enabler) and enabler(field))
+        return False
 
     def get_for_field(self, field):
-        """ returns valid functions for passed field
-            :param field Field django Model Field
-            :return list of (label, (__, param, enabler, help))
+        """returns valid functions for passed field
+        :param field Field django Model Field
+        :return list of (label, (__, param, enabler, help))
         """
-        valid = SortedDict()
-        operators = self.get(field.__class__)
-        for label, (func, param, enabler, help) in list(operators.items()):
-            if (callable(enabler) and enabler(field)) or enabler is True:
-                valid[label] = (func, param, enabler, help)
-        return valid
+        return SortedDict(
+            [
+                (label, operation)
+                for label, operation in self.get(field.__class__).items()
+                if self.operation_enabled(field, operation)
+            ]
+        )
 
     def __getitem__(self, field_class):
         return self.get(field_class)
 
 
-OPERATIONS = OperationManager({
-    df.CharField: [('upper', (str.upper, False, True, _("convert to uppercase"))),
-                   ('lower', (str.lower, False, True, _("convert to lowercase"))),
-                   ('capitalize', (str.capitalize, False, True, _("capitalize first character"))),
-                   ('trim', (str.strip, False, True, _("leading and trailing whitespace")))],
-    df.IntegerField: [('add percent', (add_percent, True, True, _("add <arg> percent to existing value"))),
-                      ('sub percent', (sub_percent, True, True, "")),
-                      ('sub', (sub_percent, True, True, "")),
-                      ('add', (add, True, True, ""))],
-    df.BooleanField: [('toggle', (negate, False, True, ""))],
-    df.NullBooleanField: [('toggle', (negate, False, True, ""))],
-    df.EmailField: [('change domain', (change_domain, True, True, "")),
-                    ('upper', (str.upper, False, True, _("convert to uppercase"))),
-                    ('lower', (str.lower, False, True, _("convert to lowercase")))],
-    df.URLField: [('change protocol', (change_protocol, True, True, ""))]
-})
+OPERATIONS = OperationManager(
+    {
+        df.CharField: [
+            ("upper", (str.upper, False, True, _("convert to uppercase"))),
+            ("lower", (str.lower, False, True, _("convert to lowercase"))),
+            (
+                "capitalize",
+                (str.capitalize, False, True, _("capitalize first character")),
+            ),
+            ("trim", (str.strip, False, True, _("leading and trailing whitespace"))),
+        ],
+        df.IntegerField: [
+            (
+                "add percent",
+                (add_percent, True, True, _("add <arg> percent to existing value")),
+            ),
+            ("sub percent", (sub_percent, True, True, "")),
+            ("sub", (sub_percent, True, True, "")),
+            ("add", (add, True, True, "")),
+        ],
+        df.BooleanField: [("toggle", (negate, False, True, ""))],
+        # df.NullBooleanField: [("toggle", (negate, False, True, ""))],
+        df.EmailField: [
+            ("change domain", (change_domain, True, True, "")),
+            ("upper", (str.upper, False, True, _("convert to uppercase"))),
+            ("lower", (str.lower, False, True, _("convert to lowercase"))),
+        ],
+        df.URLField: [("change protocol", (change_protocol, True, True, ""))],
+    }
+)
 
 
 class MassUpdateForm(GenericActionForm):
-    _async = forms.BooleanField(label='Async',
-                                required=False,
-                                help_text=_("use Celery to run update in background"))
-    _clean = forms.BooleanField(label='Clean()',
-                                required=False,
-                                help_text=_("if checked calls obj.clean()"))
-
-    _validate = forms.BooleanField(label='Validate',
-                                   required=False,
-                                   help_text=_("if checked use obj.save() instead of manager.update()"))
+    _async = forms.BooleanField(
+        label="Async",
+        required=False,
+        help_text=_("use Celery to run update in background"),
+    )
+    _clean = forms.BooleanField(
+        label="Clean()", required=False, help_text=_("if checked calls obj.clean()")
+    )
+
+    _validate = forms.BooleanField(
+        label="Validate",
+        required=False,
+        help_text=_("if checked use obj.save() instead of manager.update()"),
+    )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._errors = None
         self.update_using_queryset_allowed = True
         if not celery_present:
-            self.fields['_async'].widget = forms.HiddenInput()
-        self.fields = {k: v for k, v in sorted(self.fields.items(), key=lambda item: item[1].label or '')}
+            self.fields["_async"].widget = forms.HiddenInput()
+        self.fields = {
+            k: v
+            for k, v in sorted(
+                self.fields.items(), key=lambda item: item[1].label or ""
+            )
+        }
 
     def _get_validation_exclusions(self):
-        exclude = super()._get_validation_exclusions()
+        exclude = list(super()._get_validation_exclusions())
         for name, field in list(self.fields.items()):
-            function = self.data.get('func_id_%s' % name, False)
+            function = self.data.get("func_id_%s" % name, False)
             if function:
                 exclude.append(name)
         return exclude
 
     def _post_clean(self):
         # must be overriden to bypass instance.clean()
-        if self.cleaned_data.get('_clean', False):
+        if self.cleaned_data.get("_clean", False):
             opts = self._meta
-            self.instance = construct_instance(self, self.instance, opts.fields, opts.exclude)
+            self.instance = construct_instance(
+                self, self.instance, opts.fields, opts.exclude
+            )
             exclude = self._get_validation_exclusions()
             for f_name, field in list(self.fields.items()):
                 if isinstance(field, InlineForeignKeyField):
                     exclude.append(f_name)
                     # Clean the model instance's fields.
             try:
                 self.instance.clean_fields(exclude=exclude)
             except ValidationError as e:
                 self._update_errors(e.message_dict)
 
     def full_clean(self):
         super().full_clean()
         if not self.is_bound:  # Stop further processing.
             return
+        for field_name, value in list(self.cleaned_data.items()):
+            if isinstance(self.fields.get(field_name, ""), forms.FileField):
+                if self.cleaned_data["_async"] and self.cleaned_data.get(
+                    field_name, None
+                ):
+                    self.add_error(field_name, _("Cannot use Async with FileField"))
 
-        if not self.cleaned_data.get('_validate'):
+        if not self.cleaned_data.get("_validate"):
             if not self.update_using_queryset_allowed:
                 self.add_error(None, "Cannot use operators without 'validate'")
             else:
                 for field_name, value in list(self.cleaned_data.items()):
-                    if isinstance(self.fields.get(field_name, ''), ModelMultipleChoiceField):
-                        self.add_error(field_name, _("Unable no mass update ManyToManyField"
-                                                     " without 'validate'"))
+                    if isinstance(
+                        self.fields.get(field_name, ""), ModelMultipleChoiceField
+                    ):
+                        self.add_error(
+                            field_name,
+                            _(
+                                "Unable no mass update ManyToManyField"
+                                " without 'validate'"
+                            ),
+                        )
 
     def _clean_fields(self):
         self.update_using_queryset_allowed = True
         for name, field in list(self.fields.items()):
-            raw_value = field.widget.value_from_datadict(self.data, self.files, self.add_prefix(name))
+            raw_value = field.widget.value_from_datadict(
+                self.data, self.files, self.add_prefix(name)
+            )
             try:
                 value = raw_value
                 initial = self.initial.get(name, field.initial)
                 if isinstance(field, ff.FileField):
                     value = field.clean(raw_value, initial)
                 else:
-                    enabler = 'chk_id_%s' % name
-                    function = self.data.get('func_id_%s' % name, '')
-                    apply = self.data.get(enabler, '') == 'on'
+                    enabler = "chk_id_%s" % name
+                    function = self.data.get("func_id_%s" % name, "")
+                    apply = self.data.get(enabler, "") == "on"
                     self.cleaned_data[enabler] = apply
-                    self.cleaned_data['func_id_%s' % name] = function
+                    self.cleaned_data["func_id_%s" % name] = function
                     # self.cleaned_data[name] = field.clean(raw_value)
                     if apply:
-                        field_object, model, direct, m2m = get_field_by_name(self._meta.model, name)
+                        field_object, model, direct, m2m = get_field_by_name(
+                            self._meta.model, name
+                        )
                         value = field.clean(raw_value)
                         if function:
-                            func, hasparm, __, __ = OPERATIONS.get_for_field(field_object)[function]
+                            func, hasparm, __, __ = OPERATIONS.get_for_field(
+                                field_object
+                            )[function]
                             self.update_using_queryset_allowed &= func is None
                             if func is None:
                                 pass
                             elif hasparm:
                                 value = curry(func, value)
                             else:
                                 value = func
                         self.cleaned_data[name] = value
-                if hasattr(self, 'clean_%s' % name):
-                    value = getattr(self, 'clean_%s' % name)()
+                if hasattr(self, "clean_%s" % name):
+                    value = getattr(self, "clean_%s" % name)()
                 self.cleaned_data[name] = value
             except ValidationError as e:
                 self._errors[name] = self.error_class(e.messages)
                 if name in self.cleaned_data:
                     del self.cleaned_data[name]
 
     def clean__validate(self):
-        return bool(self.data.get('_validate', 0))
+        return bool(self.data.get("_validate", 0))
 
     def clean__async(self):
-        return bool(self.data.get('_async', 0))
+        return bool(self.data.get("_async", 0))
 
     def clean__clean(self):
-        return bool(self.data.get('_clean', 0))
+        return bool(self.data.get("_clean", 0))
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         return super().media + forms.Media(
             js=(
-                'admin/js/vendor/jquery/jquery%s.js' % extra,
-                'adminactions/js/massupdate%s.js' % extra,
+                "admin/js/vendor/jquery/jquery%s.js" % extra,
+                "adminactions/js/massupdate%s.js" % extra,
             ),
             css={
-                'screen': (
-                    'adminactions/css/massupdate.css',
-                ),
+                "screen": ("adminactions/css/massupdate.css",),
             },
         )
 
     def fix_json(self):
         for label, field in self.fields.items():
             if isinstance(field, forms.JSONField):
                 field.disabled = label not in self.data
 
 
 def mass_update_execute(queryset, rules, validate, clean, user_pk, request=None):
     errors = {}
     updated = 0
     opts = queryset.model._meta
-    adminaction_start.send(sender=queryset.model,
-                           action='mass_update',
-                           request=request,
-                           queryset=queryset)
+    adminaction_start.send(
+        sender=queryset.model, action="mass_update", request=request, queryset=queryset
+    )
     try:
         with atomic():
             if not validate:
-                values = {field_name: value for field_name, (func_name, value) in rules.items()}
+                values = {
+                    field_name: value
+                    for field_name, (func_name, value) in rules.items()
+                }
                 queryset.update(**values)
             else:
                 for record in queryset:
                     for field_name, (func_name, value) in rules.items():
-                        func = OPERATIONS.get_function(func_name)
-                        if callable(func):
-                            old_value = getattr(record, field_name)
-                            setattr(record, field_name, func(old_value))
+                        field = queryset.model._meta.get_field(field_name)
+                        if isinstance(field, FileField):
+                            file_field = getattr(record, field_name)
+                            file_field.save(value.name, File(value.file))
                         else:
-                            changed_attr = getattr(record, field_name, None)
-                            if changed_attr.__class__.__name__ == 'ManyRelatedManager':
-                                changed_attr.set(value)
+                            func = OPERATIONS.get_function(func_name)
+                            if callable(func):
+                                old_value = getattr(record, field_name)
+                                setattr(record, field_name, func(old_value))
                             else:
-                                setattr(record, field_name, value)
+                                changed_attr = getattr(record, field_name, None)
+                                if (
+                                    changed_attr.__class__.__name__
+                                    == "ManyRelatedManager"
+                                ):
+                                    changed_attr.set(value)
+                                else:
+                                    setattr(record, field_name, value)
 
                     if clean:
                         record.clean()
                     record.save()
                     updated += 1
-            adminaction_end.send(sender=queryset.model,
-                                 action='mass_update',
-                                 request=request,
-                                 queryset=queryset)
+            adminaction_end.send(
+                sender=queryset.model,
+                action="mass_update",
+                request=request,
+                queryset=queryset,
+            )
             if config.AA_ENABLE_LOG:
                 from django.contrib.admin.models import CHANGE, LogEntry
-                ids = list(queryset.only("pk").values_list('pk', flat=True))
+
+                ids = list(queryset.only("pk").values_list("pk", flat=True))
                 LogEntry.objects.log_action(
                     user_id=user_pk,
                     content_type_id=None,
                     object_id=None,
-                    object_repr=f'Mass Update {opts.model_name}',
+                    object_repr=f"Mass Update {opts.model_name}",
                     action_flag=CHANGE,
-                    change_message={"rules": str(rules),
-                                    "records": ids
-                                    }
+                    change_message={"rules": str(rules), "records": ids},
                 )
     except ActionInterrupted:
         updated, errors = 0, {}
 
     return updated, errors
 
 
 def mass_update(modeladmin, request, queryset):  # noqa
     """
-        mass update queryset
+    mass update queryset
     """
 
     def not_required(field, **kwargs):
-        """ force all fields as not required"""
-        kwargs['required'] = False
-        kwargs['request'] = request
+        """force all fields as not required"""
+        kwargs["required"] = False
+        kwargs["request"] = request
         return modeladmin.formfield_for_dbfield(field, **kwargs)
 
     def _get_sample():
         grouped = defaultdict(lambda: [])
         for f in mass_update_hints:
             if isinstance(f, ForeignKey):
                 # Filter by queryset so we only get results without our
                 # current resultset
                 filters = {"%s__in" % f.remote_field.name: queryset}
                 # Order by random to get a nice sample
-                query = f.related_model.objects.filter(**filters).distinct().order_by('?')
+                query = (
+                    f.related_model.objects.filter(**filters).distinct().order_by("?")
+                )
                 # Limit the amount of results so we don't accidently query
                 # many thousands of items and kill the database.
                 grouped[f.name] = [(a.pk, str(a)) for a in query[:10]]
-            elif hasattr(f, 'flatchoices') and f.flatchoices:
-                grouped[f.name] = dict(getattr(f, 'flatchoices')).keys()
-            elif hasattr(f, 'choices') and f.choices:
-                grouped[f.name] = dict(getattr(f, 'choices')).keys()
+            elif hasattr(f, "flatchoices") and f.flatchoices:
+                grouped[f.name] = dict(getattr(f, "flatchoices")).keys()
+            elif hasattr(f, "choices") and f.choices:
+                grouped[f.name] = dict(getattr(f, "choices")).keys()
             elif isinstance(f, df.BooleanField):
                 grouped[f.name] = [("True", True), ("False", False)]
         already_grouped = set(grouped)
         for el in queryset.all()[:10]:
             for f in modeladmin.model._meta.fields:
                 if f.name in mass_update_hints and f.name not in already_grouped:
                     value = getattr(el, f.name)
@@ -325,125 +408,154 @@
                     if value is not None and target not in grouped[f.name]:
                         grouped[f.name].append(target)
 
                     initial[f.name] = initial.get(f.name, value)
         return grouped
 
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label,
-                            get_permission_codename(mass_update.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label, get_permission_codename(mass_update.base_permission, opts)
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
-    if 'apply' not in request.POST:
+    if "apply" not in request.POST:
         try:
-            adminaction_requested.send(sender=modeladmin.model,
-                                       action='mass_update',
-                                       request=request,
-                                       queryset=queryset,
-                                       modeladmin=modeladmin)
+            adminaction_requested.send(
+                sender=modeladmin.model,
+                action="mass_update",
+                request=request,
+                queryset=queryset,
+                modeladmin=modeladmin,
+            )
         except ActionInterrupted as e:
             messages.error(request, str(e))
             return
 
-    mass_update_form = getattr(modeladmin, 'mass_update_form', MassUpdateForm)
-    mass_update_fields = getattr(modeladmin, 'mass_update_fields', None)
-    mass_update_exclude = getattr(modeladmin, 'mass_update_exclude', None)
+    mass_update_form = getattr(modeladmin, "mass_update_form", MassUpdateForm)
+    mass_update_fields = getattr(modeladmin, "mass_update_fields", None)
+    mass_update_exclude = getattr(modeladmin, "mass_update_exclude", None)
     if mass_update_fields and mass_update_exclude:
-        raise Exception("Cannot set both 'mass_update_exclude' and 'mass_update_fields'")
+        raise Exception(
+            "Cannot set both 'mass_update_exclude' and 'mass_update_fields'"
+        )
 
     if mass_update_exclude is None:
-        mass_update_exclude = ['pk']
-    elif 'pk' not in mass_update_exclude:
-        mass_update_exclude.append('pk')
-    mass_update_hints = getattr(modeladmin, 'mass_update_hints', [])
-
-    MForm = modelform_factory(modeladmin.model, form=mass_update_form,
-                              exclude=mass_update_exclude,
-                              fields=mass_update_fields,
-                              formfield_callback=not_required)
-    initial = {'_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-               'select_across': request.POST.get('select_across') == '1',
-               'action': 'mass_update'}
+        mass_update_exclude = ["pk"]
+    elif "pk" not in mass_update_exclude:
+        mass_update_exclude.append("pk")
+    mass_update_hints = getattr(modeladmin, "mass_update_hints", [])
+
+    MForm = modelform_factory(
+        modeladmin.model,
+        form=mass_update_form,
+        exclude=mass_update_exclude,
+        fields=mass_update_fields,
+        formfield_callback=not_required,
+    )
+    initial = {
+        "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+        "select_across": request.POST.get("select_across") == "1",
+        "action": "mass_update",
+    }
     rules = {}
-    if 'apply' in request.POST:
-        form = MForm(request.POST, request.FILES, initial=initial)
-        if form.is_valid():
-            # # need_transaction = form.cleaned_data.get('_unique_transaction', False)
-            validate = form.cleaned_data.get('_validate', False)
-            clean = form.cleaned_data.get('_clean', False)
-            use_celery = form.cleaned_data.get('_async', False)
-            for field_name, value in list(form.cleaned_data.items()):
-                enabler = 'chk_id_%s' % field_name
-                if form.data.get(enabler, False) == 'on':
-                    op = form.data.get('func_id_%s' % field_name)
-                    if callable(value):
-                        value = None
-                    rules[field_name] = (op, value)
-            if use_celery:
-                from .tasks import mass_update_task
-                mass_update_task.delay(f"{opts.app_label}.{opts.model_name}",
-                                       ids=list(queryset.only("pk").values_list('pk', flat=True)),
-                                       rules=rules,
-                                       validate=validate, clean=clean,
-                                       user_pk=request.user.pk)
+    if "apply" in request.POST:
+        try:
+            form = MForm(request.POST, request.FILES, initial=initial)
+            if form.is_valid():
+                # # need_transaction = form.cleaned_data.get('_unique_transaction', False)
+                validate = form.cleaned_data.get("_validate", False)
+                clean = form.cleaned_data.get("_clean", False)
+                use_celery = form.cleaned_data.get("_async", False)
+                for field_name, value in list(form.cleaned_data.items()):
+                    enabler = "chk_id_%s" % field_name
+                    if form.data.get(enabler, False) == "on":
+                        op = form.data.get("func_id_%s" % field_name)
+                        if callable(value):
+                            value = None
+                        rules[field_name] = (op, value)
+                if use_celery:
+                    from .tasks import mass_update_task
+
+                    mass_update_task.delay(
+                        f"{opts.app_label}.{opts.model_name}",
+                        ids=list(queryset.only("pk").values_list("pk", flat=True)),
+                        rules=rules,
+                        validate=validate,
+                        clean=clean,
+                        user_pk=request.user.pk,
+                    )
+                else:
+                    try:
+                        updated, errors = mass_update_execute(
+                            queryset,
+                            rules,
+                            validate,
+                            clean,
+                            user_pk=request.user.pk,
+                            request=request,
+                        )
+                        messages.info(request, _("Updated %s records") % updated)
+                    except ActionInterrupted as e:
+                        messages.error(request, str(e))
+                        return HttpResponseRedirect(request.get_full_path())
+                return HttpResponseRedirect(request.get_full_path())
             else:
-                try:
-                    updated, errors = mass_update_execute(queryset,
-                                                          rules,
-                                                          validate,
-                                                          clean,
-                                                          user_pk=request.user.pk,
-                                                          request=request)
-                    messages.info(request, _("Updated %s records") % updated)
-                except ActionInterrupted as e:
-                    messages.error(request, str(e))
-                    return HttpResponseRedirect(request.get_full_path())
+                form.fix_json()
+        except Exception as e:
+            messages.error(request, str(e))
+            logger.exception(e)
             return HttpResponseRedirect(request.get_full_path())
-        else:
-            form.fix_json()
+
     else:
-        initial.update({'action': 'mass_update', '_validate': 1})
-        prefill_with = request.POST.get('prefill-with', None)
+        initial.update({"action": "mass_update", "_validate": 1})
+        prefill_with = request.POST.get("prefill-with", None)
         prefill_instance = None
         try:
             # Gets the instance directly from the queryset for data security
             prefill_instance = queryset.get(pk=prefill_with)
         except ObjectDoesNotExist:
             pass
 
         form = MForm(initial=initial, instance=prefill_instance)
 
     if mass_update_hints:
         sample_values = _get_sample()
     else:
         sample_values = None
-    adminForm = helpers.AdminForm(form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin)
+    adminForm = helpers.AdminForm(
+        form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin
+    )
     media = modeladmin.media + adminForm.media
     # dthandler = lambda obj: obj.isoformat() if isinstance(obj, datetime.date) else str(obj)
-    tpl = 'adminactions/mass_update.html'
-    ctx = {'adminform': adminForm,
-           'form': form,
-           'action_short_description': mass_update.short_description,
-           'title': u"%s (%s)" % (
-               mass_update.short_description.capitalize(),
-               smart_str(modeladmin.opts.verbose_name_plural),
-           ),
-           'grouped': sample_values,
-           'change': True,
-           'rules': rules,
-           'is_popup': False,
-           'save_as': False,
-           'has_delete_permission': False,
-           'has_add_permission': False,
-           'has_change_permission': True,
-           'opts': modeladmin.model._meta,
-           'app_label': modeladmin.model._meta.app_label,
-           'media': mark_safe(media),
-           'selection': queryset}
+    tpl = "adminactions/mass_update.html"
+    ctx = {
+        "adminform": adminForm,
+        "form": form,
+        "action_short_description": mass_update.short_description,
+        "title": "%s (%s)"
+        % (
+            mass_update.short_description.capitalize(),
+            smart_str(modeladmin.opts.verbose_name_plural),
+        ),
+        "grouped": sample_values,
+        "change": True,
+        "rules": rules,
+        "is_popup": False,
+        "save_as": False,
+        "has_delete_permission": False,
+        "has_add_permission": False,
+        "has_change_permission": True,
+        "opts": modeladmin.model._meta,
+        "app_label": modeladmin.model._meta.app_label,
+        "media": mark_safe(media),
+        "selection": queryset,
+    }
     ctx.update(modeladmin.admin_site.each_context(request))
 
     return render(request, tpl, context=ctx)
 
 
 mass_update.short_description = _("Mass update")
-mass_update.base_permission = 'adminactions_massupdate'
+mass_update.base_permission = "adminactions_massupdate"
```

### Comparing `django-adminactions-2.0.0/src/adminactions/merge.py` & `django-adminactions-2.1.0/src/adminactions/merge.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,209 +1,273 @@
 from datetime import datetime
+
 from django import forms
 from django.contrib import messages
 from django.contrib.admin import helpers
 from django.db import models
 from django.forms import HiddenInput, TextInput
 from django.forms.formsets import formset_factory
 from django.forms.models import model_to_dict, modelform_factory
 from django.http import HttpResponseRedirect
 from django.shortcuts import render
 from django.utils.encoding import smart_str
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 
-from . import api, compat as transaction
+from . import api
+from . import compat as transaction
 from .forms import GenericActionForm
 from .perms import get_permission_codename
+from .signals import adminaction_end, adminaction_requested, adminaction_start
 from .utils import clone_instance, get_ignored_fields
 
 
 class MergeFormBase(forms.Form):
     use_required_attribute = False
 
     DEP_MOVE = 1
     DEP_DELETE = 2
     GEN_IGNORE = 1
     GEN_RELATED = 2
     GEN_DEEP = 3
 
-    dependencies = forms.ChoiceField(label=_('Dependencies'),
-                                     choices=((DEP_MOVE, _("Move")), (DEP_DELETE, _("Delete"))))
+    dependencies = forms.ChoiceField(
+        label=_("Dependencies"),
+        choices=((DEP_MOVE, _("Move")), (DEP_DELETE, _("Delete"))),
+    )
 
     master_pk = forms.CharField(widget=HiddenInput)
     other_pk = forms.CharField(widget=HiddenInput)
     field_names = forms.CharField(required=False, widget=HiddenInput)
 
     def action_fields(self):
-        for fieldname in ['dependencies', 'master_pk', 'other_pk', 'field_names']:
-            bf = self[fieldname]
-            yield HiddenInput().render(fieldname, bf.value())
+        for field_name in ["dependencies", "master_pk", "other_pk", "field_names"]:
+            bf = self[field_name]
+            yield HiddenInput().render(field_name, bf.value())
 
     def clean_dependencies(self):
-        return int(self.cleaned_data['dependencies'])
+        return int(self.cleaned_data["dependencies"])
 
     def clean_field_names(self):
-        if self.cleaned_data['field_names']:
-            return self.cleaned_data['field_names'].split(',')
+        if self.cleaned_data["field_names"]:
+            return self.cleaned_data["field_names"].split(",")
         else:
             return None
 
     def full_clean(self):
         super().full_clean()
 
     def clean(self):
         return super().clean()
 
     def is_valid(self):
         return super().is_valid()
 
     class Media:
         js = [
-            'admin/js/vendor/jquery/jquery.js',
-            'admin/js/jquery.init.js',
-            'adminactions/js/merge.min.js',
+            "admin/js/vendor/jquery/jquery.js",
+            "admin/js/jquery.init.js",
+            "adminactions/js/merge.min.js",
         ]
-        css = {'all': ['adminactions/css/adminactions.min.css']}
+        css = {"all": ["adminactions/css/adminactions.min.css"]}
 
 
 class MergeForm(GenericActionForm, MergeFormBase):
     pass
 
 
+# noinspection PyProtectedMember
 def merge(modeladmin, request, queryset):  # noqa
     """
     Merge two model instances. Move all foreign keys.
 
     """
 
     opts = modeladmin.model._meta
-    perm = "{0}.{1}".format(opts.app_label,
-                            get_permission_codename(merge.base_permission, opts))
+    perm = "{0}.{1}".format(
+        opts.app_label, get_permission_codename(merge.base_permission, opts)
+    )
     if not request.user.has_perm(perm):
-        messages.error(request, _('Sorry you do not have rights to execute this action'))
+        messages.error(
+            request, _("Sorry you do not have rights to execute this action")
+        )
         return
 
     def raw_widget(field, **kwargs):
-        """ force all fields as not required"""
-        kwargs['widget'] = TextInput({'class': 'raw-value'})
+        """force all fields as not required"""
+        kwargs["widget"] = TextInput({"class": "raw-value"})
         if isinstance(field, models.FileField):
             kwargs["form_class"] = forms.CharField
 
         return field.formfield(**kwargs)
 
-    merge_form = getattr(modeladmin, 'merge_form', MergeForm)
-    MForm = modelform_factory(modeladmin.model,
-                              form=merge_form,
-                              exclude=('pk',),
-                              formfield_callback=raw_widget)
-    OForm = modelform_factory(modeladmin.model,
-                              exclude=('pk',),
-                              formfield_callback=raw_widget)
+    merge_form = getattr(modeladmin, "merge_form", MergeForm)
+    MForm = modelform_factory(
+        modeladmin.model,
+        form=merge_form,
+        exclude=("pk",),
+        formfield_callback=raw_widget,
+    )
+    OForm = modelform_factory(
+        modeladmin.model, exclude=("pk",), formfield_callback=raw_widget
+    )
 
-    def validate(request, master, other):
+    def validate(v_request, v_master, v_other):
         """Validate the model is still valid after the merge"""
-        merge_kwargs = {}
+        v_merge_kwargs = {}
+
         with transaction.nocommit():
-            merge_form = MergeFormBase(request.POST)
-            if merge_form.is_valid():
-                form = MForm(request.POST, instance=master)
-                if merge_form.cleaned_data['dependencies'] == MergeForm.DEP_MOVE:
-                    merge_kwargs['related'] = api.ALL_FIELDS
-                    merge_kwargs['m2m'] = api.ALL_FIELDS
+            merge_form_base = MergeFormBase(v_request.POST)
+
+            if merge_form_base.is_valid():
+                validate_form = MForm(v_request.POST, instance=v_master)
+
+                if merge_form_base.cleaned_data["dependencies"] == MergeForm.DEP_MOVE:
+                    v_merge_kwargs["related"] = api.ALL_FIELDS
+                    v_merge_kwargs["m2m"] = api.ALL_FIELDS
                 else:
-                    merge_kwargs['related'] = None
-                    merge_kwargs['m2m'] = None
-                merge_kwargs['fields'] = merge_form.cleaned_data['field_names']
-                stored_pk = other.pk
-                api.merge(master, other, commit=True, **merge_kwargs)
-                other.pk = stored_pk
-                return (form.is_valid(), form, merge_kwargs)
+                    v_merge_kwargs["related"] = None
+                    v_merge_kwargs["m2m"] = None
+
+                v_merge_kwargs["fields"] = merge_form_base.cleaned_data["field_names"]
+                stored_pk = v_other.pk
+                api.merge(v_master, v_other, commit=True, **v_merge_kwargs)
+                v_other.pk = stored_pk
+
+                return validate_form.is_valid(), validate_form, v_merge_kwargs
             else:
-                return (False, merge_form, merge_kwargs)
+                return False, merge_form_base, v_merge_kwargs
 
-    tpl = 'adminactions/merge.html'
+    name = "merge"  # Action name -- currently hardcoded - sent to signal
+    tpl = "adminactions/merge.html"
     ignored_fields = get_ignored_fields(queryset.model, "MERGE_ACTION_IGNORED_FIELDS")
 
     ctx = {
-        '_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-        'transaction_supported': 'Un',
-        'select_across': request.POST.get('select_across') == '1',
-        'action': request.POST.get('action'),
-        'fields': [f for f in queryset.model._meta.fields
-                   if not f.primary_key and f.editable and f.name not in ignored_fields],
-        'app_label': queryset.model._meta.app_label,
-        'result': '',
-        'opts': queryset.model._meta}
-    if 'preview' in request.POST:
-        master = queryset.get(pk=request.POST.get('master_pk'))
+        "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+        "transaction_supported": "Un",
+        "select_across": request.POST.get("select_across") == "1",
+        "action": request.POST.get("action"),
+        "fields": [
+            f
+            for f in queryset.model._meta.fields
+            if not f.primary_key and f.editable and f.name not in ignored_fields
+        ],
+        "app_label": queryset.model._meta.app_label,
+        "result": "",
+        "opts": queryset.model._meta,
+    }
+
+    if "preview" in request.POST and "apply" not in request.POST:
+        adminaction_requested.send(
+            sender=modeladmin.model,
+            action=name,
+            request=request,
+            queryset=queryset,
+            modeladmin=modeladmin,
+        )
+
+    if "preview" in request.POST:
+        master = queryset.get(pk=request.POST.get("master_pk"))
         original = clone_instance(master)
-        other = queryset.get(pk=request.POST.get('other_pk'))
-        formset = formset_factory(OForm)(initial=[model_to_dict(master), model_to_dict(other)])
+        other = queryset.get(pk=request.POST.get("other_pk"))
+        formset = formset_factory(OForm)(
+            initial=[model_to_dict(master), model_to_dict(other)]
+        )
         is_valid, form, merge_kwargs = validate(request, master, other)
         if is_valid:
-            ctx.update({'original': original})
-            tpl = 'adminactions/merge_preview.html'
+            ctx.update({"original": original})
+            tpl = "adminactions/merge_preview.html"
         else:
-            master = queryset.get(pk=request.POST.get('master_pk'))
-            other = queryset.get(pk=request.POST.get('other_pk'))
+            master = queryset.get(pk=request.POST.get("master_pk"))
+            other = queryset.get(pk=request.POST.get("other_pk"))
             messages.error(request, form.errors)
 
-    elif 'apply' in request.POST:
-        master = queryset.get(pk=request.POST.get('master_pk'))
-        other = queryset.get(pk=request.POST.get('other_pk'))
-        formset = formset_factory(OForm)(initial=[model_to_dict(master), model_to_dict(other)])
+    elif "apply" in request.POST:
+        master = queryset.get(pk=request.POST.get("master_pk"))
+        other = queryset.get(pk=request.POST.get("other_pk"))
+        formset = formset_factory(OForm)(
+            initial=[model_to_dict(master), model_to_dict(other)]
+        )
         ok, form, merge_kwargs = validate(request, master, other)
         if ok:
+            adminaction_start.send(
+                sender=modeladmin.model,
+                action=name,
+                request=request,
+                queryset=queryset,
+                modeladmin=modeladmin,
+                form=form,
+            )
             api.merge(master, other, commit=True, **merge_kwargs)
+            adminaction_end.send(
+                sender=modeladmin.model,
+                action=name,
+                request=request,
+                queryset=queryset,
+                modeladmin=modeladmin,
+                form=form,
+            )
+
             return HttpResponseRedirect(request.get_full_path())
         else:
             messages.error(request, form.errors)
     else:
         try:
             master, other = queryset.all()
             # django 1.4 need to remove the trailing milliseconds
-            for field in master._meta.fields:
-                if isinstance(field, models.DateTimeField):
+            for master_field in master._meta.fields:
+                if isinstance(master_field, models.DateTimeField):
                     for target in (master, other):
-                        raw_value = getattr(target, field.name)
+                        raw_value = getattr(target, master_field.name)
                         if raw_value:
                             fixed_value = datetime(
                                 raw_value.year,
                                 raw_value.month,
                                 raw_value.day,
                                 raw_value.hour,
                                 raw_value.minute,
-                                raw_value.second)
-                            setattr(target, field.name, fixed_value)
+                                raw_value.second,
+                            )
+                            setattr(target, master_field.name, fixed_value)
         except ValueError:
-            messages.error(request, _('Please select exactly 2 records'))
+            messages.error(request, _("Please select exactly 2 records"))
             return
 
-        initial = {'_selected_action': request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
-                   'select_across': 0,
-                   'generic': MergeForm.GEN_IGNORE,
-                   'dependencies': MergeForm.DEP_MOVE,
-                   'action': 'merge',
-                   'master_pk': master.pk,
-                   'other_pk': other.pk}
-        formset = formset_factory(OForm)(initial=[model_to_dict(master), model_to_dict(other)])
+        initial = {
+            "_selected_action": request.POST.getlist(helpers.ACTION_CHECKBOX_NAME),
+            "select_across": 0,
+            "generic": MergeForm.GEN_IGNORE,
+            "dependencies": MergeForm.DEP_MOVE,
+            "action": "merge",
+            "master_pk": master.pk,
+            "other_pk": other.pk,
+        }
+        formset = formset_factory(OForm)(
+            initial=[model_to_dict(master), model_to_dict(other)]
+        )
         form = MForm(initial=initial, instance=master)
 
-    adminForm = helpers.AdminForm(form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin)
+    adminForm = helpers.AdminForm(
+        form, modeladmin.get_fieldsets(request), {}, [], model_admin=modeladmin
+    )
     media = modeladmin.media + adminForm.media
-    ctx.update({'adminform': adminForm,
-                'formset': formset,
-                'media': mark_safe(media),
-                'action_short_description': merge.short_description,
-                'title': u"%s (%s)" % (
-                    merge.short_description.capitalize(),
-                    smart_str(modeladmin.opts.verbose_name_plural),
-                ),
-                'master': master,
-                'other': other})
+    ctx.update(
+        {
+            "adminform": adminForm,
+            "formset": formset,
+            "media": mark_safe(media),
+            "action_short_description": merge.short_description,
+            "title": "%s (%s)"
+            % (
+                merge.short_description.capitalize(),
+                smart_str(modeladmin.opts.verbose_name_plural),
+            ),
+            "master": master,
+            "other": other,
+        }
+    )
     ctx.update(modeladmin.admin_site.each_context(request))
     return render(request, tpl, context=ctx)
 
 
 merge.short_description = _("Merge selected %(verbose_name_plural)s")
-merge.base_permission = 'adminactions_merge'
+merge.base_permission = "adminactions_merge"
```

### Comparing `django-adminactions-2.0.0/src/adminactions/models.py` & `django-adminactions-2.1.0/src/adminactions/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,12 +4,14 @@
 
 
 def create_extra_permissions_handler(sender, **kwargs):
     global TOTAL_MODELS, COUNTER
     if config.AA_PERMISSION_HANDLER == consts.AA_PERMISSION_CREATE_USE_SIGNAL:
         perms.create_extra_permissions()
     else:
-        post_migrate.disconnect(dispatch_uid='adminactions.create_extra_permissions')
+        post_migrate.disconnect(dispatch_uid="adminactions.create_extra_permissions")
 
 
-post_migrate.connect(create_extra_permissions_handler,
-                     dispatch_uid='adminactions.create_extra_permissions')
+post_migrate.connect(
+    create_extra_permissions_handler,
+    dispatch_uid="adminactions.create_extra_permissions",
+)
```

### Comparing `django-adminactions-2.0.0/src/adminactions/perms.py` & `django-adminactions-2.1.0/src/adminactions/perms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from django.apps import apps
 
-__all__ = ["create_extra_permissions"]
+__all__ = ["create_extra_permissions", "get_permission_codename"]
 
 
 def get_permission_codename(action, opts):
-    return '%s_%s' % (action, opts.object_name.lower())
+    return "%s_%s" % (action, opts.object_name.lower())
 
 
 def get_contenttype_for_model(model):
     from django.contrib.contenttypes.models import ContentType
+
     model = model._meta.concrete_model
     opts = model._meta
     ct, __ = ContentType.objects.get_or_create(
         app_label=opts.app_label,
         model=opts.model_name,
     )
     return ct
@@ -20,30 +21,35 @@
 
 def create_extra_permissions():
     from django.contrib.auth.models import Permission
     from django.contrib.contenttypes.models import ContentType
 
     from .actions import actions as aa
 
-    perm_suffix = 'adminactions_'
+    perm_suffix = "adminactions_"
     existing_perms = set(
         Permission.objects.filter(codename__startswith=perm_suffix).values_list(
-            'codename', 'content_type_id'
+            "codename", "content_type_id"
         )
     )
     models = list(apps.get_models())
     content_types = ContentType.objects.get_for_models(*models)
+    # https://github.com/saxix/django-adminactions/issues/199
+    ContentType.objects.bulk_create(content_types.values(), ignore_conflicts=True)
 
     new_permissions = []
     for model in models:
         for action in aa:
             opts = model._meta
             codename = get_permission_codename(action.base_permission, opts)[:100]
             ct = content_types[model]
             if (codename, ct.id) in existing_perms:
                 continue
-            label = 'Can {} {} (adminactions)'.format(action.base_permission.replace(perm_suffix, ""),
-                                                      opts.verbose_name_raw)
-            permission = Permission(codename=codename, content_type=ct, name=label[:255])
+            label = "Can {} {} (adminactions)".format(
+                action.base_permission.replace(perm_suffix, ""), opts.verbose_name_raw
+            )
+            permission = Permission(
+                codename=codename, content_type=ct, name=label[:255]
+            )
             new_permissions.append(permission)
 
     Permission.objects.bulk_create(new_permissions, ignore_conflicts=True)
```

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/css/adminactions.css` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/css/adminactions.css`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/MIT-LICENSE.txt` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/README.txt` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/README.txt`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.css` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.css`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.css` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.css`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/jquery.jqplot.min.js`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -143,15 +143,15 @@
             this._stackAxis = 'y';
             this.fillAxis = 'y';
         } else {
             this._primaryAxis = '_yaxis';
             this._stackAxis = 'x';
             this.fillAxis = 'x';
         }
-        // index of the currenty highlighted point, if any
+        // index of the currently highlighted point, if any
         this._highlightedPoint = null;
         // total number of values for all bar series, total number of bar series, and position of this series
         this._plotSeriesInfo = null;
         // Array of actual data colors used for each data point.
         this._dataColors = [];
         this._barPoints = [];
```

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.min.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.barRenderer.min.js`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -220,15 +220,15 @@
                     });
                 }
             }
 
             // keep a reference to these tick labels to use for redrawing plot (see bug #57)
             this.ticks = labels;
 
-            // now bin the data values to the right lables.
+            // now bin the data values to the right labels.
             for (var i = 0; i < this._series.length; i++) {
                 var s = this._series[i];
                 for (var j = 0; j < s.data.length; j++) {
                     if (this.name == 'xaxis' || this.name == 'x2axis') {
                         val = s.data[j][0];
                     } else {
                         val = s.data[j][1];
```

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.min.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.categoryAxisRenderer.min.js`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -161,15 +161,15 @@
             this.sliceMargin = 0;
         }
 
         this._diameter = null;
         this._radius = null;
         // array of [start,end] angles arrays, one for each slice.  In radians.
         this._sliceAngles = [];
-        // index of the currenty highlighted point, if any
+        // index of the currently highlighted point, if any
         this._highlightedPoint = null;
 
         // set highlight colors if none provided
         if (this.highlightColors.length == 0) {
             for (var i = 0; i < this.seriesColors.length; i++) {
                 var rgba = $.jqplot.getColorComponents(this.seriesColors[i]);
                 var newrgb = [rgba[0], rgba[1], rgba[2]];
@@ -510,15 +510,15 @@
     $.jqplot.PieAxisRenderer.prototype.init = function(options) {
         //
         this.tickRenderer = $.jqplot.PieTickRenderer;
         $.extend(true, this, options);
         // I don't think I'm going to need _dataBounds here.
         // have to go Axis scaling in a way to fit chart onto plot area
         // and provide u2p and p2u functionality for mouse cursor, etc.
-        // for convienence set _dataBounds to 0 and 100 and
+        // for convenience set _dataBounds to 0 and 100 and
         // set min/max to 0 and 100.
         this._dataBounds = {
             min: 0,
             max: 100
         };
         this.min = 0;
         this.max = 100;
```

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.min.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/jqplot/plugins/jqplot.pieRenderer.min.js`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/massupdate.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/massupdate.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,46 +1,46 @@
-"use strict";
-(function($) {
-    $(function() {
-        $('.func_select').change(function() {
-            var $option = $(this).find(':selected');
-            var target = $(this).parent().parent().find('.col_field input, .col_field select .col_field textarea');
-            if ($option.hasClass('noparam')) {
-                $(target).attr('disabled', 'disabled');
-            } else {
+    "use strict";
+    (function($) {
+        $(function() {
+            $('.func_select').change(function() {
+                var $option = $(this).find(':selected');
+                var target = $(this).parent().parent().find('.col_field input, .col_field select .col_field textarea');
+                if ($option.hasClass('noparam')) {
+                    $(target).attr('disabled', 'disabled');
+                } else {
+                    $(target).removeAttr('disabled');
+                }
+            });
+            $('.col_field input, .col_field select, .col_field textarea, .col_func select').each(function() {
+                if (!$(this).parent().parent().find('.col_enabler input[type=checkbox]').is(':checked')) {
+                    $(this).attr('disabled', 'disabled');
+                }
+            });
+            $('.fastfieldvalue').click(function() {
+                var check = $(this).parent().parent().find('.enabler');
+                var selection = $(this).data('value');
+                $(check).attr('checked', true);
+                var target = $(this).parent().parent().find('.col_field input, .col_field select, .col_field textarea').not('.enabler');
+                $(this).parent().parent().find('.col_func select').removeAttr('disabled');
                 $(target).removeAttr('disabled');
-            }
+                if ($(target).is('select')) {
+                    $('option', target).each(function(i, selected) {
+                        if ($(this).val().toString() === selection.toString()) {
+                            $(this).attr('selected', true);
+                        }
+                    });
+                } else if ($(target).is('input[type=checkbox]')) {
+                    $(target).attr('checked', selection === 'True');
+                } else {
+                    $(target).val(selection);
+                }
+            });
+            $('.enabler').click(function() {
+                var target = $(this).parent().parent().find('.col_field input, .col_field select, .col_field textarea, .col_func select');
+                if ($(this).is(':checked')) {
+                    $(target).removeAttr('disabled');
+                } else {
+                    $(target).attr('disabled', 'disabled');
+                }
+            })
         });
-        $('.col_field input, .col_field select, .col_field textarea, .col_func select').each(function() {
-            if (!$(this).parent().parent().find('.col_enabler input[type=checkbox]').is(':checked')) {
-                $(this).attr('disabled', 'disabled');
-            }
-        });
-        $('.fastfieldvalue').click(function() {
-            var check = $(this).parent().parent().find('.enabler');
-            var selection = $(this).data('value');
-            $(check).attr('checked', true);
-            var target = $(this).parent().parent().find('.col_field input, .col_field select, .col_field textarea').not('.enabler');
-            $(this).parent().parent().find('.col_func select').removeAttr('disabled');
-            $(target).removeAttr('disabled');
-            if ($(target).is('select')) {
-                $('option', target).each(function(i, selected) {
-                    if ($(this).val().toString() === selection.toString()) {
-                        $(this).attr('selected', true);
-                    }
-                });
-            } else if ($(target).is('input[type=checkbox]')) {
-                $(target).attr('checked', selection === 'True');
-            } else {
-                $(target).val(selection);
-            }
-        });
-        $('.enabler').click(function() {
-            var target = $(this).parent().parent().find('.col_field input, .col_field select, .col_field textarea, .col_func select');
-            if ($(this).is(':checked')) {
-                $(target).removeAttr('disabled');
-            } else {
-                $(target).attr('disabled', 'disabled');
-            }
-        })
-    });
-})(django.jQuery);
+    })(django.jQuery);
```

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/massupdate.min.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/massupdate.min.js`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/merge.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/merge.js`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/static/adminactions/js/merge.min.js` & `django-adminactions-2.1.0/src/adminactions/static/adminactions/js/merge.min.js`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/tasks.py` & `django-adminactions-2.1.0/src/adminactions/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
-from celery.app import default_app
+
+from celery import shared_task  # noqa
 from django.apps import apps
 
 logger = logging.getLogger(__name__)
 
 
-@default_app.task()
+@shared_task()
 def mass_update_task(model, ids, rules, validate, clean, user_pk):
     from adminactions.mass_update import mass_update_execute
+
     try:
         model = apps.get_model(*model.split("."))
         queryset = model.objects.filter(id__in=ids)
         mass_update_execute(queryset, rules, validate, clean, user_pk=user_pk)
     except Exception as e:
         logger.exception(e)
         raise
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/any_model.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/any_model.html`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/byrows_update.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/byrows_update.html`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 {% block content %}
     {% if formset.errors %}
         <p class="errornote">
             {% if formset.errors|length == 1 %}{% trans "Please correct the error below." %}{% else %}{% trans "Please correct the errors below." %}{% endif %}
         </p>
         {{ adminform.form.non_field_errors }}
     {% endif %}
-    <form action="" method="post">
+    <form action="" method="post" id="update-form">
         {% csrf_token %}
         {{ formset.non_form_errors.as_ul }}
         <div class="formset-container">
             <table id="formset" class="form">
                 {% for form in formset.forms %}
                 {% if forloop.first %}
                 <thead>
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/charts.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/charts.html`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	{{ action_short_description|capfirst }}
     </div>
 {% endif %}
 {% endblock %}
 
 {% block content %}
     <div class="left">
-        <form action="." method="post">-{% csrf_token %}=
+        <form action="." method="post" id="charts-form">-{% csrf_token %}=
             <table>
                 {{ adminform.form }}
             </table>
             <input type="hidden" name="action" value="{{ action }}"/>
             <input type="submit" name="apply" value="{% trans 'go' %}"/>
         </form>
     </div>
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/duplicates.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/duplicates.html`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/export_csv.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/export_csv.html`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         <ol>
             {% for error in adminform.form.subject.errors %}
                 <li><strong>{{ error|escape }}</strong></li>
             {% endfor %}
         </ol>
     {% endif %}
     <div id='form'>
-        <form action="" method="post">
+        <form action="" method="post" id="export-form">
             {% csrf_token %}
             <table>
                 {{ adminform.form }}
             </table>
 {#            <input type="hidden" name="action" value="{{ action }}"/>#}
             <input type="submit" name="apply" value="{% trans 'Export' %}"/>
         </form>
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/export_fixture.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/export_fixture.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             {% for error in form.subject.errors %}
                 <li><strong>{{ error|escape }}</strong></li>
             {% endfor %}
         </ol>
     {% endif %}
     {{ data }}
     <div id='form'>
-        <form method="post">
+        <form method="post" id="export-form">
             {% csrf_token %}
             <table>
                 {{ adminform.form }}
             </table>
             <input type="submit" name="apply" value="{% trans 'Export' %}"/>
         </form>
     </div>
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/export_xls.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/export_xls.html`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         <ol>
             {% for error in adminform.form.subject.errors %}
                 <li><strong>{{ error|escape }}</strong></li>
             {% endfor %}
         </ol>
     {% endif %}
     <div id='form'>
-        <form action="" method="post">
+        <form action="" method="post" id="export-form">
             {% csrf_token %}
             <table>
                 {{ adminform.form }}
             </table>
             <input type="submit" name="apply" value="{% trans 'Export' %}"/>
         </form>
     </div>
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/helpers/import_fixture.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/helpers/import_fixture.html`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/mass_update.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/mass_update.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "admin/change_form.html" %}
 {% load i18n admin_modify actions massupdate static %}
-{% block extrahead %}{{ block.super }}
+{#{% block extrahead %}{{ block.super }}#}
 {#  {{ media }}#}
-{% endblock %}
+{#{% endblock %}#}
 
 {% block breadcrumbs %}{% if not is_popup %}
     <div class="breadcrumbs">
         <a href="../../">{% trans "Home" %}</a> &rsaquo;
         <a href="../">{{ app_label|capfirst|escape }}</a> &rsaquo;
         <a href=".">{{ opts.verbose_name_plural|capfirst }}</a> &rsaquo;
 	{{ action_short_description|capfirst }}
@@ -19,15 +19,15 @@
             {% for error in form.subject.errors %}
                 <li><strong>{{ error|escape }}</strong></li>
             {% endfor %}
         </ol>
     {% endif %}
     {{ form.non_field_errors }}
     <div id='col1'>
-        <form action="" method="post">
+        <form action="" method="post" id="mass-update-form" enctype="multipart/form-data">
             {% csrf_token %}
             <table class="mass-update">
                 {% for field in adminform.form.configured_fields %}
                     <tr>
                         <td>{{ field.label_tag }}</td>
                         <td colspan="4">
                             {{ field.errors }}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "admin/change_form.html" %} {% load i18n admin_modify actions
-massupdate static %} {% block extrahead %}{{ block.super }} {# {{ media }}#} {%
-endblock %} {% block breadcrumbs %}{% if not is_popup %}
+massupdate static %} {#{% block extrahead %}{{ block.super }}#} {# {{ media
+}}#} {#{% endblock %}#} {% block breadcrumbs %}{% if not is_popup %}
 {%_trans_"Home"_%} › {{_app_label|capfirst|escape_}} › {
 {_opts.verbose_name_plural|capfirst_}} › {{ action_short_description|capfirst
 }}
 {% endif %}{% endblock %} {% block content %} {% if form.subject.errors %}
    1. {% for error in form.subject.errors %}
    2. {{ error|escape }}
    3. {% endfor %}
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/merge.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/merge.html`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             <ol>
                 {% for error in form.errors %}
                     <li><strong>{{ error|escape }}</strong></li>
                 {% endfor %}
             </ol>
         {% endif %}
         {{ adminform.form.non_field_errors }}
-        <form method="post">{% csrf_token %}
+        <form method="post" id="merge-form">{% csrf_token %}
             {% for f in adminform.form.hidden_fields %}{{ f }}{% endfor %}
             <table>
                 <tr>
                     <td>{{ adminform.form.dependencies.label }}</td>
                     <td>{{ adminform.form.dependencies }}</td>
                 </tr>
             </table>
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templates/adminactions/merge_preview.html` & `django-adminactions-2.1.0/src/adminactions/templates/adminactions/merge_preview.html`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         <a href="../">{{ app_label|capfirst|escape }}</a> &rsaquo;
         <a href=".">{{ opts.verbose_name_plural|capfirst }}</a> &rsaquo;
         <a href="javascript:history.back();">{% trans "Merge records" %}</a> &rsaquo;
         {% trans "Preview" %}
     </div>
 {% endif %}{% endblock %}
 {% block content %}
-    <form method="post">{% csrf_token %}
+    <form method="post" id="merge-form">{% csrf_token %}
         {% for f in adminform.form.hidden_fields %}{{ f }}{% endfor %}
         {% for f in adminform.form.action_fields %}{{ f }}{% endfor %}
     <table class="mergetable">
         <tr class="row1">
             <th>{% trans "Key" %}</th>
             <td colspan="2">{{ master.pk }}</td>
         </tr>
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templatetags/actions.py` & `django-adminactions-2.1.0/src/adminactions/templatetags/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 register = Library()
 
 
 @register.filter()
 def field_display(obj, field):
     """
-        returns the representation (value or ``get_FIELD_display()``) of  a field
+    returns the representation (value or ``get_FIELD_display()``) of  a field
 
-        see `adminactions.utils.get_field_value`_
+    see `adminactions.utils.get_field_value`_
     """
     return get_field_value(obj, field)
 
 
 @register.filter
 def verbose_name(model_or_queryset, field):
     """
-        templatetag wrapper to `adminactions.utils.get_verbose_name`_
+    templatetag wrapper to `adminactions.utils.get_verbose_name`_
     """
     return get_verbose_name(model_or_queryset, field)
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templatetags/massupdate.py` & `django-adminactions-2.1.0/src/adminactions/templatetags/massupdate.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,48 +34,54 @@
 
     for el in d.get(field_name, []):
         try:
             value, label = el
         except (TypeError, ValueError):
             value, label = el, el
 
-        if label == '':  # ignore empty
+        if label == "":  # ignore empty
             continue
-        ret.append('<a name="{name}"><a href="#{name}" '
-                   'data-value="{value}" '
-                   'class="fastfieldvalue {field} '
-                   'value">{label}</a>'.format(name=name,
-                                               value=value,
-                                               field=field_name,
-                                               label=str(label)))
+        ret.append(
+            '<a name="{name}"><a href="#{name}" '
+            'data-value="{value}" '
+            'class="fastfieldvalue {field} '
+            'value">{label}</a>'.format(
+                name=name, value=value, field=field_name, label=str(label)
+            )
+        )
 
     return mark_safe(", ".join(ret))
 
 
 @register.simple_tag(takes_context=True)
 def checkbox_enabler(context, field):
-    form = context['adminform'].form
+    form = context["adminform"].form
     name = "chk_id_%s" % field.name
     checked = ""
     if form.is_bound:
         chk = form.cleaned_data.get(name, False)
-        checked = {True: 'checked="checked"', False: ''}[chk]
-    return mark_safe('<input type="checkbox" name="%s" %s class="enabler">' % (name, checked))
+        checked = {True: 'checked="checked"', False: ""}[chk]
+    return mark_safe(
+        '<input type="checkbox" name="%s" %s class="enabler">' % (name, checked)
+    )
 
 
 @register.simple_tag(takes_context=True)
 def field_function(context, model, form_field):
     from adminactions.mass_update import OPERATIONS
+
     model_field, model, direct, m2m = get_field_by_name(model, form_field.name)
-    attrs = {'class': 'func_select'}
+    attrs = {"class": "func_select"}
     options_attrs = {}
     choices = []
-    classes = {True: 'param', False: 'noparam'}
-    form = context['adminform'].form
+    classes = {True: "param", False: "noparam"}
+    form = context["adminform"].form
     value = ""
     if form.is_bound:
         value = form.cleaned_data.get("func_id_%s" % form_field.name, "")
 
-    for label, (__, param, enabler, __) in list(OPERATIONS.get_for_field(model_field).items()):
-        options_attrs[label] = {'class': classes[param], 'label': label}
+    for label, (__, param, enabler, __) in list(
+        OPERATIONS.get_for_field(model_field).items()
+    ):
+        options_attrs[label] = {"class": classes[param], "label": label}
         choices.append((label, label))
     return widgets.Select(attrs, choices).render("func_id_%s" % form_field.name, value)
```

### Comparing `django-adminactions-2.0.0/src/adminactions/templatetags/merge.py` & `django-adminactions-2.1.0/src/adminactions/templatetags/merge.py`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/src/adminactions/utils.py` & `django-adminactions-2.1.0/src/adminactions/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+from functools import partial
+
 from django.conf import settings
 from django.db import models
 from django.db.models.query import QuerySet
 from django.utils.encoding import smart_str
-from functools import partial
 
 
 def get_ignored_fields(model, setting_var_name):
     """
     returns list of ignored fields which must not be modified
     """
-    ignored_setting = getattr(settings, setting_var_name, {})
-    ignored_app = ignored_setting.get(model._meta.app_label, {})
-    if ignored_app:
-        ignored_fields = ignored_app.get(model._meta.model_name, [])
-    else:
-        ignored_fields = []
-    return ignored_fields
+    return (
+        getattr(settings, setting_var_name, {})
+        .get(model._meta.app_label, {})
+        .get(model._meta.model_name, ())
+    )
 
 
 def clone_instance(instance, fieldnames=None):
     """
         returns a copy of the passed instance.
 
         .. warning: All fields are copied, even primary key
@@ -27,16 +26,15 @@
     :param instance: :py:class:`django.db.models.Model` instance
     :return: :py:class:`django.db.models.Model` instance
     """
 
     if fieldnames is None:
         fieldnames = [fld.name for fld in instance._meta.fields]
 
-    new_kwargs = dict([(name, getattr(instance, name)) for name in fieldnames])
-    return instance.__class__(**new_kwargs)
+    return instance.__class__(**{name: getattr(instance, name) for name in fieldnames})
 
 
 # def get_copy_of_instance(instance):
 # return instance.__class__.objects.get(pk=instance.pk)
 
 
 def get_attr(obj, attr, default=None):
@@ -50,19 +48,19 @@
     4
 
     >>> get_attr(a, 'b.c.y', None)
 
     >>> get_attr(a, 'b.c.y', 1)
     1
     """
-    if '.' not in attr:
+    if "." not in attr:
         ret = getattr(obj, attr, default)
     else:
-        L = attr.split('.')
-        ret = get_attr(getattr(obj, L[0], default), '.'.join(L[1:]), default)
+        L = attr.split(".")
+        ret = get_attr(getattr(obj, L[0], default), ".".join(L[1:]), default)
 
     if isinstance(ret, BaseException):
         raise ret
     return ret
 
 
 def getattr_or_item(obj, name):
@@ -88,15 +86,17 @@
     # AttributeError: dict object has no attribute/item '!!!'
     try:
         ret = get_attr(obj, name, AttributeError())
     except AttributeError:
         try:
             ret = obj[name]
         except (KeyError, TypeError):
-            raise AttributeError("%s object has no attribute/item '%s'" % (obj.__class__.__name__, name))
+            raise AttributeError(
+                "%s object has no attribute/item '%s'" % (obj.__class__.__name__, name)
+            )
     return ret
 
 
 def get_field_value(obj, field, usedisplay=True, raw_callable=False):
     """
     returns the field value or field representation if get_FIELD_display exists
 
@@ -115,23 +115,25 @@
     ValueError: Invalid value for parameter `field`: Should be a field name or a Field instance
     """
     if isinstance(field, str):
         fieldname = field
     elif isinstance(field, models.Field):
         fieldname = field.name
     else:
-        raise ValueError('Invalid value for parameter `field`: Should be a field name or a Field instance')
+        raise ValueError(
+            "Invalid value for parameter `field`: Should be a field name or a Field instance"
+        )
 
-    if usedisplay and hasattr(obj, 'get_%s_display' % fieldname):
-        value = getattr(obj, 'get_%s_display' % fieldname)()
+    if usedisplay and hasattr(obj, "get_%s_display" % fieldname):
+        value = getattr(obj, "get_%s_display" % fieldname)()
     else:
         value = getattr_or_item(obj, fieldname)
 
-    if hasattr(value, 'all'):
-        value = ';'.join(smart_str(obj) for obj in value.all())
+    if hasattr(value, "all"):
+        value = ";".join(smart_str(obj) for obj in value.all())
     if not raw_callable and callable(value):
         value = value()
 
     if isinstance(value, models.Model):
         return smart_str(value)
 
     if isinstance(value, str):
@@ -154,21 +156,23 @@
     >>> p = Permission(name='perm')
     >>> get_field_by_path(Permission, 'content_type').name
     'content_type'
     >>> p = Permission(name='perm')
     >>> get_field_by_path(p, 'content_type.app_label').name
     'app_label'
     """
-    parts = field_path.split('.')
+    parts = field_path.split(".")
     target = parts[0]
     if target in get_all_field_names(model):
         field_object, model, direct, m2m = get_field_by_name(model, target)
         if isinstance(field_object, models.fields.related.ForeignKey):
             if parts[1:]:
-                return get_field_by_path(field_object.related_model, '.'.join(parts[1:]))
+                return get_field_by_path(
+                    field_object.related_model, ".".join(parts[1:])
+                )
             else:
                 return field_object
         else:
             return field_object
     return None
 
 
@@ -211,23 +215,25 @@
     elif isinstance(model_or_queryset, QuerySet):
         model = model_or_queryset.model
     elif isinstance(model_or_queryset, models.Model):
         model = model_or_queryset
     elif type(model_or_queryset) is models.base.ModelBase:
         model = model_or_queryset
     else:
-        raise ValueError('`get_verbose_name` expects Manager, Queryset or Model as first parameter (got %s)' % type(
-            model_or_queryset))
+        raise ValueError(
+            "`get_verbose_name` expects Manager, Queryset or Model as first parameter (got %s)"
+            % type(model_or_queryset)
+        )
 
     if isinstance(field, str):
         field = get_field_by_path(model, field)
     elif isinstance(field, models.Field):
         field = field
     else:
-        raise ValueError('`get_verbose_name` field_path must be string or Field class')
+        raise ValueError("`get_verbose_name` field_path must be string or Field class")
 
     return field.verbose_name
 
 
 def flatten(iterable):
     """
     flatten(sequence) -> list
@@ -264,34 +270,47 @@
 
 
 def model_has_field(model, field_name):
     return field_name in [f.name for f in model._meta.get_fields()]
 
 
 def get_all_related_objects(model):
-    return [f for f in model._meta.get_fields()
-            if (f.one_to_many or f.one_to_one) and f.auto_created]
+    return [
+        f
+        for f in model._meta.get_fields()
+        if (f.one_to_many or f.one_to_one) and f.auto_created
+    ]
 
 
 def get_all_field_names(model):
     from itertools import chain
-    return list(set(chain.from_iterable((field.name, field.attname)
-                                        if hasattr(field, 'attname') else (field.name,)
-                                        for field in model._meta.get_fields()
-                                        if not (field.many_to_one and field.related_model is None))))
+
+    return list(
+        set(
+            chain.from_iterable(
+                (field.name, field.attname)
+                if hasattr(field, "attname")
+                else (field.name,)
+                for field in model._meta.get_fields()
+                if not (field.many_to_one and field.related_model is None)
+            )
+        )
+    )
 
 
 def curry(func, *a, **kw):
     return partial(func, *a, **kw)
 
 
 def get_common_context(modeladmin, **kwargs):
-    ctx = {'change': True,
-           'is_popup': False,
-           'save_as': False,
-           'has_delete_permission': False,
-           'has_add_permission': False,
-           'has_change_permission': True,
-           'opts': modeladmin.model._meta,
-           'app_label': modeladmin.model._meta.app_label}
+    ctx = {
+        "change": True,
+        "is_popup": False,
+        "save_as": False,
+        "has_delete_permission": False,
+        "has_add_permission": False,
+        "has_change_permission": True,
+        "opts": modeladmin.model._meta,
+        "app_label": modeladmin.model._meta.app_label,
+    }
     ctx.update(**kwargs)
     return ctx
```

### Comparing `django-adminactions-2.0.0/src/django_adminactions.egg-info/PKG-INFO` & `django-adminactions-2.1.0/src/django_adminactions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-adminactions
-Version: 2.0.0
+Version: 2.1.0
 Summary: Collections of useful actions to use with django.contrib.admin.ModelAdmin
 Home-page: https://github.com/saxix/django-adminactions
+Download-URL: https://github.com/saxix/django-adminactions
 Author: sax
 Author-email: s.apostolico@gmail.com
 License: MIT
-Download-URL: https://github.com/saxix/django-adminactions
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -45,18 +45,17 @@
 * Export as Excel
 * Export as fixture
 * Export delete tree
 * Mass update records
 * Graph queryset
 * Merge records
 * Find Duplicates
+* Bulk Update
 
 
 #### Project Links
 
 
 - Code: https://github.com/saxix/django-adminactions
 - Documentation: https://django-adminactions.readthedocs.org/en/latest/
 - Issue Tracker: https://github.com/saxix/django-adminactions/issues?sort
 - Download Package: https://pypi.org/project/django-adminactions/
-
-
```

### Comparing `django-adminactions-2.0.0/src/django_adminactions.egg-info/requires.txt` & `django-adminactions-2.1.0/src/django_adminactions.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 pytz
 xlrd>=0.9.2
 xlwt
 
 [dev]
+black
+django<4
 pdbpp
 virtualenv
 wheel
 check-manifest
 docutils
-check-manifest
 celery
 django-dynamic-fixture
 django-webtest>1.9.6
 django-admin-extra-urls
 django-environ
 flake8
 flake8-isort
@@ -25,17 +26,19 @@
 pytest-django
 pytest-echo
 pytest-pythonpath
 redis
 readme
 selenium>=2.42.0
 setuptools>=15.0
-tox
+tox<4
 
 [docs]
+black
+django<4
 pdbpp
 virtualenv
 wheel
 check-manifest
 docutils
 django
 sphinx
@@ -62,8 +65,8 @@
 pytest-django
 pytest-echo
 pytest-pythonpath
 redis
 readme
 selenium>=2.42.0
 setuptools>=15.0
-tox
+tox<4
```

### Comparing `django-adminactions-2.0.0/tests/.coveragerc` & `django-adminactions-2.1.0/tests/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/tests/conftest.py` & `django-adminactions-2.1.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import django_webtest
 import logging
+import os
+
+import django_webtest
 import pytest
 
 logger = logging.getLogger("test")
 
 levelNames = {
     logging.CRITICAL: "CRITICAL",
     logging.ERROR: "ERROR",
@@ -19,50 +21,64 @@
     "DEBUG": logging.DEBUG,
     "NOTSET": logging.NOTSET,
 }
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("selenium", "Selenium Web Browser Automation")
-    group.addoption("--selenium-enable",
-                    action='store_true',
-                    dest='selenium_enable',
-                    default=False,
-                    help="launch Selenium tests on hub"
-                    )
+    group.addoption(
+        "--selenium-enable",
+        action="store_true",
+        dest="selenium_enable",
+        default=False,
+        help="launch Selenium tests on hub",
+    )
 
     group.addoption(
-        "--chrome-driver", metavar="PATH",
+        "--chrome-driver",
+        metavar="PATH",
         help="specify the full path for the chromedriver stored in your system. This is a mandatory field "
-             "to let start Selenium tests even with Chrome. Command line sample: "
-             "py.test --selenium-enable --chrome-driver=/home/chromedriver. -k test_name."
+        "to let start Selenium tests even with Chrome. Command line sample: "
+        "py.test --selenium-enable --chrome-driver=/home/chromedriver. -k test_name.",
     )
 
-    parser.addoption("--log", default=None, action="store",
-                     dest="log_level",
-                     help="enable console log")
-
-    parser.addoption("--log-add", default="", action="store",
-                     dest="log_add",
-                     help="add package to log")
+    parser.addoption(
+        "--log",
+        default=None,
+        action="store",
+        dest="log_level",
+        help="enable console log",
+    )
+
+    parser.addoption(
+        "--log-add",
+        default="",
+        action="store",
+        dest="log_add",
+        help="add package to log",
+    )
 
 
 def pytest_configure(config):
     # import warnings
-    # enable this to removee deprecations
+    # enable this to remove deprecations
     # warnings.simplefilter('once', DeprecationWarning)
 
-    if config.option.markexpr.find("selenium") < 0 and \
-        not config.option.keyword and \
-        config.option.keyword.find('selenium') < 0:
+    if (
+        config.option.markexpr.find("selenium") < 0
+        and not config.option.keyword
+        and config.option.keyword.find("selenium") < 0
+    ):
         if not config.option.selenium_enable:
-            setattr(config.option, 'markexpr', 'not selenium')
+            setattr(config.option, "markexpr", "not selenium")
+    os.environ["CELERY_ALWAYS_EAGER"] = "1"
 
     if config.option.log_level:
         import logging
+
         level = config.option.log_level.upper()
         assert level in levelNames.keys()
         format = "%(levelname)-7s %(name)-30s %(funcName)-20s:%(lineno)3s %(message)s"
         formatter = logging.Formatter(format)
 
         handler = logging.StreamHandler()
         handler.setLevel(levelNames[level])
@@ -79,52 +95,53 @@
                 logger.setLevel(levelNames[level])
                 logger.addHandler(handler)
 
 
 @pytest.fixture(autouse=True)
 def create_aa_permissions(db):
     from adminactions.perms import create_extra_permissions
+
     create_extra_permissions()
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def app(request):
     wtm = django_webtest.WebTestMixin()
     wtm.csrf_checks = False
     wtm._patch_settings()
     request.addfinalizer(wtm._unpatch_settings)
     return django_webtest.DjangoTestApp()
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def users():
     from django.contrib.auth.models import User
     from django_dynamic_fixture import G
 
     return G(User, n=2, is_staff=False, is_active=False)
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def demomodels():
     from demo.models import DemoModel
     from django_dynamic_fixture import G
 
     return G(DemoModel, n=20)
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def admin():
     from django.contrib.auth.models import User
     from django_dynamic_fixture import G
 
     return G(User, is_staff=True, is_active=True)
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def administrator():
     from django.contrib.auth.models import User
     from utils import ADMIN, PWD
 
-    superuser = User._default_manager.create_superuser(username=ADMIN,
-                                                       password=PWD,
-                                                       email="sax@noreply.org")
+    superuser = User._default_manager.create_superuser(
+        username=ADMIN, password=PWD, email="sax@noreply.org"
+    )
     return superuser
```

### Comparing `django-adminactions-2.0.0/tests/demo/fixtures/adminactions.json` & `django-adminactions-2.1.0/tests/demo/fixtures/adminactions.json`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/tests/demo/fixtures/demoproject.json` & `django-adminactions-2.1.0/tests/demo/fixtures/demoproject.json`

 * *Files identical despite different names*

### Comparing `django-adminactions-2.0.0/tests/demo/models.py` & `django-adminactions-2.1.0/tests/demo/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class SubclassedImageField(models.ImageField):
     pass
 
 
 class DemoModel(models.Model):
-    char = models.CharField('Chäř', max_length=255)
+    char = models.CharField("Chäř", max_length=255)
     integer = models.IntegerField()
     logic = models.BooleanField(default=False)
     # null_logic = models.NullBooleanField(default=None)
     date = models.DateField()
     datetime = models.DateTimeField()
     time = models.TimeField()
     decimal = models.DecimalField(max_digits=10, decimal_places=3)
@@ -28,52 +28,58 @@
     generic_ip = models.GenericIPAddressField()
     url = models.URLField()
     text = models.TextField()
 
     unique = models.CharField(max_length=255, unique=True)
     nullable = models.CharField(max_length=255, null=True)
     blank = models.CharField(max_length=255, blank=True, null=True)
-    not_editable = models.CharField(max_length=255, editable=False, blank=True, null=True)
-    choices = models.IntegerField(choices=((1, 'Choice 1'), (2, 'Choice 2'), (3, 'Choice 3')))
+    not_editable = models.CharField(
+        max_length=255, editable=False, blank=True, null=True
+    )
+    choices = models.IntegerField(
+        choices=((1, "Choice 1"), (2, "Choice 2"), (3, "Choice 3"))
+    )
 
     image = models.ImageField(blank=True, null=True)
     subclassed_image = SubclassedImageField(blank=True, null=True)
 
     class Meta:
-        app_label = 'demo'
-        ordering = ('-id',)
+        app_label = "demo"
+        ordering = ("-id",)
 
 
 class UserDetail(models.Model):
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     note = models.CharField(max_length=10, blank=True)
 
     class Meta:
-        app_label = 'demo'
+        app_label = "demo"
 
 
 class DemoOneToOne(models.Model):
-    demo = models.OneToOneField(DemoModel, on_delete=models.CASCADE,
-                                related_name='onetoone')
+    demo = models.OneToOneField(
+        DemoModel, on_delete=models.CASCADE, related_name="onetoone"
+    )
 
     class Meta:
-        app_label = 'demo'
+        app_label = "demo"
 
 
 class UserDetailModelAdmin(ExtraUrlMixin, ModelAdmin):
     list_display = [f.name for f in UserDetail._meta.fields]
 
 
 class DemoModelAdmin(ExtraUrlMixin, ModelAdmin):
     # list_display = ('char', 'integer', 'logic', 'null_logic',)
     list_display = [f.name for f in DemoModel._meta.fields]
 
     @button()
     def import_fixture(self, request):
         from adminactions.helpers import import_fixture as _import_fixture
+
         return _import_fixture(self, request)
 
 
 class DemoOneToOneAdmin(ExtraUrlMixin, AdminActionPermMixin, ModelAdmin):
     pass
```

### Comparing `django-adminactions-2.0.0/tests/demo/settings.py` & `django-adminactions-2.1.0/tests/demo/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,178 @@
 import os
+
 from environ import Env
 
 from adminactions.consts import AA_PERMISSION_CREATE_USE_COMMAND
 
-env = Env()
+env = Env(
+    CELERY_ALWAYS_EAGER=(bool, "true"), CELERY_BROKER_URL=(str, "redis://127.0.0.1")
+)
 
 here = os.path.dirname(__file__)
 
 DEBUG = True
 TEMPLATE_DEBUG = DEBUG
+AUTHENTICATION_BACKENDS = ("demo.backends.AnyUserAuthBackend",)
+FILE_UPLOAD_HANDLERS = [
+    # "django.core.files.uploadhandler.MemoryFileUploadHandler",
+    "django.core.files.uploadhandler.TemporaryFileUploadHandler",
+]
 
-db = os.environ.get('DBENGINE', None)
-if db == 'pg':
+db = os.environ.get("DBENGINE", None)
+if db == "pg":
     DATABASES = {
-        'default': {
-            'ENGINE': 'django.db.backends.postgresql_psycopg2',
-            'NAME': 'adminactions',
-            'HOST': os.environ.get('PG_HOST', '127.0.0.1'),
-            'PORT': os.environ.get('PG_PORT', ''),
-            'USER': os.environ.get('PG_USER', 'postgres'),
-            'PASSWORD': os.environ.get('PG_PASSWORD', ''),
+        "default": {
+            "ENGINE": "django.db.backends.postgresql_psycopg2",
+            "NAME": "adminactions",
+            "HOST": os.environ.get("PG_HOST", "127.0.0.1"),
+            "PORT": os.environ.get("PG_PORT", ""),
+            "USER": os.environ.get("PG_USER", "postgres"),
+            "PASSWORD": os.environ.get("PG_PASSWORD", ""),
         }
     }
-elif db == 'mysql':
+elif db == "mysql":
     DATABASES = {
-        'default': {
-            'ENGINE': 'django.db.backends.mysql',
-            'NAME': 'adminactions',
-            'HOST': os.environ.get('MYSQL_HOST', '127.0.0.1'),
-            'PORT': os.environ.get('MYSQL_PORT', ''),
-            'USER': os.environ.get('MYSQL_USER', 'root'),
-            'PASSWORD': os.environ.get('MYSQL_PASSWORD', ''),
-
-            'CHARSET': 'utf8',
-            'COLLATION': 'utf8_general_ci',
-            'TEST': {
-                'CHARSET': 'utf8',
-                'COLLATION': 'utf8_general_ci',
+        "default": {
+            "ENGINE": "django.db.backends.mysql",
+            "NAME": "adminactions",
+            "HOST": os.environ.get("MYSQL_HOST", "127.0.0.1"),
+            "PORT": os.environ.get("MYSQL_PORT", ""),
+            "USER": os.environ.get("MYSQL_USER", "root"),
+            "PASSWORD": os.environ.get("MYSQL_PASSWORD", ""),
+            "CHARSET": "utf8",
+            "COLLATION": "utf8_general_ci",
+            "TEST": {
+                "CHARSET": "utf8",
+                "COLLATION": "utf8_general_ci",
             },
-            'TEST_CHARSET': 'utf8',
-            'TEST_COLLATION': 'utf8_general_ci'
+            "TEST_CHARSET": "utf8",
+            "TEST_COLLATION": "utf8_general_ci",
         }
     }
-elif db == 'myisam':
+elif db == "myisam":
     DATABASES = {
-        'default': {
-            'ENGINE': 'django.db.backends.mysql',
-            'NAME': 'adminactions',
-            'HOST': os.environ.get('MYSQL_HOST', '127.0.0.1'),
-            'PORT': os.environ.get('MYSQL_PORT', ''),
-            'USER': os.environ.get('MYSQL_USER', 'root'),
-            'PASSWORD': os.environ.get('MYSQL_PASSWORD', ''),
-
-            'CHARSET': 'utf8',
-            'OPTIONS': {'init_command': 'SET storage_engine=MyISAM'},
-            'COLLATION': 'utf8_general_ci',
-            'TEST': {
-                'CHARSET': 'utf8',
-                'COLLATION': 'utf8_general_ci',
+        "default": {
+            "ENGINE": "django.db.backends.mysql",
+            "NAME": "adminactions",
+            "HOST": os.environ.get("MYSQL_HOST", "127.0.0.1"),
+            "PORT": os.environ.get("MYSQL_PORT", ""),
+            "USER": os.environ.get("MYSQL_USER", "root"),
+            "PASSWORD": os.environ.get("MYSQL_PASSWORD", ""),
+            "CHARSET": "utf8",
+            "OPTIONS": {"init_command": "SET storage_engine=MyISAM"},
+            "COLLATION": "utf8_general_ci",
+            "TEST": {
+                "CHARSET": "utf8",
+                "COLLATION": "utf8_general_ci",
             },
-            'TEST_CHARSET': 'utf8',
-            'TEST_COLLATION': 'utf8_general_ci'
+            "TEST_CHARSET": "utf8",
+            "TEST_COLLATION": "utf8_general_ci",
         }
     }
 else:
     DATABASES = {
-        'default': {
-            'ENGINE': 'django.db.backends.sqlite3',
-            'NAME': 'adminactions.sqlite',
-            'TEST': {
-                'NAME': ':memory:',
+        "default": {
+            "ENGINE": "django.db.backends.sqlite3",
+            "NAME": "adminactions.sqlite",
+            "TEST": {
+                "NAME": ":memory:",
             },
-            'TEST_NAME': ':memory:',
-            'HOST': '',
-            'PORT': '',
-            'ATOMIC_REQUESTS': True
+            "TEST_NAME": ":memory:",
+            "HOST": "",
+            "PORT": "",
+            "ATOMIC_REQUESTS": True,
         }
     }
 
-TIME_ZONE = 'Asia/Bangkok'
-LANGUAGE_CODE = 'en-us'
+TIME_ZONE = "Asia/Bangkok"
+LANGUAGE_CODE = "en-us"
 SITE_ID = 1
 USE_I18N = True
 USE_L10N = True
 USE_TZ = True
-MEDIA_ROOT = os.path.join(here, 'media')
-MEDIA_URL = ''
-STATIC_ROOT = os.path.join(here, 'static')
-STATIC_URL = '/static/'
-SECRET_KEY = 'c73*n!y=)tziu^2)y*@5i2^)$8z$tx#b9*_r3i6o1ohxo%*2^a'
+MEDIA_ROOT = os.path.join(here, "media")
+MEDIA_URL = ""
+STATIC_ROOT = os.path.join(here, "static")
+STATIC_URL = "/static/"
+SECRET_KEY = "c73*n!y=)tziu^2)y*@5i2^)$8z$tx#b9*_r3i6o1ohxo%*2^a"
 
 MIDDLEWARE = (
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',)
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+)
 
-MESSAGE_STORAGE = 'demo.storage.PlainCookieStorage'
+MESSAGE_STORAGE = "demo.storage.PlainCookieStorage"
 
-ROOT_URLCONF = 'demo.urls'
+ROOT_URLCONF = "demo.urls"
 
 AA_PERMISSION_HANDLER = AA_PERMISSION_CREATE_USE_COMMAND
 
 INSTALLED_APPS = [
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'django.contrib.admin',
-    'admin_extra_urls',
-    'adminactions.apps.Config',
-    'demo']
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "django.contrib.admin",
+    "admin_extra_urls",
+    "adminactions.apps.Config",
+    "demo",
+]
 
 CACHES = {
-    'default': {
-        'BACKEND': 'django.core.cache.backends.dummy.DummyCache',
-        'LOCATION': 'unique-snowflake'
+    "default": {
+        "BACKEND": "django.core.cache.backends.dummy.DummyCache",
+        "LOCATION": "unique-snowflake",
     }
 }
 
 ENABLE_SELENIUM = True
 
-DATE_FORMAT = 'd-m-Y'
-TIME_FORMAT = 'H:i'
-DATETIME_FORMAT = 'd-m-Y H:i'
-YEAR_MONTH_FORMAT = 'F Y'
-MONTH_DAY_FORMAT = 'F j'
-SHORT_DATE_FORMAT = 'm/d/Y'
-SHORT_DATETIME_FORMAT = 'm/d/Y P'
+DATE_FORMAT = "d-m-Y"
+TIME_FORMAT = "H:i"
+DATETIME_FORMAT = "d-m-Y H:i"
+YEAR_MONTH_FORMAT = "F Y"
+MONTH_DAY_FORMAT = "F j"
+SHORT_DATE_FORMAT = "m/d/Y"
+SHORT_DATETIME_FORMAT = "m/d/Y P"
 FIRST_DAY_OF_WEEK = 1
 
 # CSRF_COOKIE_DOMAIN = 'localhost'
 CSRF_COOKIE_HTTPONLY = False
-CSRF_COOKIE_NAME = 'csrftoken'
-CSRF_COOKIE_PATH = '/'
+CSRF_COOKIE_NAME = "csrftoken"
+CSRF_COOKIE_PATH = "/"
 CSRF_COOKIE_SECURE = False
-CSRF_HEADER_NAME = 'HTTP_X_CSRFTOKEN'
+CSRF_HEADER_NAME = "HTTP_X_CSRFTOKEN"
 # CSRF_TRUSTED_ORIGINS = ['localhost']
 
 # Django 1.9
 
 TEMPLATES = [
-    {'BACKEND': 'django.template.backends.django.DjangoTemplates',
-     'DIRS': [],
-     'APP_DIRS': True,
-     'OPTIONS': {
-         'debug': DEBUG,
-         'context_processors': [
-             'django.contrib.auth.context_processors.auth',
-             'django.template.context_processors.debug',
-             'django.template.context_processors.i18n',
-             'django.template.context_processors.media',
-             'django.template.context_processors.static',
-             'django.template.context_processors.tz',
-             "django.template.context_processors.request",
-             'django.contrib.messages.context_processors.messages',
-         ],
-     },
-     }
+    {
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "debug": DEBUG,
+            "context_processors": [
+                "django.contrib.auth.context_processors.auth",
+                "django.template.context_processors.debug",
+                "django.template.context_processors.i18n",
+                "django.template.context_processors.media",
+                "django.template.context_processors.static",
+                "django.template.context_processors.tz",
+                "django.template.context_processors.request",
+                "django.contrib.messages.context_processors.messages",
+            ],
+        },
+    }
 ]
 AUTH_PASSWORD_VALIDATORS = [
     # {
     # 'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
     # },
     # {
     #     'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
@@ -177,12 +186,12 @@
 ]
 
 # CELERY STUFF
 BROKER_URL = env("CELERY_BROKER_URL")
 # CELERY_RESULT_BACKEND = env("CELERY_RESULT_BACKEND")
 # CELERY_ACCEPT_CONTENT = ["application/json"]
 # CELERY_TASK_SERIALIZER = "json"
-CELERY_TASK_ALWAYS_EAGER = env("CELERY_ALWAYS_EAGER")
-# CELERY_ALWAYS_EAGER = env("CELERY_ALWAYS_EAGER")
+CELERY_TASK_ALWAYS_EAGER = True
+CELERY_ALWAYS_EAGER = True
 # CELERY_RESULT_SERIALIZER = "json"
 # CELERY_TIMEZONE = TIME_ZONE
 # CELERY_BEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
```

### Comparing `django-adminactions-2.0.0/tests/demo/storage.py` & `django-adminactions-2.1.0/tests/demo/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
+
 from django.conf import settings
 from django.contrib.messages.storage.base import BaseStorage, Message
 from django.core import signing
 from django.http import SimpleCookie
 from django.utils.crypto import constant_time_compare, salted_hmac
 from django.utils.safestring import SafeData, mark_safe
 
 
 class MessageEncoder(json.JSONEncoder):
     """
     Compactly serialize instances of the ``Message`` class as JSON.
     """
-    message_key = '__json_message'
+
+    message_key = "__json_message"
 
     def default(self, obj):
         if isinstance(obj, Message):
             # Using 0/1 here instead of False/True to produce more compact json
             is_safedata = 1 if isinstance(obj.message, SafeData) else 0
             message = [self.message_key, is_safedata, obj.level, obj.message]
             if obj.extra_tags:
@@ -33,34 +35,34 @@
         if isinstance(obj, list) and obj:
             if obj[0] == MessageEncoder.message_key:
                 if obj[1]:
                     obj[3] = mark_safe(obj[3])
                 return Message(*obj[2:])
             return [self.process_messages(item) for item in obj]
         if isinstance(obj, dict):
-            return {key: self.process_messages(value)
-                    for key, value in obj.items()}
+            return {key: self.process_messages(value) for key, value in obj.items()}
         return obj
 
     def decode(self, s, **kwargs):
         decoded = super().decode(s, **kwargs)
         return self.process_messages(decoded)
 
 
 class PlainCookieStorage(BaseStorage):
     """
     Store messages in a cookie.
     """
-    cookie_name = 'messages'
+
+    cookie_name = "messages"
     # uwsgi's default configuration enforces a maximum size of 4kb for all the
     # HTTP headers. In order to leave some room for other cookies and headers,
     # restrict the session cookie to 1/2 of 4kb. See #18781.
     max_cookie_size = 2048
-    not_finished = '__messagesnotfinished__'
-    key_salt = 'django.contrib.messages'
+    not_finished = "__messagesnotfinished__"
+    key_salt = "django.contrib.messages"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.signer = signing.get_cookie_signer(salt=self.key_salt)
 
     def _get(self, *args, **kwargs):
         """
@@ -80,23 +82,23 @@
     def _update_cookie(self, encoded_data, response):
         """
         Either set the cookie with the encoded data if there is any data to
         store, or delete the cookie.
         """
         if encoded_data:
             response.set_cookie(
-                self.cookie_name, encoded_data,
+                self.cookie_name,
+                encoded_data,
                 domain=settings.SESSION_COOKIE_DOMAIN,
                 secure=None,
-                httponly=None
+                httponly=None,
             )
         else:
             response.delete_cookie(
-                self.cookie_name,
-                domain=settings.SESSION_COOKIE_DOMAIN
+                self.cookie_name, domain=settings.SESSION_COOKIE_DOMAIN
             )
 
     def _store(self, messages, response, remove_oldest=True, *args, **kwargs):
         """
         Store the messages to a cookie and return a list of any messages which
         could not be stored.
 
@@ -115,41 +117,42 @@
                 return len(cookie.value_encode(val)[1])
 
             while encoded_data and stored_length(encoded_data) > self.max_cookie_size:
                 if remove_oldest:
                     unstored_messages.append(messages.pop(0))
                 else:
                     unstored_messages.insert(0, messages.pop())
-                encoded_data = self._encode(messages + [self.not_finished],
-                                            encode_empty=unstored_messages)
+                encoded_data = self._encode(
+                    messages + [self.not_finished], encode_empty=unstored_messages
+                )
         self._update_cookie(encoded_data, response)
         return unstored_messages
 
     def _legacy_hash(self, value):
         """
         # RemovedInDjango40Warning: pre-Django 3.1 hashes will be invalid.
         Create an HMAC/SHA1 hash based on the value and the project setting's
         SECRET_KEY, modified to make it unique for the present purpose.
         """
         # The class wide key salt is not reused here since older Django
         # versions had it fixed and making it dynamic would break old hashes if
         # self.key_salt is changed.
-        key_salt = 'django.contrib.messages'
+        key_salt = "django.contrib.messages"
         return salted_hmac(key_salt, value).hexdigest()
 
     def _encode(self, messages, encode_empty=False):
         """
         Return an encoded version of the messages list which can be stored as
         plain text.
 
         Since the data will be retrieved from the client-side, the encoded data
         also contains a hash to ensure that the data was not tampered with.
         """
         if messages or encode_empty:
-            encoder = MessageEncoder(separators=(',', ':'))
+            encoder = MessageEncoder(separators=(",", ":"))
             value = encoder.encode(messages)
             return self.signer.sign(value)
 
     def _decode(self, data):
         """
         Safely decode an encoded text stream back into a list of messages.
 
@@ -173,13 +176,13 @@
         # Mark the data as used (so it gets removed) since something was wrong
         # with the data.
         self.used = True
         return None
 
     def _legacy_decode(self, data):
         # RemovedInDjango40Warning: pre-Django 3.1 hashes will be invalid.
-        bits = data.split('$', 1)
+        bits = data.split("$", 1)
         if len(bits) == 2:
             hash_, value = bits
             if constant_time_compare(hash_, self._legacy_hash(value)):
                 return value
         return None
```

### Comparing `django-adminactions-2.0.0/tests/selenium_tests/conftest.py` & `django-adminactions-2.1.0/tests/selenium_tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import os
-import pytest
 import types
+
+import pytest
 from django_dynamic_fixture import G
 from selenium import webdriver
 
 # from demo.common import *  # noqa
 
 browsers = {
-    'firefox': webdriver.Firefox,
+    "firefox": webdriver.Firefox,
     # 'chrome': webdriver.Chrome,
 }
 
 
-@pytest.fixture(scope='session',
-                params=list(browsers.keys()))
+@pytest.fixture(scope="session", params=list(browsers.keys()))
 def driver(request):
-    if 'DISPLAY' not in os.environ:
-        pytest.skip('Test requires display server (export DISPLAY)')
+    if "DISPLAY" not in os.environ:
+        pytest.skip("Test requires display server (export DISPLAY)")
 
     b = browsers[request.param]()
 
     request.addfinalizer(lambda *args: b.quit())
 
     return b
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def browser(live_server, driver):
-    '''Open a Selenium browser with window size and wait time set.'''
+    """Open a Selenium browser with window size and wait time set."""
 
     def go(self, url):
         self._last_url = url
         return self.get(self.live_server.url + url)
 
     def dump(self, filename=None):
-        dest = filename or self._last_url.replace('/', '_').replace('#', '~')
-        self.get_screenshot_as_file('./{}.jpg'.format(dest))
+        dest = filename or self._last_url.replace("/", "_").replace("#", "~")
+        self.get_screenshot_as_file("./{}.jpg".format(dest))
 
     b = driver
     b.live_server = live_server
     b.set_window_size(1024, 768)
     b.implicitly_wait(10)
 
     b.go = types.MethodType(go, b)
@@ -47,28 +47,28 @@
 
     return b
 
 
 def login(browser):
     from utils import ADMIN, PWD
 
-    browser.go('/admin/')
+    browser.go("/admin/")
 
-    username = browser.find_element_by_id('id_username')
-    password = browser.find_element_by_id('id_password')
+    username = browser.find_element_by_id("id_username")
+    password = browser.find_element_by_id("id_password")
 
     username.send_keys(ADMIN)
     password.send_keys(PWD)
 
-    browser.find_element_by_css_selector("input[type=\"submit\"]").click()
+    browser.find_element_by_css_selector('input[type="submit"]').click()
 
     return browser
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def admin_site(browser, administrator):
     from demo.models import DemoModel, UserDetail
 
     G(DemoModel, n=5)
     G(UserDetail, n=5)
     login(browser)
     return browser, administrator
```

### Comparing `django-adminactions-2.0.0/tests/selenium_tests/test_export_csv.py` & `django-adminactions-2.1.0/tests/selenium_tests/test_export_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import datetime
+from time import sleep
+
 import pytest
 from selenium.webdriver.support.select import Select
-from time import sleep
 
 FAKE_TIME = datetime.datetime(2020, 12, 25, 17, 5, 55)
 
 pytestmark = pytest.mark.selenium
 
 
 @pytest.fixture
 def now(monkeypatch):
-
     class FixedDateTime:
         @classmethod
         def now(cls):
             return FAKE_TIME
 
-    monkeypatch.setattr('adminactions.views.datetime', FixedDateTime)
+    monkeypatch.setattr("adminactions.views.datetime", FixedDateTime)
 
 
 def test_export_as_csv(admin_site):
     browser, administrator = admin_site
     browser.find_element_by_link_text("Demo models").click()
     browser.find_element_by_id("action-toggle").click()
-    Select(browser.find_element_by_name("action")).select_by_visible_text("Export as CSV")
+    Select(browser.find_element_by_name("action")).select_by_visible_text(
+        "Export as CSV"
+    )
     browser.find_element_by_name("index").click()
     browser.find_element_by_name("apply").click()
 
 
 @pytest.fixture
 def export_csv_page(admin_site):
     browser, administrator = admin_site
-    browser.go('/admin/')
+    browser.go("/admin/")
     browser.find_element_by_link_text("Demo models").click()
     browser.find_element_by_id("action-toggle").click()
-    Select(browser.find_element_by_name("action")).select_by_visible_text("Export as CSV")
+    Select(browser.find_element_by_name("action")).select_by_visible_text(
+        "Export as CSV"
+    )
     browser.find_element_by_name("index").click()
     return browser, administrator
 
 
 def _test(browser, target, format, sample_num, expected_value):
     fmt = browser.find_element_by_id(target)
     fmt.clear()
@@ -48,10 +52,10 @@
     # expected_value = dateformat.format(datetime.datetime.now(), format)
     assert sample.text == expected_value, "Failed Ajax call on %s" % target
 
 
 # @pytest.mark.skipif('django.VERSION[:2]==(1,8)')
 def test_datetime_format_ajax(export_csv_page, now):
     browser, administrator = export_csv_page
-    _test(browser, "id_datetime_format", 'l, d F Y', 0, 'Friday, 25 December 2020')
-    _test(browser, "id_date_format", 'd F Y', 1, '25 December 2020')
-    _test(browser, "id_time_format", 'H:i', 2, '17:05')
+    _test(browser, "id_datetime_format", "l, d F Y", 0, "Friday, 25 December 2020")
+    _test(browser, "id_date_format", "d F Y", 1, "25 December 2020")
+    _test(browser, "id_time_format", "H:i", 2, "17:05")
```

### Comparing `django-adminactions-2.0.0/tests/selenium_tests/test_export_xls.py` & `django-adminactions-2.1.0/tests/selenium_tests/test_export_xls.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from selenium.webdriver.support.select import Select
 
 pytestmark = pytest.mark.selenium
 
 
 def test_export_xls(admin_site):
     browser, administrator = admin_site
-    browser.go('/admin/')
+    browser.go("/admin/")
     browser.find_element_by_link_text("Demo models").click()
     browser.find_element_by_id("action-toggle").click()
-    Select(browser.find_element_by_name("action")).select_by_visible_text("Export as XLS")
+    Select(browser.find_element_by_name("action")).select_by_visible_text(
+        "Export as XLS"
+    )
     browser.find_element_by_name("index").click()
     browser.find_element_by_name("apply").click()
     return browser, administrator
```

### Comparing `django-adminactions-2.0.0/tests/selenium_tests/test_mass_update.py` & `django-adminactions-2.1.0/tests/selenium_tests/test_mass_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 
 def test_mass_update_1(admin_site):
     """
     Check Boolean Field.
     Common values are not filled in boolean fields ( there is no reason to do that ).
     """
     assert User.objects.filter(is_active=True).count() > 1  # sanity check
-    sax = User.objects.get(username='sax')
+    sax = User.objects.get(username="sax")
     browser, administrator = admin_site
     browser.find_element_by_link_text("Users").click()
     browser.find_element_by_id("action-toggle").click()
-    browser.find_element_by_xpath("//input[@name='_selected_action' and @value='%s']" % sax.pk).click()  # unselect sax
+    browser.find_element_by_xpath(
+        "//input[@name='_selected_action' and @value='%s']" % sax.pk
+    ).click()  # unselect sax
 
     Select(browser.find_element_by_name("action")).select_by_visible_text("Mass update")
     browser.find_element_by_name("index").click()  # execute
 
     assert "Mass update (users)" in browser.title
     browser.find_element_by_name("chk_id_is_active").click()
     browser.find_element_by_id("id_is_active").click()
```

### Comparing `django-adminactions-2.0.0/tests/test_api.py` & `django-adminactions-2.1.0/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,154 +1,168 @@
 import csv
-import django
 import io
 import unittest
-import xlrd
 from collections import namedtuple
+
+import django
+import xlrd
 from django.contrib.auth.models import Permission
 from django.http import HttpResponse
 from django.test import TestCase
 
 from adminactions.api import export_as_csv, export_as_xls
 
 
 class TestExportQuerySetAsCsv(TestCase):
     def test_default_params(self):
         with self.assertNumQueries(1):
-            qs = Permission.objects.select_related().filter(codename='add_user')
+            qs = Permission.objects.select_related().filter(codename="add_user")
             ret = export_as_csv(queryset=qs)
         self.assertIsInstance(ret, HttpResponse)
         if django.VERSION[0] == 2:
-            self.assertEqual(ret.content.decode('utf8'), u'"%s";"Can add user";"user";"add_user"\r\n' % qs[0].pk)
+            self.assertEqual(
+                ret.content.decode("utf8"),
+                '"%s";"Can add user";"user";"add_user"\r\n' % qs[0].pk,
+            )
         elif django.VERSION[0] == 3:
-            self.assertEqual(ret.content.decode('utf8'), u'"%s";"Can add user";"auth | user";"add_user"\r\n' % qs[0].pk)
+            self.assertEqual(
+                ret.content.decode("utf8"),
+                '"%s";"Can add user";"auth | user";"add_user"\r\n' % qs[0].pk,
+            )
 
     def test_header_is_true(self):
         mem = io.StringIO()
         with self.assertNumQueries(1):
-            qs = Permission.objects.select_related().filter(codename='add_user')
+            qs = Permission.objects.select_related().filter(codename="add_user")
             export_as_csv(queryset=qs, header=True, out=mem)
         mem.seek(0)
         csv_reader = csv.reader(mem)
-        self.assertEqual(next(csv_reader), [u'id;"name";"content_type";"codename"'])
+        self.assertEqual(next(csv_reader), ['id;"name";"content_type";"codename"'])
 
     def test_queryset_values(self):
-        fields = ['codename', 'content_type__app_label']
-        header = ['Name', 'Application']
+        fields = ["codename", "content_type__app_label"]
+        header = ["Name", "Application"]
         mem = io.StringIO()
         with self.assertNumQueries(1):
-            qs = Permission.objects.filter(codename='add_user').values('codename', 'content_type__app_label')
+            qs = Permission.objects.filter(codename="add_user").values(
+                "codename", "content_type__app_label"
+            )
             export_as_csv(queryset=qs, fields=fields, header=header, out=mem)
         mem.seek(0)
         csv_dump = mem.read()
         self.assertEqual(csv_dump, '"Name";"Application"\r\n"add_user";"auth"\r\n')
 
     def test_callable_method(self):
-        fields = ['codename', 'natural_key']
+        fields = ["codename", "natural_key"]
         mem = io.StringIO()
         with self.assertNumQueries(2):
-            qs = Permission.objects.filter(codename='add_user')
+            qs = Permission.objects.filter(codename="add_user")
             export_as_csv(queryset=qs, fields=fields, out=mem)
         mem.seek(0)
         csv_dump = mem.read()
-        self.assertEqual(csv_dump, '"add_user";"(\'add_user\', \'auth\', \'user\')"\r\n')
+        self.assertEqual(csv_dump, "\"add_user\";\"('add_user', 'auth', 'user')\"\r\n")
 
     def test_deep_attr(self):
-        fields = ['codename', 'content_type.app_label']
+        fields = ["codename", "content_type.app_label"]
         mem = io.StringIO()
         with self.assertNumQueries(1):
-            qs = Permission.objects.select_related().filter(codename='add_user')
+            qs = Permission.objects.select_related().filter(codename="add_user")
             export_as_csv(queryset=qs, fields=fields, out=mem)
         mem.seek(0)
         csv_dump = mem.read()
         self.assertEqual(csv_dump, '"add_user";"auth"\r\n')
 
 
 class TestExportAsCsv(unittest.TestCase):
     def test_export_as_csv(self):
-        fields = ['field1', 'field2']
-        header = ['Field 1', 'Field 2']
-        Row = namedtuple('Row', fields)
-        rows = [Row(1, 4),
-                Row(2, 5),
-                Row(3, u'ӼӳӬԖԊ')]
+        fields = ["field1", "field2"]
+        header = ["Field 1", "Field 2"]
+        Row = namedtuple("Row", fields)
+        rows = [Row(1, 4), Row(2, 5), Row(3, "ӼӳӬԖԊ")]
         mem = io.StringIO()
         export_as_csv(queryset=rows, fields=fields, header=header, out=mem)
         mem.seek(0)
         csv_dump = mem.read()
-        self.assertEqual(csv_dump, '"Field 1";"Field 2"\r\n"1";"4"\r\n"2";"5"\r\n"3";"ӼӳӬԖԊ"\r\n')
+        self.assertEqual(
+            csv_dump, '"Field 1";"Field 2"\r\n"1";"4"\r\n"2";"5"\r\n"3";"ӼӳӬԖԊ"\r\n'
+        )
 
     def test_dialect(self):
-        fields = ['field1', 'field2']
-        header = ['Field 1', 'Field 2']
-        Row = namedtuple('Row', fields)
-        rows = [Row(1, 4),
-                Row(2, 5),
-                Row(3, 'ӼӳӬԖԊ')]
-        mem = io.StringIO()
-        export_as_csv(queryset=rows, fields=fields, header=header,
-                      out=mem, options={'dialect': 'excel'})
+        fields = ["field1", "field2"]
+        header = ["Field 1", "Field 2"]
+        Row = namedtuple("Row", fields)
+        rows = [Row(1, 4), Row(2, 5), Row(3, "ӼӳӬԖԊ")]
+        mem = io.StringIO()
+        export_as_csv(
+            queryset=rows,
+            fields=fields,
+            header=header,
+            out=mem,
+            options={"dialect": "excel"},
+        )
         mem.seek(0)
         csv_dump = mem.read()
-        self.assertEqual(csv_dump, 'Field 1,Field 2\r\n1,4\r\n2,5\r\n3,ӼӳӬԖԊ\r\n')
+        self.assertEqual(csv_dump, "Field 1,Field 2\r\n1,4\r\n2,5\r\n3,ӼӳӬԖԊ\r\n")
 
 
 class TestExportAsExcel(TestCase):
     def test_default_params(self):
         with self.assertNumQueries(1):
-            qs = Permission.objects.select_related().filter(codename='add_user')
+            qs = Permission.objects.select_related().filter(codename="add_user")
             ret = export_as_xls(queryset=qs)
         self.assertIsInstance(ret, HttpResponse)
 
     def test_header_is_true(self):
         mem = io.BytesIO()
         with self.assertNumQueries(1):
-            qs = Permission.objects.select_related().filter(codename='add_user')
+            qs = Permission.objects.select_related().filter(codename="add_user")
             export_as_xls(queryset=qs, header=True, out=mem)
         mem.seek(0)
         xls_workbook = xlrd.open_workbook(file_contents=mem.read())
         xls_sheet = xls_workbook.sheet_by_index(0)
-        self.assertEqual(xls_sheet.row_values(0)[:], ['#', 'ID', 'name', 'content type', 'codename'])
+        self.assertEqual(
+            xls_sheet.row_values(0)[:], ["#", "ID", "name", "content type", "codename"]
+        )
 
     def test_export_as_xls(self):
-        fields = ['field1', 'field2']
-        header = ['Field 1', 'Field 2']
-        Row = namedtuple('Row', fields)
-        rows = [Row(111, 222),
-                Row(333, 444),
-                Row(555, 'ӼӳӬԖԊ')]
+        fields = ["field1", "field2"]
+        header = ["Field 1", "Field 2"]
+        Row = namedtuple("Row", fields)
+        rows = [Row(111, 222), Row(333, 444), Row(555, "ӼӳӬԖԊ")]
         mem = io.BytesIO()
         export_as_xls(queryset=rows, fields=fields, header=header, out=mem)
         mem.seek(0)
 
         xls_workbook = xlrd.open_workbook(file_contents=mem.read())
         xls_sheet = xls_workbook.sheet_by_index(0)
-        self.assertEqual(xls_sheet.row_values(0)[:], ['#', 'Field 1', 'Field 2'])
+        self.assertEqual(xls_sheet.row_values(0)[:], ["#", "Field 1", "Field 2"])
         self.assertEqual(xls_sheet.row_values(1)[:], [1.0, 111.0, 222.0])
         self.assertEqual(xls_sheet.row_values(2)[:], [2.0, 333.0, 444.0])
-        self.assertEqual(xls_sheet.row_values(3)[:], [3.0, 555.0, u'ӼӳӬԖԊ'])
+        self.assertEqual(xls_sheet.row_values(3)[:], [3.0, 555.0, "ӼӳӬԖԊ"])
 
 
 class TestExportQuerySetAsExcel(TestCase):
     def test_queryset_values(self):
-        fields = ['codename', 'content_type__app_label']
-        header = ['Name', 'Application']
-        qs = Permission.objects.filter(codename='add_user').values('codename', 'content_type__app_label')
+        fields = ["codename", "content_type__app_label"]
+        header = ["Name", "Application"]
+        qs = Permission.objects.filter(codename="add_user").values(
+            "codename", "content_type__app_label"
+        )
         mem = io.BytesIO()
         export_as_xls(queryset=qs, fields=fields, header=header, out=mem)
         mem.seek(0)
         w = xlrd.open_workbook(file_contents=mem.read())
         sheet = w.sheet_by_index(0)
-        self.assertEqual(sheet.cell_value(1, 1), u'add_user')
-        self.assertEqual(sheet.cell_value(1, 2), u'auth')
+        self.assertEqual(sheet.cell_value(1, 1), "add_user")
+        self.assertEqual(sheet.cell_value(1, 2), "auth")
 
     def test_callable_method(self):
-        fields = ['codename', 'natural_key']
-        qs = Permission.objects.filter(codename='add_user')
+        fields = ["codename", "natural_key"]
+        qs = Permission.objects.filter(codename="add_user")
         mem = io.BytesIO()
         export_as_xls(queryset=qs, fields=fields, out=mem)
         mem.seek(0)
         content = mem.read()
         w = xlrd.open_workbook(file_contents=content)
         sheet = w.sheet_by_index(0)
-        self.assertEqual(sheet.cell_value(1, 1), u'add_user')
-        self.assertEqual(sheet.cell_value(1, 2), u'add_userauthuser')
+        self.assertEqual(sheet.cell_value(1, 1), "add_user")
+        self.assertEqual(sheet.cell_value(1, 2), "add_userauthuser")
```

### Comparing `django-adminactions-2.0.0/tests/test_byrows_update.py` & `django-adminactions-2.1.0/tests/test_byrows_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,100 +12,111 @@
 
 
 class MockRequest:
     pass
 
 
 class TestByRowsUpdateAction(WebTestMixin, SelectRowsMixin, TestCase):
-    fixtures = ['adminactions', 'demoproject']
-    urls = 'demo.urls'
-    action_name = 'byrows_update'
+    fixtures = ["adminactions", "demoproject"]
+    urls = "demo.urls"
+    action_name = "byrows_update"
     sender_model = DemoModel
     _selected_rows = [0, 1]
     csrf_checks = False
 
     def setUp(self):
         super().setUp()
-        self._url = reverse('admin:demo_demomodel_changelist')
-        self.user = G(User, username='user', is_staff=True, is_active=True)
+        self._url = reverse("admin:demo_demomodel_changelist")
+        self.user = G(User, username="user", is_staff=True, is_active=True)
         self.site = AdminSite()
         self.mockRequest = MockRequest()
 
     def _get_changelist_form_response(self):
-        res = self.app.get('/', user='user')
-        res = res.click('Demo models')
+        res = self.app.get("/", user="user")
+        res = res.click("Demo models")
         return res
 
     def _get_action_form_response(self, change_list_response=None):
-        form = change_list_response.forms['changelist-form']
-        form['action'] = 'byrows_update'
+        form = change_list_response.forms["changelist-form"]
+        form["action"] = "byrows_update"
         res = form.submit()
         return res
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel']):
+        with user_grant_permission(self.user, ["demo.change_demomodel"]):
             res = self._get_changelist_form_response()
 
-            form = res.forms['changelist-form']
-            form['action'] = 'byrows_update'
+            form = res.forms["changelist-form"]
+            form["action"] = "byrows_update"
             self._select_rows(form, selected_rows=self._selected_rows)
             res = form.submit().follow()
-            assert 'Sorry you do not have rights to execute this action' in str(res.body)
+            assert "Sorry you do not have rights to execute this action" in str(
+                res.body
+            )
 
     def test_form_rows_count(self):
         """
-            Count the selected items appear in the action form
+        Count the selected items appear in the action form
         """
         self.renew_app()
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_byrowsupdate_demomodel']):
+        with user_grant_permission(
+            self.user,
+            ["demo.change_demomodel", "demo.adminactions_byrowsupdate_demomodel"],
+        ):
             res = self._get_changelist_form_response()
 
-            form = res.forms['changelist-form']
+            form = res.forms["changelist-form"]
             self._select_rows(form, selected_rows=self._selected_rows)
             res = self._get_action_form_response(change_list_response=res)
-            self.assertEqual(len(res.html.find(id="formset").find_all(class_="row")), len(self._selected_rows))
+            self.assertEqual(
+                len(res.html.find(id="formset").find_all(class_="row")),
+                len(self._selected_rows),
+            )
 
     def test_form_rows_fields_exists(self):
         """
-            Check model fields appear in action form for each selected models
+        Check model fields appear in action form for each selected models
         """
-        with user_grant_permission(self.user, ['demo.change_demomodel', 'demo.adminactions_byrowsupdate_demomodel']):
+        with user_grant_permission(
+            self.user,
+            ["demo.change_demomodel", "demo.adminactions_byrowsupdate_demomodel"],
+        ):
             res = self._get_changelist_form_response()
 
-            form = res.forms['changelist-form']
+            form = res.forms["changelist-form"]
             self._select_rows(form, selected_rows=self._selected_rows)
             res = self._get_action_form_response(change_list_response=res)
             byrows_update_get_fields(ModelAdmin(DemoModel, self.site))
             for r, value in enumerate(self._selected_values):
                 for fname in byrows_update_get_fields(ModelAdmin(DemoModel, self.site)):
-                    fname = 'form-%d-%s' % (r, fname)
+                    fname = "form-%d-%s" % (r, fname)
 
                     try:
                         # Attempt split (admin datetime widget) fields first
-                        assert res.form[fname + '_0']
+                        assert res.forms["update-form"][fname + "_0"]
                     except AssertionError:
                         # assert for non-split fields to return the regular
                         # field name upon errors
-                        assert res.form[fname]
+                        assert res.forms["update-form"][fname]
 
     def test_form_rows_edit(self):
         """
-            Modify a value in action form and see if its stored upon form submit
+        Modify a value in action form and see if its stored upon form submit
         """
-        with user_grant_permission(self.user, ['demo.change_demomodel', 'demo.adminactions_byrowsupdate_demomodel']):
+        with user_grant_permission(
+            self.user,
+            ["demo.change_demomodel", "demo.adminactions_byrowsupdate_demomodel"],
+        ):
             res = self._get_changelist_form_response()
 
-            form = res.forms['changelist-form']
+            form = res.forms["changelist-form"]
             self._select_rows(form, selected_rows=self._selected_rows)
             res = self._get_action_form_response(change_list_response=res)
 
             row_to_modify = 0
-            new_values = {
-                'char': 'Bob Marley'
-            }
+            new_values = {"char": "Bob Marley"}
             for k, v in new_values.items():
-                res.form["form-%d-%s" % (row_to_modify, k)] = v
-            res.form.submit('apply')
+                res.forms["update-form"]["form-%d-%s" % (row_to_modify, k)] = v
+            res.forms["update-form"].submit("apply")
             obj = DemoModel.objects.get(id=self._selected_values[row_to_modify])
             for k, v in new_values.items():
                 self.assertEqual(v, getattr(obj, k))
```

### Comparing `django-adminactions-2.0.0/tests/test_duplicates.py` & `django-adminactions-2.1.0/tests/test_duplicates.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,66 +3,73 @@
 from django.contrib.auth.models import User
 from django.test import TestCase
 from django.urls import reverse
 from django_dynamic_fixture import G
 from django_webtest import WebTestMixin
 from utils import CheckSignalsMixin, SelectRowsMixin, user_grant_permission
 
-__all__ = ['FindDuplicatesTest', ]
+__all__ = [
+    "FindDuplicatesTest",
+]
 
 
 class FindDuplicatesTest(SelectRowsMixin, CheckSignalsMixin, WebTestMixin, TestCase):
-    fixtures = ['adminactions', 'demoproject']
-    urls = 'demo.urls'
+    fixtures = ["adminactions", "demoproject"]
+    urls = "demo.urls"
     csrf_checks = True
 
     _selected_rows = [0, 1]
 
-    action_name = 'find_duplicates_action'
+    action_name = "find_duplicates_action"
     sender_model = DemoModel
 
     def setUp(self):
         super().setUp()
-        self._url = reverse('admin:demo_demomodel_changelist')
-        self.user = G(User, username='user', is_staff=True, is_active=True)
+        self._url = reverse("admin:demo_demomodel_changelist")
+        self.user = G(User, username="user", is_staff=True, is_active=True)
 
     def _run_action(self, steps=2, **kwargs):
-        selected_rows = kwargs.pop('selected_rows', self._selected_rows)
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_find_duplicates_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
+        selected_rows = kwargs.pop("selected_rows", self._selected_rows)
+        with user_grant_permission(
+            self.user,
+            ["demo.change_demomodel", "demo.adminactions_find_duplicates_demomodel"],
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
             if steps >= 1:
-                form = res.forms['changelist-form']
-                form['action'] = 'find_duplicates_action'
+                form = res.forms["changelist-form"]
+                form["action"] = "find_duplicates_action"
                 self._select_rows(form, selected_rows)
                 res = form.submit()
             if steps >= 2:
-                res.form['email'].checked = True
+                res.form["email"].checked = True
                 # res.form['func_id_char'] = 'upper'
                 # res.form['chk_id_choices'].checked = True
                 # res.form['func_id_choices'] = 'set'
                 # res.form['choices'] = '1'
                 for k, v in kwargs.items():
                     res.form[k] = v
-                res = res.form.submit('apply')
+                res = res.form.submit("apply")
         return res
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
-            form = res.forms['changelist-form']
-            form['action'] = 'find_duplicates_action'
-            form.set('_selected_action', True, 0)
+        with user_grant_permission(self.user, ["demo.change_demomodel"]):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
+            form = res.forms["changelist-form"]
+            form["action"] = "find_duplicates_action"
+            form.set("_selected_action", True, 0)
             res = form.submit().follow()
-            assert 'Sorry you do not have rights to execute this action' in str(res.body)
+            assert "Sorry you do not have rights to execute this action" in str(
+                res.body
+            )
 
     def test_validate_on(self):
         self._run_action()
+
     #
     # def test_validate_off(self):
     #     res = self._run_action(**{'_validate': 0})
     #     assert res.status_code == 200
     #     form = res.context['adminform'].form
     #     assert form.errors['__all__'] == ["Cannot use operators without 'validate'"]
     #
```

### Comparing `django-adminactions-2.0.0/tests/test_exports.py` & `django-adminactions-2.1.0/tests/test_exports.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,426 +1,477 @@
 import csv
 import io
-import mock
 import time
 import unittest
+
+import mock
 import xlrd
 from django.contrib.auth.models import User
 from django.test.utils import override_settings
 from django.utils.encoding import smart_str
 from django_dynamic_fixture import G
 from django_webtest import WebTest
-from utils import (CheckSignalsMixin, SelectRowsMixin,
-                   admin_register, user_grant_permission,)
-
-__all__ = ['ExportAsCsvTest', 'ExportAsFixtureTest', 'ExportAsCsvTest',
-           'ExportDeleteTreeTest', 'ExportAsXlsTest']
+from utils import (
+    CheckSignalsMixin,
+    SelectRowsMixin,
+    admin_register,
+    user_grant_permission,
+)
+
+__all__ = [
+    "ExportAsCsvTest",
+    "ExportAsFixtureTest",
+    "ExportAsCsvTest",
+    "ExportDeleteTreeTest",
+    "ExportAsXlsTest",
+]
 
 
 class ExportMixin:
-    fixtures = ['adminactions', 'demoproject']
-    urls = 'demo.urls'
+    fixtures = ["adminactions", "demoproject"]
+    urls = "demo.urls"
     csrf_checks = True
 
     def setUp(self):
         super().setUp()
-        self.user = G(User, username='user', is_staff=True, is_active=True)
+        self.user = G(User, username="user", is_staff=True, is_active=True)
 
 
 class ExportAsFixtureTest(ExportMixin, SelectRowsMixin, CheckSignalsMixin, WebTest):
     sender_model = User
-    action_name = 'export_as_fixture'
+    action_name = "export_as_fixture"
     _selected_rows = [0, 1, 2]
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['auth.change_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
-            form.set('_selected_action', True, 0)
+        with user_grant_permission(self.user, ["auth.change_user"]):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
+            form.set("_selected_action", True, 0)
             res = form.submit().follow()
-            assert b'Sorry you do not have rights to execute this action' in res.body
+            assert b"Sorry you do not have rights to execute this action" in res.body
 
     def test_success(self):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
-            form.set('_selected_action', True, 0)
-            form.set('_selected_action', True, 1)
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
+            form.set("_selected_action", True, 0)
+            form.set("_selected_action", True, 1)
             res = form.submit()
-            res.form['use_natural_pk'] = False
-            res.form['use_natural_fk'] = True
-            res = res.form.submit('apply')
-            assert res.json[0]['pk'] == 1
+            res.forms["export-form"]["use_natural_pk"] = False
+            res.forms["export-form"]["use_natural_fk"] = True
+            res = res.forms["export-form"].submit("apply")
+            assert res.json[0]["pk"] == 1
 
     def test_add_foreign_keys(self):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
-            form.set('_selected_action', True, 0)
-            form.set('_selected_action', True, 1)
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
+            form.set("_selected_action", True, 0)
+            form.set("_selected_action", True, 1)
             res = form.submit()
-            res.form['use_natural_pk'] = False
-            res.form['use_natural_fk'] = True
-            res.form['add_foreign_keys'] = True
-            res = res.form.submit('apply')
-            assert res.json[0]['pk'] == 1
+            res.forms["export-form"]["use_natural_pk"] = False
+            res.forms["export-form"]["use_natural_fk"] = True
+            res.forms["export-form"]["add_foreign_keys"] = True
+            res = res.forms["export-form"].submit("apply")
+            assert res.json[0]["pk"] == 1
 
     def _run_action(self, steps=2):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
             if steps >= 1:
-                form = res.forms['changelist-form']
-                form['action'] = self.action_name
+                form = res.forms["changelist-form"]
+                form["action"] = self.action_name
                 self._select_rows(form)
                 res = form.submit()
             if steps >= 2:
-                res = res.form.submit('apply')
+                res = res.forms["export-form"].submit("apply")
         return res
 
 
 class ExportDeleteTreeTest(ExportMixin, SelectRowsMixin, CheckSignalsMixin, WebTest):
     sender_model = User
-    action_name = 'export_delete_tree'
+    action_name = "export_delete_tree"
     _selected_rows = [0, 1, 2]
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['auth.change_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
-            form.set('_selected_action', True, 0)
+        with user_grant_permission(self.user, ["auth.change_user"]):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
+            form.set("_selected_action", True, 0)
             res = form.submit().follow()
-            assert b'Sorry you do not have rights to execute this action' in res.body
+            assert b"Sorry you do not have rights to execute this action" in res.body
 
     def test_success(self):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
             self._select_rows(form, [0, 1])
             res = form.submit()
-            res.form['use_natural_fk'] = True
-            res = res.form.submit('apply')
-            assert res.json[0]['pk'] == 1
+            res.forms["export-form"]["use_natural_fk"] = True
+            res = res.forms["export-form"].submit("apply")
+            assert res.json[0]["pk"] == 1
 
     def _run_action(self, steps=2):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
             if steps >= 1:
-                form = res.forms['changelist-form']
-                form['action'] = self.action_name
+                form = res.forms["changelist-form"]
+                form["action"] = self.action_name
                 self._select_rows(form)
                 res = form.submit()
             if steps >= 2:
-                res = res.form.submit('apply')
+                res = res.forms["export-form"].submit("apply")
         return res
 
     def test_custom_filename(self):
         """
-            if the ModelAdmin has `get_export_as_csv_filename()`
-            use that method to get the attachment filename
+        if the ModelAdmin has `get_export_as_csv_filename()`
+        use that method to get the attachment filename
         """
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
             with admin_register(User) as md:
-                with mock.patch.object(md, 'get_export_delete_tree_filename',
-                                       lambda r, q: 'new.test', create=True):
-                    res = res.click('Users')
-                    form = res.forms['changelist-form']
-                    form['action'] = self.action_name
-                    form.set('_selected_action', True, 0)
-                    form['select_across'] = 1
+                with mock.patch.object(
+                    md,
+                    "get_export_delete_tree_filename",
+                    lambda r, q: "new.test",
+                    create=True,
+                ):
+                    res = res.click("Users")
+                    form = res.forms["changelist-form"]
+                    form["action"] = self.action_name
+                    form.set("_selected_action", True, 0)
+                    form["select_across"] = 1
                     res = form.submit()
-                    res = res.form.submit('apply')
-                    self.assertEqual(res.content_disposition,
-                                     'attachment;filename="new.test"')
+                    res = res.forms["export-form"].submit("apply")
+                    self.assertEqual(
+                        res.content_disposition, 'attachment;filename="new.test"'
+                    )
 
 
 class ExportAsCsvTest(ExportMixin, SelectRowsMixin, CheckSignalsMixin, WebTest):
     sender_model = User
-    action_name = 'export_as_csv'
+    action_name = "export_as_csv"
     _selected_rows = [0, 1]
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['auth.change_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = 'export_as_csv'
-            form.set('_selected_action', True, 0)
+        with user_grant_permission(self.user, ["auth.change_user"]):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = "export_as_csv"
+            form.set("_selected_action", True, 0)
             res = form.submit().follow()
-            assert b'Sorry you do not have rights to execute this action' in res.body
+            assert b"Sorry you do not have rights to execute this action" in res.body
 
     def test_success(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_export_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
+        with user_grant_permission(
+            self.user, ["demo.change_demomodel", "demo.adminactions_export_demomodel"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
             # form.set('_selected_action', True, 1)
             self._select_rows(form)
             res = form.submit()
-            res = res.form.submit('apply')
+            res = res.forms["export-form"].submit("apply")
             buff = io.StringIO(smart_str(res.body))
             csv_reader = csv.reader(buff)
 
             self.assertEqual(len(list(csv_reader)), 2)
 
     def test_custom_filename(self):
         """
-            if the ModelAdmin has `get_export_as_csv_filename()` use that method to get the
-            attachment filename
+        if the ModelAdmin has `get_export_as_csv_filename()` use that method to get the
+        attachment filename
         """
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
             with admin_register(User) as md:
-                with mock.patch.object(md, 'get_export_as_csv_filename',
-                                       lambda r, q: 'new.test', create=True):
-                    res = res.click('Users')
-                    form = res.forms['changelist-form']
-                    form['action'] = 'export_as_csv'
-                    form.set('_selected_action', True, 0)
-                    form['select_across'] = 1
+                with mock.patch.object(
+                    md,
+                    "get_export_as_csv_filename",
+                    lambda r, q: "new.test",
+                    create=True,
+                ):
+                    res = res.click("Users")
+                    form = res.forms["changelist-form"]
+                    form["action"] = "export_as_csv"
+                    form.set("_selected_action", True, 0)
+                    form["select_across"] = 1
                     res = form.submit()
-                    res = res.form.submit('apply')
-                    self.assertEqual(res.content_disposition,
-                                     u'attachment;filename="new.test"')
+                    res = res.forms["export-form"].submit("apply")
+                    self.assertEqual(
+                        res.content_disposition, 'attachment;filename="new.test"'
+                    )
 
     def _run_action(self, steps=2):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
             if steps >= 1:
-                form = res.forms['changelist-form']
-                form['action'] = self.action_name
+                form = res.forms["changelist-form"]
+                form["action"] = self.action_name
                 self._select_rows(form)
                 res = form.submit()
             if steps >= 2:
-                res = res.form.submit('apply')
+                res = res.forms["export-form"].submit("apply")
         return res
 
     @override_settings(ADMINACTIONS_STREAM_CSV=True)
     def test_streaming_export(self):
         res = self._run_action()
         buff = io.StringIO(smart_str(res.body))
         csv_reader = csv.reader(buff)
 
         self.assertEqual(len(list(csv_reader)), 2)
 
 
 class ExportAsXlsTest(ExportMixin, SelectRowsMixin, CheckSignalsMixin, WebTest):
     sender_model = User
-    action_name = 'export_as_xls'
+    action_name = "export_as_xls"
     _selected_rows = [0, 1]
 
     def _run_action(self, step=3):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
             if step >= 1:
-                form = res.forms['changelist-form']
-                form['action'] = self.action_name
+                form = res.forms["changelist-form"]
+                form["action"] = self.action_name
                 self._select_rows(form)
                 res = form.submit()
             if step >= 2:
-                res.form['header'] = 1
-                res = res.form.submit('apply')
+                res.forms["export-form"]["header"] = 1
+                res = res.forms["export-form"].submit("apply")
             return res
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['auth.change_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = 'export_as_xls'
-            form.set('_selected_action', True, 0)
+        with user_grant_permission(self.user, ["auth.change_user"]):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = "export_as_xls"
+            form.set("_selected_action", True, 0)
             res = form.submit().follow()
-            assert b'Sorry you do not have rights to execute this action' in res.body
+            assert b"Sorry you do not have rights to execute this action" in res.body
 
     def test_success(self):
-        with user_grant_permission(self.user, ['auth.change_user',
-                                               'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
             # form.set('_selected_action', True, 0)
             # form.set('_selected_action', True, 1)
             # form.set('_selected_action', True, 2)
             self._select_rows(form)
             res = form.submit()
-            res.form['header'] = 1
-            res.form['columns'] = ['id', 'username', 'first_name'
-                                                     '']
-            res = res.form.submit('apply')
+            res.forms["export-form"]["header"] = 1
+            res.forms["export-form"]["columns"] = ["id", "username", "first_name" ""]
+            res = res.forms["export-form"].submit("apply")
             buff = io.BytesIO(res.body)
 
             buff.seek(0)
             w = xlrd.open_workbook(file_contents=buff.read())
             sheet = w.sheet_by_index(0)
-            self.assertEqual(sheet.cell_value(0, 0), u'#')
-            self.assertEqual(sheet.cell_value(0, 1), u'ID')
-            self.assertEqual(sheet.cell_value(0, 2), u'username')
-            self.assertEqual(sheet.cell_value(0, 3), u'first name')
+            self.assertEqual(sheet.cell_value(0, 0), "#")
+            self.assertEqual(sheet.cell_value(0, 1), "ID")
+            self.assertEqual(sheet.cell_value(0, 2), "username")
+            self.assertEqual(sheet.cell_value(0, 3), "first name")
             self.assertEqual(sheet.cell_value(1, 1), 1.0)
-            self.assertEqual(sheet.cell_value(1, 2), u'sax')
-            self.assertEqual(sheet.cell_value(2, 2), u'user')
+            self.assertEqual(sheet.cell_value(1, 2), "sax")
+            self.assertEqual(sheet.cell_value(2, 2), "user")
             # self.assertEqual(sheet.cell_value(3, 2), u'user_00')
 
     def test_use_display_ok(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_export_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
+        with user_grant_permission(
+            self.user, ["demo.change_demomodel", "demo.adminactions_export_demomodel"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
             self._select_rows(form)
             res = form.submit()
-            res.form['header'] = 1
-            res.form['use_display'] = 1
-            res.form['columns'] = ['char', 'text', 'bigint', 'choices'
-                                                             '']
-            res = res.form.submit('apply')
+            res.forms["export-form"]["header"] = 1
+            res.forms["export-form"]["use_display"] = 1
+            res.forms["export-form"]["columns"] = [
+                "char",
+                "text",
+                "bigint",
+                "choices" "",
+            ]
+            res = res.forms["export-form"].submit("apply")
             buff = io.BytesIO(res.body)
 
             buff.seek(0)
             w = xlrd.open_workbook(file_contents=buff.read())
             sheet = w.sheet_by_index(0)
-            self.assertEqual(sheet.cell_value(0, 1), u'Chäř')
-            self.assertEqual(sheet.cell_value(0, 2), u'bigint')
-            self.assertEqual(sheet.cell_value(0, 3), u'text')
-            self.assertEqual(sheet.cell_value(0, 4), u'choices')
-            self.assertEqual(sheet.cell_value(1, 1), u'Pizzä ïs Gööd')
+            self.assertEqual(sheet.cell_value(0, 1), "Chäř")
+            self.assertEqual(sheet.cell_value(0, 2), "bigint")
+            self.assertEqual(sheet.cell_value(0, 3), "text")
+            self.assertEqual(sheet.cell_value(0, 4), "choices")
+            self.assertEqual(sheet.cell_value(1, 1), "Pizzä ïs Gööd")
             self.assertEqual(sheet.cell_value(1, 2), 333333333.0)
-            self.assertEqual(sheet.cell_value(1, 3), u'lorem ipsum')
-            self.assertEqual(sheet.cell_value(1, 4), u'Choice 2')
+            self.assertEqual(sheet.cell_value(1, 3), "lorem ipsum")
+            self.assertEqual(sheet.cell_value(1, 4), "Choice 2")
 
     def test_use_display_ko(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_export_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
+        with user_grant_permission(
+            self.user, ["demo.change_demomodel", "demo.adminactions_export_demomodel"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
             self._select_rows(form)
             res = form.submit()
-            res.form['header'] = 1
-            res.form['columns'] = ['char', 'text', 'bigint', 'choices'
-                                                             '']
-            res = res.form.submit('apply')
+            res.forms["export-form"]["header"] = 1
+            res.forms["export-form"]["columns"] = [
+                "char",
+                "text",
+                "bigint",
+                "choices" "",
+            ]
+            res = res.forms["export-form"].submit("apply")
             buff = io.BytesIO(res.body)
 
             buff.seek(0)
             w = xlrd.open_workbook(file_contents=buff.read())
             sheet = w.sheet_by_index(0)
-            self.assertEqual(sheet.cell_value(0, 1), u'Chäř')
-            self.assertEqual(sheet.cell_value(0, 2), u'bigint')
-            self.assertEqual(sheet.cell_value(0, 3), u'text')
-            self.assertEqual(sheet.cell_value(0, 4), u'choices')
-            self.assertEqual(sheet.cell_value(1, 1), u'Pizzä ïs Gööd')
+            self.assertEqual(sheet.cell_value(0, 1), "Chäř")
+            self.assertEqual(sheet.cell_value(0, 2), "bigint")
+            self.assertEqual(sheet.cell_value(0, 3), "text")
+            self.assertEqual(sheet.cell_value(0, 4), "choices")
+            self.assertEqual(sheet.cell_value(1, 1), "Pizzä ïs Gööd")
             self.assertEqual(sheet.cell_value(1, 2), 333333333.0)
-            self.assertEqual(sheet.cell_value(1, 3), u'lorem ipsum')
+            self.assertEqual(sheet.cell_value(1, 3), "lorem ipsum")
             self.assertEqual(sheet.cell_value(1, 4), 2.0)
 
     def test_unicode(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_export_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
+        with user_grant_permission(
+            self.user, ["demo.change_demomodel", "demo.adminactions_export_demomodel"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
             self._select_rows(form)
             res = form.submit()
-            res.form['header'] = 1
-            res.form['columns'] = ['char', ]
-            res = res.form.submit('apply')
+            res.forms["export-form"]["header"] = 1
+            res.forms["export-form"]["columns"] = [
+                "char",
+            ]
+            res = res.forms["export-form"].submit("apply")
             buff = io.BytesIO(res.body)
 
             buff.seek(0)
             w = xlrd.open_workbook(file_contents=buff.read())
             sheet = w.sheet_by_index(0)
-            self.assertEqual(sheet.cell_value(0, 1), u'Chäř')
-            self.assertEqual(sheet.cell_value(1, 1), u'Pizzä ïs Gööd')
+            self.assertEqual(sheet.cell_value(0, 1), "Chäř")
+            self.assertEqual(sheet.cell_value(1, 1), "Pizzä ïs Gööd")
 
     def test_issue_93(self):
         # default date(time) format in XLS export doesn't import well on excel
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_export_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
+        with user_grant_permission(
+            self.user, ["demo.change_demomodel", "demo.adminactions_export_demomodel"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
             self._select_rows(form)
             res = form.submit()
-            res.form['header'] = 1
-            res.form['columns'] = ['date', ]
-            res = res.form.submit('apply')
+            res.forms["export-form"]["header"] = 1
+            res.forms["export-form"]["columns"] = [
+                "date",
+            ]
+            res = res.forms["export-form"].submit("apply")
             buff = io.BytesIO(res.body)
 
             buff.seek(0)
             w = xlrd.open_workbook(file_contents=buff.read(), formatting_info=True)
             sheet = w.sheet_by_index(0)
 
             cell = sheet.cell(1, 1)
             fmt = w.xf_list[cell.xf_index]
             format_key = fmt.format_key
             format = w.format_map[format_key]  # gets a Format object
 
             self.assertEqual(cell.value, 41303.0)
             self.assertEqual(cell.ctype, 3)
-            self.assertEqual(format.format_str, u'd/m/Y')
+            self.assertEqual(format.format_str, "d/m/Y")
 
     @unittest.skip("Impossible to reliably time different machine runs")
     def test_faster_export(self):
         # generate 3k users
         start = time.time()
         user_count = User.objects.count()
-        User.objects.bulk_create([User(
-            username='bulk_user_%s' % i) for i in range(3000)])
+        User.objects.bulk_create(
+            [User(username="bulk_user_%s" % i) for i in range(3000)]
+        )
         # print('created 3k users in %.1f seconds' % (time.time() - start))
         self.assertEqual(User.objects.count(), 3000 + user_count)
 
         start = time.time()
-        with user_grant_permission(self.user, [
-                'auth.change_user', 'auth.adminactions_export_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = self.action_name
-            form['select_across'] = 1
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_export_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = self.action_name
+            form["select_across"] = 1
             self._select_rows(form)
             res = form.submit()
-            res.form['header'] = 1
-            res = res.form.submit('apply')
+            res.forms["export-form"]["header"] = 1
+            res = res.form.submit("apply")
 
-        res_time = (time.time() - start)
+        res_time = time.time() - start
         # print('Response returned in %.1f seconds' % res_time)
 
         buff = io.BytesIO(res.body)
 
         buff.seek(0)
         w = xlrd.open_workbook(file_contents=buff.read())
         sheet = w.sheet_by_index(0)
 
         self.assertEqual(sheet.nrows, 3000 + user_count + 1)
-        self.assertLessEqual(res_time, 6.5, "Response should return under 6.5 "
-                             "seconds, was %.2f" % res_time)
+        self.assertLessEqual(
+            res_time,
+            6.5,
+            "Response should return under 6.5 " "seconds, was %.2f" % res_time,
+        )
```

### Comparing `django-adminactions-2.0.0/tests/test_mass_update.py` & `django-adminactions-2.1.0/tests/test_mass_update.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,156 @@
 # from adminactions.signals import adminaction_requested, adminaction_start, adminaction_end
+from pathlib import Path
+from unittest import skipIf
+from unittest.mock import patch
+
 from demo.models import DemoModel
 from django.contrib.auth.models import User
+from django.db.models import fields
 from django.test import TestCase
 from django.urls import reverse
 from django_dynamic_fixture import G
 from django_webtest import WebTestMixin
-from unittest.mock import patch
 from utils import CheckSignalsMixin, SelectRowsMixin, user_grant_permission
+from webtest import Upload
+
+from adminactions.compat import celery_present
+from adminactions.mass_update import OPERATIONS
+
+__all__ = [
+    "MassUpdateTest",
+]
 
-__all__ = ['MassUpdateTest', ]
+
+def test_operationmanager():
+    assert OPERATIONS[fields.IntegerField] == OPERATIONS[fields.BigIntegerField]
+    assert OPERATIONS[fields.BooleanField] == OPERATIONS[fields.NullBooleanField]
 
 
 class MassUpdateTest(SelectRowsMixin, CheckSignalsMixin, WebTestMixin, TestCase):
-    fixtures = ['adminactions', 'demoproject']
-    urls = 'demo.urls'
+    fixtures = ["adminactions", "demoproject"]
+    urls = "demo.urls"
     csrf_checks = True
 
     _selected_rows = [0, 1]
 
-    action_name = 'mass_update'
+    action_name = "mass_update"
     sender_model = DemoModel
 
     def setUp(self):
         super().setUp()
-        self._url = reverse('admin:demo_demomodel_changelist')
-        self.user = G(User, username='user', is_staff=True, is_active=True)
+        self._url = reverse("admin:demo_demomodel_changelist")
+        self.user = G(User, username="user", is_staff=True, is_active=True)
 
     def _run_action(self, steps=2, **kwargs):
-        selected_rows = kwargs.pop('selected_rows', self._selected_rows)
-        with user_grant_permission(self.user, ['demo.change_demomodel',
-                                               'demo.adminactions_massupdate_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
+        selected_rows = kwargs.pop("selected_rows", self._selected_rows)
+        with user_grant_permission(
+            self.user,
+            ["demo.change_demomodel", "demo.adminactions_massupdate_demomodel"],
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
             if steps >= 1:
-                form = res.forms['changelist-form']
-                form['action'] = 'mass_update'
+                form = res.forms["changelist-form"]
+                form["action"] = "mass_update"
                 self._select_rows(form, selected_rows)
                 res = form.submit()
             if steps >= 2:
-                res.form['chk_id_char'].checked = True
-                res.form['func_id_char'] = 'upper'
-                res.form['chk_id_choices'].checked = True
-                res.form['func_id_choices'] = 'set'
-                res.form['choices'] = '1'
+                res.forms["mass-update-form"]["chk_id_char"].checked = True
+                res.forms["mass-update-form"]["func_id_char"] = "upper"
+                res.forms["mass-update-form"]["chk_id_choices"].checked = True
+                res.forms["mass-update-form"]["func_id_choices"] = "set"
+                res.forms["mass-update-form"]["choices"] = "1"
                 for k, v in kwargs.items():
-                    res.form[k] = v
-                res = res.form.submit('apply')
+                    res.forms["mass-update-form"][k] = v
+                res = res.forms["mass-update-form"].submit("apply")
         return res
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel']):
-            res = self.app.get('/', user='user')
-            res = res.click('Demo models')
-            form = res.forms['changelist-form']
-            form['action'] = 'mass_update'
-            form.set('_selected_action', True, 0)
+        with user_grant_permission(self.user, ["demo.change_demomodel"]):
+            res = self.app.get("/", user="user")
+            res = res.click("Demo models")
+            form = res.forms["changelist-form"]
+            form["action"] = "mass_update"
+            form.set("_selected_action", True, 0)
             res = form.submit().follow()
-            assert 'Sorry you do not have rights to execute this action' in str(res.body)
+            assert "Sorry you do not have rights to execute this action" in str(
+                res.body
+            )
 
     def test_validate_on(self):
-        self._run_action(**{'_validate': 1})
-        assert DemoModel.objects.filter(char='CCCCC').exists()
-        assert not DemoModel.objects.filter(char='ccccc').exists()
+        self._run_action(**{"_validate": 1})
+        assert DemoModel.objects.filter(char="CCCCC").exists()
+        assert not DemoModel.objects.filter(char="ccccc").exists()
 
     def test_validate_off(self):
-        res = self._run_action(**{'_validate': 0})
+        res = self._run_action(**{"_validate": 0})
         assert res.status_code == 200
-        form = res.context['adminform'].form
-        assert form.errors['__all__'] == ["Cannot use operators without 'validate'"]
+        form = res.context["adminform"].form
+        assert form.errors["__all__"] == ["Cannot use operators without 'validate'"]
 
     def test_clean_on(self):
-        self._run_action(**{'_clean': 1})
+        self._run_action(**{"_clean": 1})
 
-        assert DemoModel.objects.filter(char='CCCCC').exists()
-        assert not DemoModel.objects.filter(char='ccccc').exists()
+        assert DemoModel.objects.filter(char="CCCCC").exists()
+        assert not DemoModel.objects.filter(char="ccccc").exists()
 
     def test_messages(self):
-        with user_grant_permission(self.user, ['demo.change_demomodel', 'demo.adminactions_massupdate_demomodel']):
-            res = self._run_action(**{'_clean': 1})
+        with user_grant_permission(
+            self.user,
+            ["demo.change_demomodel", "demo.adminactions_massupdate_demomodel"],
+        ):
+            res = self._run_action(**{"_clean": 1})
             res = res.follow()
-            messages = [m.message for m in list(res.context['messages'])]
+            messages = [m.message for m in list(res.context["messages"])]
             self.assertTrue(messages)
-            self.assertEqual('Updated 2 records', messages[0])
+            self.assertEqual("Updated 2 records", messages[0])
 
             res = self._run_action(selected_rows=[1]).follow()
-            messages = [m.message for m in list(res.context['messages'])]
+            messages = [m.message for m in list(res.context["messages"])]
             self.assertTrue(messages)
-            self.assertEqual('Updated 1 records', messages[0])
+            self.assertEqual("Updated 1 records", messages[0])
 
+    @skipIf(not celery_present, "Celery not installed")
     def test_async_qs(self):
         # Create handler
-        res = self._run_action(**{'_async': 1, '_validate': 0, 'chk_id_char': False})
+
+        res = self._run_action(**{"_async": 1, "_validate": 0, "chk_id_char": False})
         assert res.status_code == 302
         assert DemoModel.objects.filter(choices=1).exists()
 
-    @patch('adminactions.mass_update.adminaction_end.send')
-    @patch('adminactions.mass_update.adminaction_start.send')
-    @patch('adminactions.mass_update.adminaction_requested.send')
+    @patch("adminactions.mass_update.adminaction_end.send")
+    @patch("adminactions.mass_update.adminaction_start.send")
+    @patch("adminactions.mass_update.adminaction_requested.send")
+    @skipIf(not celery_present, "Celery not installed")
     def test_async_single(self, req, start, end):
-        res = self._run_action(**{'_async': 1, '_validate': 1})
+        res = self._run_action(**{"_async": 1, "_validate": 1})
         assert res.status_code == 302
         assert req.called
         assert start.called
         assert end.called
-        assert DemoModel.objects.filter(char='CCCCC').exists()
-        assert not DemoModel.objects.filter(char='ccccc').exists()
+        assert DemoModel.objects.filter(char="CCCCC").exists()
+        assert not DemoModel.objects.filter(char="ccccc").exists()
+
+    def test_file_field(self):
+        self._run_action(
+            **{
+                "_validate": 1,
+                "select_across": 1,
+                "chk_id_image": True,
+                "image": Upload(str(Path(__file__).parent / "test.jpeg")),
+            }
+        )
+        obj1 = DemoModel.objects.get(pk=1)
+        obj2 = DemoModel.objects.get(pk=2)
+        assert obj1.image.read() == obj2.image.read()
+
+    def test_file_field_prevent_async(self):
+        res = self._run_action(
+            **{
+                "_async": 1,
+                "select_across": 1,
+                "chk_id_image": True,
+                "image": Upload(str(Path(__file__).parent / "test.jpeg")),
+            }
+        )
+        assert res.status_code == 200
```

### Comparing `django-adminactions-2.0.0/tests/test_merge.py` & `django-adminactions-2.1.0/tests/test_merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
+
 from demo.models import DemoModel, DemoOneToOne, UserDetail
 from django.conf import settings
 from django.contrib.admin.models import LogEntry
 from django.contrib.auth.models import Group, Permission, User
 from django.test import TestCase
 from django.urls import reverse
 from django_dynamic_fixture import G
 from django_webtest import WebTestMixin
 from utils import BaseTestCaseMixin, SelectRowsMixin, user_grant_permission
 
 from adminactions.api import ALL_FIELDS, merge
 
-PROFILE_MODULE = getattr(settings, 'AUTH_PROFILE_MODULE', 'tests.UserProfile')
+PROFILE_MODULE = getattr(settings, "AUTH_PROFILE_MODULE", "tests.UserProfile")
 
 
 def get_profile(user):
     return UserDetail.objects.get_or_create(user=user, note="")[0]
 
 
 class MergeTestApi(BaseTestCaseMixin, TestCase):
-    fixtures = ['adminactions.json', 'demoproject.json']
+    fixtures = ["adminactions.json", "demoproject.json"]
 
     def setUp(self):
         super().setUp()
         self.master_pk = 2
         self.other_pk = 3
 
     def tearDown(self):
@@ -41,15 +42,15 @@
         self.assertEqual(result.first_name, master.first_name)
         self.assertEqual(result.last_name, master.last_name)
         self.assertEqual(result.password, master.password)
 
     def test_merge_success_fields_no_commit(self):
         master = User.objects.get(pk=self.master_pk)
         other = User.objects.get(pk=self.other_pk)
-        result = merge(master, other, ['password', 'last_login'])
+        result = merge(master, other, ["password", "last_login"])
 
         master = User.objects.get(pk=master.pk)
 
         self.assertTrue(User.objects.filter(pk=master.pk).exists())
         self.assertTrue(User.objects.filter(pk=other.pk).exists())
 
         self.assertNotEqual(result.last_login, master.last_login)
@@ -71,40 +72,40 @@
         self.assertEqual(master.first_name, old_master.first_name)
         self.assertEqual(master.last_name, old_master.last_name)
         self.assertEqual(master.password, old_master.password)
 
     def test_merge_success_m2m(self):
         master = User.objects.get(pk=self.master_pk)
         other = User.objects.get(pk=self.other_pk)
-        group = Group.objects.get_or_create(name='G1')[0]
+        group = Group.objects.get_or_create(name="G1")[0]
         other.groups.add(group)
         other.save()
 
-        result = merge(master, other, commit=True, m2m=['groups'])
+        result = merge(master, other, commit=True, m2m=["groups"])
         master = User.objects.get(pk=result.pk)  # reload
         self.assertSequenceEqual(master.groups.all(), [group])
 
     def test_merge_success_m2m_all(self):
         master = User.objects.get(pk=self.master_pk)
         other = User.objects.get(pk=self.other_pk)
-        group = Group.objects.get_or_create(name='G1')[0]
+        group = Group.objects.get_or_create(name="G1")[0]
         perm = Permission.objects.all()[0]
         other.groups.add(group)
         other.user_permissions.add(perm)
         other.save()
 
         merge(master, other, commit=True, m2m=ALL_FIELDS)
 
         self.assertSequenceEqual(master.groups.all(), [group])
         self.assertSequenceEqual(master.user_permissions.all(), [perm])
 
     def test_merge_success_related_all(self):
         master = User.objects.get(pk=self.master_pk)
         other = User.objects.get(pk=self.other_pk)
-        entry = other.logentry_set.get_or_create(object_repr='test', action_flag=1)[0]
+        entry = other.logentry_set.get_or_create(object_repr="test", action_flag=1)[0]
 
         result = merge(master, other, commit=True, related=ALL_FIELDS)
 
         master = User.objects.get(pk=result.pk)  # reload
         self.assertSequenceEqual(master.logentry_set.all(), [entry])
         self.assertTrue(LogEntry.objects.filter(pk=entry.pk).exists())
 
@@ -123,28 +124,30 @@
 
     # @skipIf(not hasattr(settings, 'AUTH_PROFILE_MODULE'), "")
     def test_merge_one_to_one_field(self):
         master = User.objects.get(pk=self.master_pk)
         other = User.objects.get(pk=self.other_pk)
         profile = get_profile(other)
         if profile:
-            entry = other.logentry_set.get_or_create(object_repr='test', action_flag=1)[0]
+            entry = other.logentry_set.get_or_create(object_repr="test", action_flag=1)[
+                0
+            ]
 
             result = merge(master, other, commit=True, related=ALL_FIELDS)
 
             master = User.objects.get(pk=result.pk)  # reload
             self.assertSequenceEqual(master.logentry_set.all(), [entry])
             self.assertTrue(LogEntry.objects.filter(pk=entry.pk).exists())
             self.assertEqual(get_profile(result), profile)
             # self.assertEqual(master.get_profile(), profile)
 
     def test_merge_ignore_related(self):
         master = User.objects.get(pk=self.master_pk)
         other = User.objects.get(pk=self.other_pk)
-        entry = other.logentry_set.get_or_create(object_repr='test', action_flag=1)[0]
+        entry = other.logentry_set.get_or_create(object_repr="test", action_flag=1)[0]
         result = merge(master, other, commit=True, related=None)
 
         master = User.objects.get(pk=result.pk)  # reload
         self.assertSequenceEqual(master.logentry_set.all(), [])
         self.assertFalse(User.objects.filter(pk=other.pk).exists())
         self.assertFalse(LogEntry.objects.filter(pk=entry.pk).exists())
 
@@ -153,250 +156,302 @@
         other = DemoModel.objects.get(pk=1)
         img1 = other.image
         img2 = other.subclassed_image
 
         assert master.image != other.image
         assert master.subclassed_image != other.subclassed_image
 
-        result = merge(master, other,
-                       fields=['image', 'subclassed_image'],
-                       commit=True, related=None)
+        result = merge(
+            master,
+            other,
+            fields=["image", "subclassed_image"],
+            commit=True,
+            related=None,
+        )
 
         master = DemoModel.objects.get(pk=result.pk)  # reload
         self.assertFalse(DemoModel.objects.filter(pk=other.pk).exists())
         self.assertEqual(master.image, img1)
         self.assertEqual(master.subclassed_image, img2)
 
 
 class TestMergeAction(SelectRowsMixin, WebTestMixin, TestCase):
     csrf_checks = True
-    fixtures = ['adminactions.json', 'demoproject.json']
-    urls = 'demo.urls'
+    fixtures = ["adminactions.json", "demoproject.json"]
+    urls = "demo.urls"
     sender_model = User
-    action_name = 'merge'
+    action_name = "merge"
     _selected_rows = [1, 2]
 
     def setUp(self):
         super().setUp()
-        self.url = reverse('admin:auth_user_changelist')
-        self.user = G(User, username='user', is_staff=True, is_active=True)
+        self.url = reverse("admin:auth_user_changelist")
+        self.user = G(User, username="user", is_staff=True, is_active=True)
 
     def _run_action(self, steps=3, page_start=None):
-        with user_grant_permission(self.user, ['auth.change_user', 'auth.adminactions_merge_user']):
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_merge_user"]
+        ):
             if isinstance(steps, int):
                 steps = list(range(1, steps + 1))
-                res = self.app.get('/', user='user')
-                res = res.click('Users')
+                res = self.app.get("/", user="user")
+                res = res.click("Users")
             else:
                 res = page_start
             if 1 in steps:
-                form = res.forms['changelist-form']
-                form['action'] = 'merge'
+                form = res.forms["changelist-form"]
+                form["action"] = "merge"
                 self._select_rows(form)
                 res = form.submit()
-                assert not hasattr(res.form, 'errors')
+                assert not hasattr(res.forms["merge-form"], "errors")
 
             if 2 in steps:
-                res.form['username'] = res.form['form-1-username'].value
-                res.form['email'] = res.form['form-1-email'].value
-                res.form['last_login'] = res.form['form-1-last_login'].value
-                res.form['date_joined'] = res.form['form-1-date_joined'].value
-                res = res.form.submit('preview')
-                assert not hasattr(res.form, 'errors')
+                res.forms["merge-form"]["username"] = res.forms["merge-form"][
+                    "form-1-username"
+                ].value
+                res.forms["merge-form"]["email"] = res.forms["merge-form"][
+                    "form-1-email"
+                ].value
+                res.forms["merge-form"]["last_login"] = res.forms["merge-form"][
+                    "form-1-last_login"
+                ].value
+                res.forms["merge-form"]["date_joined"] = res.forms["merge-form"][
+                    "form-1-date_joined"
+                ].value
+                res = res.forms["merge-form"].submit("preview")
+                assert not hasattr(res.forms["merge-form"], "errors")
 
             if 3 in steps:
-                res = res.form.submit('apply')
+                res = res.forms["merge-form"].submit("apply")
             return res
 
     def test_no_permission(self):
-        with user_grant_permission(self.user, ['auth.change_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = 'merge'
+        with user_grant_permission(self.user, ["auth.change_user"]):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = "merge"
             self._select_rows(form)
             res = form.submit().follow()
-            assert 'Sorry you do not have rights to execute this action' in str(res.body)
+            assert "Sorry you do not have rights to execute this action" in str(
+                res.body
+            )
 
+    # noinspection PyTypeChecker
     def test_success(self):
         res = self._run_action(1)
         preserved = User.objects.get(pk=self._selected_values[0])
         removed = User.objects.get(pk=self._selected_values[1])
 
         assert preserved.email != removed.email  # sanity check
 
-        res = self._run_action([2, 3], res)
+        self._run_action([2, 3], res)
 
         self.assertFalse(User.objects.filter(pk=removed.pk).exists())
         self.assertTrue(User.objects.filter(pk=preserved.pk).exists())
 
         preserved_after = User.objects.get(pk=self._selected_values[0])
         self.assertEqual(preserved_after.email, removed.email)
         self.assertFalse(LogEntry.objects.filter(pk=removed.pk).exists())
 
     def test_error_if_too_many_records(self):
-        with user_grant_permission(self.user, ['auth.change_user', 'auth.adminactions_merge_user']):
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = 'merge'
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_merge_user"]
+        ):
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = "merge"
             self._select_rows(form, [1, 2, 3])
             res = form.submit().follow()
-            self.assertContains(res, 'Please select exactly 2 records')
+            self.assertContains(res, "Please select exactly 2 records")
 
     def test_swap(self):
-        with user_grant_permission(self.user, ['auth.change_user', 'auth.adminactions_merge_user']):
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_merge_user"]
+        ):
             # removed = User.objects.get(pk=self._selected_rows[0])
             # preserved = User.objects.get(pk=self._selected_rows[1])
 
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = 'merge'
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = "merge"
             self._select_rows(form, [1, 2])
             res = form.submit()
             removed = User.objects.get(pk=self._selected_values[0])
             preserved = User.objects.get(pk=self._selected_values[1])
 
             # steps = 2 (swap):
-            res.form['master_pk'] = self._selected_values[1]
-            res.form['other_pk'] = self._selected_values[0]
+            res.forms["merge-form"]["master_pk"] = self._selected_values[1]
+            res.forms["merge-form"]["other_pk"] = self._selected_values[0]
 
-            res.form['username'] = res.form['form-0-username'].value
-            res.form['email'] = res.form['form-0-email'].value
-            res.form['last_login'] = res.form['form-1-last_login'].value
-            res.form['date_joined'] = res.form['form-1-date_joined'].value
+            res.forms["merge-form"]["username"] = res.forms["merge-form"][
+                "form-0-username"
+            ].value
+            res.forms["merge-form"]["email"] = res.forms["merge-form"][
+                "form-0-email"
+            ].value
+            res.forms["merge-form"]["last_login"] = res.forms["merge-form"][
+                "form-1-last_login"
+            ].value
+            res.forms["merge-form"]["date_joined"] = res.forms["merge-form"][
+                "form-1-date_joined"
+            ].value
 
             # res.form['field_names'] = 'username,email'
 
-            res = res.form.submit('preview')
+            res = res.forms["merge-form"].submit("preview")
             # steps = 3:
-            res = res.form.submit('apply')
+            res = res.forms["merge-form"].submit("apply")
 
             preserved_after = User.objects.get(pk=self._selected_values[1])
             self.assertFalse(User.objects.filter(pk=removed.pk).exists())
             self.assertTrue(User.objects.filter(pk=preserved.pk).exists())
 
             self.assertEqual(preserved_after.email, removed.email)
             self.assertFalse(LogEntry.objects.filter(pk=removed.pk).exists())
 
     def test_merge_move_detail(self):
         from adminactions.merge import MergeForm
 
-        with user_grant_permission(self.user, ['auth.change_user', 'auth.adminactions_merge_user']):
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_merge_user"]
+        ):
             # removed = User.objects.get(pk=self._selected_rows[0])
             # preserved = User.objects.get(pk=self._selected_rows[1])
 
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = 'merge'
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = "merge"
             self._select_rows(form, [1, 2])
             res = form.submit()
             removed = User.objects.get(pk=self._selected_values[0])
             preserved = User.objects.get(pk=self._selected_values[1])
 
-            removed.userdetail_set.create(note='1')
-            preserved.userdetail_set.create(note='2')
+            removed.userdetail_set.create(note="1")
+            preserved.userdetail_set.create(note="2")
 
             # steps = 2:
-            res.form['master_pk'] = self._selected_values[1]
-            res.form['other_pk'] = self._selected_values[0]
+            res.forms["merge-form"]["master_pk"] = self._selected_values[1]
+            res.forms["merge-form"]["other_pk"] = self._selected_values[0]
 
-            res.form['username'] = res.form['form-0-username'].value
-            res.form['email'] = res.form['form-0-email'].value
-            res.form['last_login'] = res.form['form-1-last_login'].value
-            res.form['date_joined'] = res.form['form-1-date_joined'].value
-            res.form['dependencies'] = MergeForm.DEP_MOVE
-            res = res.form.submit('preview')
+            res.forms["merge-form"]["username"] = res.forms["merge-form"][
+                "form-0-username"
+            ].value
+            res.forms["merge-form"]["email"] = res.forms["merge-form"][
+                "form-0-email"
+            ].value
+            res.forms["merge-form"]["last_login"] = res.forms["merge-form"][
+                "form-1-last_login"
+            ].value
+            res.forms["merge-form"]["date_joined"] = res.forms["merge-form"][
+                "form-1-date_joined"
+            ].value
+            res.forms["merge-form"]["dependencies"] = MergeForm.DEP_MOVE
+            res = res.forms["merge-form"].submit("preview")
             # steps = 3:
-            res = res.form.submit('apply')
+            res = res.forms["merge-form"].submit("apply")
 
             preserved_after = User.objects.get(pk=self._selected_values[1])
             self.assertEqual(preserved_after.userdetail_set.count(), 2)
             self.assertFalse(User.objects.filter(pk=removed.pk).exists())
 
     def test_merge_delete_detail(self):
         from adminactions.merge import MergeForm
 
-        with user_grant_permission(self.user, ['auth.change_user', 'auth.adminactions_merge_user']):
+        with user_grant_permission(
+            self.user, ["auth.change_user", "auth.adminactions_merge_user"]
+        ):
             # removed = User.objects.get(pk=self._selected_rows[0])
             # preserved = User.objects.get(pk=self._selected_rows[1])
 
-            res = self.app.get('/', user='user')
-            res = res.click('Users')
-            form = res.forms['changelist-form']
-            form['action'] = 'merge'
+            res = self.app.get("/", user="user")
+            res = res.click("Users")
+            form = res.forms["changelist-form"]
+            form["action"] = "merge"
             self._select_rows(form, [1, 2])
             res = form.submit()
             removed = User.objects.get(pk=self._selected_values[0])
             preserved = User.objects.get(pk=self._selected_values[1])
 
-            removed.userdetail_set.create(note='1')
-            preserved.userdetail_set.create(note='2')
+            removed.userdetail_set.create(note="1")
+            preserved.userdetail_set.create(note="2")
 
             # steps = 2:
-            res.form['master_pk'] = self._selected_values[1]
-            res.form['other_pk'] = self._selected_values[0]
+            res.forms["merge-form"]["master_pk"] = self._selected_values[1]
+            res.forms["merge-form"]["other_pk"] = self._selected_values[0]
 
-            res.form['username'] = res.form['form-0-username'].value
-            res.form['email'] = res.form['form-0-email'].value
-            res.form['last_login'] = res.form['form-1-last_login'].value
-            res.form['date_joined'] = res.form['form-1-date_joined'].value
-            res.form['dependencies'] = MergeForm.DEP_DELETE
-            res = res.form.submit('preview')
+            res.forms["merge-form"]["username"] = res.forms["merge-form"][
+                "form-0-username"
+            ].value
+            res.forms["merge-form"]["email"] = res.forms["merge-form"][
+                "form-0-email"
+            ].value
+            res.forms["merge-form"]["last_login"] = res.forms["merge-form"][
+                "form-1-last_login"
+            ].value
+            res.forms["merge-form"]["date_joined"] = res.forms["merge-form"][
+                "form-1-date_joined"
+            ].value
+            res.forms["merge-form"]["dependencies"] = MergeForm.DEP_DELETE
+            res = res.forms["merge-form"].submit("preview")
             # steps = 3:
-            res = res.form.submit('apply')
+            res = res.forms["merge-form"].submit("apply")
 
             preserved_after = User.objects.get(pk=self._selected_values[1])
             self.assertEqual(preserved_after.userdetail_set.count(), 1)
             self.assertFalse(User.objects.filter(pk=removed.pk).exists())
 
 
 class TestMergeImageAction(SelectRowsMixin, WebTestMixin, TestCase):
     csrf_checks = True
-    fixtures = ['adminactions.json', 'demoproject.json']
-    urls = 'demo.urls'
+    fixtures = ["adminactions.json", "demoproject.json"]
+    urls = "demo.urls"
     sender_model = User
-    action_name = 'merge'
+    action_name = "merge"
     _selected_rows = [0, 2]
 
     def setUp(self):
         super().setUp()
-        self.url = reverse('admin:demo_demomodel_changelist')
-        self.user = G(User, username='user', is_staff=True, is_active=True)
+        self.url = reverse("admin:demo_demomodel_changelist")
+        self.user = G(User, username="user", is_staff=True, is_active=True)
 
     def _run_action(self, steps=3, page_start=None):
-        with user_grant_permission(self.user,
-                                   ['demo.change_demomodel',
-                                    'demo.adminactions_merge_demomodel']):
+        with user_grant_permission(
+            self.user, ["demo.change_demomodel", "demo.adminactions_merge_demomodel"]
+        ):
             if isinstance(steps, int):
                 steps = list(range(1, steps + 1))
-                res = self.app.get('/', user='user')
-                res = res.click('Demo models')
+                res = self.app.get("/", user="user")
+                res = res.click("Demo models")
             else:
                 res = page_start
 
             if 1 in steps:
-                form = res.forms['changelist-form']
-                form['action'] = 'merge'
+                form = res.forms["changelist-form"]
+                form["action"] = "merge"
                 self._select_rows(form)
                 res = form.submit()
-                assert not hasattr(res.form, 'errors')
+                assert not hasattr(res.forms["merge-form"], "errors")
 
             if 2 in steps:
-                res.form['image'] = res.form['form-1-image'].value
-                res.form['field_names'] = 'image,subclassed_image'
-                res = res.form.submit('preview')
-                assert not hasattr(res.form, 'errors')
+                res.forms["merge-form"]["image"] = res.forms["merge-form"][
+                    "form-1-image"
+                ].value
+                res.forms["merge-form"]["field_names"] = "image,subclassed_image"
+                res = res.forms["merge-form"].submit("preview")
+                assert not hasattr(res.forms["merge-form"], "errors")
 
             if 3 in steps:
-                res = res.form.submit('apply')
+                res = res.forms["merge-form"].submit("apply")
             return res
 
+    # noinspection PyTypeChecker
     def test_success(self):
         res = self._run_action(1)
         preserved = DemoModel.objects.get(pk=self._selected_values[0])
         removed = DemoModel.objects.get(pk=self._selected_values[1])
 
         img1 = removed.image
         img2 = removed.subclassed_image
```

### Comparing `django-adminactions-2.0.0/tests/test_permissions.py` & `django-adminactions-2.1.0/tests/test_permissions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 import logging
+
 import pytest
 from django.contrib.auth.models import Permission
 from django.urls import reverse
 from utils import user_grant_permission
 
 logger = logging.getLogger(__name__)
 
 
-@pytest.mark.parametrize("action", ['export_as_csv', 'export_as_xls', 'merge',
-                                    'export_as_fixture', 'export_delete_tree',
-                                    'graph_queryset', 'mass_update'])
+@pytest.mark.parametrize(
+    "action",
+    [
+        "export_as_csv",
+        "export_as_xls",
+        "merge",
+        "export_as_fixture",
+        "export_delete_tree",
+        "graph_queryset",
+        "mass_update",
+    ],
+)
 @pytest.mark.django_db()
 def test_permission_needed(app, admin, demomodels, action):
-    permission_mapping = {'export_as_csv': 'adminactions_export',
-                          'export_as_fixture': 'adminactions_export',
-                          'export_as_xls': 'adminactions_export',
-                          'export_delete_tree': 'adminactions_export',
-                          'mass_update': 'adminactions_massupdate',
-                          'merge': 'adminactions_merge',
-                          'graph_queryset': 'adminactions_chart',
-                          }
+    permission_mapping = {
+        "export_as_csv": "adminactions_export",
+        "export_as_fixture": "adminactions_export",
+        "export_as_xls": "adminactions_export",
+        "export_delete_tree": "adminactions_export",
+        "mass_update": "adminactions_massupdate",
+        "merge": "adminactions_merge",
+        "graph_queryset": "adminactions_chart",
+    }
     perm = "demo.{}_demomodel".format(permission_mapping[action])
-    url = reverse('admin:demo_demomodel_changelist')
+    url = reverse("admin:demo_demomodel_changelist")
     pks = [demomodels[0].pk, demomodels[1].pk]
-    with user_grant_permission(admin, ['demo.change_demomodel']):
-        res = app.post(url, params=[('action', action),
-                             ('_selected_action', pks)],
-                       extra_environ={'wsgi.url_scheme': 'https'},
-                       user=admin.username,
-                       expect_errors=True)
+    with user_grant_permission(admin, ["demo.change_demomodel"]):
+        res = app.post(
+            url,
+            params=[("action", action), ("_selected_action", pks)],
+            extra_environ={"wsgi.url_scheme": "https"},
+            user=admin.username,
+            expect_errors=True,
+        )
         assert res.status_code == 302
         res = res.follow()
-        assert 'Sorry you do not have rights to execute this action' in [str(m) for m in res.context['messages']]
+        assert "Sorry you do not have rights to execute this action" in [
+            str(m) for m in res.context["messages"]
+        ]
 
         with user_grant_permission(admin, [perm]):
-            res = app.post(url, params=[('action', action),
-                                 ('_selected_action', pks)],
-                           extra_environ={'wsgi.url_scheme': 'https'},
-                           user=admin.username,
-                           expect_errors=True)
+            res = app.post(
+                url,
+                params=[("action", action), ("_selected_action", pks)],
+                extra_environ={"wsgi.url_scheme": "https"},
+                user=admin.username,
+                expect_errors=True,
+            )
             assert res.status_code == 200
 
 
 @pytest.mark.django_db()
 def test_permissions(admin):
-    assert Permission.objects.filter(codename__startswith='adminactions').count() == 54
+    assert Permission.objects.filter(codename__startswith="adminactions").count() == 63
 
-    with user_grant_permission(admin, ['demo.adminactions_export_demomodel']):
-        assert admin.get_all_permissions() == set([u'demo.adminactions_export_demomodel'])
+    with user_grant_permission(admin, ["demo.adminactions_export_demomodel"]):
+        assert admin.get_all_permissions() == set(
+            ["demo.adminactions_export_demomodel"]
+        )
```

### Comparing `django-adminactions-2.0.0/tests/test_transaction.py` & `django-adminactions-2.1.0/tests/test_transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 
 pytestmarker = pytest.mark.skip
 
 
 @pytest.mark.django_db()
 def test_nocommit():
     with compat.nocommit():
-        G(Group, name='name')
-    assert not Group.objects.filter(name='name').exists()
+        G(Group, name="name")
+    assert not Group.objects.filter(name="name").exists()
 
 
 @pytest.mark.django_db()
 def test_transaction_merge(users):
     master, other = users
     with atomic():
-
-        with mock.patch('django.contrib.auth.models.User.delete', side_effect=IntegrityError):
+        with mock.patch(
+            "django.contrib.auth.models.User.delete", side_effect=IntegrityError
+        ):
             with pytest.raises(IntegrityError):
                 merge(master, other, commit=True)
 
         assert User.objects.filter(pk=master.pk).exists()
         assert User.objects.filter(pk=other.pk).exists()
 
         assert master.first_name != other.first_name
@@ -40,33 +41,33 @@
 def test_transaction_mass_update(app, users, administrator):
     assert User.objects.filter(is_staff=True).count() == 1  # sanity check
 
     def _handler(*args, **kwargs):
         raise ActionInterrupted()
 
     with atomic():
-        res = app.get('/admin/', user=administrator.username)
-        res = res.click('Users')
-        form = res.forms['changelist-form']
-        form['action'] = 'mass_update'
-
-        form.get('_selected_action', index=0).checked = True
-        form.get('_selected_action', index=1).checked = True
-        form.get('_selected_action', index=2).checked = True
+        res = app.get("/admin/", user=administrator.username)
+        res = res.click("Users")
+        form = res.forms["changelist-form"]
+        form["action"] = "mass_update"
+
+        form.get("_selected_action", index=0).checked = True
+        form.get("_selected_action", index=1).checked = True
+        form.get("_selected_action", index=2).checked = True
 
         res = form.submit()
-        res.form['chk_id_is_staff'].checked = True
-        res.form['is_staff'].checked = True
+        res.forms["mass-update-form"]["chk_id_is_staff"].checked = True
+        res.forms["mass-update-form"]["is_staff"].checked = True
 
         # res.form.submit('apply').follow()
         # assert User.objects.filter(is_staff=True).count() == 1
 
         with pytest.raises(BaseException):
             adminaction_end.connect(_handler)
-            res.form.submit('apply').follow()
+            res.forms["mass-update-form"].submit("apply").follow()
             assert res.status_code == 302
             adminaction_end.disconnect(_handler)
 
         assert User.objects.filter(is_staff=True).count() == 1
 
 
 class TestIsLibero(TransactionTestCase):
```

### Comparing `django-adminactions-2.0.0/tests/test_utils.py` & `django-adminactions-2.1.0/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,46 @@
 
 
 def test_get_verbose_name():
     from django.contrib.auth.models import Permission, User
 
     user = User()
     p = Permission()
-    assert get_verbose_name(user, 'username') == 'username'
+    assert get_verbose_name(user, "username") == "username"
 
-    assert get_verbose_name(User, 'username') == 'username'
+    assert get_verbose_name(User, "username") == "username"
 
-    assert get_verbose_name(User.objects.all(), 'username') == 'username'
+    assert get_verbose_name(User.objects.all(), "username") == "username"
 
-    assert get_verbose_name(User.objects, 'username') == 'username'
+    assert get_verbose_name(User.objects, "username") == "username"
 
-    assert get_verbose_name(User.objects, get_field_by_name(user, 'username')[0]) == 'username'
+    assert (
+        get_verbose_name(User.objects, get_field_by_name(user, "username")[0])
+        == "username"
+    )
 
-    assert get_verbose_name(p, 'content_type.model') == 'python model class name'
+    assert get_verbose_name(p, "content_type.model") == "python model class name"
 
     with pytest.raises(ValueError):
-        get_verbose_name(object, 'aaa')
+        get_verbose_name(object, "aaa")
 
     with pytest.raises(ValueError):
         get_verbose_name(p, None)
 
 
 def test_flatten():
     from adminactions.utils import flatten
 
-    assert flatten([[[1, 2, 3], (42, None)], [4, 5], [6], 7, (8, 9, 10)]) == [1, 2, 3, 42, None, 4, 5, 6, 7, 8, 9, 10]
+    assert flatten([[[1, 2, 3], (42, None)], [4, 5], [6], 7, (8, 9, 10)]) == [
+        1,
+        2,
+        3,
+        42,
+        None,
+        4,
+        5,
+        6,
+        7,
+        8,
+        9,
+        10,
+    ]
```

### Comparing `django-adminactions-2.0.0/tests/test_views.py` & `django-adminactions-2.1.0/tests/test_views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import datetime
+
 import pytest
 from django.urls import reverse
 from django.utils import dateformat
 from django.utils.encoding import smart_str
 
 
 @pytest.mark.django_db()
 def test_format_date(app):
     d = datetime.datetime.now()
 
-    url = reverse('adminactions.format_date')
-    fmt = 'd-m-Y'
+    url = reverse("adminactions.format_date")
+    fmt = "d-m-Y"
     res = app.get("{}?fmt={}".format(url, fmt))
     assert smart_str(res.body) == dateformat.format(d, fmt)
 
-    fmt = 'd mm Y'
+    fmt = "d mm Y"
     res = app.get("{}?fmt={}".format(url, fmt))
     assert smart_str(res.body) == dateformat.format(d, fmt)
```

### Comparing `django-adminactions-2.0.0/tests/utils.py` & `django-adminactions-2.1.0/tests/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import os
 import string
+from random import choice, randrange, shuffle
+
 from django.conf import global_settings
 from django.contrib import admin
 from django.contrib.admin.sites import AlreadyRegistered
 from django.contrib.auth import authenticate
 from django.contrib.auth.models import Group, Permission, User
 from django.contrib.contenttypes.models import ContentType
 from django.test.testcases import TestCase
 from django_dynamic_fixture import G
-from django_dynamic_fixture.fixture_algorithms.random_fixture import \
-    RandomDataFixture
-from random import choice, randrange, shuffle
+from django_dynamic_fixture.fixture_algorithms.random_fixture import RandomDataFixture
 
 from adminactions.exceptions import ActionInterrupted
-from adminactions.signals import (adminaction_end, adminaction_requested,
-                                  adminaction_start,)
+from adminactions.signals import (
+    adminaction_end,
+    adminaction_requested,
+    adminaction_start,
+)
 
 
 class admin_register:
     def __init__(self, model, model_admin=None, unregister=False):
         self.model = model
         self.model_admin = model_admin
         self.unregister = unregister
@@ -42,52 +45,52 @@
 
     def stop(self):
         """Stop an active patch."""
         return self.__exit__()
 
 
 def text(length, choices=string.ascii_letters):
-    """ returns a random (fixed length) string
+    """returns a random (fixed length) string
 
     :param length: string length
     :param choices: string containing all the chars can be used to build the string
 
     .. seealso::
        :py:func:`rtext`
     """
-    return ''.join(choice(choices) for x in range(length))
+    return "".join(choice(choices) for x in range(length))
 
 
 def get_group(name=None, permissions=None):
     group = G(Group, name=(name or text(5)))
     permission_names = permissions or []
     for permission_name in permission_names:
         try:
-            app_label, codename = permission_name.split('.')
+            app_label, codename = permission_name.split(".")
         except ValueError:
             raise ValueError("Invalid permission name `{0}`".format(permission_name))
-        __, model_name = codename.rsplit('_', 1)
-        ct = ContentType.objects.get(app_label__iexact=app_label,
-                                     model__iexact=model_name)
-        permission = Permission.objects.get(content_type=ct,
-                                            codename=codename)
+        __, model_name = codename.rsplit("_", 1)
+        ct = ContentType.objects.get(
+            app_label__iexact=app_label, model__iexact=model_name
+        )
+        permission = Permission.objects.get(content_type=ct, codename=codename)
         group.permissions.add(permission)
     return group
 
 
 class user_grant_permission:
     def __init__(self, user, permissions=None):
         self.user = user
         self.permissions = permissions
         self.group = None
 
     def __enter__(self):
-        if hasattr(self.user, '_group_perm_cache'):
+        if hasattr(self.user, "_group_perm_cache"):
             del self.user._group_perm_cache
-        if hasattr(self.user, '_perm_cache'):
+        if hasattr(self.user, "_perm_cache"):
             del self.user._perm_cache
         self.group = get_group(permissions=self.permissions or [])
         self.user.groups.add(self.group)
 
     def __exit__(self, *exc_info):
         if self.group:
             self.user.groups.remove(self.group)
@@ -110,100 +113,110 @@
 
     def _select_rows(self, form, selected_rows=None):
         if selected_rows is None:
             selected_rows = self._selected_rows
 
         self._selected_values = []
         for r in selected_rows:
-            chk = form.get('_selected_action', r, default=None)
+            chk = form.get("_selected_action", r, default=None)
             if chk:
-                form.set('_selected_action', True, r)
+                form.set("_selected_action", True, r)
                 self._selected_values.append(int(chk.value))
 
 
 class CheckSignalsMixin:
-    MESSAGE = 'Action Interrupted Test'
+    MESSAGE = "Action Interrupted Test"
 
     def test_signal_sent(self):
         def handler_factory(name):
             def myhandler(sender, action, request, queryset, **kwargs):
                 handler_factory.invoked[name] = True
                 self.assertEqual(action, self.action_name)
-                self.assertSequenceEqual(queryset.order_by('id').values_list('id', flat=True),
-                                         sorted(self._selected_values))
+                self.assertSequenceEqual(
+                    queryset.order_by("id").values_list("id", flat=True),
+                    sorted(self._selected_values),
+                )
 
             return myhandler
 
         handler_factory.invoked = {}
 
         try:
-            m1 = handler_factory('adminaction_requested')
+            m1 = handler_factory("adminaction_requested")
             adminaction_requested.connect(m1, sender=self.sender_model)
 
-            m2 = handler_factory('adminaction_start')
+            m2 = handler_factory("adminaction_start")
             adminaction_start.connect(m2, sender=self.sender_model)
 
-            m3 = handler_factory('adminaction_end')
+            m3 = handler_factory("adminaction_end")
             adminaction_end.connect(m3, sender=self.sender_model)
 
             self._run_action()
-            self.assertIn('adminaction_requested', handler_factory.invoked)
-            self.assertIn('adminaction_start', handler_factory.invoked)
-            self.assertIn('adminaction_end', handler_factory.invoked)
+            self.assertIn("adminaction_requested", handler_factory.invoked)
+            self.assertIn("adminaction_start", handler_factory.invoked)
+            self.assertIn("adminaction_end", handler_factory.invoked)
 
         finally:
             adminaction_requested.disconnect(m1, sender=self.sender_model)
             adminaction_start.disconnect(m2, sender=self.sender_model)
             adminaction_end.disconnect(m3, sender=self.sender_model)
 
     def test_signal_requested(self):
         # test if adminaction_requested Signal can stop the action
 
         def myhandler(sender, action, request, queryset, **kwargs):
             myhandler.invoked = True
             self.assertEqual(action, self.action_name)
-            self.assertSequenceEqual(queryset.order_by('id').values_list('id', flat=True),
-                                     sorted(self._selected_values))
+            self.assertSequenceEqual(
+                queryset.order_by("id").values_list("id", flat=True),
+                sorted(self._selected_values),
+            )
             raise ActionInterrupted(self.MESSAGE)
+
         myhandler.invoked = False
 
         try:
             adminaction_requested.connect(myhandler, sender=self.sender_model)
             self._run_action(1)
             self.assertTrue(myhandler.invoked)
-            self.assertIn(self.MESSAGE, self.app.cookies['messages'])
+            self.assertIn(self.MESSAGE, self.app.cookies["messages"])
         finally:
             adminaction_requested.disconnect(myhandler, sender=self.sender_model)
 
     def test_signal_start(self):
         # test if adminaction_start Signal can stop the action
 
         def myhandler(sender, action, request, queryset, **kwargs):
             myhandler.invoked = True
             self.assertEqual(action, self.action_name)
-            self.assertSequenceEqual(queryset.order_by('id').values_list('id', flat=True),
-                                     sorted(self._selected_values))
+            self.assertSequenceEqual(
+                queryset.order_by("id").values_list("id", flat=True),
+                sorted(self._selected_values),
+            )
             raise ActionInterrupted(self.MESSAGE)
 
         try:
             adminaction_start.connect(myhandler, sender=self.sender_model)
             self._run_action(2)
             self.assertTrue(myhandler.invoked)
-            self.assertIn(self.MESSAGE, self.app.cookies['messages'])
+            self.assertIn(self.MESSAGE, self.app.cookies["messages"])
         finally:
             adminaction_start.disconnect(myhandler, sender=self.sender_model)
 
     def test_signal_end(self):
         # test if adminaction_start Signal can stop the action
 
         def myhandler(sender, action, request, queryset, **kwargs):
             myhandler.invoked = True
             self.assertEqual(action, self.action_name)
-            self.assertSequenceEqual(queryset.order_by('id').values_list('id', flat=True),
-                                     sorted(self._selected_values))
+            self.assertSequenceEqual(
+                queryset.order_by("id").values_list("id", flat=True),
+                sorted(self._selected_values),
+            )
+
         myhandler.invoked = False
         try:
             adminaction_end.connect(myhandler, sender=self.sender_model)
             self._run_action(2)
             self.assertTrue(myhandler.invoked)
         finally:
             adminaction_end.disconnect(myhandler, sender=self.sender_model)
@@ -217,80 +230,101 @@
     """
     not_valid_class_A = not_valid or []
 
     class_a = [r for r in range(1, 256) if r not in not_valid_class_A]
     shuffle(class_a)
     first = class_a.pop()
 
-    return ".".join([str(first), str(randrange(1, 256)),
-                     str(randrange(1, 256)), str(randrange(1, 256))])
+    return ".".join(
+        [
+            str(first),
+            str(randrange(1, 256)),
+            str(randrange(1, 256)),
+            str(randrange(1, 256)),
+        ]
+    )
 
 
-class DataFixtureClass(RandomDataFixture):  # it can inherit of SequentialDataFixture, RandomDataFixture etc.
-    def genericipaddressfield_config(self, field, key):  # method name must have the format: FIELDNAME_config
+class DataFixtureClass(
+    RandomDataFixture
+):  # it can inherit of SequentialDataFixture, RandomDataFixture etc.
+    def genericipaddressfield_config(
+        self, field, key
+    ):  # method name must have the format: FIELDNAME_config
         return ipaddress()
 
 
-TEST_TEMPLATES_DIR = os.path.join(os.path.dirname(__file__),
-                                  os.pardir, 'tests', 'templates')
-
-SETTINGS = {'TEMPLATE_DIRS': [TEST_TEMPLATES_DIR],
-            'AUTHENTICATION_BACKENDS': ('django.contrib.auth.backends.ModelBackend',),
-            'TEMPLATE_LOADERS': ('django.template.loaders.filesystem.Loader',
-                                 'django.template.loaders.app_directories.Loader'),
-            # 'AUTH_PROFILE_MODULE': None,
-            'TEMPLATE_CONTEXT_PROCESSORS': ("django.contrib.auth.context_processors.auth",
-                                            "django.core.context_processors.debug",
-                                            "django.core.context_processors.i18n",
-                                            "django.core.context_processors.media",
-                                            "django.core.context_processors.static",
-                                            "django.core.context_processors.request",
-                                            "django.core.context_processors.tz",
-                                            "django.contrib.messages.context_processors.messages")}
-
-SETTINGS['MIDDLEWARE'] = global_settings.MIDDLEWARE
-
-ADMIN = 'sax'
-USER = 'user'
-PWD = '123'
-USER_EMAIL = 'user@moreply.org'
+TEST_TEMPLATES_DIR = os.path.join(
+    os.path.dirname(__file__), os.pardir, "tests", "templates"
+)
+
+SETTINGS = {
+    "TEMPLATE_DIRS": [TEST_TEMPLATES_DIR],
+    "AUTHENTICATION_BACKENDS": ("django.contrib.auth.backends.ModelBackend",),
+    "TEMPLATE_LOADERS": (
+        "django.template.loaders.filesystem.Loader",
+        "django.template.loaders.app_directories.Loader",
+    ),
+    # 'AUTH_PROFILE_MODULE': None,
+    "TEMPLATE_CONTEXT_PROCESSORS": (
+        "django.contrib.auth.context_processors.auth",
+        "django.core.context_processors.debug",
+        "django.core.context_processors.i18n",
+        "django.core.context_processors.media",
+        "django.core.context_processors.static",
+        "django.core.context_processors.request",
+        "django.core.context_processors.tz",
+        "django.contrib.messages.context_processors.messages",
+    ),
+}
+
+SETTINGS["MIDDLEWARE"] = global_settings.MIDDLEWARE
+
+ADMIN = "sax"
+USER = "user"
+PWD = "123"
+USER_EMAIL = "user@moreply.org"
 
 
 class BaseTestCaseMixin:
-    fixtures = ['adminactions.json', ]
+    fixtures = [
+        "adminactions.json",
+    ]
 
     def setUp(self):
         super().setUp()
         self.sett = self.settings(**SETTINGS)
         self.sett.enable()
         self.login()
 
     def tearDown(self):
         self.sett.disable()
 
-    def login(self, username='user_00', password='123'):
+    def login(self, username="user_00", password="123"):
         user = User.objects.get(username=username)
         try:
             self.client.force_login(user)
         except AttributeError:  # for Django<1.8
             logged = self.client.login(username=username, password=password)
-            assert logged, 'Unable login with credentials'
+            assert logged, "Unable login with credentials"
         self._user = authenticate(username=username, password=password)
 
     def add_permission(self, *perms, **kwargs):
-        """ add the right permission to the user """
-        target = kwargs.pop('user', self._user)
-        if hasattr(target, '_perm_cache'):
+        """add the right permission to the user"""
+        target = kwargs.pop("user", self._user)
+        if hasattr(target, "_perm_cache"):
             del target._perm_cache
         for perm_name in perms:
-            app_label, code = perm_name.split('.')
-            if code == '*':
+            app_label, code = perm_name.split(".")
+            if code == "*":
                 perms = Permission.objects.filter(content_type__app_label=app_label)
             else:
-                perms = Permission.objects.filter(codename=code, content_type__app_label=app_label)
+                perms = Permission.objects.filter(
+                    codename=code, content_type__app_label=app_label
+                )
             target.user_permissions.add(*perms)
 
         target.save()
 
 
 class BaseTestCase(BaseTestCaseMixin, TestCase):
     pass
```

### Comparing `django-adminactions-2.0.0/tox.ini` & `django-adminactions-2.1.0/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tox]
 # as per https://docs.djangoproject.com/en/1.11/faq/install/#what-python-version-can-i-use-with-django
-envlist = d{32,40}-py{38,39,310}
-
-skip_missing_interpreters = true
-
+envlist = d{32,41}-py{39,310,311}
+;
+;skip_missing_interpreters = true
+;
 [pytest]
 python_paths=./src ./tests
 DJANGO_SETTINGS_MODULE=demo.settings
 norecursedirs = demo .tox
 addopts =
         -v
         --doctest-modules
@@ -24,41 +24,51 @@
 python_files=tests/test_*.py tests/**/test_*.py
 markers =
     functional: mark a test as functional
     selenium: selenium test
     skip: skip test
 
 [testenv]
-passenv = TRAVIS TRAVIS_JOB_ID TRAVIS_BRANCH PYTHONDONTWRITEBYTECODE DISPLAY CELERY_BROKER_URL
+passenv =
+    DISPLAY
+    CELERY_BROKER_URL
+
 setenv =
     PYTHONDONTWRITEBYTECODE=true
     CRYPTOGRAPHY_DONT_BUILD_RUST=1
-    PYTHONPATH=
+    PYTHONPATH=./src:./tests
     CELERY_ALWAYS_EAGER=1
 
 whitelist_externals = mkdir
 
 deps=
     -rsrc/requirements/testing.pip
     pypy: psycopg2cffi
     d22: django==2.2.*
     d32: django==3.2.*
     d40: django==4.0.*
+    d41: django==4.1.*
 
     ; only for local development
     dev: git+https://github.com/django/django.git
 
 
 commands=
     {posargs:py.test tests/ src --doctest-modules --create-db}
 
 [testenv:lint]
 envdir={toxworkdir}/d32-py39/
 skip_install = true
+deps=
+    black
+    flake8
+    isort
+
 commands =
+    black --check ./src ./tests
     flake8 src tests
     isort src tests --check
 
 [testenv:package]
 deps=
     build
     twine
@@ -66,9 +76,10 @@
 setenv =
     TWINE_USERNAME = {env:TWINE_TEST_USERNAME:__token__}
     TWINE_PASSWORD = {env:TWINE_TEST_PASSWORD}
 
 commands =
     python -c "import shutil; shutil.rmtree('dist', ignore_errors=True)"
     python -m build
+    python -m twine check dist/*
     python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

### Comparing `django-adminactions-2.0.0/~setup.py` & `django-adminactions-2.1.0/~setup.py`

 * *Files identical despite different names*


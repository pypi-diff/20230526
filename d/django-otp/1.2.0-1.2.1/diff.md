# Comparing `tmp/django_otp-1.2.0.tar.gz` & `tmp/django_otp-1.2.1.tar.gz`

## Comparing `django_otp-1.2.0.tar` & `django_otp-1.2.1.tar`

### file list

```diff
@@ -1,97 +1,99 @@
--rw-r--r--   0        0        0    15815 2020-02-02 00:00:00.000000 django_otp-1.2.0/CHANGES.rst
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 django_otp-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/ext/otpdocs.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/.spell.utf-8.add
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/auth.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/changes.rst
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/contributing.rst
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/extend.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 django_otp-1.2.0/docs/source/overview.rst
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/__init__.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/admin.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/conf.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/decorators.py
--rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/forms.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/middleware.py
--rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/models.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/oath.py
--rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/tests.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/util.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/views.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/admin.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/apps.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/conf.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/models.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/tests.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/__init__.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/admin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/apps.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/models.py
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/tests.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/__init__.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/admin.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/apps.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/lib.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/models.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/management/commands/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/__init__.py
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/admin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/apps.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/models.py
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/tests.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 django_otp-1.2.0/src/django_otp/templates/otp/admin111/login.html
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/config/github.toml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/config/sample.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/backends.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/config.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/settings.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/urls.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/views.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/about.html
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/home.html
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/navbar.html
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/root.html
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/bs5/input.html
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/bs5/select.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/otp/email/custom.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/otp/email/token.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 django_otp-1.2.0/test/test_project/templates/registration/login.html
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 django_otp-1.2.0/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp-1.2.0/.hgignore
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp-1.2.0/LICENSE
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 django_otp-1.2.0/README.rst
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 django_otp-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 django_otp-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    16071 2020-02-02 00:00:00.000000 django_otp-1.2.1/CHANGES.rst
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 django_otp-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/ext/otpdocs.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/.spell.utf-8.add
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/auth.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/changes.rst
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/contributing.rst
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/extend.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 django_otp-1.2.1/docs/source/overview.rst
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/admin.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/conf.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/decorators.py
+-rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/forms.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/middleware.py
+-rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/models.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/oath.py
+-rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/tests.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/util.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/views.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/admin.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/apps.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/conf.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/models.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/tests.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/0001_initial.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/__init__.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/apps.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/models.py
+-rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/tests.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/admin.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/apps.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/lib.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/models.py
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/management/commands/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/migrations/0001_initial.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_static/migrations/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/__init__.py
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/apps.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/models.py
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/tests.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 django_otp-1.2.1/src/django_otp/templates/otp/admin111/login.html
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/config/github.toml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/config/sample.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/backends.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/config.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/settings.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/urls.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/views.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/about.html
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/home.html
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/navbar.html
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/root.html
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/bs5/input.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/bs5/select.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/otp/email/custom.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/otp/email/token.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 django_otp-1.2.1/test/test_project/templates/registration/login.html
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 django_otp-1.2.1/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp-1.2.1/.hgignore
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp-1.2.1/LICENSE
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 django_otp-1.2.1/README.rst
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 django_otp-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 django_otp-1.2.1/PKG-INFO
```

### Comparing `django_otp-1.2.0/CHANGES.rst` & `django_otp-1.2.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,25 @@
+v1.2.1 - May 26, 2023 - pt-BR translations
+--------------------------------------------------------------------------------
+
+- `#124`_: Add pt-BR translations.
+
+.. _#124: https://github.com/django-otp/django-otp/pull/124
+
+
 v1.2.0 - May 11, 2023 - Tooling, TOTP images
 --------------------------------------------------------------------------------
 
 - This project is now managed with `hatch`_, which replaces setuptools, pipenv,
   and tox. Users of the package should not be impacted. Developers can refer to
   the readme for details. If you're packaging this project from source, I
   suggest relying on pip's isolated builds rather than using hatch directly.
 
 - `#123`_: Add support for passing an image parameter in the otpauth URL.
+  See :setting:`OTP_TOTP_IMAGE`.
 
 
 .. _hatch: https://hatch.pypa.io/
 .. _#123: https://github.com/django-otp/django-otp/pull/123
 
 
 v1.1.6 - March 07, 2023 - German translation
```

### Comparing `django_otp-1.2.0/CONTRIBUTING.rst` & `django_otp-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/docs/Makefile` & `django_otp-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/docs/source/.spell.utf-8.add` & `django_otp-1.2.1/docs/source/.spell.utf-8.add`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/docs/source/auth.rst` & `django_otp-1.2.1/docs/source/auth.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/docs/source/conf.py` & `django_otp-1.2.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 #  copyright = ''
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '1.2.0'
+release = '1.2.1'
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `django_otp-1.2.0/docs/source/extend.rst` & `django_otp-1.2.1/docs/source/extend.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/docs/source/overview.rst` & `django_otp-1.2.1/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/__init__.py` & `django_otp-1.2.1/src/django_otp/__init__.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/admin.py` & `django_otp-1.2.1/src/django_otp/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/conf.py` & `django_otp-1.2.1/src/django_otp/conf.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/decorators.py` & `django_otp-1.2.1/src/django_otp/decorators.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/forms.py` & `django_otp-1.2.1/src/django_otp/forms.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/middleware.py` & `django_otp-1.2.1/src/django_otp/middleware.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/models.py` & `django_otp-1.2.1/src/django_otp/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/oath.py` & `django_otp-1.2.1/src/django_otp/oath.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/tests.py` & `django_otp-1.2.1/src/django_otp/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/util.py` & `django_otp-1.2.1/src/django_otp/util.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/views.py` & `django_otp-1.2.1/src/django_otp/views.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.mo` & `django_otp-1.2.1/src/django_otp/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/locale/de/LC_MESSAGES/django.po` & `django_otp-1.2.1/src/django_otp/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.mo` & `django_otp-1.2.1/src/django_otp/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/locale/es/LC_MESSAGES/django.po` & `django_otp-1.2.1/src/django_otp/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo` & `django_otp-1.2.1/src/django_otp/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/locale/fr/LC_MESSAGES/django.po` & `django_otp-1.2.1/src/django_otp/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_email/admin.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_email/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_email/conf.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_email/conf.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_email/models.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_email/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_email/tests.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_email/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_email/migrations/0004_throttling.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/admin.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_hotp/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/models.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_hotp/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/tests.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_hotp/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html` & `django_otp-1.2.1/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_static/admin.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_static/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_static/lib.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_static/lib.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_static/models.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_static/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_static/tests.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_static/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_static/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_static/migrations/0002_throttling.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_totp/admin.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_totp/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_totp/models.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_totp/models.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_totp/tests.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_totp/tests.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_totp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.2.1/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html` & `django_otp-1.2.1/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/src/django_otp/templates/otp/admin111/login.html` & `django_otp-1.2.1/src/django_otp/templates/otp/admin111/login.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/config/sample.toml` & `django_otp-1.2.1/test/config/sample.toml`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/config.py` & `django_otp-1.2.1/test/test_project/config.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/settings.py` & `django_otp-1.2.1/test/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/urls.py` & `django_otp-1.2.1/test/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/views.py` & `django_otp-1.2.1/test/test_project/views.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/templates/about.html` & `django_otp-1.2.1/test/test_project/templates/about.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/templates/home.html` & `django_otp-1.2.1/test/test_project/templates/home.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/templates/navbar.html` & `django_otp-1.2.1/test/test_project/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/templates/root.html` & `django_otp-1.2.1/test/test_project/templates/root.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/test/test_project/templates/registration/login.html` & `django_otp-1.2.1/test/test_project/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/LICENSE` & `django_otp-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_otp-1.2.0/README.rst` & `django_otp-1.2.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 
 Status
 ------
 
 This project is stable and maintained, but is no longer actively used by the
 author and is not seeing much ongoing investment.
 
-Well-formed issues and pull requests are welcome, but please see CONTRIBUTING.md
-first. General questions and ideas should be directed to the Discussions
-section; issues should be reserved for confirmed bugs.
+Well-formed issues and pull requests are welcome, but please see
+CONTRIBUTING.rst first. General questions and ideas should be directed to the
+Discussions section; issues should be reserved for confirmed bugs.
 
 .. end-of-doc-intro
 
 
 Development
 -----------
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_qwgx33j4_/tmpdzbm2l98_TarContainer/0/94.rst", line 150, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_qwgx33j4_/tmpdzbm2l98_TarContainer/0/94.rst", line 150, column 0: CDATA terminal not found*

```diff
@@ -16,15 +16,15 @@
 tools.ietf.org/html/rfc4226>`_ and `TOTP
 tools.ietf.org/html/rfc6238>`_ for convenience, as these are standard OTP
 algorithms used by multiple plugins. If you're looking for a higher-level or
 more opinionated solution, you might be interested in `django-two-factor-auth
 github.com/Bouke/django-two-factor-auth>`_. Status ------ This project is
 stable and maintained, but is no longer actively used by the author and is not
 seeing much ongoing investment. Well-formed issues and pull requests are
-welcome, but please see CONTRIBUTING.md first. General questions and ideas
+welcome, but please see CONTRIBUTING.rst first. General questions and ideas
 should be directed to the Discussions section; issues should be reserved for
 confirmed bugs. .. end-of-doc-intro Development ----------- This project is
 built and managed with `hatch`_. If you don't have hatch, I recommend
 installing it with `pipx`_: ``pipx install hatch``. ``pyproject.toml`` defines
 several useful scripts for development and testing. The default environment
 includes all dev and test dependencies for quickly running tests. The ``test``
 environment defines the test matrix for running the full validation suite.
```

### Comparing `django_otp-1.2.0/pyproject.toml` & `django_otp-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-otp"
-version = "1.2.0"
+version = "1.2.1"
 description = "A pluggable framework for adding two-factor authentication to Django using one-time passwords."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = "Unlicense"
 authors = [
     { name = "Peter Sagerson", email = "psagers@ignorare.net" },
 ]
```

### Comparing `django_otp-1.2.0/PKG-INFO` & `django_otp-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-otp
-Version: 1.2.0
+Version: 1.2.1
 Summary: A pluggable framework for adding two-factor authentication to Django using one-time passwords.
 Project-URL: Homepage, https://github.com/django-otp/django-otp
 Project-URL: Documentation, https://django-otp-official.readthedocs.io/
 Author-email: Peter Sagerson <psagers@ignorare.net>
 License-Expression: Unlicense
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,17 +56,17 @@
 
 Status
 ------
 
 This project is stable and maintained, but is no longer actively used by the
 author and is not seeing much ongoing investment.
 
-Well-formed issues and pull requests are welcome, but please see CONTRIBUTING.md
-first. General questions and ideas should be directed to the Discussions
-section; issues should be reserved for confirmed bugs.
+Well-formed issues and pull requests are welcome, but please see
+CONTRIBUTING.rst first. General questions and ideas should be directed to the
+Discussions section; issues should be reserved for confirmed bugs.
 
 .. end-of-doc-intro
 
 
 Development
 -----------
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_qwgx33j4_/tmpdzbm2l98_TarContainer/0/96", line 173, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_qwgx33j4_/tmpdzbm2l98_TarContainer/0/96", line 173, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-otp Version: 1.2.0 Summary: A pluggable
+Metadata-Version: 2.1 Name: django-otp Version: 1.2.1 Summary: A pluggable
 framework for adding two-factor authentication to Django using one-time
 passwords. Project-URL: Homepage, https://github.com/django-otp/django-otp
 Project-URL: Documentation, https://django-otp-official.readthedocs.io/ Author-
 email: Peter Sagerson
 ignorare.net> License-Expression: Unlicense License-File: LICENSE Classifier:
 Development Status :: 5 - Production/Stable Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -29,15 +29,15 @@
 tools.ietf.org/html/rfc4226>`_ and `TOTP
 tools.ietf.org/html/rfc6238>`_ for convenience, as these are standard OTP
 algorithms used by multiple plugins. If you're looking for a higher-level or
 more opinionated solution, you might be interested in `django-two-factor-auth
 github.com/Bouke/django-two-factor-auth>`_. Status ------ This project is
 stable and maintained, but is no longer actively used by the author and is not
 seeing much ongoing investment. Well-formed issues and pull requests are
-welcome, but please see CONTRIBUTING.md first. General questions and ideas
+welcome, but please see CONTRIBUTING.rst first. General questions and ideas
 should be directed to the Discussions section; issues should be reserved for
 confirmed bugs. .. end-of-doc-intro Development ----------- This project is
 built and managed with `hatch`_. If you don't have hatch, I recommend
 installing it with `pipx`_: ``pipx install hatch``. ``pyproject.toml`` defines
 several useful scripts for development and testing. The default environment
 includes all dev and test dependencies for quickly running tests. The ``test``
 environment defines the test matrix for running the full validation suite.
```


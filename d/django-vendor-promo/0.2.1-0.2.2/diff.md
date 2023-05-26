# Comparing `tmp/django-vendor-promo-0.2.1.tar.gz` & `tmp/django-vendor-promo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-promo-0.2.1.tar", last modified: Wed May 24 17:29:24 2023, max compression
+gzip compressed data, was "django-vendor-promo-0.2.2.tar", last modified: Fri May 26 13:22:47 2023, max compression
```

## Comparing `django-vendor-promo-0.2.1.tar` & `django-vendor-promo-0.2.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.690613 django-vendor-promo-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/LICENSE.mit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-24 17:29:24.690613 django-vendor-promo-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:29:24.690613 django-vendor-promo-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.674613 django-vendor-promo-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.678613 django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-24 17:29:24.000000 django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-24 17:29:24.000000 django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:29:24.000000 django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-24 17:29:24.000000 django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 17:29:24.000000 django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.678613 django-vendor-promo-0.2.1/src/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.678613 django-vendor-promo-0.2.1/src/vendorpromo/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.682613 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.682613 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/vouchery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/vouchery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/vouchery/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/api/v1/vouchery/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.682613 django-vendor-promo-0.2.1/src/vendorpromo/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/migrations/0003_auto_20230524_1701.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.682613 django-vendor-promo-0.2.1/src/vendorpromo/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/processors/DummyProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/processors/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/processors/vouchery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.674613 django-vendor-promo-0.2.1/src/vendorpromo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.686613 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/affiliate_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.686613 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/processor_site_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promo_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promocode_formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/vouchery_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:29:24.690613 django-vendor-promo-0.2.1/src/vendorpromo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/test_affiliate.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/test_coupon_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/test_promo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/test_promotional_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/tests/test_stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-05-24 17:28:16.000000 django-vendor-promo-0.2.1/src/vendorpromo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.460409 django-vendor-promo-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/LICENSE.mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:22:47.460409 django-vendor-promo-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.440410 django-vendor-promo-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.444410 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 13:22:47.000000 django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.448410 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.452410 django-vendor-promo-0.2.2/src/vendorpromo/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/0003_auto_20230524_1701.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.452410 django-vendor-promo-0.2.2/src/vendorpromo/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/DummyProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/processors/vouchery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.440410 django-vendor-promo-0.2.2/src/vendorpromo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promocode_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:22:47.456410 django-vendor-promo-0.2.2/src/vendorpromo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_affiliate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_coupon_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promotional_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/tests/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-05-26 13:21:28.000000 django-vendor-promo-0.2.2/src/vendorpromo/views.py
```

### Comparing `django-vendor-promo-0.2.1/PKG-INFO` & `django-vendor-promo-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.1/pyproject.toml` & `django-vendor-promo-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "django-vendor-promo"
-version = "0.2.1"
+version = "0.2.2"
 
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
   { name="Roberto Himmelbauer" }
 ]
 description = "Extension to Django Vendor to add Promo Code capabilities"
 readme = "README.md"
```

### Comparing `django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/PKG-INFO` & `django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.1/src/django_vendor_promo.egg-info/SOURCES.txt` & `django-vendor-promo-0.2.2/src/django_vendor_promo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/admin.py` & `django-vendor-promo-0.2.2/src/vendorpromo/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/api/v1/urls.py` & `django-vendor-promo-0.2.2/src/vendorpromo/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/api/v1/views.py` & `django-vendor-promo-0.2.2/src/vendorpromo/api/v1/views.py`

 * *Files 19% similar despite different names*

```diff
@@ -117,14 +117,18 @@
         # csrf_token = get_token(request)
         # # csrf_token_html = '<input type="hidden" name="csrfmiddlewaretoken" value="{}" />'.format(csrf_token)
         # request.POST['csrf_token'] = csrf_token
         # self.kwargs['slug'] = promo.offer.slug
         # return super().post(request, args, kwargs)
 
 
+def does_coupon_apply_to_order_item(coupon_code, order_item_products):
+    return next((product for product in coupon_code.promo.applies_to.products.all() if product in order_item_products), False)
+
+
 class ValidateCouponCodeCheckoutProcessAPIView(LoginRequiredMixin, View):
     """
     When a customer is applying a code during the checkout process
     the function will check if the entered code is valid to the items
     in the cart. If valsid it will swap the Offer with the Offer that
     has that promo code. If not it will display an error message.
     In both cases it will redirect to the view that called the
@@ -140,29 +144,49 @@
         if invoice.order_items.filter(offer__is_promotional=True).exists():
             return JsonResponse({'error': "You can only apply one promo code per checkout session"}, status=404)
 
         processor = get_site_promo_processor(invoice.site)(invoice.site, invoice=invoice)
         if not processor.is_code_valid(coupon_code):
             return JsonResponse({'error': _("Invalid Code")}, status=404)
 
+        invoice_products = invoice.get_products()
+        if not next((product for product in coupon_code.promo.applies_to.products.all() if product in invoice_products), False):
+            return JsonResponse({'error': _("Code does not apply to any of the products in you cart")}, status=404)
+        
         coupon_code.invoice.add(invoice)
         invoice.add_offer(coupon_code.promo.applies_to)
-        if coupon_code.promo.is_percent_off:
-            # Calculate global_discount
-            invoice.global_discount = (invoice.subtotal * coupon_code.promo.applies_to.current_price()) / 100
-            invoice.update_totals()
-            invoice.save()
-            # TODO: Implement percent discount on specific or individual products by using MSRP
-            # if coupon_code.promo.applies_to.products.count():
-                # loop through offers in invoice to see if any match the product form the Promo.offer instance
-                # for order_item in invoice.order_items.all():
-                #     if order_item.offer.products in coupon_code.promo.applies_to.products():
-                #         invoice.global_discount = (order_item.offer.current_price() * coupon_code.promo.applies_to.current_price() / 100)  # Use the price.cost as a % value
-                #         invoice.global_discount -= coupon_code.promo.applies_to.current_price()  # Subtract the price.cost from the discount so it is not subtracted from the total
-                #         break
-            # else:  # If no applies_to.products are selecte we assume that the discount if on the total of the Invoice
-            #     invoice.global_discount = (invoice.subtotal * coupon_code.promo.applies_to.current_price()) / 100
-            #     invoice.update_totals()
-            #     invoice.save()
+
+        coupon_order_item = invoice.order_items.get(offer=coupon_code.promo.applies_to)
+        if coupon_code.promo.applies_to.products.count():  # Calculate discount independently 
+            invoice_order_items = invoice.order_items.all().exclude(offer=coupon_code.promo.applies_to)
+            
+            if coupon_code.promo.is_percent_off:
+                # Calculate global_discount
+                total_global_discount = 0
+                for order_item in invoice_order_items:
+                    order_item_products = list(order_item.offer.products.all())
+                    if does_coupon_apply_to_order_item(coupon_code, order_item_products):
+                        total_global_discount += (order_item.total * coupon_code.promo.applies_to.current_price()) / 100
+                
+                invoice.global_discount = total_global_discount - coupon_code.promo.applies_to.current_price()
+                invoice.update_totals()
+                invoice.save()
+
+            else:
+                coupon_count = 0
+                for order_item in invoice_order_items:
+                    order_item_products = list(order_item.offer.products.all())
+                    if does_coupon_apply_to_order_item(coupon_code, order_item_products):
+                        coupon_count += order_item.quantity
+
+                coupon_order_item.quantity = coupon_count
+                coupon_order_item.save()
+                invoice.update_totals()
+        else:
+            if coupon_code.promo.is_percent_off:
+                # Calculate global_discount
+                invoice.global_discount = (invoice.subtotal * coupon_code.promo.applies_to.current_price()) / 100
+                invoice.update_totals()
+                invoice.save()
                 
         messages.success(request, _("Promo Code Applied"))
         return HttpResponse(_("Promo Code Applied"))
```

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/api/v1/vouchery/views.py` & `django-vendor-promo-0.2.2/src/vendorpromo/api/v1/vouchery/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/config.py` & `django-vendor-promo-0.2.2/src/vendorpromo/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/forms.py` & `django-vendor-promo-0.2.2/src/vendorpromo/forms.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/integrations.py` & `django-vendor-promo-0.2.2/src/vendorpromo/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/migrations/0001_initial.py` & `django-vendor-promo-0.2.2/src/vendorpromo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py` & `django-vendor-promo-0.2.2/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/migrations/0003_auto_20230524_1701.py` & `django-vendor-promo-0.2.2/src/vendorpromo/migrations/0003_auto_20230524_1701.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/models.py` & `django-vendor-promo-0.2.2/src/vendorpromo/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import uuid
 
 from autoslug import AutoSlugField
-
 from django.contrib.sites.models import Site
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-
-from vendor.models import CustomerProfile, Offer, Invoice
+from vendor.models import CustomerProfile, Invoice, Offer
 
 
 #######################################
 # ABSTRACT MODELS
 class CreateUpdateModelBase(models.Model):
     '''
     This is a shared models base that provides created & updated timestamp fields
@@ -83,15 +81,15 @@
 
     def __str__(self):
         return self.name
     
     class Meta:
         verbose_name = "Promotional Campaign"
         verbose_name_plural = "Promotional Campaigns"
-
+    
 
 class CouponCode(CreateUpdateModelBase):
     uuid = models.UUIDField(default=uuid.uuid4, editable=False, unique=True)
     active = models.BooleanField(_("Active"), default=True)
     code = AutoSlugField(unique_with=('promo__site'), editable=True, blank=True, null=True, verbose_name=_("Affiliate Code"))
     max_redemptions = models.IntegerField(_("Max Redemptions"), blank=True, null=True)
     end_date = models.DateTimeField(_("End Date"), blank=True, null=True, help_text=_("When will the code be unavailable"))
@@ -152,39 +150,7 @@
         if self.email:
             return self.email
         
         if self.company:
             return self.company
         
         return self.uuid
-
-"""
-Stripe Structure
-{
-    "coupon": {
-        "amount_off": offer.current_price(),
-        "percent_off": offer.current_price(),
-        "currency": offer.currency(),
-        "duration": 'once' if offer.term_details['trial_occurrences'] <= 1 else 'repeating',
-        "duration_in_months": offer.term_details['trial_occurrences'],
-        "name": promo.campaign_name and offer.name,
-        "applies_to": promo.offer.products,
-        "max_redemptions": promo.max_redemptions,
-        "redeem_by": promo.end_date,
-        "promo": {
-            "code": PromoCode.code,
-            "metadata": {
-                "site": id,
-                "promo_id": promo.id,
-                "offer_id": offer.id
-            },
-            "expires_at": offer.end_date,
-            "max_redemptions": promo.meta['max_redemptions'],
-            "restrictions": {
-                "first_time_transaction": promo.meta["first_time_transaction"],
-                "minimum_amount": promo.meta["minimum_amount"],
-                ""
-            }
-        }
-    }
-}
-"""
```

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/processors/base.py` & `django-vendor-promo-0.2.2/src/vendorpromo/processors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     ################
     # Processor Functions
     def is_code_valid(self, code):
         """
         Overwrite funtion to call external promo services.
         Eg. call Vouchary.io API to see if the code entered is valid.
         """
-        raise NotImplementedError
+        return True
 
     def redeem_code(self, code):
         """
         Overwrite funtion to call external promo services to redeem code.
         Eg. call Vouchary.io API to redeem the code.
         """
         raise NotImplementedError
```

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/processors/stripe.py` & `django-vendor-promo-0.2.2/src/vendorpromo/processors/stripe.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         '''
         Override if you need to do additional steps when deleting a Promo instance,
         such as editing the promo code in an external service if needed.
         '''
         stripe_id = promo_campaign.meta.get('stripe_id')
         
         if stripe_id:
-            self.stripe_builder.stripe_delete_object(self.stripe.Coupon, stripe_id)
+            self.stripe_builder.stripe_delete_object(self.stripe_builder.stripe.Coupon, stripe_id)
         
         super().delete_promo(promo_campaign)
 
     ################
     # Coupon Code Management
     def create_coupon_code(self, coupon_form):
         coupon_code = super().create_coupon_code(coupon_form)
```

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/processors/vouchery.py` & `django-vendor-promo-0.2.2/src/vendorpromo/processors/vouchery.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/affiliate_detail.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/affiliate_list.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/affiliate_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/coupon_code_list.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/coupon_code_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promo.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promo_list.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promo_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promocode_formset.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promocode_formset.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/vouchery_detail.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/vouchery_integration.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_integration.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/templates/vendorpromo/vouchery_list.html` & `django-vendor-promo-0.2.2/src/vendorpromo/templates/vendorpromo/vouchery_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/tests/test_affiliate.py` & `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_affiliate.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/tests/test_coupon_code.py` & `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_coupon_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.auth import get_user_model
-from django.contrib.sites.models import Site
-from django.test import TestCase, Client
+from django.test import Client, TestCase
 from django.urls import reverse
 from vendor.models import CustomerProfile
+
 from vendorpromo.models import CouponCode, PromotionalCampaign
 
 User = get_user_model()
 
 
 class CouponCodeModelTests(TestCase):
```

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/tests/test_processor.py` & `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/tests/test_promo.py` & `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promo.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/tests/test_promotional_campaign.py` & `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_promotional_campaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/tests/test_stripe.py` & `django-vendor-promo-0.2.2/src/vendorpromo/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/urls.py` & `django-vendor-promo-0.2.2/src/vendorpromo/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.1/src/vendorpromo/views.py` & `django-vendor-promo-0.2.2/src/vendorpromo/views.py`

 * *Files identical despite different names*


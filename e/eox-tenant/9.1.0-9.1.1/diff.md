# Comparing `tmp/eox-tenant-9.1.0.tar.gz` & `tmp/eox-tenant-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eox-tenant-9.1.0.tar", last modified: Mon May 15 20:18:26 2023, max compression
+gzip compressed data, was "eox-tenant-9.1.1.tar", last modified: Fri May 26 13:49:53 2023, max compression
```

## Comparing `eox-tenant-9.1.0.tar` & `eox-tenant-9.1.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.555141 eox-tenant-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-15 20:18:26.555141 eox-tenant-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.543141 eox-tenant-9.1.0/eox_tenant/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.547140 eox-tenant-9.1.0/eox_tenant/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.547140 eox-tenant-9.1.0/eox_tenant/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.547140 eox-tenant-9.1.0/eox_tenant/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_microsites.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_tenant_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/api/v1/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.547140 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/users_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/users_test_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/bearer_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/branding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/edxmako_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/get_common_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/oauth_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/site_configuration_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/theming_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/filters/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/filters/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/filters/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/filters/test/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/management/commands/change_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/management/commands/change_signup_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/management/commands/edit_tenant_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/management/commands/synchronize_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/migrations/0003_auto_20190620_1704.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/migrations/0005_auto_20191226_1225.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/migrations/0006_tenantorganization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/migrations/0007_auto_20200922_1421.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/migrations/0008_synchronize_tenants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/receivers_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.539141 eox-tenant-9.1.0/eox_tenant/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/templates/eox-tenant/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/templates/eox-tenant/not_found.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/templates/eox-tenant/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/templates/eox-tenant/widgets/json_widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/templatetags/ednx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/tenant_aware_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/tenant_aware_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/tenant_aware_functions/enrollments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.551141 eox-tenant-9.1.0/eox_tenant/tenant_wise/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/tenant_wise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/tenant_wise/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/tenant_wise/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.555141 eox-tenant-9.1.0/eox_tenant/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_change_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_change_signupsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_edit_tenant_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_receivers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_tenant_aware_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_tenant_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test/test_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/eox_tenant/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:18:26.547140 eox-tenant-9.1.0/eox_tenant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-15 20:18:26.000000 eox-tenant-9.1.0/eox_tenant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-15 20:18:26.000000 eox-tenant-9.1.0/eox_tenant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:18:26.000000 eox-tenant-9.1.0/eox_tenant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 20:18:26.000000 eox-tenant-9.1.0/eox_tenant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:18:26.000000 eox-tenant-9.1.0/eox_tenant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 20:18:26.000000 eox-tenant-9.1.0/eox_tenant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-15 20:18:26.555141 eox-tenant-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-15 20:18:14.000000 eox-tenant-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_microsites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_tenant_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/api/v1/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/branding_api_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/edxmako_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/oauth_dispatch_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_i_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/theming_helpers_h_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/theming_helpers_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/users_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/users_test_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/bearer_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/edxmako_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/get_common_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/oauth_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/site_configuration_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/theming_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/filters/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/filters/test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/change_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/change_signup_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/edit_tenant_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/management/commands/synchronize_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0003_auto_20190620_1704.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0005_auto_20191226_1225.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0006_tenantorganization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0007_auto_20200922_1421.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/0008_synchronize_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/receivers_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.567823 eox-tenant-9.1.1/eox_tenant/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.559823 eox-tenant-9.1.1/eox_tenant/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/not_found.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templates/eox-tenant/widgets/json_widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/templatetags/ednx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/enrollments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/tenant_wise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_wise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_wise/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/tenant_wise/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.571823 eox-tenant-9.1.1/eox_tenant/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_change_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_change_signupsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_edit_tenant_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_receivers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_tenant_aware_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_tenant_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/eox_tenant/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:49:53.563823 eox-tenant-9.1.1/eox_tenant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 13:49:53.000000 eox-tenant-9.1.1/eox_tenant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-26 13:49:53.575823 eox-tenant-9.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-26 13:49:42.000000 eox-tenant-9.1.1/setup.py
```

### Comparing `eox-tenant-9.1.0/LICENSE.txt` & `eox-tenant-9.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/PKG-INFO` & `eox-tenant-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-tenant
-Version: 9.1.0
+Version: 9.1.1
 Summary: Edunext Open edx extensions tenant.
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-tenant-9.1.0/README.rst` & `eox-tenant-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/admin.py` & `eox-tenant-9.1.1/eox_tenant/admin.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/api/v1/permissions.py` & `eox-tenant-9.1.1/eox_tenant/api/v1/permissions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """
 Permission for eox_tenant api v1.
 """
 from django.conf import settings
 from django.contrib.auth.models import Permission, User
 from django.contrib.contenttypes.models import ContentType
+from django.core.exceptions import ImproperlyConfigured
 from django.db.utils import ProgrammingError
 from rest_framework import exceptions, permissions
 
 
 def load_permissions():
     """
     Helper method to load a custom permission on DB that will be
     used to give access to the eox-tenant API.
     """
-    if settings.EOX_TENANT_LOAD_PERMISSIONS:
-        try:
-            content_type = ContentType.objects.get_for_model(User)
-            Permission.objects.get_or_create(
-                codename='can_call_eox_tenant',
-                name='Can access eox-tenant API',
-                content_type=content_type,
-            )
-        except ProgrammingError:
-            # This code runs when the app is loaded, if a migration has not been
-            # done a ProgrammingError exception is raised.
-            # we are bypassing those cases to let migrations run smoothly.
-            pass
+    try:
+        if settings.EOX_TENANT_LOAD_PERMISSIONS:
+            try:
+                content_type = ContentType.objects.get_for_model(User)
+                Permission.objects.get_or_create(
+                    codename='can_call_eox_tenant',
+                    name='Can access eox-tenant API',
+                    content_type=content_type,
+                )
+            except ProgrammingError:
+                # This code runs when the app is loaded, if a migration has not been
+                # done a ProgrammingError exception is raised.
+                # we are bypassing those cases to let migrations run smoothly.
+                pass
+    except ImproperlyConfigured:
+        pass
 
 
 class EoxTenantAPIPermission(permissions.BasePermission):
     """
     Defines a custom permissions to access eox-tenant API.
     These permissions make sure that a token is created with the client credentials of the same site is
     being used on, and the user has a valid SignUp source for the site.
```

### Comparing `eox-tenant-9.1.0/eox_tenant/api/v1/serializers.py` & `eox-tenant-9.1.1/eox_tenant/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_microsites.py` & `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_microsites.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_permissions.py` & `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_routes.py` & `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/api/v1/tests/test_tenant_config.py` & `eox-tenant-9.1.1/eox_tenant/api/v1/tests/test_tenant_config.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/api/v1/viewsets.py` & `eox-tenant-9.1.1/eox_tenant/api/v1/viewsets.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/apps.py` & `eox-tenant-9.1.1/eox_tenant/apps.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/async_utils.py` & `eox-tenant-9.1.1/eox_tenant/async_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/auth.py` & `eox-tenant-9.1.1/eox_tenant/auth.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/auth.py` & `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/auth.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py` & `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/bearer_authentication_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py` & `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/edx_auth_i_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py` & `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/backends/site_configuration_module_test_v1.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/edxapp_wrapper/site_configuration_module.py` & `eox-tenant-9.1.1/eox_tenant/edxapp_wrapper/site_configuration_module.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/filters/pipeline.py` & `eox-tenant-9.1.1/eox_tenant/filters/pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/filters/test/test_pipeline.py` & `eox-tenant-9.1.1/eox_tenant/filters/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/management/commands/change_domain.py` & `eox-tenant-9.1.1/eox_tenant/management/commands/change_domain.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/management/commands/change_signup_sources.py` & `eox-tenant-9.1.1/eox_tenant/management/commands/change_signup_sources.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/management/commands/edit_tenant_values.py` & `eox-tenant-9.1.1/eox_tenant/management/commands/edit_tenant_values.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/management/commands/synchronize_organizations.py` & `eox-tenant-9.1.1/eox_tenant/management/commands/synchronize_organizations.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/middleware.py` & `eox-tenant-9.1.1/eox_tenant/middleware.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/migrations/0001_initial.py` & `eox-tenant-9.1.1/eox_tenant/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/migrations/0003_auto_20190620_1704.py` & `eox-tenant-9.1.1/eox_tenant/migrations/0003_auto_20190620_1704.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/migrations/0005_auto_20191226_1225.py` & `eox-tenant-9.1.1/eox_tenant/migrations/0005_auto_20191226_1225.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/migrations/0006_tenantorganization.py` & `eox-tenant-9.1.1/eox_tenant/migrations/0006_tenantorganization.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/migrations/0007_auto_20200922_1421.py` & `eox-tenant-9.1.1/eox_tenant/migrations/0007_auto_20200922_1421.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/models.py` & `eox-tenant-9.1.1/eox_tenant/models.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/permissions.py` & `eox-tenant-9.1.1/eox_tenant/permissions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/pipeline.py` & `eox-tenant-9.1.1/eox_tenant/pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/receivers_helpers.py` & `eox-tenant-9.1.1/eox_tenant/receivers_helpers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/settings/common.py` & `eox-tenant-9.1.1/eox_tenant/settings/common.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/settings/production.py` & `eox-tenant-9.1.1/eox_tenant/settings/production.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/settings/test.py` & `eox-tenant-9.1.1/eox_tenant/settings/test.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/signals.py` & `eox-tenant-9.1.1/eox_tenant/signals.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/templatetags/ednx.py` & `eox-tenant-9.1.1/eox_tenant/templatetags/ednx.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/tenant_aware_functions/enrollments.py` & `eox-tenant-9.1.1/eox_tenant/tenant_aware_functions/enrollments.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/tenant_wise/__init__.py` & `eox-tenant-9.1.1/eox_tenant/tenant_wise/__init__.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/tenant_wise/context_managers.py` & `eox-tenant-9.1.1/eox_tenant/tenant_wise/context_managers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/tenant_wise/proxies.py` & `eox-tenant-9.1.1/eox_tenant/tenant_wise/proxies.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_admin.py` & `eox-tenant-9.1.1/eox_tenant/test/test_admin.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_async_utils.py` & `eox-tenant-9.1.1/eox_tenant/test/test_async_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_auth_backend.py` & `eox-tenant-9.1.1/eox_tenant/test/test_auth_backend.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_change_domain.py` & `eox-tenant-9.1.1/eox_tenant/test/test_change_domain.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_change_signupsource.py` & `eox-tenant-9.1.1/eox_tenant/test/test_change_signupsource.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_edit_tenant_values.py` & `eox-tenant-9.1.1/eox_tenant/test/test_edit_tenant_values.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_middleware.py` & `eox-tenant-9.1.1/eox_tenant/test/test_middleware.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_models.py` & `eox-tenant-9.1.1/eox_tenant/test/test_models.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_pipeline.py` & `eox-tenant-9.1.1/eox_tenant/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_receivers_helpers.py` & `eox-tenant-9.1.1/eox_tenant/test/test_receivers_helpers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_signals.py` & `eox-tenant-9.1.1/eox_tenant/test/test_signals.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_tenant_aware_functions.py` & `eox-tenant-9.1.1/eox_tenant/test/test_tenant_aware_functions.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_tenant_wise.py` & `eox-tenant-9.1.1/eox_tenant/test/test_tenant_wise.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_utils.py` & `eox-tenant-9.1.1/eox_tenant/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_views.py` & `eox-tenant-9.1.1/eox_tenant/test/test_views.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/test/test_wrappers.py` & `eox-tenant-9.1.1/eox_tenant/test/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/utils.py` & `eox-tenant-9.1.1/eox_tenant/utils.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/validators.py` & `eox-tenant-9.1.1/eox_tenant/validators.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/views.py` & `eox-tenant-9.1.1/eox_tenant/views.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant/widgets.py` & `eox-tenant-9.1.1/eox_tenant/widgets.py`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/eox_tenant.egg-info/PKG-INFO` & `eox-tenant-9.1.1/eox_tenant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-tenant
-Version: 9.1.0
+Version: 9.1.1
 Summary: Edunext Open edx extensions tenant.
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-tenant-9.1.0/eox_tenant.egg-info/SOURCES.txt` & `eox-tenant-9.1.1/eox_tenant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eox-tenant-9.1.0/setup.cfg` & `eox-tenant-9.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 9.1.0
+current_version = 9.1.1
 commit = False
 tag = False
 
 [bumpversion:file:eox_tenant/__init__.py]
 
 [coverage:run]
 data_file = .coverage
```

### Comparing `eox-tenant-9.1.0/setup.py` & `eox-tenant-9.1.1/setup.py`

 * *Files identical despite different names*


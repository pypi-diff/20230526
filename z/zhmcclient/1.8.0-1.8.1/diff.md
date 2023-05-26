# Comparing `tmp/zhmcclient-1.8.0.tar.gz` & `tmp/zhmcclient-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmcclient-1.8.0.tar", last modified: Tue May 16 07:25:52 2023, max compression
+gzip compressed data, was "zhmcclient-1.8.1.tar", last modified: Fri May 26 15:03:24 2023, max compression
```

## Comparing `zhmcclient-1.8.0.tar` & `zhmcclient-1.8.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-16 07:25:48.000000 zhmcclient-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/extra-testutils-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.220788 zhmcclient-1.8.0/zhmcclient/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_activation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_capacity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32528 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    94301 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_ldap_server_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    78470 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_nic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_resource_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    65630 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_group_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_storage_volume_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_timestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_unmanaged_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_user_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_virtual_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_virtual_storage_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/_virtual_switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.220788 zhmcclient-1.8.0/zhmcclient/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_cpc_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_inventory_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient/testutils/_hmc_vault_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.220788 zhmcclient-1.8.0/zhmcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 07:25:52.000000 zhmcclient-1.8.0/zhmcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:25:12.000000 zhmcclient-1.8.0/zhmcclient.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:25:52.224789 zhmcclient-1.8.0/zhmcclient_mock/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_idpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    41808 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-05-16 07:24:57.000000 zhmcclient-1.8.0/zhmcclient_mock/_urihandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.336064 zhmcclient-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-26 15:03:20.000000 zhmcclient-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/extra-testutils-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:03:24.336064 zhmcclient-1.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.328064 zhmcclient-1.8.1/zhmcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_activation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27187 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_capacity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32528 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94301 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78470 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33251 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_nic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15902 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_resource_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69538 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_group_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25230 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_storage_volume_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_timestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_user_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_virtual_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_virtual_storage_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/_virtual_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/zhmcclient/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_cpc_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_inventory_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient/testutils/_hmc_vault_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/zhmcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 15:03:24.000000 zhmcclient-1.8.1/zhmcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:02:39.000000 zhmcclient-1.8.1/zhmcclient.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:03:24.332064 zhmcclient-1.8.1/zhmcclient_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134108 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_idpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42583 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   201548 2023-05-26 15:02:29.000000 zhmcclient-1.8.1/zhmcclient_mock/_urihandler.py
```

### Comparing `zhmcclient-1.8.0/LICENSE` & `zhmcclient-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/MANIFEST.in` & `zhmcclient-1.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/PKG-INFO` & `zhmcclient-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.8.0
+Version: 1.8.1
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.8.0/README.rst` & `zhmcclient-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/extra-testutils-requirements.txt` & `zhmcclient-1.8.1/extra-testutils-requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/requirements.txt` & `zhmcclient-1.8.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/setup.py` & `zhmcclient-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/__init__.py` & `zhmcclient-1.8.1/zhmcclient/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_activation_profile.py` & `zhmcclient-1.8.1/zhmcclient/_activation_profile.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_adapter.py` & `zhmcclient-1.8.1/zhmcclient/_adapter.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_capacity_group.py` & `zhmcclient-1.8.1/zhmcclient/_capacity_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_certificates.py` & `zhmcclient-1.8.1/zhmcclient/_certificates.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_client.py` & `zhmcclient-1.8.1/zhmcclient/_client.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_console.py` & `zhmcclient-1.8.1/zhmcclient/_console.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_constants.py` & `zhmcclient-1.8.1/zhmcclient/_constants.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_cpc.py` & `zhmcclient-1.8.1/zhmcclient/_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_debug_info.py` & `zhmcclient-1.8.1/zhmcclient/_debug_info.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_exceptions.py` & `zhmcclient-1.8.1/zhmcclient/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_group.py` & `zhmcclient-1.8.1/zhmcclient/_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_hba.py` & `zhmcclient-1.8.1/zhmcclient/_hba.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_ldap_server_definition.py` & `zhmcclient-1.8.1/zhmcclient/_ldap_server_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_logging.py` & `zhmcclient-1.8.1/zhmcclient/_logging.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_lpar.py` & `zhmcclient-1.8.1/zhmcclient/_lpar.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_manager.py` & `zhmcclient-1.8.1/zhmcclient/_manager.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_metrics.py` & `zhmcclient-1.8.1/zhmcclient/_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_nic.py` & `zhmcclient-1.8.1/zhmcclient/_nic.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_notification.py` & `zhmcclient-1.8.1/zhmcclient/_notification.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_partition.py` & `zhmcclient-1.8.1/zhmcclient/_partition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_password_rule.py` & `zhmcclient-1.8.1/zhmcclient/_password_rule.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_port.py` & `zhmcclient-1.8.1/zhmcclient/_port.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_resource.py` & `zhmcclient-1.8.1/zhmcclient/_resource.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_resource_updater.py` & `zhmcclient-1.8.1/zhmcclient/_resource_updater.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_session.py` & `zhmcclient-1.8.1/zhmcclient/_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -455,36 +455,38 @@
             format(classname=self.__class__.__name__, id=id(self), s=self,
                    headers=headers, blanked_out=BLANKED_OUT))
         return ret
 
     @property
     def host(self):
         """
-        :term:`string`: HMC host, in one of the following formats:
+        :term:`string`: HMC host for this session.
+
+        The string will have one of the following formats:
 
           * a short or fully qualified DNS hostname
           * a literal (= dotted) IPv4 address
           * a literal IPv6 address, formatted as defined in :term:`RFC3986`
             with the extensions for zone identifiers as defined in
             :term:`RFC6874`, supporting ``-`` (minus) for the delimiter
             before the zone ID string, as an additional choice to ``%25``
         """
         return self._host
 
     @property
     def port(self):
         """
-        :term:`integer`: HMC TCP port to be used.
+        :term:`integer`: HMC TCP port that is used for this session.
         """
         return self._port
 
     @property
     def userid(self):
         """
-        :term:`string`: Userid of the HMC user to be used.
+        :term:`string`: HMC userid that is used for this session.
 
         If `None`, only operations that do not require authentication, can be
         performed.
         """
         return self._userid
 
     @property
@@ -515,28 +517,29 @@
         taking into account the defaults and the session-specific overrides.
         """
         return self._retry_timeout_config
 
     @property
     def base_url(self):
         """
-        :term:`string`: Base URL of the HMC in this session.
+        :term:`string`: Base URL of the HMC that is used for this session.
 
         Example:
 
         .. code-block:: text
 
             https://myhmc.acme.com:6794
         """
         return self._base_url
 
     @property
     def headers(self):
         """
-        :term:`header dict`: HTTP headers to be used in each request.
+        :term:`header dict`: HTTP headers that are used in requests sent
+        for this session.
 
         Initially, this is the following set of headers:
 
         .. code-block:: text
 
             Content-type: application/json
             Accept: */*
@@ -557,42 +560,51 @@
         :ref:`Time Statistics`).
         """
         return self._time_stats_keeper
 
     @property
     def session_id(self):
         """
-        :term:`string`: Session ID for this session, returned by the HMC.
+        :term:`string`: Session ID (= session token) used for this session.
+
+        If `None`, this session object is considered in a logged-off state.
+        In that state, any request that requires logon will first cause a
+        session to be created on the HMC and will store the session ID
+        returned by the HMC in this property.
+
+        If not `None`, this session object is considered in a logged-on state,
+        and the session ID stored in this property will be used for any
+        requests to the HMC.
         """
         return self._session_id
 
     @property
     def session(self):
         """
         :term:`string`: :class:`requests.Session` object for this session.
         """
         return self._session
 
     @property
     def object_topic(self):
         """
         :term:`string`: Name of the notification topic the HMC will use to send
-        object-related notification messages to this API session.
+        object-related notification messages to this session.
 
         When not logged on, this property is `None`.
 
         The associated topic type is "object-notification".
         """
         return self._object_topic
 
     @property
     def job_topic(self):
         """
         :term:`string`: Name of the notification topic the HMC will use to send
-        job notification messages to this API session.
+        job notification messages to this session.
 
         When not logged on, this property is `None`.
 
         The associated topic type is "job-notification".
         """
         return self._job_topic
 
@@ -603,103 +615,142 @@
         :ref:`auto-updating <Auto-updating of resources>` of resources.
         """
         return self._resource_updater
 
     @logged_api_call
     def logon(self, verify=False):
         """
-        Make sure the session is logged on to the HMC.
+        Make sure this session object is logged on to the HMC.
 
-        By default, this method checks whether there is a session-id set
-        and considers that sufficient for determining that the session is
-        logged on. The `verify` parameter can be used to verify the validity
-        of a session-id that is already set, by issuing a dummy operation
-        ("Get Console Properties") to the HMC.
-
-        After successful logon to the HMC, the following is stored in this
-        session object for reuse in subsequent operations:
-
-        * the HMC session-id, in order to avoid extra userid authentications,
-        * a :class:`requests.Session` object, in order to enable connection
-          pooling. Connection pooling avoids repetitive SSL/TLS handshakes.
+        If `verify=False`, this method determines the logged-on state of this
+        session object based on whether there is a session ID set in this
+        session object. If a session ID is set, it is assumed to be valid and
+        no new session is created on the HMC. Otherwise, a new session will be
+        created on the HMC.
+
+        If `verify=True`, this method determines the logged-on state of this
+        session object in addition by performing a read operation on the HMC
+        that requires to be logged on but no specific authorizations. If a
+        session ID is set and if that operation succeeds, no new session is
+        created on the HMC. Any failure of that read operation will be ignored.
+        Otherwise, a new session will be created on the HMC.
+
+        When a new session has been successfully created on the HMC, the
+        :attr:`session_id` attribute of this session object will be set to the
+        session ID returned by the HMC to put it into the logged-on state.
+
+        Any exceptions raised from this method are always related to the
+        creation of a new session on the HMC - any failures of the read
+        operation in the verification case are always ignored.
 
         Parameters:
 
-          verify (bool): If a session-id is already set, verify its validity.
+          verify (bool): Verify the validity of an existing session ID.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.ClientAuthError`
           :exc:`~zhmcclient.ServerAuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-        if not self.is_logon(verify):
+        need_logon = False
+        if self._session_id is None:
+            need_logon = True
+        elif verify:
+            try:
+                self.get('/api/console', logon_required=False,
+                         renew_session=False)
+            except Error:
+                need_logon = True
+        if need_logon:
             self._do_logon()
 
     @logged_api_call
     def logoff(self, verify=False):
+        # pylint: disable=unused-argument
         """
-        Make sure the session is logged off from the HMC.
+        Make sure this session object is logged off from the HMC.
 
-        After successful logoff, the HMC session-id and
-        :class:`requests.Session` object stored in this object are reset.
+        If a session ID is set in this session object, its session will be
+        deleted on the HMC. If that delete operation fails due to an invalid
+        session ID, that failure will be ignored. Any other failures of that
+        delete operation will be raised as exceptions.
+
+        When the session has been successfully deleted on the HMC, the
+        :attr:`session_id` attribute of this session object will be set to
+        `None` to put it into the logged-off state.
 
         Parameters:
 
-          verify (bool): If a session-id is already set, verify its validity.
+          verify (bool): Deprecated: This parameter will be ignored.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
-          :exc:`~zhmcclient.ServerAuthError`
           :exc:`~zhmcclient.ConnectionError`
         """
-        if self.is_logon(verify):
+        if self._session_id:
             self._do_logoff()
 
     @logged_api_call
     def is_logon(self, verify=False):
         """
-        Return a boolean indicating whether the session is currently logged on
-        to the HMC.
+        Return a boolean indicating whether this session object is logged on to
+        the HMC.
 
-        By default, this method checks whether there is a session-id set
-        and considers that sufficient for determining that the session is
-        logged on. The `verify` parameter can be used to verify the validity
-        of a session-id that is already set, by issuing a dummy operation
-        ("Get Console Properties") to the HMC.
+        If `verify=False`, this method determines the logged-on state based
+        on whether there is a session ID set in this object. If a session ID is
+        set, it is assumed to be valid, and `True` is returned. Otherwise,
+        `False` is returned. In that case, no exception is ever raised.
+
+        If `verify=True`, this method determines the logged-on state in
+        addition by verifying a session ID that is set, by performing a read
+        operation on the HMC that requires to be logged on but no specific
+        authorizations. If a session ID is set and if that read operation
+        succeeds, `True` is returned. If no session ID is set or if that read
+        operation fails due to an invalid session ID, `False` is returned.
+        Any other failures of that read operation are raised as exceptions,
+        because that indicates that a verification with the HMC could not be
+        performed.
 
         Parameters:
 
-          verify (bool): If a session-id is already set, verify its validity.
+          verify (bool): Verify the validity of an existing session ID.
+
+        Raises:
+
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.ConnectionError`
         """
         if self._session_id is None:
             return False
         if verify:
             try:
-                self.get('/api/console', logon_required=True)
+                self.get('/api/console', logon_required=False,
+                         renew_session=False)
             except ServerAuthError:
                 return False
         return True
 
     def _do_logon(self):
         """
         Log on, unconditionally. This can be used to re-logon.
         This requires credentials to be provided.
 
         Raises:
 
+          :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.ClientAuthError`
           :exc:`~zhmcclient.ServerAuthError`
           :exc:`~zhmcclient.ConnectionError`
-          :exc:`~zhmcclient.ParseError`
-          :exc:`~zhmcclient.HTTPError`
         """
         if self._userid is None:
             raise ClientAuthError("Userid is not provided.")
         if self._password is None:
             if self._get_password:
                 self._password = self._get_password(self._host, self._userid)
             else:
@@ -735,23 +786,28 @@
                       requests.adapters.HTTPAdapter(max_retries=retry))
         return session
 
     def _do_logoff(self):
         """
         Log off, unconditionally.
 
+        This deletes the session on the HMC. If that deletion operation fails
+        due to an invalid session ID, that failure is ignored.
+
         Raises:
 
-          :exc:`~zhmcclient.ServerAuthError`
-          :exc:`~zhmcclient.ConnectionError`
-          :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.HTTPError`
+          :exc:`~zhmcclient.ParseError`
+          :exc:`~zhmcclient.ConnectionError`
         """
         session_uri = '/api/sessions/this-session'
-        self.delete(session_uri, logon_required=False)
+        try:
+            self.delete(session_uri, logon_required=False, renew_session=False)
+        except ServerAuthError:
+            pass
         self._session_id = None
         self._session = None
         self._headers.pop('X-API-Session', None)
         self._object_topic = None
         self._job_topic = None
 
     @staticmethod
@@ -866,15 +922,15 @@
             content_msg = content
 
         HMC_LOGGER.debug("Respons: %s %s, status: %s, headers: %r, %s: %r",
                          method, url, status, _headers_for_logging(headers),
                          content_label, content_msg)
 
     @logged_api_call
-    def get(self, uri, logon_required=True):
+    def get(self, uri, logon_required=True, renew_session=True):
         """
         Perform the HTTP GET method against the resource identified by a URI.
 
         A set of standard HTTP headers is automatically part of the request.
 
         If the HMC session token is expired, this method re-logs on and retries
         the operation.
@@ -888,14 +944,18 @@
             Must not be `None`.
 
           logon_required (bool):
             Boolean indicating whether the operation requires that the session
             is logged on to the HMC. For example, the API version retrieval
             operation does not require that.
 
+          renew_session (bool):
+            Boolean indicating whether the session should be renewed in case
+            it is expired.
+
         Returns:
 
           :term:`json object` with the operation result.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
@@ -928,31 +988,41 @@
                                 content=result.content)
 
         if result.status_code == 200:
             return _result_object(result)
         if result.status_code == 403:
             result_object = _result_object(result)
             reason = result_object.get('reason', None)
-            if reason == 5:
-                # API session token expired: re-logon and retry
-                self._do_logon()
-                return self.get(uri, logon_required)
+
+            if reason in (4, 5):
+                # 403.4: No session ID was provided
+                # 403.5: Session ID was invalid
+                if renew_session:
+                    self._do_logon()
+                    return self.get(
+                        uri, logon_required=False, renew_session=False)
+
             if reason == 1:
                 # Login user's authentication is fine; this is an authorization
                 # issue, so we don't raise ServerAuthError.
                 raise HTTPError(result_object)
+
             msg = result_object.get('message', None)
-            raise ServerAuthError("HTTP authentication failed: {}".
-                                  format(msg), HTTPError(result_object))
+            raise ServerAuthError(
+                "HTTP authentication failed with {},{}: {}".
+                format(result.status_code, reason, msg),
+                HTTPError(result_object))
+
         result_object = _result_object(result)
         raise HTTPError(result_object)
 
     @logged_api_call
     def post(self, uri, body=None, logon_required=True,
-             wait_for_completion=False, operation_timeout=None):
+             wait_for_completion=False, operation_timeout=None,
+             renew_session=True):
         """
         Perform the HTTP POST method against the resource identified by a URI,
         using a provided request body.
 
         A set of standard HTTP headers is automatically part of the request.
 
         HMC operations using HTTP POST are either synchronous or asynchronous.
@@ -1024,14 +1094,18 @@
 
             For `wait_for_completion=True`, a
             :exc:`~zhmcclient.OperationTimeout` is raised when the timeout
             expires.
 
             For `wait_for_completion=False`, this parameter has no effect.
 
+          renew_session (bool):
+            Boolean indicating whether the session should be renewed in case
+            it is expired.
+
         Returns:
 
           : A :term:`json object` or `None` or a :class:`~zhmcclient.Job`
           object, as follows:
 
           * For synchronous HMC operations, and for asynchronous HMC
             operations with `wait_for_completion=True`:
@@ -1163,38 +1237,46 @@
                 if wait_for_completion:
                     return job.wait_for_completion(operation_timeout)
                 return job
 
             if result.status_code == 403:
                 result_object = _result_object(result)
                 reason = result_object.get('reason', None)
-                if reason == 5:
-                    # API session token expired: re-logon and retry
-                    self._do_logon()
-                    return self.post(uri, body, logon_required)
+
+                if reason in (4, 5):
+                    # 403.4: No session ID was provided
+                    # 403.5: Session ID was invalid
+                    if renew_session:
+                        self._do_logon()
+                        return self.post(
+                            uri, body,
+                            logon_required=False, renew_session=False,
+                            wait_for_completion=wait_for_completion,
+                            operation_timeout=operation_timeout)
 
                 if reason == 1:
                     # Login user's authentication is fine; this is an
                     # authorization issue, so we don't raise ServerAuthError.
                     raise HTTPError(result_object)
 
                 msg = result_object.get('message', None)
-                raise ServerAuthError("HTTP authentication failed: {}".
-                                      format(msg),
-                                      HTTPError(result_object))
+                raise ServerAuthError(
+                    "HTTP authentication failed with {},{}: {}".
+                    format(result.status_code, reason, msg),
+                    HTTPError(result_object))
 
             result_object = _result_object(result)
             raise HTTPError(result_object)
 
         finally:
             if wait_for_completion:
                 stats_total.end()
 
     @logged_api_call
-    def delete(self, uri, logon_required=True):
+    def delete(self, uri, logon_required=True, renew_session=True):
         """
         Perform the HTTP DELETE method against the resource identified by a
         URI.
 
         A set of standard HTTP headers is automatically part of the request.
 
         If the HMC session token is expired, this method re-logs on and retries
@@ -1210,14 +1292,19 @@
             Must not be `None`.
 
           logon_required (bool):
             Boolean indicating whether the operation requires that the session
             is logged on to the HMC. For example, for the logoff operation, it
             does not make sense to first log on.
 
+          renew_session (bool):
+            Boolean indicating whether the session should be renewed in case
+            it is expired. For example, for the logoff operation, it does not
+            make sense to do that.
+
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError`
           :exc:`~zhmcclient.ClientAuthError`
           :exc:`~zhmcclient.ServerAuthError`
           :exc:`~zhmcclient.ConnectionError`
@@ -1247,38 +1334,42 @@
 
         if result.status_code in (200, 204):
             return
 
         if result.status_code == 403:
             result_object = _result_object(result)
             reason = result_object.get('reason', None)
-            if reason == 5:
-                # API session token expired: re-logon and retry
-                self._do_logon()
-                self.delete(uri, logon_required)
-                return
+
+            if reason in (4, 5):
+                # 403.4: No session ID was provided
+                # 403.5: Session ID was invalid
+                if renew_session:
+                    self._do_logon()
+                    self.delete(uri, logon_required=False, renew_session=False)
+                    return
 
             if reason == 1:
                 # Login user's authentication is fine; this is an authorization
                 # issue, so we don't raise ServerAuthError.
                 raise HTTPError(result_object)
 
             msg = result_object.get('message', None)
-            raise ServerAuthError("HTTP authentication failed: {}".
-                                  format(msg), HTTPError(result_object))
+            raise ServerAuthError(
+                "HTTP authentication failed with {},{}: {}".
+                format(result.status_code, reason, msg),
+                HTTPError(result_object))
 
         result_object = _result_object(result)
         raise HTTPError(result_object)
 
     @logged_api_call
     def get_notification_topics(self):
         """
         The 'Get Notification Topics' operation returns a structure that
-        describes the JMS notification topics associated with the
-        API session.
+        describes the JMS notification topics associated with this session.
 
         Returns:
 
           : A list with one item for each notification topic. Each item is a
           dictionary with the following keys:
 
           * ``"topic-type"`` (string): Topic type, e.g. "job-notification".
@@ -1587,15 +1678,15 @@
     """
     Return the JSON payload in the HTTP response as a Python dict.
 
     Parameters:
         result (requests.Response): HTTP response object.
 
     Raises:
-        zhmcclient.ParseError: Error parsing the returned JSON.
+        :exc:`~zhmcclient.ParseError`: Error parsing the returned JSON.
     """
     content_type = result.headers.get('content-type', None)
 
     if content_type is None or content_type.startswith('application/json'):
         # This function is only called when there is content expected.
         # Therefore, a response without content will result in a ParseError.
         try:
```

### Comparing `zhmcclient-1.8.0/zhmcclient/_storage_group.py` & `zhmcclient-1.8.1/zhmcclient/_storage_group.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_storage_group_template.py` & `zhmcclient-1.8.1/zhmcclient/_storage_group_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_storage_volume.py` & `zhmcclient-1.8.1/zhmcclient/_storage_volume.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_storage_volume_template.py` & `zhmcclient-1.8.1/zhmcclient/_storage_volume_template.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_task.py` & `zhmcclient-1.8.1/zhmcclient/_task.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_timestats.py` & `zhmcclient-1.8.1/zhmcclient/_timestats.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_unmanaged_cpc.py` & `zhmcclient-1.8.1/zhmcclient/_unmanaged_cpc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_user.py` & `zhmcclient-1.8.1/zhmcclient/_user.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_user_pattern.py` & `zhmcclient-1.8.1/zhmcclient/_user_pattern.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_user_role.py` & `zhmcclient-1.8.1/zhmcclient/_user_role.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_utils.py` & `zhmcclient-1.8.1/zhmcclient/_utils.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_version.py` & `zhmcclient-1.8.1/zhmcclient/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.8.0'
+__version__ = '1.8.1'
 
 # Check supported Python versions
 # Keep these Python versions in sync with:
 # - python_requires and classifiers in setup.py
 # - Section "Supported environments" in docs/intro.rst
 _PYTHON_M = sys.version_info[0]
 _PYTHON_N = sys.version_info[1]
```

### Comparing `zhmcclient-1.8.0/zhmcclient/_virtual_function.py` & `zhmcclient-1.8.1/zhmcclient/_virtual_function.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_virtual_storage_resource.py` & `zhmcclient-1.8.1/zhmcclient/_virtual_storage_resource.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/_virtual_switch.py` & `zhmcclient-1.8.1/zhmcclient/_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/testutils/__init__.py` & `zhmcclient-1.8.1/zhmcclient/testutils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/testutils/_cpc_fixtures.py` & `zhmcclient-1.8.1/zhmcclient/testutils/_cpc_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition.py` & `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definition_fixtures.py` & `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definition_fixtures.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_definitions.py` & `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_definitions.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_inventory_file.py` & `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_inventory_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient/testutils/_hmc_vault_file.py` & `zhmcclient-1.8.1/zhmcclient/testutils/_hmc_vault_file.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient.egg-info/PKG-INFO` & `zhmcclient-1.8.1/zhmcclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmcclient
-Version: 1.8.0
+Version: 1.8.1
 Summary: A pure Python client library for the IBM Z HMC Web Services API.
 Home-page: https://github.com/zhmcclient/python-zhmcclient
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmcclient-1.8.0/zhmcclient.egg-info/SOURCES.txt` & `zhmcclient-1.8.1/zhmcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient.egg-info/requires.txt` & `zhmcclient-1.8.1/zhmcclient.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient_mock/__init__.py` & `zhmcclient-1.8.1/zhmcclient_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient_mock/_hmc.py` & `zhmcclient-1.8.1/zhmcclient_mock/_hmc.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient_mock/_idpool.py` & `zhmcclient-1.8.1/zhmcclient_mock/_idpool.py`

 * *Files identical despite different names*

### Comparing `zhmcclient-1.8.0/zhmcclient_mock/_session.py` & `zhmcclient-1.8.1/zhmcclient_mock/_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -943,15 +943,15 @@
                     resource_uri=resource_uri,
                     timestamp=timestamp,
                     values=values)
                 session.hmc.add_metric_values(mv)
 
         return session
 
-    def get(self, uri, logon_required=True):
+    def get(self, uri, logon_required=True, renew_session=True):
         """
         Perform the HTTP GET method against the resource identified by a URI,
         on the faked HMC.
 
         Parameters:
 
           uri (:term:`string`):
@@ -963,14 +963,21 @@
           logon_required (bool):
             Boolean indicating whether the operation requires that the session
             is logged on to the HMC.
 
             Because this is a faked HMC, this does not perform a real logon,
             but it is still used to update the state in the faked HMC.
 
+          renew_session (bool):
+            Boolean indicating whether the session should be renewed in case
+            it is expired.
+
+            This parameter exists for compatibility with real HMCs, but is
+            ignored.
+
         Returns:
 
           :term:`json object` with the operation result.
 
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
@@ -986,15 +993,16 @@
             raise new_exc  # zhmcclient.HTTPError
         except ConnectionError as exc:
             new_exc = zhmcclient.ConnectionError(exc.message, None)
             new_exc.__cause__ = None
             raise new_exc  # zhmcclient.ConnectionError
 
     def post(self, uri, body=None, logon_required=True,
-             wait_for_completion=True, operation_timeout=None):
+             wait_for_completion=True, operation_timeout=None,
+             renew_session=True):
         """
         Perform the HTTP POST method against the resource identified by a URI,
         using a provided request body, on the faked HMC.
 
         HMC operations using HTTP POST are either synchronous or asynchronous.
         Asynchronous operations return the URI of an asynchronously executing
         job that can be queried for status and result.
@@ -1061,14 +1069,21 @@
 
             For `wait_for_completion=True`, a
             :exc:`~zhmcclient.OperationTimeout` is raised when the timeout
             expires.
 
             For `wait_for_completion=False`, this parameter has no effect.
 
+          renew_session (bool):
+            Boolean indicating whether the session should be renewed in case
+            it is expired.
+
+            This parameter exists for compatibility with real HMCs, but is
+            ignored.
+
         Returns:
 
           :term:`json object`:
 
             If `wait_for_completion` is `True`, returns a JSON object
             representing the response body of the synchronous operation, or the
             response body of the completed job that performed the asynchronous
@@ -1102,15 +1117,15 @@
             new_exc.__cause__ = None
             raise new_exc  # zhmcclient.HTTPError
         except ConnectionError as exc:
             new_exc = zhmcclient.ConnectionError(exc.message, None)
             new_exc.__cause__ = None
             raise new_exc  # zhmcclient.ConnectionError
 
-    def delete(self, uri, logon_required=True):
+    def delete(self, uri, logon_required=True, renew_session=True):
         """
         Perform the HTTP DELETE method against the resource identified by a
         URI, on the faked HMC.
 
         Parameters:
 
           uri (:term:`string`):
@@ -1124,14 +1139,21 @@
             Boolean indicating whether the operation requires that the session
             is logged on to the HMC. For example, for the logoff operation, it
             does not make sense to first log on.
 
             Because this is a faked HMC, this does not perform a real logon,
             but it is still used to update the state in the faked HMC.
 
+          renew_session (bool):
+            Boolean indicating whether the session should be renewed in case
+            it is expired.
+
+            This parameter exists for compatibility with real HMCs, but is
+            ignored.
+
         Raises:
 
           :exc:`~zhmcclient.HTTPError`
           :exc:`~zhmcclient.ParseError` (not implemented)
           :exc:`~zhmcclient.AuthError` (not implemented)
           :exc:`~zhmcclient.ConnectionError`
         """
```

### Comparing `zhmcclient-1.8.0/zhmcclient_mock/_urihandler.py` & `zhmcclient-1.8.1/zhmcclient_mock/_urihandler.py`

 * *Files identical despite different names*


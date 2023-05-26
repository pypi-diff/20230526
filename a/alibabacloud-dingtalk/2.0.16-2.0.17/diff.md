# Comparing `tmp/alibabacloud_dingtalk-2.0.16.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.16.tar", last modified: Wed May 24 08:33:20 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.17.tar", last modified: Fri May 26 10:34:14 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.16.tar` & `alibabacloud_dingtalk-2.0.17.tar`

### file list

```diff
@@ -1,365 +1,365 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/
--rw-r--r--   0 root         (0) root         (0)    19687 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322772 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138814 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   331545 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312544 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   433417 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   606316 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   855474 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131349 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   159547 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44880 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81308 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377583 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12014 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/
+-rw-r--r--   0 root         (0) root         (0)    19752 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322772 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138814 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   331545 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48073 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    67303 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312544 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   433417 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   606316 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   855474 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138339 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   166104 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12014 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.16/ChangeLog.md` & `alibabacloud_dingtalk-2.0.17/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-24 Version: 2.0.16
+- Update AddOfficialAccountFollower.
+
 2023-05-18 Version: 2.0.15
 - Update AddOfficialAccountFollower.
 
 2023-05-17 Version: 2.0.14
 - Update AddOfficialAccountFollower.
 
 2023-05-16 Version: 2.0.13
```

### Comparing `alibabacloud_dingtalk-2.0.16/LICENSE` & `alibabacloud_dingtalk-2.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/PKG-INFO` & `alibabacloud_dingtalk-2.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.16
+Version: 2.0.17
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.16/README-CN.md` & `alibabacloud_dingtalk-2.0.17/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/README.md` & `alibabacloud_dingtalk-2.0.17/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.core import TeaCore
+from typing import Dict
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_dingtalk.diot_1_0 import models as dingtalkdiot__1__0_models
@@ -21,14 +22,15 @@
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
+        self._signature_algorithm = 'v2'
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
     def batch_delete_device_with_options(
         self,
         request: dingtalkdiot__1__0_models.BatchDeleteDeviceRequest,
@@ -1044,7 +1046,65 @@
     async def register_device_async(
         self,
         request: dingtalkdiot__1__0_models.RegisterDeviceRequest,
     ) -> dingtalkdiot__1__0_models.RegisterDeviceResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkdiot__1__0_models.RegisterDeviceHeaders()
         return await self.register_device_with_options_async(request, headers, runtime)
+
+    def workbench_transform_info_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.WorkbenchTransformInfoResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='WorkbenchTransformInfo',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/workbench/transform',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.WorkbenchTransformInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def workbench_transform_info_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkdiot__1__0_models.WorkbenchTransformInfoResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='WorkbenchTransformInfo',
+            version='diot_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/diot/workbench/transform',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkdiot__1__0_models.WorkbenchTransformInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def workbench_transform_info(self) -> dingtalkdiot__1__0_models.WorkbenchTransformInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.workbench_transform_info_with_options(headers, runtime)
+
+    async def workbench_transform_info_async(self) -> dingtalkdiot__1__0_models.WorkbenchTransformInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.workbench_transform_info_with_options_async(headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2105,7 +2105,78 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RegisterDeviceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class WorkbenchTransformInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class WorkbenchTransformInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: WorkbenchTransformInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = WorkbenchTransformInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -391,14 +391,206 @@
         return self.anhei_test_888with_options(headers, runtime)
 
     async def anhei_test_888_async(self) -> dingtalkmicro_app__1__0_models.AnheiTest888Response:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.anhei_test_888with_options_async(headers, runtime)
 
+    def anhei_test_bwith_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiTestBResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiTestB',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiTestB',
+            method='PUT',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiTestBResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def anhei_test_bwith_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiTestBResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiTestB',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiTestB',
+            method='PUT',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiTestBResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def anhei_test_b(self) -> dingtalkmicro_app__1__0_models.AnheiTestBResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.anhei_test_bwith_options(headers, runtime)
+
+    async def anhei_test_b_async(self) -> dingtalkmicro_app__1__0_models.AnheiTestBResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.anhei_test_bwith_options_async(headers, runtime)
+
+    def app_status_manager_test_with_options(
+        self,
+        request: dingtalkmicro_app__1__0_models.AppStatusManagerTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AppStatusManagerTestResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.request_id):
+            query['requestId'] = request.request_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AppStatusManagerTest',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/manager/test',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AppStatusManagerTestResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def app_status_manager_test_with_options_async(
+        self,
+        request: dingtalkmicro_app__1__0_models.AppStatusManagerTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AppStatusManagerTestResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.request_id):
+            query['requestId'] = request.request_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AppStatusManagerTest',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/manager/test',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AppStatusManagerTestResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def app_status_manager_test(
+        self,
+        request: dingtalkmicro_app__1__0_models.AppStatusManagerTestRequest,
+    ) -> dingtalkmicro_app__1__0_models.AppStatusManagerTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.app_status_manager_test_with_options(request, headers, runtime)
+
+    async def app_status_manager_test_async(
+        self,
+        request: dingtalkmicro_app__1__0_models.AppStatusManagerTestRequest,
+    ) -> dingtalkmicro_app__1__0_models.AppStatusManagerTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.app_status_manager_test_with_options_async(request, headers, runtime)
+
+    def ayun_test_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AyunTestResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AyunTest',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/ayun/test',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AyunTestResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def ayun_test_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AyunTestResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AyunTest',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/ayun/test',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AyunTestResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def ayun_test(self) -> dingtalkmicro_app__1__0_models.AyunTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.ayun_test_with_options(headers, runtime)
+
+    async def ayun_test_async(self) -> dingtalkmicro_app__1__0_models.AyunTestResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.ayun_test_with_options_async(headers, runtime)
+
     def create_apaas_app_with_options(
         self,
         request: dingtalkmicro_app__1__0_models.CreateApaasAppRequest,
         headers: dingtalkmicro_app__1__0_models.CreateApaasAppHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkmicro_app__1__0_models.CreateApaasAppResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -612,14 +612,254 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AnheiTest888ResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AnheiTestBResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class AnheiTestBResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AnheiTestBResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AnheiTestBResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class AppStatusManagerTestRequest(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class AppStatusManagerTestResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class AppStatusManagerTestResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AppStatusManagerTestResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AppStatusManagerTestResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class AyunTestResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class AyunTestResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AyunTestResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AyunTestResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateApaasAppHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -629,14 +629,194 @@
         dentry_uuid: str,
         request: dingtalkstorage__2__0_models.ListPermissionsRequest,
     ) -> dingtalkstorage__2__0_models.ListPermissionsResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkstorage__2__0_models.ListPermissionsHeaders()
         return await self.list_permissions_with_options_async(dentry_uuid, request, headers, runtime)
 
+    def manager_get_default_hand_over_user_with_options(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserRequest,
+        headers: dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ManagerGetDefaultHandOverUser',
+            version='storage_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/storage/managementSettings/defaultHandOverUsers',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def manager_get_default_hand_over_user_with_options_async(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserRequest,
+        headers: dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ManagerGetDefaultHandOverUser',
+            version='storage_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/storage/managementSettings/defaultHandOverUsers',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def manager_get_default_hand_over_user(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserRequest,
+    ) -> dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserHeaders()
+        return self.manager_get_default_hand_over_user_with_options(request, headers, runtime)
+
+    async def manager_get_default_hand_over_user_async(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserRequest,
+    ) -> dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkstorage__2__0_models.ManagerGetDefaultHandOverUserHeaders()
+        return await self.manager_get_default_hand_over_user_with_options_async(request, headers, runtime)
+
+    def manager_set_default_hand_over_user_with_options(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserRequest,
+        headers: dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.default_handover_user_id):
+            body['defaultHandoverUserId'] = request.default_handover_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ManagerSetDefaultHandOverUser',
+            version='storage_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/storage/managementSettings/defaultHandOverUsers/set',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def manager_set_default_hand_over_user_with_options_async(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserRequest,
+        headers: dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.default_handover_user_id):
+            body['defaultHandoverUserId'] = request.default_handover_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ManagerSetDefaultHandOverUser',
+            version='storage_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/storage/managementSettings/defaultHandOverUsers/set',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def manager_set_default_hand_over_user(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserRequest,
+    ) -> dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserHeaders()
+        return self.manager_set_default_hand_over_user_with_options(request, headers, runtime)
+
+    async def manager_set_default_hand_over_user_async(
+        self,
+        request: dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserRequest,
+    ) -> dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkstorage__2__0_models.ManagerSetDefaultHandOverUserHeaders()
+        return await self.manager_set_default_hand_over_user_with_options_async(request, headers, runtime)
+
     def search_dentries_with_options(
         self,
         request: dingtalkstorage__2__0_models.SearchDentriesRequest,
         headers: dingtalkstorage__2__0_models.SearchDentriesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkstorage__2__0_models.SearchDentriesResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1681,14 +1681,282 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListPermissionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ManagerGetDefaultHandOverUserHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class ManagerGetDefaultHandOverUserRequest(TeaModel):
+    def __init__(
+        self,
+        operator_id: str = None,
+    ):
+        self.operator_id = operator_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class ManagerGetDefaultHandOverUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        default_handover_user_id: str = None,
+    ):
+        self.default_handover_user_id = default_handover_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.default_handover_user_id is not None:
+            result['defaultHandoverUserId'] = self.default_handover_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('defaultHandoverUserId') is not None:
+            self.default_handover_user_id = m.get('defaultHandoverUserId')
+        return self
+
+
+class ManagerGetDefaultHandOverUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ManagerGetDefaultHandOverUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ManagerGetDefaultHandOverUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ManagerSetDefaultHandOverUserHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class ManagerSetDefaultHandOverUserRequest(TeaModel):
+    def __init__(
+        self,
+        default_handover_user_id: str = None,
+        operator_id: str = None,
+    ):
+        self.default_handover_user_id = default_handover_user_id
+        self.operator_id = operator_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.default_handover_user_id is not None:
+            result['defaultHandoverUserId'] = self.default_handover_user_id
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('defaultHandoverUserId') is not None:
+            self.default_handover_user_id = m.get('defaultHandoverUserId')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class ManagerSetDefaultHandOverUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class ManagerSetDefaultHandOverUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ManagerSetDefaultHandOverUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ManagerSetDefaultHandOverUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SearchDentriesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4495,14 +4495,15 @@
 
 class GetProcessInstanceResponseBodyResult(TeaModel):
     def __init__(
         self,
         approver_user_ids: List[str] = None,
         attached_process_instance_ids: List[str] = None,
         biz_action: str = None,
+        biz_data: str = None,
         business_id: str = None,
         cc_user_ids: List[str] = None,
         create_time: str = None,
         finish_time: str = None,
         form_component_values: List[GetProcessInstanceResponseBodyResultFormComponentValues] = None,
         main_process_instance_id: str = None,
         operation_records: List[GetProcessInstanceResponseBodyResultOperationRecords] = None,
@@ -4513,14 +4514,15 @@
         status: str = None,
         tasks: List[GetProcessInstanceResponseBodyResultTasks] = None,
         title: str = None,
     ):
         self.approver_user_ids = approver_user_ids
         self.attached_process_instance_ids = attached_process_instance_ids
         self.biz_action = biz_action
+        self.biz_data = biz_data
         self.business_id = business_id
         self.cc_user_ids = cc_user_ids
         self.create_time = create_time
         self.finish_time = finish_time
         self.form_component_values = form_component_values
         self.main_process_instance_id = main_process_instance_id
         self.operation_records = operation_records
@@ -4554,14 +4556,16 @@
         result = dict()
         if self.approver_user_ids is not None:
             result['approverUserIds'] = self.approver_user_ids
         if self.attached_process_instance_ids is not None:
             result['attachedProcessInstanceIds'] = self.attached_process_instance_ids
         if self.biz_action is not None:
             result['bizAction'] = self.biz_action
+        if self.biz_data is not None:
+            result['bizData'] = self.biz_data
         if self.business_id is not None:
             result['businessId'] = self.business_id
         if self.cc_user_ids is not None:
             result['ccUserIds'] = self.cc_user_ids
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.finish_time is not None:
@@ -4598,14 +4602,16 @@
         m = m or dict()
         if m.get('approverUserIds') is not None:
             self.approver_user_ids = m.get('approverUserIds')
         if m.get('attachedProcessInstanceIds') is not None:
             self.attached_process_instance_ids = m.get('attachedProcessInstanceIds')
         if m.get('bizAction') is not None:
             self.biz_action = m.get('bizAction')
+        if m.get('bizData') is not None:
+            self.biz_data = m.get('bizData')
         if m.get('businessId') is not None:
             self.business_id = m.get('businessId')
         if m.get('ccUserIds') is not None:
             self.cc_user_ids = m.get('ccUserIds')
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('finishTime') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.16
+Version: 2.0.17
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.16/setup.py` & `alibabacloud_dingtalk-2.0.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 24/05/2023
+Created on 26/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```


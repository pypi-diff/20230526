# Comparing `tmp/infobip-api-python-sdk-5.0.0.tar.gz` & `tmp/infobip-api-python-sdk-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infobip-api-python-sdk-5.0.0.tar", last modified: Wed Apr  5 19:28:30 2023, max compression
+gzip compressed data, was "infobip-api-python-sdk-5.0.1.tar", last modified: Fri May 26 15:09:19 2023, max compression
```

## Comparing `infobip-api-python-sdk-5.0.0.tar` & `infobip-api-python-sdk-5.0.1.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.520016 infobip-api-python-sdk-5.0.0/
--rw-r--r--   0 ecorona    (502) staff       (20)     1114 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/LICENSE
--rw-r--r--   0 ecorona    (502) staff       (20)     4498 2023-04-05 19:28:30.520884 infobip-api-python-sdk-5.0.0/PKG-INFO
--rw-r--r--   0 ecorona    (502) staff       (20)     3854 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/README.md
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.517870 infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/
--rw-r--r--   0 ecorona    (502) staff       (20)     4498 2023-04-05 19:28:30.000000 infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ecorona    (502) staff       (20)    11318 2023-04-05 19:28:30.000000 infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ecorona    (502) staff       (20)        1 2023-04-05 19:28:30.000000 infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ecorona    (502) staff       (20)       50 2023-04-05 19:28:30.000000 infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/requires.txt
--rw-r--r--   0 ecorona    (502) staff       (20)       34 2023-04-05 19:28:30.000000 infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.254553 infobip-api-python-sdk-5.0.0/infobip_channels/
--rw-r--r--   0 ecorona    (502) staff       (20)      370 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.259288 infobip-api-python-sdk-5.0.0/infobip_channels/core/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/core/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     9640 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/core/channel.py
--rw-r--r--   0 ecorona    (502) staff       (20)     3827 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/core/http_client.py
--rw-r--r--   0 ecorona    (502) staff       (20)    11583 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/core/models.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.262508 infobip-api-python-sdk-5.0.0/infobip_channels/email/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)    15405 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/channel.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.265053 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.274777 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      128 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/add_new_domain.py
--rw-r--r--   0 ecorona    (502) staff       (20)      416 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/reschedule_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1684 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/send_email.py
--rw-r--r--   0 ecorona    (502) staff       (20)      157 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/update_scheduled_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      300 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/update_tracking_events.py
--rw-r--r--   0 ecorona    (502) staff       (20)      129 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/validate_email_addresses.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.284102 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/path_parameters/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/path_parameters/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      119 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/path_parameters/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      154 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/path_parameters/delete_existing_domain.py
--rw-r--r--   0 ecorona    (502) staff       (20)      150 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/path_parameters/get_domain_details.py
--rw-r--r--   0 ecorona    (502) staff       (20)      154 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/path_parameters/update_tracking_events.py
--rw-r--r--   0 ecorona    (502) staff       (20)      146 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/path_parameters/verify_domain.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.293987 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      119 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      244 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/delivery_reports.py
--rw-r--r--   0 ecorona    (502) staff       (20)      265 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/get_all_domains.py
--rw-r--r--   0 ecorona    (502) staff       (20)      540 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/get_logs.py
--rw-r--r--   0 ecorona    (502) staff       (20)      153 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/get_sent_bulks.py
--rw-r--r--   0 ecorona    (502) staff       (20)      159 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/get_sent_bulks_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      159 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/reschedule_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      162 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/update_scheduled_status.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.314881 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      190 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/add_new_domain.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1128 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      433 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/delivery_reports.py
--rw-r--r--   0 ecorona    (502) staff       (20)      374 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/get_all_domains.py
--rw-r--r--   0 ecorona    (502) staff       (20)      194 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/get_domain_details.py
--rw-r--r--   0 ecorona    (502) staff       (20)      323 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/get_logs.py
--rw-r--r--   0 ecorona    (502) staff       (20)      215 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/get_sent_bulk_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      210 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/get_sent_bulks.py
--rw-r--r--   0 ecorona    (502) staff       (20)      138 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/reschedule_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      390 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/send_email.py
--rw-r--r--   0 ecorona    (502) staff       (20)      140 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/update_scheduled_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      198 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/update_tracking_events.py
--rw-r--r--   0 ecorona    (502) staff       (20)      290 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/validate_email_addresses.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.316866 infobip-api-python-sdk-5.0.0/infobip_channels/mms/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     3936 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/channel.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.318753 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.320011 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/body/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/body/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1899 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/body/send_mms.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.323000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/query_parameters/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/query_parameters/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      179 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/query_parameters/get_inbound_mms_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      250 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/query_parameters/get_mms_delivery_reports.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.328476 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      195 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      632 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/get_inbound_mms_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      991 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/get_mms_delivery_reports.py
--rw-r--r--   0 ecorona    (502) staff       (20)      418 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/send_mms.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.330225 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.331797 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.335041 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/body/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/body/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      239 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/body/send_bulk_rcs_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)     5528 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/body/send_rcs_message.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.336450 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/response/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/response/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      816 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/response/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     2205 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/rcs/channel.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.337897 infobip-api-python-sdk-5.0.0/infobip_channels/sms/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)    26676 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/channel.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.338939 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.355627 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     2730 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      209 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/create_tfa_application.py
--rw-r--r--   0 ecorona    (502) staff       (20)      226 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/create_tfa_message_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      296 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/preview_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      481 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/reschedule_sms_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      214 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/resend_pin_over_sms.py
--rw-r--r--   0 ecorona    (502) staff       (20)      133 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/resend_pin_over_voice.py
--rw-r--r--   0 ecorona    (502) staff       (20)      875 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/send_binary_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1061 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/send_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      402 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/send_pin_over_sms.py
--rw-r--r--   0 ecorona    (502) staff       (20)      125 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/send_pin_over_voice.py
--rw-r--r--   0 ecorona    (502) staff       (20)      162 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/update_scheduled_messages_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      209 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/update_tfa_application.py
--rw-r--r--   0 ecorona    (502) staff       (20)      226 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/update_tfa_message_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      202 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/verify_phone_number.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.361969 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      436 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/tfa_application.py
--rw-r--r--   0 ecorona    (502) staff       (20)      396 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/tfa_application_configuration.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1190 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/tfa_message_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      238 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/tfa_pin_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      234 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/tfa_pin_verification.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.379026 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      119 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      219 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/get_inbound_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      298 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/get_outbound_delivery_reports.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1045 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/get_outbound_logs.py
--rw-r--r--   0 ecorona    (502) staff       (20)      162 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/get_scheduled_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      168 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/get_scheduled_messages_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      220 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/get_tfa_verification_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      160 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/reschedule_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1907 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/send_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      170 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/send_pin_over_sms.py
--rw-r--r--   0 ecorona    (502) staff       (20)      172 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/send_pin_over_voice.py
--rw-r--r--   0 ecorona    (502) staff       (20)      165 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/update_scheduled_messages_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      182 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/verify_phone_number.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.416958 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1151 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      207 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/create_tfa_application.py
--rw-r--r--   0 ecorona    (502) staff       (20)      224 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/create_tfa_message_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      155 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/get_scheduled_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      233 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/get_scheduled_messages_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      204 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/get_tfa_application.py
--rw-r--r--   0 ecorona    (502) staff       (20)      236 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/get_tfa_applications.py
--rw-r--r--   0 ecorona    (502) staff       (20)      221 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/get_tfa_message_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      253 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/get_tfa_message_templates.py
--rw-r--r--   0 ecorona    (502) staff       (20)      300 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/get_tfa_verification_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      770 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/inbound_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      227 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/outbound_delivery_reports.py
--rw-r--r--   0 ecorona    (502) staff       (20)      293 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/outbound_message_logs.py
--rw-r--r--   0 ecorona    (502) staff       (20)      605 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/preview_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      153 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/reschedule_sms_messages.py
--rw-r--r--   0 ecorona    (502) staff       (20)      150 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/resend_pin_over_sms.py
--rw-r--r--   0 ecorona    (502) staff       (20)      158 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/resend_pin_over_voice.py
--rw-r--r--   0 ecorona    (502) staff       (20)      418 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/send_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      190 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/send_pin_over_sms.py
--rw-r--r--   0 ecorona    (502) staff       (20)      192 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/send_pin_over_voice.py
--rw-r--r--   0 ecorona    (502) staff       (20)      163 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/update_scheduled_messages_status.py
--rw-r--r--   0 ecorona    (502) staff       (20)      207 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/update_tfa_application.py
--rw-r--r--   0 ecorona    (502) staff       (20)      224 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/update_tfa_message_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      211 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/verify_phone_number.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.419732 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     4954 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/channel.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.421308 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.428563 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      761 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1234 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/generate_token.py
--rw-r--r--   0 ecorona    (502) staff       (20)      125 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/save_application.py
--rw-r--r--   0 ecorona    (502) staff       (20)      127 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/update_application.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.435511 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/path_parameters/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/path_parameters/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      107 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/path_parameters/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      133 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/path_parameters/web_rtc_application.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.442552 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/response/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/response/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      911 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/response/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      141 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/response/generate_token.py
--rw-r--r--   0 ecorona    (502) staff       (20)      250 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/response/get_applications.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.444651 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)    15555 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/channel.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.449586 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.488370 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      629 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/action_sections.py
--rw-r--r--   0 ecorona    (502) staff       (20)      478 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/audio_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)     2006 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/buttons_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)     2030 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/contact_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      654 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)     3569 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/create_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      626 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/document_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      569 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/image_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)     2357 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/list_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      471 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/location_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)     1239 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/multi_product_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      600 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/product_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      480 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/sticker_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)     2926 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/template_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      379 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/text_message.py
--rw-r--r--   0 ecorona    (502) staff       (20)      569 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/video_message.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.492589 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/path_parameters/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/path_parameters/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      118 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/path_parameters/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      174 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/path_parameters/delete_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      161 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/path_parameters/manage_templates.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.498722 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      630 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      198 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/create_template.py
--rw-r--r--   0 ecorona    (502) staff       (20)      770 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/get_templates.py
--rw-r--r--   0 ecorona    (502) staff       (20)      303 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/template_message.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.499704 infobip-api-python-sdk-5.0.0/infobip_platform/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.501053 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)     4184 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/api.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.501949 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/__init__.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.504142 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/body/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/body/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      185 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/body/create_entity.py
--rw-r--r--   0 ecorona    (502) staff       (20)      221 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/body/modify_entity.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.505607 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/core/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/core/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      268 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/core/entity.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.507047 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/query_parameters/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/query_parameters/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      255 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/query_parameters/get_entities.py
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.512088 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/response/
--rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/response/__init__.py
--rw-r--r--   0 ecorona    (502) staff       (20)      318 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/response/core.py
--rw-r--r--   0 ecorona    (502) staff       (20)      107 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/response/create_entity.py
--rw-r--r--   0 ecorona    (502) staff       (20)      305 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/response/get_entities.py
--rw-r--r--   0 ecorona    (502) staff       (20)      180 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/response/get_entity.py
--rw-r--r--   0 ecorona    (502) staff       (20)      107 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/models/response/modify_entity.py
--rw-r--r--   0 ecorona    (502) staff       (20)      104 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/pyproject.toml
--rw-r--r--   0 ecorona    (502) staff       (20)      847 2023-04-05 19:28:30.523033 infobip-api-python-sdk-5.0.0/setup.cfg
-drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-04-05 19:28:30.518866 infobip-api-python-sdk-5.0.0/tests/
--rw-r--r--   0 ecorona    (502) staff       (20)     2388 2023-04-05 19:19:02.000000 infobip-api-python-sdk-5.0.0/tests/test_core.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.828525 infobip-api-python-sdk-5.0.1/
+-rw-r--r--   0 ecorona    (502) staff       (20)     1114 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/LICENSE
+-rw-r--r--   0 ecorona    (502) staff       (20)     4498 2023-05-26 15:09:19.828838 infobip-api-python-sdk-5.0.1/PKG-INFO
+-rw-r--r--   0 ecorona    (502) staff       (20)     3854 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/README.md
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.827136 infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/
+-rw-r--r--   0 ecorona    (502) staff       (20)     4498 2023-05-26 15:09:19.000000 infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ecorona    (502) staff       (20)    11318 2023-05-26 15:09:19.000000 infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ecorona    (502) staff       (20)        1 2023-05-26 15:09:19.000000 infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ecorona    (502) staff       (20)       51 2023-05-26 15:09:19.000000 infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 ecorona    (502) staff       (20)       34 2023-05-26 15:09:19.000000 infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.671911 infobip-api-python-sdk-5.0.1/infobip_channels/
+-rw-r--r--   0 ecorona    (502) staff       (20)      370 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.676569 infobip-api-python-sdk-5.0.1/infobip_channels/core/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/core/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     9640 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/core/channel.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     3827 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/core/http_client.py
+-rw-r--r--   0 ecorona    (502) staff       (20)    11583 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/core/models.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.678083 infobip-api-python-sdk-5.0.1/infobip_channels/email/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)    15405 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/channel.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.678834 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.684449 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      128 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/add_new_domain.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      416 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/reschedule_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1684 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/send_email.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      157 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/update_scheduled_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      300 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/update_tracking_events.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      129 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/validate_email_addresses.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.689285 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/path_parameters/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/path_parameters/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      119 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/path_parameters/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      154 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/path_parameters/delete_existing_domain.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      150 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/path_parameters/get_domain_details.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      154 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/path_parameters/update_tracking_events.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      146 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/path_parameters/verify_domain.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.697199 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      119 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      244 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/delivery_reports.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      265 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/get_all_domains.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      540 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/get_logs.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      153 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/get_sent_bulks.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      159 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/get_sent_bulks_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      159 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/reschedule_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      162 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/update_scheduled_status.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.709026 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      190 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/add_new_domain.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1128 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      433 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/delivery_reports.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      374 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/get_all_domains.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      194 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/get_domain_details.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      323 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/get_logs.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      215 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/get_sent_bulk_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      210 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/get_sent_bulks.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      138 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/reschedule_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      390 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/send_email.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      140 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/update_scheduled_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      198 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/update_tracking_events.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      290 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/validate_email_addresses.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.710534 infobip-api-python-sdk-5.0.1/infobip_channels/mms/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     3936 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/channel.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.711444 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.713492 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/body/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/body/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1899 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/body/send_mms.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.716579 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/query_parameters/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/query_parameters/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      179 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/query_parameters/get_inbound_mms_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      250 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/query_parameters/get_mms_delivery_reports.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.720291 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      195 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      632 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/get_inbound_mms_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      991 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/get_mms_delivery_reports.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      418 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/send_mms.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.721706 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.722658 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.725343 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/body/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/body/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      239 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/body/send_bulk_rcs_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     5528 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/body/send_rcs_message.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.726840 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/response/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/response/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      816 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/response/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     2205 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/rcs/channel.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.729025 infobip-api-python-sdk-5.0.1/infobip_channels/sms/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)    26676 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/channel.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.729871 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.742406 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     2730 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      209 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/create_tfa_application.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      226 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/create_tfa_message_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      296 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/preview_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      481 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/reschedule_sms_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      214 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/resend_pin_over_sms.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      133 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/resend_pin_over_voice.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      875 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/send_binary_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1061 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/send_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      402 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/send_pin_over_sms.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      125 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/send_pin_over_voice.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      162 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/update_scheduled_messages_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      209 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/update_tfa_application.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      226 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/update_tfa_message_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      202 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/verify_phone_number.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.746224 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      436 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/tfa_application.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      396 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/tfa_application_configuration.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1190 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/tfa_message_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      238 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/tfa_pin_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      234 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/tfa_pin_verification.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.758878 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      119 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      219 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/get_inbound_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      298 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/get_outbound_delivery_reports.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1045 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/get_outbound_logs.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      162 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/get_scheduled_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      168 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/get_scheduled_messages_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      220 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/get_tfa_verification_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      160 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/reschedule_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1907 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/send_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      170 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/send_pin_over_sms.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      172 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/send_pin_over_voice.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      165 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/update_scheduled_messages_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      182 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/verify_phone_number.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.779396 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1151 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      207 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/create_tfa_application.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      224 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/create_tfa_message_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      155 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/get_scheduled_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      233 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/get_scheduled_messages_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      204 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/get_tfa_application.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      236 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/get_tfa_applications.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      221 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/get_tfa_message_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      253 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/get_tfa_message_templates.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      300 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/get_tfa_verification_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      770 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/inbound_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      227 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/outbound_delivery_reports.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      293 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/outbound_message_logs.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      605 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/preview_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      153 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/reschedule_sms_messages.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      150 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/resend_pin_over_sms.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      158 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/resend_pin_over_voice.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      418 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/send_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      190 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/send_pin_over_sms.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      192 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/send_pin_over_voice.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      163 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/update_scheduled_messages_status.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      207 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/update_tfa_application.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      224 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/update_tfa_message_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      211 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/verify_phone_number.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.781301 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     4954 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/channel.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.782081 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.785164 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      761 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1234 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/generate_token.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      125 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/save_application.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      127 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/update_application.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.787057 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/path_parameters/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/path_parameters/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      107 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/path_parameters/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      133 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/path_parameters/web_rtc_application.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.789400 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/response/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/response/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      911 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/response/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      141 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/response/generate_token.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      250 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/response/get_applications.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.791233 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)    15555 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/channel.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.792114 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.803492 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      629 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/action_sections.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      478 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/audio_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     2006 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/buttons_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     2030 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/contact_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      654 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     3569 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/create_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      626 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/document_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      569 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/image_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     2357 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/list_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      471 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/location_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     1239 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/multi_product_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      600 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/product_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      480 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/sticker_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     2926 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/template_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      379 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/text_message.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      569 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/video_message.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.806115 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/path_parameters/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/path_parameters/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      118 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/path_parameters/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      174 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/path_parameters/delete_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      161 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/path_parameters/manage_templates.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.810446 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      630 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      198 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/create_template.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      770 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/get_templates.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      303 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/template_message.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.811221 infobip-api-python-sdk-5.0.1/infobip_platform/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.812811 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)     4184 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/api.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.813553 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/__init__.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.815607 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/body/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/body/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      185 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/body/create_entity.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      221 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/body/modify_entity.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.816611 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/core/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/core/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      268 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/core/entity.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.817524 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/query_parameters/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/query_parameters/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      255 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/query_parameters/get_entities.py
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.821707 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/response/
+-rw-r--r--   0 ecorona    (502) staff       (20)        0 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/response/__init__.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      318 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/response/core.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      107 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/response/create_entity.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      305 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/response/get_entities.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      180 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/response/get_entity.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      107 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/models/response/modify_entity.py
+-rw-r--r--   0 ecorona    (502) staff       (20)      104 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/pyproject.toml
+-rw-r--r--   0 ecorona    (502) staff       (20)      848 2023-05-26 15:09:19.830455 infobip-api-python-sdk-5.0.1/setup.cfg
+drwxr-xr-x   0 ecorona    (502) staff       (20)        0 2023-05-26 15:09:19.827854 infobip-api-python-sdk-5.0.1/tests/
+-rw-r--r--   0 ecorona    (502) staff       (20)     2388 2023-05-26 15:01:35.000000 infobip-api-python-sdk-5.0.1/tests/test_core.py
```

### Comparing `infobip-api-python-sdk-5.0.0/LICENSE` & `infobip-api-python-sdk-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/PKG-INFO` & `infobip-api-python-sdk-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infobip-api-python-sdk
-Version: 5.0.0
+Version: 5.0.1
 Summary: Python sdk for Infobip's API
 Home-page: https://github.com/infobip-community/infobip-api-python-sdk
 Author: Luka Kilic, Dino Lozina, Erick Corona
 Author-email: DevRel@infobip.com
 Project-URL: Bug Tracker, https://github.com/infobip-community/infobip-api-python-sdk/issues
 Keywords: infobip,sdk,channels,sms,whatsapp,email,webrtc,mms,api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infobip-api-python-sdk-5.0.0/README.md` & `infobip-api-python-sdk-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/PKG-INFO` & `infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infobip-api-python-sdk
-Version: 5.0.0
+Version: 5.0.1
 Summary: Python sdk for Infobip's API
 Home-page: https://github.com/infobip-community/infobip-api-python-sdk
 Author: Luka Kilic, Dino Lozina, Erick Corona
 Author-email: DevRel@infobip.com
 Project-URL: Bug Tracker, https://github.com/infobip-community/infobip-api-python-sdk/issues
 Keywords: infobip,sdk,channels,sms,whatsapp,email,webrtc,mms,api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infobip-api-python-sdk-5.0.0/infobip_api_python_sdk.egg-info/SOURCES.txt` & `infobip-api-python-sdk-5.0.1/infobip_api_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/core/channel.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/core/channel.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/core/http_client.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/core/http_client.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/core/models.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/core/models.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/email/channel.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/email/channel.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/email/models/body/send_email.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/email/models/body/send_email.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/email/models/query_parameters/get_logs.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/email/models/query_parameters/get_logs.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/email/models/response/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/email/models/response/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/mms/channel.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/mms/channel.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/body/send_mms.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/body/send_mms.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/get_inbound_mms_messages.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/get_inbound_mms_messages.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/mms/models/response/get_mms_delivery_reports.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/mms/models/response/get_mms_delivery_reports.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/body/send_rcs_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/body/send_rcs_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/rcs/Models/response/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/rcs/Models/response/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/rcs/channel.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/rcs/channel.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/channel.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/channel.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/send_binary_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/send_binary_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/body/send_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/body/send_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/core/tfa_message_template.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/core/tfa_message_template.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/get_outbound_logs.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/get_outbound_logs.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/query_parameters/send_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/query_parameters/send_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/inbound_messages.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/inbound_messages.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/sms/models/response/preview_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/sms/models/response/preview_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/channel.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/channel.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/body/generate_token.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/body/generate_token.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/web_rtc/models/response/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/web_rtc/models/response/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/channel.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/channel.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/action_sections.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/action_sections.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/buttons_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/buttons_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/contact_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/contact_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/create_template.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/create_template.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/document_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/document_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/image_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/image_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/list_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/list_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/multi_product_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/multi_product_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/product_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/product_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/template_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/template_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/body/video_message.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/body/video_message.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/core.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/core.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_channels/whatsapp/models/response/get_templates.py` & `infobip-api-python-sdk-5.0.1/infobip_channels/whatsapp/models/response/get_templates.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/infobip_platform/app_entities/api.py` & `infobip-api-python-sdk-5.0.1/infobip_platform/app_entities/api.py`

 * *Files identical despite different names*

### Comparing `infobip-api-python-sdk-5.0.0/setup.cfg` & `infobip-api-python-sdk-5.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = infobip-api-python-sdk
-version = 5.0.0
+version = 5.0.1
 author = Luka Kilic, Dino Lozina, Erick Corona
 author_email = DevRel@infobip.com
 description = Python sdk for Infobip's API
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = infobip, sdk, channels, sms, whatsapp, email, webrtc, mms, api
 url = https://github.com/infobip-community/infobip-api-python-sdk
@@ -17,17 +17,17 @@
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	pydantic==1.9.0
-	requests==2.27.1
-	regex==2022.3.15
+	pydantic~=1.10.8
+	requests~=2.31.0
+	regex~=2022.3.15
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `infobip-api-python-sdk-5.0.0/tests/test_core.py` & `infobip-api-python-sdk-5.0.1/tests/test_core.py`

 * *Files identical despite different names*


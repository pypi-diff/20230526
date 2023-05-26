# Comparing `tmp/cherwell_pydantic_api-0.0.3.tar.gz` & `tmp/cherwell_pydantic_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherwell_pydantic_api-0.0.3.tar", max compression
+gzip compressed data, was "cherwell_pydantic_api-0.0.4.tar", max compression
```

## Comparing `cherwell_pydantic_api-0.0.3.tar` & `cherwell_pydantic_api-0.0.4.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1116 2023-03-22 07:46:47.868533 cherwell_pydantic_api-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     1319 2023-03-24 16:48:45.840721 cherwell_pydantic_api-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-03-24 10:49:18.447842 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/__init__.py
--rw-r--r--   0        0        0       61 2023-03-21 17:35:37.123101 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/__main__.py
--rw-r--r--   0        0        0        0 2023-03-19 11:38:25.782849 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/__init__.py
--rw-r--r--   0        0        0     3729 2023-03-22 21:12:46.838028 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Approval.py
--rw-r--r--   0        0        0    69093 2023-03-22 21:12:47.276035 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py
--rw-r--r--   0        0        0    17154 2023-03-22 21:12:47.394037 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Core.py
--rw-r--r--   0        0        0     6515 2023-03-22 21:12:47.439037 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Forms.py
--rw-r--r--   0        0        0     7155 2023-03-22 21:12:47.484038 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py
--rw-r--r--   0        0        0     9966 2023-03-22 21:12:47.549039 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py
--rw-r--r--   0        0        0     8838 2023-03-22 21:12:47.608040 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Queues.py
--rw-r--r--   0        0        0    42096 2023-03-22 21:12:47.954046 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Searches.py
--rw-r--r--   0        0        0    25601 2023-03-22 21:12:48.114049 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Security.py
--rw-r--r--   0        0        0     4662 2023-03-22 21:12:48.142049 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Service.py
--rw-r--r--   0        0        0    15417 2023-03-22 21:12:48.314052 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Teams.py
--rw-r--r--   0        0        0    15747 2023-03-22 21:12:48.410054 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Users.py
--rw-r--r--   0        0        0      788 2023-03-22 21:12:48.417054 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/__init__.py
--rw-r--r--   0        0        0     1016 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py
--rw-r--r--   0        0        0    14554 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py
--rw-r--r--   0        0        0     8790 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Core.py
--rw-r--r--   0        0        0     1517 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py
--rw-r--r--   0        0        0     2865 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Lifecycle.py
--rw-r--r--   0        0        0     1086 2023-03-22 20:34:06.750498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py
--rw-r--r--   0        0        0     2777 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py
--rw-r--r--   0        0        0    15593 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Searches.py
--rw-r--r--   0        0        0     8542 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Security.py
--rw-r--r--   0        0        0     4787 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Teams.py
--rw-r--r--   0        0        0     7824 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Users.py
--rw-r--r--   0        0        0      481 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/__init__.py
--rw-r--r--   0        0        0      106 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/__init__.py
--rw-r--r--   0        0        0      642 2023-03-22 20:34:06.751499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py
--rw-r--r--   0        0        0   774308 2023-03-22 20:34:06.754499 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/__init__.py
--rw-r--r--   0        0        0     8096 2023-03-26 11:47:33.549850 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/api.py
--rw-r--r--   0        0        0        0 2023-03-22 21:08:27.552764 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/__init__.py
--rw-r--r--   0        0        0     2433 2023-03-23 18:10:18.008072 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/model_base.py
--rw-r--r--   0        0        0        0 2023-03-21 10:59:09.605023 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/__init__.py
--rw-r--r--   0        0        0     8693 2023-04-13 18:11:05.072587 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/collector.py
--rw-r--r--   0        0        0     4504 2023-04-13 18:11:19.745824 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/model_generator.py
--rw-r--r--   0        0        0     7132 2023-04-13 18:11:31.563014 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/repo.py
--rw-r--r--   0        0        0     9015 2023-03-28 09:22:12.005006 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/registry.py
--rw-r--r--   0        0        0      504 2023-04-13 17:50:00.815498 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/base.py.j2
--rw-r--r--   0        0        0      949 2023-03-21 16:09:57.127883 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/dot_gitignore
--rw-r--r--   0        0        0     1618 2023-04-13 15:40:06.593367 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/model.py.j2
--rw-r--r--   0        0        0     2507 2023-04-13 17:21:15.916322 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/valid_schema.py
--rw-r--r--   0        0        0     1859 2023-03-22 18:17:35.702277 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/wrapper.py
--rw-r--r--   0        0        0     3514 2023-04-13 20:28:04.639752 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/__init__.py
--rw-r--r--   0        0        0      720 2023-03-24 17:04:55.919724 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/check.py
--rwxr-xr-x   0        0        0     3700 2023-03-24 19:02:21.683110 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/ipython.py
--rw-r--r--   0        0        0     2262 2023-04-13 18:10:09.585693 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/repo.py
--rw-r--r--   0        0        0      530 2023-04-13 17:00:06.941981 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/utils.py
--rw-r--r--   0        0        0     3775 2023-04-13 17:10:51.016290 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/welcome.py
--rw-r--r--   0        0        0    15776 2023-04-13 20:36:03.816552 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/examples/GettingStarted.ipynb
--rw-r--r--   0        0        0     4839 2023-04-11 17:44:23.221370 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/generated_api_utils.py
--rw-r--r--   0        0        0     4504 2023-03-26 11:50:21.378612 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/instance.py
--rw-r--r--   0        0        0     5392 2023-03-27 13:23:32.152829 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interactive.py
--rw-r--r--   0        0        0     1013 2023-03-21 13:34:01.763557 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interfaces.py
--rw-r--r--   0        0        0        0 2023-03-15 17:53:17.042051 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/py.typed
--rw-r--r--   0        0        0     9766 2023-04-11 17:44:47.629821 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/__init__.py
--rw-r--r--   0        0        0     2253 2023-03-15 16:15:32.831474 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/fields.py
--rw-r--r--   0        0        0     3557 2023-03-24 14:12:48.922113 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/settings.py
--rw-r--r--   0        0        0     3916 2023-03-23 18:05:54.954794 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/types.py
--rw-r--r--   0        0        0     1149 2023-03-26 12:00:50.198963 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/utils.py
--rw-r--r--   0        0        0     1348 2023-03-24 12:08:49.757333 cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/validators.py
--rw-r--r--   0        0        0     2356 2023-04-13 18:42:00.570801 cherwell_pydantic_api-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3378 1970-01-01 00:00:00.000000 cherwell_pydantic_api-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1116 2023-03-22 07:46:47.868533 cherwell_pydantic_api-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1319 2023-03-24 16:48:45.840721 cherwell_pydantic_api-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-24 10:49:18.447842 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-21 17:35:37.123101 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-19 11:38:25.782849 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/__init__.py
+-rw-r--r--   0        0        0     3809 2023-04-16 20:21:51.418689 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Approval.py
+-rw-r--r--   0        0        0    69706 2023-04-16 20:21:52.247703 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py
+-rw-r--r--   0        0        0    17493 2023-04-16 20:21:52.376705 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Core.py
+-rw-r--r--   0        0        0     6659 2023-04-16 20:21:52.430706 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Forms.py
+-rw-r--r--   0        0        0     7283 2023-04-16 20:21:52.504707 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py
+-rw-r--r--   0        0        0    10190 2023-04-16 20:21:52.705710 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py
+-rw-r--r--   0        0        0     9046 2023-04-16 20:21:52.769711 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Queues.py
+-rw-r--r--   0        0        0    43004 2023-04-16 20:21:53.025716 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Searches.py
+-rw-r--r--   0        0        0    25857 2023-04-16 20:21:53.270720 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Security.py
+-rw-r--r--   0        0        0     4713 2023-04-16 20:21:53.303720 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Service.py
+-rw-r--r--   0        0        0    15618 2023-04-16 20:21:53.404722 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Teams.py
+-rw-r--r--   0        0        0    16019 2023-04-16 20:21:53.513724 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Users.py
+-rw-r--r--   0        0        0      788 2023-04-16 20:21:53.521724 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     1148 2023-04-16 20:21:51.187685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py
+-rw-r--r--   0        0        0    16930 2023-04-16 20:21:51.187685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py
+-rw-r--r--   0        0        0     9978 2023-04-16 20:21:51.187685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Core.py
+-rw-r--r--   0        0        0     1715 2023-04-16 20:21:51.187685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py
+-rw-r--r--   0        0        0     3525 2023-04-16 20:21:51.187685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Lifecycle.py
+-rw-r--r--   0        0        0     1218 2023-04-16 20:21:51.188685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py
+-rw-r--r--   0        0        0     3305 2023-04-16 20:21:51.188685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py
+-rw-r--r--   0        0        0    17573 2023-04-16 20:21:51.188685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Searches.py
+-rw-r--r--   0        0        0    10060 2023-04-16 20:21:51.188685 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Security.py
+-rw-r--r--   0        0        0     5843 2023-04-16 20:21:51.198686 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Teams.py
+-rw-r--r--   0        0        0     9210 2023-04-16 20:21:51.198686 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Users.py
+-rw-r--r--   0        0        0      547 2023-04-16 20:21:51.198686 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-16 20:21:51.198686 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/__init__.py
+-rw-r--r--   0        0        0      708 2023-04-16 20:21:51.198686 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py
+-rw-r--r--   0        0        0   774410 2023-04-16 20:21:51.201686 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/__init__.py
+-rw-r--r--   0        0        0     8339 2023-04-25 14:39:19.727619 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/api.py
+-rw-r--r--   0        0        0        0 2023-03-22 21:08:27.552764 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/__init__.py
+-rw-r--r--   0        0        0    16341 2023-04-26 11:23:48.178890 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/model_base.py
+-rw-r--r--   0        0        0        0 2023-03-21 10:59:09.605023 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/modelgen/__init__.py
+-rw-r--r--   0        0        0     9501 2023-04-19 14:00:56.270725 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/modelgen/collector.py
+-rw-r--r--   0        0        0     6579 2023-04-26 12:41:47.082279 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/modelgen/model_generator.py
+-rw-r--r--   0        0        0     7790 2023-04-16 20:10:49.992750 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/modelgen/repo.py
+-rw-r--r--   0        0        0    11513 2023-04-18 16:10:32.008739 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/registry.py
+-rw-r--r--   0        0        0      591 2023-04-19 12:24:44.942673 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/templates/base.py.j2
+-rw-r--r--   0        0        0      949 2023-03-21 16:09:57.127883 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/templates/dot_gitignore
+-rw-r--r--   0        0        0     4039 2023-04-20 15:28:11.499420 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/templates/model.py.j2
+-rw-r--r--   0        0        0     4091 2023-04-19 13:58:30.582383 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/valid_schema.py
+-rw-r--r--   0        0        0     1859 2023-03-22 18:17:35.702277 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/wrapper.py
+-rw-r--r--   0        0        0     3633 2023-04-27 12:01:33.359450 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/__init__.py
+-rw-r--r--   0        0        0      823 2023-04-27 12:31:20.074658 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/check.py
+-rwxr-xr-x   0        0        0     3895 2023-04-27 12:31:13.235545 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/ipython.py
+-rw-r--r--   0        0        0     3904 2023-04-27 12:30:46.123102 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/repo.py
+-rw-r--r--   0        0        0      724 2023-04-19 16:13:08.995868 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/utils.py
+-rw-r--r--   0        0        0     4191 2023-04-19 16:18:40.693351 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/welcome.py
+-rw-r--r--   0        0        0    15776 2023-04-13 20:36:03.816552 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/examples/GettingStarted.ipynb
+-rw-r--r--   0        0        0     5516 2023-04-18 16:01:03.780305 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/generated_api_utils.py
+-rw-r--r--   0        0        0     4786 2023-04-17 08:56:12.663755 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/instance.py
+-rw-r--r--   0        0        0     5555 2023-04-19 13:29:33.250417 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/interactive.py
+-rw-r--r--   0        0        0     2425 2023-04-21 15:25:39.169733 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/intercept_transport.py
+-rw-r--r--   0        0        0     1013 2023-03-21 13:34:01.763557 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/interfaces.py
+-rw-r--r--   0        0        0        0 2023-03-15 17:53:17.042051 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/py.typed
+-rw-r--r--   0        0        0     9863 2023-04-16 20:15:27.907344 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/schema/__init__.py
+-rw-r--r--   0        0        0     2352 2023-04-16 20:15:42.031578 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/schema/fields.py
+-rw-r--r--   0        0        0     3890 2023-04-25 14:39:19.727619 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/settings.py
+-rw-r--r--   0        0        0     4305 2023-04-19 12:17:06.775267 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/types.py
+-rw-r--r--   0        0        0     1387 2023-04-19 13:52:32.694632 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/utils.py
+-rw-r--r--   0        0        0     3091 2023-04-25 16:41:07.537516 cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/validators.py
+-rw-r--r--   0        0        0     2702 2023-05-26 07:10:51.897549 cherwell_pydantic_api-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3280 1970-01-01 00:00:00.000000 cherwell_pydantic_api-0.0.4/PKG-INFO
```

### Comparing `cherwell_pydantic_api-0.0.3/LICENSE.md` & `cherwell_pydantic_api-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.3/README.md` & `cherwell_pydantic_api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Approval.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Approval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class ApprovalInterface(GeneratedInterfaceBase):
     async def ActionApprovalV1(
         self,
         approvalRecId: str,
         approvalAction: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse
+    ):
         """Action an Approval
 
         Operation that actions an Approval Business Object. Use this method, passing either approve, abstain or deny to update the Business Object's state
          :param approvalRecId:
          :param approvalAction:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse
         """
@@ -25,15 +27,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse,
         )
 
     async def GetApprovalByRecIdV1(
         self,
         approvalRecId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.ApprovalReadResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.ApprovalReadResponse
+    ):
         """Get Approval
 
         Operation that returns an Approval Business Object.  Use the provided links to action the Approval
          :param approvalRecId:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.ApprovalReadResponse
         """
         self.validate_path_param(approvalRecId, str)
@@ -41,29 +45,33 @@
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.ApprovalReadResponse,
         )
 
     async def GetMyApprovalsV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.GetApprovalsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.GetApprovalsResponse
+    ):
         """Get all waiting Approvals for the current user
 
         Operation that returns a list of Approval Business Objects that are in a state of 'Waiting' for the current user.  Use the provided links to action the Approval
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.GetApprovalsResponse
         """
         response = await self.get("/api/V1/getmyapprovals")
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.GetApprovalsResponse,
         )
 
     async def GetMyPendingApprovalsV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.GetApprovalsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.GetApprovalsResponse
+    ):
         """Get all waiting approvals that were created by the current user
 
         Operation that returns a list of Approval Business Objects that are in a state of 'Waiting' that were created by the current user.  Use the provided links to action the Approval
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Approval.GetApprovalsResponse
         """
         response = await self.get("/api/V1/getmypendingapprovals")
         return self.parse_response(
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/BusinessObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches
 import cherwell_pydantic_api.types
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class BusinessObjectInterface(GeneratedInterfaceBase):
     async def DeleteBusinessObjectBatchV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchDeleteRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchDeleteResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchDeleteResponse
+    ):
         """Delete Business Objects in a batch
 
         Operation to delete a batch of Business Objects.
          :param request: Specify an array of Business Object IDs and record IDs or public IDs. Use a flag to stop on error or continue on error.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchDeleteResponse
         """
         response = await self.post_body(
@@ -27,15 +29,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchDeleteResponse,
         )
 
     async def DeleteBusinessObjectByPublicIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         publicid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.DeleteResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.DeleteResponse
+    ):
         """Delete a Business Object by public ID
 
         Operation to delete a Business Object by Business Object ID.
          :param busobid: Specify the Business Object ID.
          :param publicid: Specify the Business Object public ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.DeleteResponse
         """
@@ -49,15 +53,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.DeleteResponse,
         )
 
     async def DeleteBusinessObjectByRecIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.DeleteResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.DeleteResponse
+    ):
         """Delete a Business Object by record ID
 
         Operation to delete a single Business Object.
          :param busobid: Specify the Business Object ID.
          :param busobrecid:  Specify the Business Object record ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.DeleteResponse
         """
@@ -73,15 +79,17 @@
 
     async def DeleteRelatedBusinessObjectByPublicIdV1(
         self,
         parentbusobid: cherwell_pydantic_api.types.BusObIDParamType,
         parentbusobrecid: cherwell_pydantic_api.types.BusObRecID,
         relationshipid: cherwell_pydantic_api.types.RelationshipID,
         publicid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
+    ):
         """Delete a related Business Object by public ID
 
         Operation to delete a related Business Object. (Use "Unlink Related Business Object" to unlink two Business Objects rather that deleting the related Business Object.)
          :param parentbusobid: Specify the Business Object ID for the parent Business Object.
          :param parentbusobrecid: Specify the record ID for the parent Business Object
          :param relationshipid: Specify the Relationship ID for the related Business Object you want to delete.
          :param publicid: Specify the public ID for the related Business Object you want to delete. Use only for Business Objects with unique public IDs. Use "Delete a related Business Object by record ID" when public IDs are not unique.
@@ -107,15 +115,17 @@
 
     async def DeleteRelatedBusinessObjectByRecIdV1(
         self,
         parentbusobid: cherwell_pydantic_api.types.BusObIDParamType,
         parentbusobrecid: cherwell_pydantic_api.types.BusObRecID,
         relationshipid: cherwell_pydantic_api.types.RelationshipID,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
+    ):
         """Delete a related Business Object by record ID
 
         Operation to delete a related Business Object. (Use "Unlink Related Business Object" to unlink two Business Objects rather that deleting the related Business Object.)
          :param parentbusobid: Specify the Business Object ID for the parent Business Object.
          :param parentbusobrecid: Specify the record ID for the parent Business Object
          :param relationshipid: Specify the Relationship ID for the related Business Object you want to delete.
          :param busobrecid: Specify the record ID for the related Business Object you want to delete.
@@ -138,15 +148,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse,
         )
 
     async def FieldValuesLookupV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.FieldValuesLookupRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.FieldValuesLookupResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.FieldValuesLookupResponse
+    ):
         """Get lookup values for fields
 
         Operation to get potentially valid values for Business Object fields.
          :param request: Request object that specifies the Business Object and fields for which values are to be returned.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.FieldValuesLookupResponse
         """
         response = await self.post_body(
@@ -178,15 +190,15 @@
          :param pageSize: Specify the number of rows to return per page. Maximum value is 2000 per page.
          :param pageNumber: Specify the page number of the result set to return.
          :param activityType: The category of activities to retrieve. Will default to All if not specified.
          :return: list[cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BusObActivity]
         """
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
-        params = {}
+        params: dict[str, Any] = {}
         if pageNumber is not None:
             params["pageNumber"] = pageNumber
         if activityType is not None:
             params["activityType"] = activityType
         response = await self.get(
             f"/api/V1/getactivities/busobid/{busobid}/busobrecid/{busobrecid}/pagesize/{pageSize}",
             params=params,
@@ -213,24 +225,26 @@
          :return: cherwell_pydantic_api.types.FileDownload"""
         self.validate_path_param(attachmentid, str)
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
         response = await self.get(
             f"/api/V1/getbusinessobjectattachment/attachmentid/{attachmentid}/busobid/{busobid}/busobrecid/{busobrecid}"
         )
-        return self.parse_response(response, cherwell_pydantic_api.types.FileDownload)
+        return self.download_response(response)
 
     async def GetBusinessObjectAttachmentsByIdAndPublicIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         publicid: str,
         type: cherwell_pydantic_api.types.RecordAttachmentType,
         attachmenttype: cherwell_pydantic_api.types.AttachmentType,
         includelinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Get attachments by Business Object public ID
 
         Operation to get attachments for a Business Object by Business Object ID and public ID.
          :param busobid: Specify the Business Object ID.
          :param publicid: Specify the Business Object public ID for the record that contains the attachments.
          :param type: Record attachment type:
 
@@ -258,15 +272,15 @@
         """
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(publicid, str)
         self.validate_path_param(type, cherwell_pydantic_api.types.RecordAttachmentType)
         self.validate_path_param(
             attachmenttype, cherwell_pydantic_api.types.AttachmentType
         )
-        params = {}
+        params: dict[str, Any] = {}
         if includelinks is not None:
             params["includelinks"] = includelinks
         response = await self.get(
             f"/api/V1/getbusinessobjectattachments/busobid/{busobid}/publicid/{publicid}/type/{type}/attachmenttype/{attachmenttype}",
             params=params,
         )
         return self.parse_response(
@@ -277,15 +291,17 @@
     async def GetBusinessObjectAttachmentsByIdAndRecIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
         type: cherwell_pydantic_api.types.RecordAttachmentType,
         attachmenttype: cherwell_pydantic_api.types.AttachmentType,
         includelinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Get attachments by Business Object record ID
 
         Operation to get attachments for a Business Object by Business Object ID and record ID.
          :param busobid: Specify the Business Object ID.
          :param busobrecid: Specify the Business Object record ID.
          :param type: Record attachment type:
 
@@ -313,15 +329,15 @@
         """
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
         self.validate_path_param(type, cherwell_pydantic_api.types.RecordAttachmentType)
         self.validate_path_param(
             attachmenttype, cherwell_pydantic_api.types.AttachmentType
         )
-        params = {}
+        params: dict[str, Any] = {}
         if includelinks is not None:
             params["includelinks"] = includelinks
         response = await self.get(
             f"/api/V1/getbusinessobjectattachments/busobid/{busobid}/busobrecid/{busobrecid}/type/{type}/attachmenttype/{attachmenttype}",
             params=params,
         )
         return self.parse_response(
@@ -332,15 +348,17 @@
     async def GetBusinessObjectAttachmentsByNameAndPublicIdV1(
         self,
         busobname: str,
         publicid: str,
         type: cherwell_pydantic_api.types.RecordAttachmentType,
         attachmenttype: cherwell_pydantic_api.types.AttachmentType,
         includelinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Get attachments by Business Object name and public ID
 
         Operation to get attachments for a Business Object by Business Object Name and public ID.
          :param busobname: Specify the Business Object name.
          :param publicid: Specify the Business Object public ID for the record that contains the attachments.
          :param type: Record attachment type:
 
@@ -368,15 +386,15 @@
         """
         self.validate_path_param(busobname, str)
         self.validate_path_param(publicid, str)
         self.validate_path_param(type, cherwell_pydantic_api.types.RecordAttachmentType)
         self.validate_path_param(
             attachmenttype, cherwell_pydantic_api.types.AttachmentType
         )
-        params = {}
+        params: dict[str, Any] = {}
         if includelinks is not None:
             params["includelinks"] = includelinks
         response = await self.get(
             f"/api/V1/getbusinessobjectattachments/busobname/{busobname}/publicid/{publicid}/type/{type}/attachmenttype/{attachmenttype}",
             params=params,
         )
         return self.parse_response(
@@ -387,15 +405,17 @@
     async def GetBusinessObjectAttachmentsByNameAndRecIdV1(
         self,
         busobname: str,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
         type: cherwell_pydantic_api.types.RecordAttachmentType,
         attachmenttype: cherwell_pydantic_api.types.AttachmentType,
         includelinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Get attachments by Business Object name and record ID
 
         Operation to get attachments for a Business Object by name and record ID.
          :param busobname: Specify the Business Object name.
          :param busobrecid: Specify the Business Object record ID.
          :param type: Record attachment type:
 
@@ -423,30 +443,32 @@
         """
         self.validate_path_param(busobname, str)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
         self.validate_path_param(type, cherwell_pydantic_api.types.RecordAttachmentType)
         self.validate_path_param(
             attachmenttype, cherwell_pydantic_api.types.AttachmentType
         )
-        params = {}
+        params: dict[str, Any] = {}
         if includelinks is not None:
             params["includelinks"] = includelinks
         response = await self.get(
             f"/api/V1/getbusinessobjectattachments/busobname/{busobname}/busobrecid/{busobrecid}/type/{type}/attachmenttype/{attachmenttype}",
             params=params,
         )
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse,
         )
 
     async def GetBusinessObjectAttachmentsV1(
         self,
         attachmentsRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Get Business Object attachments by request object
 
         Operation to get attachments for a Business Object by attachments request object.
          :param attachmentsRequest: Object with all the parameters to request an attachments list. You can also request a list of types to get more than just one type at a time.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
         """
         response = await self.post_body(
@@ -457,15 +479,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse,
         )
 
     async def GetBusinessObjectBatchV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchReadRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchReadResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchReadResponse
+    ):
         """Get a batch of Business Object records
 
         Operation that returns a batch of Business Object records that includes a list of field record IDs, display names, and values for each record.
          :param request: Specify an array of Business Object IDs, record IDs, or public IDs. Use a flag to stop on error or continue on error.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchReadResponse
         """
         response = await self.post_body(
@@ -477,15 +501,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchReadResponse,
         )
 
     async def GetBusinessObjectByPublicIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         publicid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse
+    ):
         """Get a Business Object record
 
         Operation that returns a Business Object record that includes a list of fields and their record IDs, names, and set values.
          :param busobid: Specify the Business Object ID.
          :param publicid: Specify the Business Object public ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse
         """
@@ -499,15 +525,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse,
         )
 
     async def GetBusinessObjectByRecIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse
+    ):
         """Get a Business Object record
 
         Operation that returns a Business Object record that includes a list of fields and their record IDs, names, and set values.
          :param busobid: Specify the Business Object ID.
          :param busobrecid: Specify the Business Object record ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse
         """
@@ -521,15 +549,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.ReadResponse,
         )
 
     async def GetBusinessObjectByScanCodeBusObIdV1(
         self,
         scanCode: str,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse
+    ):
         """Get a Business Object by its scan code and Business Object ID
 
         Operation to get a Business Object based on its associated scan code and Business Object ID.
          :param scanCode: The scan code for a Business Object record.
          :param busobid: The Business Object ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse
         """
@@ -543,15 +573,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse,
         )
 
     async def GetBusinessObjectByScanCodeBusObNameV1(
         self,
         scanCode: str,
         busobname: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse
+    ):
         """Get a Business Object by its scan code and Business Object name
 
         Operation to get a Business Object based on its associated scan code and Business Object name.
          :param scanCode: The scan code for a Business Object record.
          :param busobname: The Business Bbject name.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse
         """
@@ -565,24 +597,26 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BarcodeLookupResponse,
         )
 
     async def GetBusinessObjectSchemaV1(
         self,
         busobId: cherwell_pydantic_api.types.BusObIDParamType,
         includerelationships: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SchemaResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SchemaResponse
+    ):
         """Get a Business Object schema
 
         Operation that returns the schema for a Business Object and, optionally, its related Business Objects.
          :param busobId: Specify the Business Object ID.
          :param includerelationships: Flag to include schemas for related Business Object. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SchemaResponse
         """
         self.validate_path_param(busobId, cherwell_pydantic_api.types.BusObIDParamType)
-        params = {}
+        params: dict[str, Any] = {}
         if includerelationships is not None:
             params["includerelationships"] = includerelationships
         response = await self.get(
             f"/api/V1/getbusinessobjectschema/busobid/{busobId}", params=params
         )
         return self.parse_response(
             response,
@@ -658,15 +692,17 @@
                 cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.Summary
             ],
         )
 
     async def GetBusinessObjectTemplateV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.TemplateRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.TemplateResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.TemplateResponse
+    ):
         """Get Business Object templates for create
 
         Operation that returns a template to create Business Objects.  The template includes placeholders for field values. You can then send the template with these values to the Business Object Save operation.
          :param request: Specify the Business Object ID. Use true to include all required fields or all fields. Specify an optional fields list by adding field names in a comma-delimited list ["field1", "field2"].
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.TemplateResponse
         """
         response = await self.post_body(
@@ -678,23 +714,25 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.TemplateResponse,
         )
 
     async def GetRelatedBusinessObjectByRequestV1(
         self,
         relatedBusinessObjectRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectRequest,
         includelinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
+    ):
         """Get related Business Objects using a request object
 
         Operation to get related Business Objects for a specific relationship. Specify a list of fields to include in the response. The order of parameter usage and overrides is: all fields set to true overrides default overrides;  custom grid overrides field list settings.
          :param relatedBusinessObjectRequest: Request object containing all the possible parameters to get related Business Objects.
          :param includelinks: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
         """
-        params = {}
+        params: dict[str, Any] = {}
         if includelinks is not None:
             params["includelinks"] = includelinks
         response = await self.post_body(
             "/api/V1/getrelatedbusinessobject",
             params=params,
             content=relatedBusinessObjectRequest.json(
                 exclude_unset=True, by_alias=True
@@ -711,15 +749,17 @@
         parentbusobrecid: cherwell_pydantic_api.types.BusObRecID,
         relationshipid: cherwell_pydantic_api.types.RelationshipID,
         pageNumber: Optional[int] = None,
         pageSize: Optional[int] = None,
         allfields: Optional[bool] = None,
         usedefaultgrid: Optional[bool] = None,
         includelinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
+    ):
         """Get related Business Objects by ID
 
         Operation to get the related objects for a Business Object relationship specifying all fields or default grid as the field to return.
          :param parentbusobid: Specify the Business Object ID for the parent Business Object.
          :param parentbusobrecid: Specify the record ID for the parent Business Object.
          :param relationshipid: Specify the Relationship ID for the related Business Object you want to return.
          :param pageNumber: Specify the page number of the result set to return.
@@ -734,15 +774,15 @@
         )
         self.validate_path_param(
             parentbusobrecid, cherwell_pydantic_api.types.BusObRecID
         )
         self.validate_path_param(
             relationshipid, cherwell_pydantic_api.types.RelationshipID
         )
-        params = {}
+        params: dict[str, Any] = {}
         if pageNumber is not None:
             params["pageNumber"] = pageNumber
         if pageSize is not None:
             params["pageSize"] = pageSize
         if allfields is not None:
             params["allfields"] = allfields
         if usedefaultgrid is not None:
@@ -763,15 +803,17 @@
         parentbusobid: cherwell_pydantic_api.types.BusObIDParamType,
         parentbusobrecid: cherwell_pydantic_api.types.BusObRecID,
         relationshipid: cherwell_pydantic_api.types.RelationshipID,
         gridid: str,
         pageNumber: Optional[int] = None,
         pageSize: Optional[int] = None,
         includelinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
+    ):
         """Get related Business Objects custom grid
 
         Operation to get related Business Objects for a specific relationship. Specify a custom grid ID as the fields to return.
          :param parentbusobid: Specify the Business Object ID for the parent Business Object.
          :param parentbusobrecid: Specify the record ID for the parent Business Object.
          :param relationshipid: Specify the Relationship ID for the related Business Object you want to return.
          :param gridid: Specify the ID for the custom grid that contains the field list.
@@ -786,15 +828,15 @@
         self.validate_path_param(
             parentbusobrecid, cherwell_pydantic_api.types.BusObRecID
         )
         self.validate_path_param(
             relationshipid, cherwell_pydantic_api.types.RelationshipID
         )
         self.validate_path_param(gridid, str)
-        params = {}
+        params: dict[str, Any] = {}
         if pageNumber is not None:
             params["pageNumber"] = pageNumber
         if pageSize is not None:
             params["pageSize"] = pageSize
         if includelinks is not None:
             params["includelinks"] = includelinks
         response = await self.get(
@@ -809,15 +851,17 @@
     async def LinkRelatedBusinessObjectByRecIdV1(
         self,
         parentbusobid: cherwell_pydantic_api.types.BusObIDParamType,
         parentbusobrecid: cherwell_pydantic_api.types.BusObRecID,
         relationshipid: cherwell_pydantic_api.types.RelationshipID,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
+    ):
         """Link related Business Objects
 
         Operation to link related Business Objects.
          :param parentbusobid: Specify the Business Object ID for the parent Business Object.
          :param parentbusobrecid: Specify the record ID for the parent Business Object.
          :param relationshipid: Specify the Relationship ID for the related Business Object you want to link.
          :param busobid: Specify the Business Object ID of the Business Object to be linked.
@@ -846,15 +890,17 @@
     async def LinkRelatedBusinessObjectByRecIdV2(
         self,
         parentbusobid: cherwell_pydantic_api.types.BusObIDParamType,
         parentbusobrecid: cherwell_pydantic_api.types.BusObRecID,
         relationshipid: cherwell_pydantic_api.types.RelationshipID,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.ResponseBase:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.ResponseBase
+    ):
         """Link related Business Objects
 
         Operation to link related Business Objects.
          :param parentbusobid: Specify the Business Object ID for the parent Business Object.
          :param parentbusobrecid: Specify the record ID for the parent Business Object.
          :param relationshipid: Specify the Relationship ID for the related Business Object you want to link.
          :param busobid: Specify the Business Object ID of the Business Object to be linked.
@@ -895,15 +941,15 @@
          :return: None"""
         self.validate_path_param(attachmentid, str)
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(publicid, str)
         response = await self.delete(
             f"/api/V1/removebusinessobjectattachment/attachmentid/{attachmentid}/busobid/{busobid}/publicid/{publicid}"
         )
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def RemoveBusinessObjectAttachmentByIdAndRecIdV1(
         self,
         attachmentid: str,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
     ) -> None:
@@ -916,15 +962,15 @@
          :return: None"""
         self.validate_path_param(attachmentid, str)
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
         response = await self.delete(
             f"/api/V1/removebusinessobjectattachment/attachmentid/{attachmentid}/busobid/{busobid}/busobrecid/{busobrecid}"
         )
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def RemoveBusinessObjectAttachmentByNameAndPublicIdV1(
         self,
         attachmentid: str,
         busobname: str,
         publicid: str,
     ) -> None:
@@ -937,15 +983,15 @@
          :return: None"""
         self.validate_path_param(attachmentid, str)
         self.validate_path_param(busobname, str)
         self.validate_path_param(publicid, str)
         response = await self.delete(
             f"/api/V1/removebusinessobjectattachment/attachmentid/{attachmentid}/busobname/{busobname}/publicid/{publicid}"
         )
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def RemoveBusinessObjectAttachmentByNameAndRecIdV1(
         self,
         attachmentid: str,
         busobname: str,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
     ) -> None:
@@ -958,20 +1004,22 @@
          :return: None"""
         self.validate_path_param(attachmentid, str)
         self.validate_path_param(busobname, str)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
         response = await self.delete(
             f"/api/V1/removebusinessobjectattachment/attachmentid/{attachmentid}/busobname/{busobname}/busobrecid/{busobrecid}"
         )
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def SaveBusinessObjectAttachmentBusObV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveBusObAttachmentRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Attach a Business Object to a Business Object
 
         Operation to attach a Business Object to a Business Object. This links the Business Object but does not create a relationship between the two. (Use "Link Related Business Objects" to create a relationship.)
          :param request: Request object used to specify the Business Objects to attach. You can use Business Object name or ID and Business Object record ID or public ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
         """
         response = await self.post_body(
@@ -982,15 +1030,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse,
         )
 
     async def SaveBusinessObjectAttachmentLinkV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveLinkAttachmentRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Attach a file via UNC
 
         Operation to attach a file to a Business Object via a path (UNC recommended).
          :param request: Request object used to specify the file path (UNC recommended) and the Business Object. You can use Business Object name or ID and Business Object record ID or public ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
         """
         response = await self.post_body(
@@ -1001,15 +1051,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse,
         )
 
     async def SaveBusinessObjectAttachmentUrlV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveUrlAttachmentRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
+    ):
         """Attach a URL path
 
         Operation to attach a URL path to a Business Object.
          :param request: Request object used to specify the URL path and Business Object. You can use Business Object name or ID and Business Object record ID or public ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse
         """
         response = await self.post_body(
@@ -1020,15 +1072,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.AttachmentsResponse,
         )
 
     async def SaveBusinessObjectBatchV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchSaveRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchSaveResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchSaveResponse
+    ):
         """Create or update a batch of Business Objects
 
         Operation that creates or updates an array of Business Objects in a batch. To update, specify record ID or public ID. To create, leave record ID and public ID empty.
          :param request: Specify the array of Business Object templates.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchSaveResponse
         """
         response = await self.post_body(
@@ -1039,15 +1093,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.BatchSaveResponse,
         )
 
     async def SaveBusinessObjectV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse
+    ):
         """Create or Update a Business Object
 
         Operation that creates a new Business Object or updates an existing Business Object. To create, leave record ID and public ID empty. Upon creating or saving, a cache key is returned to use for subsequent requests. If the object is not found in the cache with said cache key, specify record ID or public ID to save and return a new cache key. Set persist = true, to actually save the Business Object to disk, persist = false will just cache it.
          :param request: Specify a list of fields from a Business Object template.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse
         """
         response = await self.post_body(
@@ -1058,15 +1114,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.SaveResponse,
         )
 
     async def SaveRelatedBusinessObjectV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.RelatedSaveRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.RelatedSaveResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.RelatedSaveResponse
+    ):
         """Create or update a related Business Object
 
         Operation that creates or updates a related Business Object. To update, specify record ID or public ID. To create, leave record ID and public ID empty.
          :param request: Request object specifying the parent the Business Object, the Relationship, and field values for the Business Object to create or update.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject.RelatedSaveResponse
         """
         response = await self.post_body(
@@ -1081,15 +1139,17 @@
     async def UnLinkRelatedBusinessObjectByRecIdV1(
         self,
         parentbusobid: cherwell_pydantic_api.types.BusObIDParamType,
         parentbusobrecid: cherwell_pydantic_api.types.BusObRecID,
         relationshipid: cherwell_pydantic_api.types.RelationshipID,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.RelatedBusinessObjectResponse
+    ):
         """UnLink related Business Objects
 
         Operation to unlink related Business Objects.
          :param parentbusobid: Specify the Business Object ID for the parent Business Object.
          :param parentbusobrecid: Specify the record ID for the parent Business Object.
          :param relationshipid: Specify the Relationship ID for the related Business Object you want to unlink.
          :param busobid: Specify the Business Object ID of the Business Object to be unlinked.
@@ -1137,15 +1197,15 @@
          :param totalsize: The entire file size in bytes.
          :param attachmentid: Specify the attachment ID of an uploaded file to upload subsequent parts and ensure each part gets appended to the parts that have already been uploaded.
          :param displaytext: Specify the attachment name, which is the display text for the attachment record.
          :return: cherwell_pydantic_api.types.StringResponse"""
         self.validate_path_param(filename, str)
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(publicid, str)
-        params = {}
+        params: dict[str, Any] = {}
         if attachmentid is not None:
             params["attachmentid"] = attachmentid
         if displaytext is not None:
             params["displaytext"] = displaytext
         response = await self.post_body(
             f"/api/V1/uploadbusinessobjectattachment/filename/{filename}/busobid/{busobid}/publicid/{publicid}/offset/{offset}/totalsize/{totalsize}",
             params=params,
@@ -1176,15 +1236,15 @@
          :param totalsize: The entire file size in bytes.
          :param attachmentid: Specify the attachment ID of an uploaded file to upload subsequent parts and ensure each part gets appended to the parts that have already been uploaded.
          :param displaytext: Specify the attachment name, which is the display text for the attachment record.
          :return: cherwell_pydantic_api.types.StringResponse"""
         self.validate_path_param(filename, str)
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
-        params = {}
+        params: dict[str, Any] = {}
         if attachmentid is not None:
             params["attachmentid"] = attachmentid
         if displaytext is not None:
             params["displaytext"] = displaytext
         response = await self.post_body(
             f"/api/V1/uploadbusinessobjectattachment/filename/{filename}/busobid/{busobid}/busobrecid/{busobrecid}/offset/{offset}/totalsize/{totalsize}",
             params=params,
@@ -1215,15 +1275,15 @@
          :param totalsize: The entire file size in bytes.
          :param attachmentid: Specify the attachment ID of an uploaded file to upload subsequent parts and ensure each part gets appended to the parts that have already been uploaded.
          :param displaytext: Specify the attachment name, which is the display text for the attachment record.
          :return: cherwell_pydantic_api.types.StringResponse"""
         self.validate_path_param(filename, str)
         self.validate_path_param(busobname, str)
         self.validate_path_param(publicid, str)
-        params = {}
+        params: dict[str, Any] = {}
         if attachmentid is not None:
             params["attachmentid"] = attachmentid
         if displaytext is not None:
             params["displaytext"] = displaytext
         response = await self.post_body(
             f"/api/V1/uploadbusinessobjectattachment/filename/{filename}/busobname/{busobname}/publicid/{publicid}/offset/{offset}/totalsize/{totalsize}",
             params=params,
@@ -1254,15 +1314,15 @@
          :param totalsize: The entire file size in bytes.
          :param attachmentid: Specify the attachment ID of an uploaded file to upload subsequent parts and ensure each part gets appended to the parts that have already been uploaded.
          :param displaytext: Specify the attachment name, which is the display text for the attachment record.
          :return: cherwell_pydantic_api.types.StringResponse"""
         self.validate_path_param(filename, str)
         self.validate_path_param(busobname, str)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
-        params = {}
+        params: dict[str, Any] = {}
         if attachmentid is not None:
             params["attachmentid"] = attachmentid
         if displaytext is not None:
             params["displaytext"] = displaytext
         response = await self.post_body(
             f"/api/V1/uploadbusinessobjectattachment/filename/{filename}/busobname/{busobname}/busobrecid/{busobrecid}/offset/{offset}/totalsize/{totalsize}",
             params=params,
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Core.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core
 import cherwell_pydantic_api.types
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class CoreInterface(GeneratedInterfaceBase):
@@ -15,36 +15,38 @@
         Endpoint to delete a gallery image.
          :param standinkey: The StandIn key for the gallery image to delete.
          :return: None"""
         self.validate_path_param(standinkey, str)
         response = await self.delete(
             f"/api/V1/deletegalleryimage/standinkey/{standinkey}"
         )
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def GetGalleryImagesFolderV1(
         self,
         scope: str,
         scopeowner: str,
         folder: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get gallery images by scope, scopeowner, and folder
 
         Get gallery images for the specified scope, scopeowner, and folder.
          :param scope: The scope to get gallery images for.
          :param scopeowner: the scopeowner to get gallery images for.
          :param folder: The folder to get gallery images for.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(folder, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getgalleryimages/scope/{scope}/scopeowner/{scopeowner}/folder/{folder}",
             params=params,
         )
         return self.parse_response(
@@ -53,26 +55,28 @@
         )
 
     async def GetGalleryImagesScopeOwnerV1(
         self,
         scope: str,
         scopeowner: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get gallery images by scope and scopeowner
 
         Get all gallery images for the specified scope and scope owner.
          :param scope: The scope to get gallery images for.
          :param scopeowner: The scopeowner to get gallery images for.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getgalleryimages/scope/{scope}/scopeowner/{scopeowner}",
             params=params,
         )
         return self.parse_response(
@@ -80,45 +84,49 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetGalleryImagesScopeV1(
         self,
         scope: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get gallery images by scope
 
         Get all gallery images for the specified scope.
          :param scope: The scope to get the images for.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getgalleryimages/scope/{scope}", params=params
         )
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetGalleryImagesV1(
         self,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get all gallery images
 
         Get all the gallery images in the system.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get("/api/V1/getgalleryimages", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
@@ -133,42 +141,44 @@
 
         Operation that gets built-in images. If you are requesting an icon (.ico), you can specify width and height.
          :param name: Image name and folder location in the Image Manager. Parameter must begin with "[PlugIn]Images;" and then a period-separated list of folders. Example: "[PlugIn]Images;Images.Common.Cherwell.ico".
          :param width: Specify the width (icons only).
          :param height: Specify the height (icons only).
          :return: cherwell_pydantic_api.types.StringResponse"""
         self.validate_path_param(name, str)
-        params = {}
+        params: dict[str, Any] = {}
         if width is not None:
             params["width"] = width
         if height is not None:
             params["height"] = height
         response = await self.get(f"/api/V1/getgalleryimage/name/{name}", params=params)
         return self.parse_response(response, cherwell_pydantic_api.types.StringResponse)
 
     async def GetStoredValuesFolderV1(
         self,
         scope: str,
         scopeowner: str,
         folder: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get stored values by folder
 
         Get stored values for the specified folder.
          :param scope: The scope for which to get stored values.
          :param scopeowner: The scope owner for which to get stored values.
          :param folder: The folder for which to get stored values.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(folder, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/storedvalues/scope/{scope}/scopeowner/{scopeowner}/folder/{folder}",
             params=params,
         )
         return self.parse_response(
@@ -177,81 +187,89 @@
         )
 
     async def GetStoredValuesScopeOwnerV1(
         self,
         scope: str,
         scopeowner: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get stored values by scope owner
 
         Get stored values for the specified scope and scope owner.
          :param scope: The scope for which to get stored values.
          :param scopeowner: The scope owner for which to get stored values.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/storedvalues/scope/{scope}/scopeowner/{scopeowner}", params=params
         )
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetStoredValuesScopeV1(
         self,
         scope: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get stored values by scope
 
         Get all the stored values for the specified scope.
          :param scope: The scope for which to get stored values.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(f"/api/V1/storedvalues/scope/{scope}", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetStoredValuesV1(
         self,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Gets all the stored values in the system
 
         Get all the stored values in the system.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get("/api/V1/storedvalues", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetStoredValueV1(
         self,
         standInKey: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.StoredValueResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.StoredValueResponse
+    ):
         """Get a  stored value
 
         Get a stored value by its StandIn key.
          :param standInKey: The StandIn key for the Stored Value you would like to retrieve.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.StoredValueResponse
         """
         self.validate_path_param(standInKey, str)
@@ -259,30 +277,34 @@
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.StoredValueResponse,
         )
 
     async def GetViewsV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ViewsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ViewsResponse
+    ):
         """Get a list of the views
 
         Operation to get a list of views that are configured in the system.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ViewsResponse
         """
         response = await self.get("/api/V1/getviews")
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ViewsResponse,
         )
 
     async def SaveGalleryImageV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.SaveGalleryImageRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.SaveGalleryImageResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.SaveGalleryImageResponse
+    ):
         """Create or update a gallery image
 
         Endpoint to Create or update a gallery image. To create a new gallery image leave the StandIn key blank. To update a gallery image provide the StandIn key of the gallery image you want to update.
         There are three different ImageTypes allowed: Imported, Url, and File. To use the Imported image type, provide the filename in the Name property, with extension, and provide the image data in a Base64 encoded format in the Base64EncodedImageData property. The max file size is 512k.
         To use the Url image type,  provide the full network share path to the file in the Name property, ie: "&#92;&#92;&#92;&#92;&#92;&#92;&#92;&#92;networkshare&#92;&#92;&#92;somefolder&#92;&#92;&#92;somefile.jpg". If the file is not accessible to all users it will not visible to all users.
         To use the File image type, provide the full path to the file in the Name property, ie: "C:&#92;&#92;&#92;somefolder&#92;&#92;&#92;somfile.jpg". If the file is not accessible to all users it will not visible to all users.
         When creating or updating an image, Name and ImageType are always required, and if the image type is "Imported", then the Base64EncodedImageData is also required.
@@ -303,15 +325,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.SaveGalleryImageResponse,
         )
 
     async def SaveStoredValueV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.SaveStoredValueRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.StoredValueResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.StoredValueResponse
+    ):
         """Create or update a stored value
 
         Operation to create or update a stored value. To update, specify the StandIn key for the stored value to update. To create leave StandIn key blank, and provide a name, a scope, a type, and a value.
          :param request: The stored value to create or update. To update include the StandIn key for the associated stored value. To create, name, scope, type, and value are required.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.StoredValueResponse
         """
         response = await self.post_body(
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Forms.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms
 import cherwell_pydantic_api.types
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class FormsInterface(GeneratedInterfaceBase):
     async def GetMobileFormForBusObByIdAndPublicIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         publicid: str,
         foredit: Optional[bool] = None,
         formid: Optional[str] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
+    ):
         """Get mobile form by BusObId and Public ID
 
         Operation that gets a mobile form for a specific Business Object by Business Object ID and Public ID.
          :param busobid: Specify the Business Object ID.
          :param publicid: Specify the Business Object Public ID.
          :param foredit: Flag to get the edit mode version of a form.
          :param formid: Specify the form ID if the default is not desired.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
         """
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(publicid, str)
-        params = {}
+        params: dict[str, Any] = {}
         if foredit is not None:
             params["foredit"] = foredit
         if formid is not None:
             params["formid"] = formid
         response = await self.get(
             f"/api/V1/getmobileformforbusob/busobid/{busobid}/publicid/{publicid}",
             params=params,
@@ -40,27 +42,29 @@
 
     async def GetMobileFormForBusObByIdAndRecIdV1(
         self,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
         foredit: Optional[bool] = None,
         formid: Optional[str] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
+    ):
         """Get mobile form by Business Object ID and Business Object Record ID.
 
         Operation that gets a mobile form for a specific Business Object by Business Object ID and record ID.
          :param busobid: Specify the Business Object ID.
          :param busobrecid: Specify the Business Object Record ID.
          :param foredit: Flag to get the edit mode version of a form.
          :param formid: Specify the form ID if the default is not desired.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
         """
         self.validate_path_param(busobid, cherwell_pydantic_api.types.BusObIDParamType)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
-        params = {}
+        params: dict[str, Any] = {}
         if foredit is not None:
             params["foredit"] = foredit
         if formid is not None:
             params["formid"] = formid
         response = await self.get(
             f"/api/V1/getmobileformforbusob/busobid/{busobid}/busobrecid/{busobrecid}",
             params=params,
@@ -72,27 +76,29 @@
 
     async def GetMobileFormForBusObByNameAndPublicIdV1(
         self,
         busobname: str,
         publicid: str,
         foredit: Optional[bool] = None,
         formid: Optional[str] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
+    ):
         """Get mobile form by Business Object name and Public ID
 
         Operation that gets a mobile form for a specific Business Object by Business Object name and public ID.
          :param busobname: Specify the Business Object name.
          :param publicid: Specify the Business Object public ID.
          :param foredit: Flag to get the edit mode version of a form.
          :param formid: Specify the form ID if the default is not desired.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
         """
         self.validate_path_param(busobname, str)
         self.validate_path_param(publicid, str)
-        params = {}
+        params: dict[str, Any] = {}
         if foredit is not None:
             params["foredit"] = foredit
         if formid is not None:
             params["formid"] = formid
         response = await self.get(
             f"/api/V1/getmobileformforbusob/busobname/{busobname}/publicid/{publicid}",
             params=params,
@@ -104,27 +110,29 @@
 
     async def GetMobileFormForBusObByNameAndRecIdV1(
         self,
         busobname: str,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
         foredit: Optional[bool] = None,
         formid: Optional[str] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
+    ):
         """Get mobile form by Business Object name and record ID.
 
         Operation that gets a mobile form for a specific Business Object by Business Object name and record ID.
          :param busobname: Specify the Business Object name.
          :param busobrecid: Specify the Business Object record ID.
          :param foredit: Flag to get the edit mode version of a form.
          :param formid: Specify the form ID if the default is not desired.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Forms.MobileFormResponse
         """
         self.validate_path_param(busobname, str)
         self.validate_path_param(busobrecid, cherwell_pydantic_api.types.BusObRecID)
-        params = {}
+        params: dict[str, Any] = {}
         if foredit is not None:
             params["foredit"] = foredit
         if formid is not None:
             params["formid"] = formid
         response = await self.get(
             f"/api/V1/getmobileformforbusob/busobname/{busobname}/busobrecid/{busobrecid}",
             params=params,
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class LifecycleInterface(GeneratedInterfaceBase):
     async def GetStages(
         self,
         businessObjectDefinitionId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStagesResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStagesResponse
+    ):
         """Get lifecycle stages
 
         Gets all of the stages on the lifecycle for a Business Object
          :param businessObjectDefinitionId:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStagesResponse
         """
         self.validate_path_param(businessObjectDefinitionId, str)
@@ -24,15 +26,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStagesResponse,
         )
 
     async def GetStatuses(
         self,
         businessObjectDefinitionId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStatusesResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStatusesResponse
+    ):
         """Get lifecycle statuses
 
         Gets all of the statuses on the lifecycle for a Business Object
          :param businessObjectDefinitionId:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStatusesResponse
         """
         self.validate_path_param(businessObjectDefinitionId, str)
@@ -43,15 +47,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetStatusesResponse,
         )
 
     async def GetTransitions(
         self,
         businessObjectDefinitionId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetTransitionsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetTransitionsResponse
+    ):
         """Get lifecycle transitions
 
         Gets all of the transitions on the lifecycle for a Business Object
          :param businessObjectDefinitionId:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetTransitionsResponse
         """
         self.validate_path_param(businessObjectDefinitionId, str)
@@ -63,15 +69,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetTransitionsResponse,
         )
 
     async def GetRecordStatus(
         self,
         businessObjectDefinitionId: str,
         recordId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse
+    ):
         """Get current lifecycle status for record
 
         Gets the current lifecycle status of a business object record
          :param businessObjectDefinitionId:
          :param recordId:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse
         """
@@ -85,15 +93,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse,
         )
 
     async def GetRecordStage(
         self,
         businessObjectDefinitionId: str,
         recordId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse
+    ):
         """Get current lifecycle stage for record
 
         Gets the current lifecycle stage of a business object record
          :param businessObjectDefinitionId:
          :param recordId:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse
         """
@@ -107,15 +117,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetRecordStatusResponse,
         )
 
     async def GetTransitionOptions(
         self,
         businessObjectDefinitionId: str,
         recordId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetTransitionOptionsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetTransitionOptionsResponse
+    ):
         """Get lifecycle transition options for record
 
         Gets the lifecycle transition options currently available to a business object record
          :param businessObjectDefinitionId:
          :param recordId:
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.GetTransitionOptionsResponse
         """
@@ -130,15 +142,17 @@
         )
 
     async def TransitionRecord(
         self,
         businessObjectDefinitionId: str,
         recordId: str,
         transitionRecordRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Lifecycle.TransitionRecordRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.ResponseBase:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.ResponseBase
+    ):
         """Transition a business object record
 
         Transitions a business object record in to the specified lifecycle status
          :param businessObjectDefinitionId:
          :param recordId:
          :param transitionRecordRequest: The request body
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.ResponseBase
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/OneStepActions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions
 import cherwell_pydantic_api.types
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
@@ -10,30 +10,32 @@
     async def GetOneStepActionsByAssociation_Scope_ScopeOwner_FolderV1(
         self,
         association: str,
         scope: str,
         scopeowner: str,
         folder: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get One-Step Actions by Folder
 
         Operation to get One-Step Actions by Association, Scope, Scope Owner in a specific folder.
          :param association: Business Object association to get One-Step Actions for
          :param scope: Scope to get One-Step Actions for
          :param scopeowner: Scope owner to get One-Step Actions for
          :param folder: Folder to get One-Step Actions from
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(folder, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getonestepactions/association/{association}/scope/{scope}/scopeowner/{scopeowner}/folder/{folder}",
             params=params,
         )
         return self.parse_response(
@@ -43,28 +45,30 @@
 
     async def GetOneStepActionsByAssociation_Scope_ScopeOwnerV1(
         self,
         association: str,
         scope: str,
         scopeowner: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get One-Step Actions by Scope Owner
 
         Operation to get One-Step Actions by Association, Scope, Scope Owner
          :param association: Business Object association to get One-Step Actions for
          :param scope: Scope to get One-Step Actions for
          :param scopeowner: Scope owner to get One-Step Actions for
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getonestepactions/association/{association}/scope/{scope}/scopeowner/{scopeowner}",
             params=params,
         )
         return self.parse_response(
@@ -73,26 +77,28 @@
         )
 
     async def GetOneStepActionsByAssociation_ScopeV1(
         self,
         association: str,
         scope: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get One-Step Actions by Scope
 
         Operation to get One-Step Actions by Association, Scope
          :param association: Business Object association to get One-Step Actions for
          :param scope: Scope to get One-Step Actions for
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getonestepactions/association/{association}/scope/{scope}",
             params=params,
         )
         return self.parse_response(
@@ -100,59 +106,65 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetOneStepActionsByAssociationV1(
         self,
         association: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get One-Step Actions by Association
 
         Operation to get One-Step Actions by Association
          :param association: Business Object association to get One-Step Actions for
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getonestepactions/association/{association}", params=params
         )
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetOneStepActionsV1(
         self,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get One-Step Actions by default Association
 
         Operation to get One-Step Actions by default Association
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get("/api/V1/getonestepactions", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def RunOneStepActionByKeyForRecordByRecIdV1(
         self,
         standinkey: str,
         busobid: cherwell_pydantic_api.types.BusObIDParamType,
         busobrecid: cherwell_pydantic_api.types.BusObRecID,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse
+    ):
         """Run a One-Step Action for a Business Object record
 
         Operation to run a One-Step Action for a Business Object record by Business Object ID and Business Object Record ID.
          :param standinkey: The key to find the One-Step Action to run
          :param busobid: Specify the Business Object ID.
          :param busobrecid: Specify the Business Object record ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse
@@ -167,15 +179,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse,
         )
 
     async def RunOneStepActionByStandInKeyV1(
         self,
         standinkey: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse
+    ):
         """Run a stand alone One-Step Action
 
         Operation to run a One-Step Action that doesn't run against a Business Object Record.
          :param standinkey: The key to find the One-Step Action to run
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse
         """
         self.validate_path_param(standinkey, str)
@@ -184,15 +198,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse,
         )
 
     async def RunOneStepActionV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse
+    ):
         """Run a One-Step Action using a OneStepActionRequest
 
         Operation to run a One-Step Action using a OneStepActionRequest. This request is used to start a One-Step Action run with additional information such as prompt values.
          :param request: Request object containing all the properties need to start a One-Step Action.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.OneStepActions.OneStepActionResponse
         """
         response = await self.post_body(
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Queues.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Queues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class QueuesInterface(GeneratedInterfaceBase):
     async def AddItemToQueueV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.AddItemToQueueRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.AddItemToQueueResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.AddItemToQueueResponse
+    ):
         """Add a Business Object to a queue
 
         Operation to add a Business Object to a queue
          :param request: Request object containing all properties necessary to add an item to a queue. All properties are required. The standin key defines the queue to which we want to add the Business Object.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.AddItemToQueueResponse
         """
         response = await self.post_body(
@@ -24,15 +26,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.AddItemToQueueResponse,
         )
 
     async def CheckInQueueItemV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckInQueueItemRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckInQueueItemResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckInQueueItemResponse
+    ):
         """Check a Business Object in to a queue
 
         Operation to check in a queue item
          :param request: The request object for checking in an item to a queue. All properties are required except for historyNotes
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckInQueueItemResponse
         """
         response = await self.post_body(
@@ -43,15 +47,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckInQueueItemResponse,
         )
 
     async def CheckOutQueueItemV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckOutQueueItemRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckOutQueueItemResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckOutQueueItemResponse
+    ):
         """Check a Business Object out of a queue
 
         Operation to check out a queue item
          :param request: The request object for checking out an item from a queue. All properties are required except for historyNotes
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.CheckOutQueueItemResponse
         """
         response = await self.post_body(
@@ -65,28 +71,30 @@
 
     async def GetQueuesFolderV1(
         self,
         scope: str,
         scopeowner: str,
         folder: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get available queues.
 
         Get available queues for a specific Business Object type based on scope, scope owner, and folder.
          :param scope: The scope to get available queues for.
          :param scopeowner: The scope owner to get available queues for.
          :param folder: The folder to get available queues for.  This has to be the folder ID which can be retrieved by doing a getqueues operation without the folder including links option then the links will have the folder IDs.
          :param links: Whether or not to include links.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(folder, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getqueues/scope/{scope}/scopeowner/{scopeowner}/folder/{folder}",
             params=params,
         )
         return self.parse_response(
@@ -95,81 +103,89 @@
         )
 
     async def GetQueuesScopeOwnerV1(
         self,
         scope: str,
         scopeowner: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get available queues.
 
         Get available queues for a specific Business Object type based on scope, and scope owner.
          :param scope: The scope to get available queues for.
          :param scopeowner: The scope owner to get available queues for.
          :param links: Whether or not to include links.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getqueues/scope/{scope}/scopeowner/{scopeowner}", params=params
         )
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetQueuesScopeV1(
         self,
         scope: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get available queues.
 
         Get available queues for a specific Business Object type based on scope.
          :param scope: The scope to get available queues for.
          :param links: Whether or not to include links.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(scope, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(f"/api/V1/getqueues/scope/{scope}", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetQueuesV1(
         self,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get available queues.
 
         Get available queues for a specific Business Object.
          :param links: Whether or not to include links.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get("/api/V1/getqueues", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def RemoveItemFromQueueV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.RemoveItemFromQueueRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.RemoveItemFromQueueResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.RemoveItemFromQueueResponse
+    ):
         """Remove an item from a queue
 
         Operation to remove an item from a queue
          :param request: The request object to remove an item from a queue. All properties are required except for historyNotes
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Queues.RemoveItemFromQueueResponse
         """
         response = await self.post_body(
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Searches.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Searches.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches
 import cherwell_pydantic_api.types
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class SearchesInterface(GeneratedInterfaceBase):
     async def GetQuickSearchConfigurationForBusObsV1(
         self,
         dataRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchConfigurationRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchConfigurationResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchConfigurationResponse
+    ):
         """Get a Quick Search from a list of Business Object IDs
 
         Operation to build a Quick Search configuration that you can use to execute a Quick Search for multiple Business Objects. The configuration  includes supplied Business Object IDs and specific search items with the following options. Use the Option Key to determine if you can change the options.
 
 
         ChangedOption
 
@@ -55,15 +57,17 @@
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchConfigurationResponse,
         )
 
     async def GetQuickSearchConfigurationForBusObsWithViewRightsV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchConfigurationResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchConfigurationResponse
+    ):
         """Get a Quick Search by Business Objects with view rights
 
         Operation to get a Quick Search configuration that you can use to execute a Quick Search based the current user's Business Object view rights. The configuration  includes supplied Business Object IDs and specific search items with the following options. Use the Option Key to determine if you can change the options.
 
         ChangedOption
 
         NonFinalStateOption
@@ -103,23 +107,25 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchConfigurationResponse,
         )
 
     async def GetQuickSearchResultsV1(
         self,
         dataRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchRequest,
         includeLinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SimpleResultsList:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SimpleResultsList
+    ):
         """Execute a Quick Search from a list of Business Object IDs and search text
 
         Operation to execute a Quick Search using a list of Business Object IDs and search text.
          :param dataRequest: Request object listing Business Object IDs and search text. Leave out the entire Business Object IDs parameter and all configured quick search Business Objects will be searched.
          :param includeLinks: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SimpleResultsList
         """
-        params = {}
+        params: dict[str, Any] = {}
         if includeLinks is not None:
             params["includeLinks"] = includeLinks
         response = await self.post_body(
             "/api/V1/getquicksearchresults",
             params=params,
             content=dataRequest.json(exclude_unset=True, by_alias=True),
         )
@@ -130,25 +136,27 @@
 
     async def GetQuickSearchSpecificResultsV1(
         self,
         dataRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchSpecificRequest,
         includeSchema: Optional[bool] = None,
         includeLocationFields: Optional[bool] = None,
         includeLinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsTableResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsTableResponse
+    ):
         """Execute a Quick Search on a specific Business Object
 
         Operation to execute a Quick Search for a specific Business Object ID. Use "Get a Quick Search from a list of Business Object IDs" to find values for specific search item options, such as NonFinalStateOption.
          :param dataRequest: Request object containing the parameters for specific Business Object Quick Search execution.
          :param includeSchema: Flag to include the schema for the results.
          :param includeLocationFields: Flag to include location fields in the results.
          :param includeLinks: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsTableResponse
         """
-        params = {}
+        params: dict[str, Any] = {}
         if includeSchema is not None:
             params["includeSchema"] = includeSchema
         if includeLocationFields is not None:
             params["includeLocationFields"] = includeLocationFields
         if includeLinks is not None:
             params["includeLinks"] = includeLinks
         response = await self.post_body(
@@ -163,25 +171,27 @@
 
     async def GetQuickSearchSpecificResultsV2(
         self,
         dataRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchSpecificRequest,
         includeSchema: Optional[bool] = None,
         includeLocationFields: Optional[bool] = None,
         includeLinks: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchResponse
+    ):
         """Execute a Quick Search on a specific Business Object
 
         Operation to execute a Quick Search for a specific Business Object ID. Use "Get a Quick Search from a list of Business Object IDs" to find values for specific search item options, such as NonFinalStateOption.
          :param dataRequest: Request object containing the parameters for specific Business Object Quick Search execution.
          :param includeSchema: Flag to include the schema for the results.
          :param includeLocationFields: Flag to include location fields in the results.
          :param includeLinks: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.QuickSearchResponse
         """
-        params = {}
+        params: dict[str, Any] = {}
         if includeSchema is not None:
             params["includeSchema"] = includeSchema
         if includeLocationFields is not None:
             params["includeLocationFields"] = includeLocationFields
         if includeLinks is not None:
             params["includeLinks"] = includeLinks
         response = await self.post_body(
@@ -197,30 +207,32 @@
     async def GetSearchItemsByAssociation_Scope_ScopeOwner_FolderV1(
         self,
         association: str,
         scope: str,
         scopeowner: str,
         folder: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
+    ):
         """Get all saved searches by Folder ID
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param scope: Use to filter results by scope name or ID.
          :param scopeowner: Use to filter results by scope owner ID.
          :param folder: Use to filter results by Search Group folder ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(folder, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getsearchitems/association/{association}/scope/{scope}/scopeowner/{scopeowner}/folder/{folder}",
             params=params,
         )
         return self.parse_response(
@@ -231,30 +243,32 @@
     async def GetSearchItemsByAssociation_Scope_ScopeOwner_FolderV2(
         self,
         association: str,
         scope: str,
         scopeowner: str,
         folder: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get all saved searches by Folder ID
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param scope: Use to filter results by scope name or ID.
          :param scopeowner: Use to filter results by scope owner ID.
          :param folder: Use to filter results by Search Group folder ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(folder, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V2/getsearchitems/association/{association}/scope/{scope}/scopeowner/{scopeowner}/folder/{folder}",
             params=params,
         )
         return self.parse_response(
@@ -264,28 +278,30 @@
 
     async def GetSearchItemsByAssociation_Scope_ScopeOwnerV1(
         self,
         association: str,
         scope: str,
         scopeowner: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
+    ):
         """Get all saved searches by scope owner (sub scope)
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param scope: Use to filter results by scope name or ID.
          :param scopeowner: Use to filter results by scope owner ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getsearchitems/association/{association}/scope/{scope}/scopeowner/{scopeowner}",
             params=params,
         )
         return self.parse_response(
@@ -295,28 +311,30 @@
 
     async def GetSearchItemsByAssociation_Scope_ScopeOwnerV2(
         self,
         association: str,
         scope: str,
         scopeowner: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get all saved searches by scope owner (sub scope)
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param scope: Use to filter results by scope name or ID.
          :param scopeowner: Use to filter results by scope owner ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V2/getsearchitems/association/{association}/scope/{scope}/scopeowner/{scopeowner}",
             params=params,
         )
         return self.parse_response(
@@ -325,26 +343,28 @@
         )
 
     async def GetSearchItemsByAssociation_ScopeV1(
         self,
         association: str,
         scope: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
+    ):
         """Get all saved searches by scope
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param scope: Use to filter results by scope name or ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getsearchitems/association/{association}/scope/{scope}",
             params=params,
         )
         return self.parse_response(
@@ -353,26 +373,28 @@
         )
 
     async def GetSearchItemsByAssociation_ScopeV2(
         self,
         association: str,
         scope: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get all saved searches by scope
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param scope: Use to filter results by scope name or ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V2/getsearchitems/association/{association}/scope/{scope}",
             params=params,
         )
         return self.parse_response(
@@ -380,100 +402,110 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetSearchItemsByAssociationV1(
         self,
         association: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
+    ):
         """Get all saved searches by Business Object association
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
         """
         self.validate_path_param(association, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V1/getsearchitems/association/{association}", params=params
         )
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse,
         )
 
     async def GetSearchItemsByAssociationV2(
         self,
         association: str,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get all saved searches by Business Object association
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param association: Use to filter results by Business Object association ID.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
         self.validate_path_param(association, str)
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get(
             f"/api/V2/getsearchitems/association/{association}", params=params
         )
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetSearchItemsV1(
         self,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
+    ):
         """Get all saved searches by default Business Object association
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse
         """
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get("/api/V1/getsearchitems", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchItemResponse,
         )
 
     async def GetSearchItemsV2(
         self,
         links: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
+    ):
         """Get all saved searches by default Business Object association
 
         Operation that returns a tree of saved queries, including scope, search name, IDs, and location within the tree.
          :param links: Flag to include hyperlinks in results. Default is false.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData
         """
-        params = {}
+        params: dict[str, Any] = {}
         if links is not None:
             params["links"] = links
         response = await self.get("/api/V2/getsearchitems", params=params)
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ManagerData,
         )
 
     async def GetSearchResultsAdHocV1(
         self,
         dataRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse
+    ):
         """Run an ad-hoc search
 
         Operation that runs an ad-hoc Business Object search. To execute a search with Prompts, the PromptId and Value are required in the Prompt request object.
 
         PromptType is a FieldSubType enum as described below:
         FieldSubType
         None = 0
@@ -509,15 +541,17 @@
         scopeowner: str,
         searchid: str,
         searchTerm: Optional[str] = None,
         pagenumber: Optional[int] = None,
         pagesize: Optional[int] = None,
         includeschema: Optional[bool] = None,
         resultsAsSimpleResultsList: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse
+    ):
         """Run a saved search by internal ID
 
         Operation that returns the paged results of a saved search. When the search contains Prompts, the response contains the Prompt. Send the Prompt and the original operation parameters to  SearchResultsRequest to the getsearchresults ad-hoc http post operation.
 
         PromptType is a FieldSubType enum as described below:
         FieldSubType
         None = 0
@@ -545,15 +579,15 @@
          :param resultsAsSimpleResultsList: Indicates if the results should be returned in a simple results list format or a table format. Default is a table format.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(searchid, str)
-        params = {}
+        params: dict[str, Any] = {}
         if searchTerm is not None:
             params["searchTerm"] = searchTerm
         if pagenumber is not None:
             params["pagenumber"] = pagenumber
         if pagesize is not None:
             params["pagesize"] = pagesize
         if includeschema is not None:
@@ -576,15 +610,17 @@
         scopeowner: str,
         searchname: str,
         searchTerm: Optional[str] = None,
         pagenumber: Optional[int] = None,
         pagesize: Optional[int] = None,
         includeschema: Optional[bool] = None,
         resultsAsSimpleResultsList: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse
+    ):
         """Run a saved search by name
 
         Operation that returns the paged results of a saved search. When the search contains Prompts, the response contains the Prompt. Send the Prompt and the original operation parameters to  SearchResultsRequest to the getsearchresults ad-hoc http post operation.
 
         PromptType is a FieldSubType enum as described below:
         FieldSubType
         None = 0
@@ -612,15 +648,15 @@
          :param resultsAsSimpleResultsList: Indicates if the results should be returned in a simple results list format or a table format. Default is a table format.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.SearchResultsResponse
         """
         self.validate_path_param(association, str)
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(searchname, str)
-        params = {}
+        params: dict[str, Any] = {}
         if searchTerm is not None:
             params["searchTerm"] = searchTerm
         if pagenumber is not None:
             params["pagenumber"] = pagenumber
         if pagesize is not None:
             params["pagesize"] = pagesize
         if includeschema is not None:
@@ -712,15 +748,15 @@
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(searchid, str)
         self.validate_path_param(
             exportformat,
             Literal["CSV", "Excel", "Tab", "Word", "CustomSeparator", "Json"],
         )
-        params = {}
+        params: dict[str, Any] = {}
         if searchTerm is not None:
             params["searchTerm"] = searchTerm
         if pagenumber is not None:
             params["pagenumber"] = pagenumber
         if pagesize is not None:
             params["pagesize"] = pagesize
         response = await self.get(
@@ -773,15 +809,15 @@
         self.validate_path_param(scope, str)
         self.validate_path_param(scopeowner, str)
         self.validate_path_param(searchname, str)
         self.validate_path_param(
             exportformat,
             Literal["CSV", "Excel", "Tab", "Word", "CustomSeparator", "Json"],
         )
-        params = {}
+        params: dict[str, Any] = {}
         if searchTerm is not None:
             params["searchTerm"] = searchTerm
         if pagenumber is not None:
             params["pagenumber"] = pagenumber
         if pagesize is not None:
             params["pagesize"] = pagesize
         response = await self.get(
@@ -792,49 +828,51 @@
 
     async def GetSearchResultsAsStringByNameV1(
         self,
         scope: str,
         associationName: str,
         searchName: str,
         scopeOwner: Optional[str] = None,
-    ) -> list[dict]:
+    ) -> list[cherwell_pydantic_api.types.CherwellObjectID]:
         """Get results of a saved search
 
         Operation that returns the results of a saved search in JSON format.
 
                         This API is protected by a rate limiter and will reject any requests sent from an IP Address when a certain threshold of active concurrent requests has been hit.
 
                         This value can be configured by the Max Concurrent Requests configuration value in the Web API config.
 
                         Once this limit has been reached, all subsequent requests will receive a status code of 429 (Too Many Requests).
 
          :param scope: Specify the scope name for the saved search.
          :param associationName: Specify the Business Object association Name for the saved search.
          :param searchName: Specify the name of the saved search.
          :param scopeOwner: Specify the scope owner ID for the saved search. Use (None) when no scope owner exists.
-         :return: list[dict]"""
+         :return: list[cherwell_pydantic_api.types.CherwellObjectID]"""
         self.validate_path_param(scope, str)
         self.validate_path_param(associationName, str)
         self.validate_path_param(searchName, str)
-        params = {}
+        params: dict[str, Any] = {}
         if scopeOwner is not None:
             params["scopeOwner"] = scopeOwner
         response = await self.get(
             f"/api/V1/storedsearches/{scope}/{associationName}/{searchName}",
             params=params,
         )
-        return self.parse_response(response, list[dict])
+        return self.parse_response(
+            response, list[cherwell_pydantic_api.types.CherwellObjectID]
+        )
 
     async def GetSearchResultsAsStringByNameV2(
         self,
         scope: str,
         associationName: str,
         searchName: str,
         scopeOwner: Optional[str] = None,
-    ) -> list[dict]:
+    ) -> list[cherwell_pydantic_api.types.CherwellObjectID]:
         """Get results of a saved search
 
         Operation that returns the results of a saved search in JSON format.
 
         This API is protected by a rate limiter and will reject any requests sent from an IP Address when a certain threshold of active concurrent requests has been hit.
 
         This value can be configured by the Max Concurrent Requests configuration value in the Web API config.
@@ -843,31 +881,35 @@
 
         This version is not subject to row limits and will return the entire result set of the stored search.
 
          :param scope: Specify the scope name for the saved search.
          :param associationName: Specify the Business Object association Name for the saved search.
          :param searchName: Specify the name of the saved search.
          :param scopeOwner: Specify the scope owner ID for the saved search. Use (None) when no scope owner exists.
-         :return: list[dict]"""
+         :return: list[cherwell_pydantic_api.types.CherwellObjectID]"""
         self.validate_path_param(scope, str)
         self.validate_path_param(associationName, str)
         self.validate_path_param(searchName, str)
-        params = {}
+        params: dict[str, Any] = {}
         if scopeOwner is not None:
             params["scopeOwner"] = scopeOwner
         response = await self.get(
             f"/api/V2/storedsearches/{scope}/{associationName}/{searchName}",
             params=params,
         )
-        return self.parse_response(response, list[dict])
+        return self.parse_response(
+            response, list[cherwell_pydantic_api.types.CherwellObjectID]
+        )
 
     async def GetSearchResultsAsStringByIdV2(
         self,
         searchRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.StoredSearchRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.StoredSearchResults:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Searches.StoredSearchResults
+    ):
         """Get results of a saved search
 
         Operation that returns the results of a saved search in JSON format.
 
         This API is protected by a rate limiter and will reject any requests sent from an IP Address when a certain threshold of active concurrent requests has been hit.
 
         This value can be configured by the Max Concurrent Requests configuration value in the Web API config.
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Security.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Security.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users
 import cherwell_pydantic_api.types
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
@@ -13,15 +13,17 @@
             "NotSet",
             "RichClient",
             "BrowserClient",
             "BrowserPortal",
             "MobileClient",
             "ServiceMonitor",
         ],
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.ClientSecuritySettingsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.ClientSecuritySettingsResponse
+    ):
         """Get client security settings
 
         Operation to get the configured client security settings. Returns true if internal, Windows, LDAP, or SAML are enabled as authentication methods.
          :param applicationtype: The type of CSM application to return security settings for.  Application type is Desktop Client, Browser Client, Browser Portal or Cherwell Mobile.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.ClientSecuritySettingsResponse
         """
         self.validate_path_param(
@@ -41,29 +43,33 @@
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.ClientSecuritySettingsResponse,
         )
 
     async def GetRolesV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RoleReadResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RoleReadResponse
+    ):
         """Get all available Roles
 
         Operation to get all available Roles.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RoleReadResponse
         """
         response = await self.get("/api/V1/getroles")
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RoleReadResponse,
         )
 
     async def GetRolesV2(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RoleReadV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RoleReadV2Response
+    ):
         """Get all available Roles
 
         Operation to get all available Roles.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RoleReadV2Response
         """
         response = await self.get("/api/V2/getroles")
         return self.parse_response(
@@ -97,15 +103,17 @@
             ],
         )
 
     async def GetSecurityGroupBusinessObjectPermissionsByBusObIdV2(
         self,
         groupid: str,
         busObId: cherwell_pydantic_api.types.BusObIDParamType,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
+    ):
         """Get Business Object permissions by Security Group
 
         Operation to get specific Business Object permissions for a Security Group.
          :param groupid: Specify the Security Group ID.
          :param busObId: Specify the Business Object ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
         """
@@ -145,15 +153,17 @@
             ],
         )
 
     async def GetSecurityGroupBusinessObjectPermissionsByBusObNameV2(
         self,
         groupname: str,
         busobname: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
+    ):
         """Get Business Object permissions by Security Group
 
         Operation to get specific Business Object permissions for a Security Group.
          :param groupname: Specify the Security Group name.
          :param busobname: Specify the Business Object name.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
         """
@@ -189,15 +199,17 @@
                 cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.BusinessObjectPermission
             ],
         )
 
     async def GetSecurityGroupBusinessObjectPermissionsForCurrentUserByBusObIdV2(
         self,
         busObId: cherwell_pydantic_api.types.BusObIDParamType,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
+    ):
         """Get Business Object permission for current user
 
         Operation to get Business Object permissions for the currently logged-in user's Security Group.
          :param busObId: Specify the Business Object ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
         """
         self.validate_path_param(busObId, cherwell_pydantic_api.types.BusObIDParamType)
@@ -231,15 +243,17 @@
                 cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.BusinessObjectPermission
             ],
         )
 
     async def GetSecurityGroupBusinessObjectPermissionsForCurrentUserByBusObNameV2(
         self,
         busobname: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
+    ):
         """Get Business Object permissions for current user
 
         Operation to get Business Object permissions for currently logged in user's Security Group.
          :param busobname: Specify the Business Object name.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.GetSecurityGroupBusinessObjectPermissionsResponse
         """
         self.validate_path_param(busobname, str)
@@ -267,15 +281,17 @@
             list[
                 cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.RightCategory
             ],
         )
 
     async def GetSecurityGroupCategoriesV2(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightCategoriesResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightCategoriesResponse
+    ):
         """Get all Security Group categories
 
         Operation to get IDs and names for all available Security Group categories.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightCategoriesResponse
         """
         response = await self.get("/api/V2/getsecuritygroupcategories")
         return self.parse_response(
@@ -309,15 +325,17 @@
             ],
         )
 
     async def GetSecurityGroupRightsByGroupIdAndCategoryIdV2(
         self,
         groupid: str,
         categoryid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
+    ):
         """Get permissions for a Security Group by category
 
         Operation to get permissions for a Security Group by category. To get Security Group IDs, use "Get all available Security Groups." To get Security Group category IDs, use "Get all Security Group categories."
          :param groupid: Specify the Security Group ID
          :param categoryid: Specify the Security Group category ID
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
         """
@@ -357,15 +375,17 @@
             ],
         )
 
     async def GetSecurityGroupRightsByGroupNameAndCategoryNameV2(
         self,
         groupname: str,
         categoryname: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
+    ):
         """Get permissions for a Security Group by category
 
         Operation to get permissions for a Security Group by category.
          :param groupname: Specify the Security Group name.
          :param categoryname: Specify the Security Group category name.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
         """
@@ -401,15 +421,17 @@
                 cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.Right
             ],
         )
 
     async def GetSecurityGroupRightsForCurrentUserByCategoryIdV2(
         self,
         categoryid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
+    ):
         """Get current user's permissions by Security Group category by ID
 
         Operation to get permissions for the current user's Security Group by category. To get Security Group category IDs, use "Get all Security Group categories."
          :param categoryid: Specify the Security Group category ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
         """
         self.validate_path_param(categoryid, str)
@@ -443,15 +465,17 @@
                 cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.Right
             ],
         )
 
     async def GetSecurityGroupRightsForCurrentUserByCategoryNameV2(
         self,
         categoryname: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
+    ):
         """Get current user's permissions by Security Group category by name
 
         Operation to get permissions for the current user's Security Group by category.
          :param categoryname: Specify the Security Group category name.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse
         """
         self.validate_path_param(categoryname, str)
@@ -461,29 +485,33 @@
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityRightsResponse,
         )
 
     async def GetSecurityGroupsV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityGroupResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityGroupResponse
+    ):
         """Get all available Security Groups
 
         Operation to get IDs, names, and descriptions for all available Security Groups.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityGroupResponse
         """
         response = await self.get("/api/V1/getsecuritygroups")
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityGroupResponse,
         )
 
     async def GetSecurityGroupsV2(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityGroupV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityGroupV2Response
+    ):
         """Get all available Security Groups
 
         Operation to get IDs, names, and descriptions for all available Security Groups.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.SecurityGroupV2Response
         """
         response = await self.get("/api/V2/getsecuritygroups")
         return self.parse_response(
@@ -511,15 +539,17 @@
                 cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User
             ],
         )
 
     async def GetUsersInSecurityGroupV2(
         self,
         groupid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadV2Response
+    ):
         """Get users in a Security Group
 
         Operation to get the users in a specified Security Group. Use "Get all available Security Groups" to get Security Group record IDs.
          :param groupid: Specify the Security Group ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadV2Response
         """
         self.validate_path_param(groupid, str)
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Service.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import pydantic
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class ServiceInterface(GeneratedInterfaceBase):
     async def GetServiceInfoV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ServiceInfoResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ServiceInfoResponse
+    ):
         """Get information about the REST Api and CSM
 
         Operation to get information about the REST API and CSM.  The response is latest REST API operation version, CSM version, and CSM system date and time.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core.ServiceInfoResponse
         """
         response = await self.get("/api/V1/serviceinfo")
         return self.parse_response(
@@ -24,29 +26,31 @@
 
     async def LogoutUserV1(self) -> None:
         """Log out user by token
 
         Operation that logs out the user referenced in the authentication token.
          :return: None"""
         response = await self.delete("/api/V1/logout")
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def Token(
         self,
         grant_type: str,
         client_id: pydantic.SecretStr,
         client_secret: Optional[pydantic.SecretStr] = None,
         username: Optional[str] = None,
         password: Optional[pydantic.SecretStr] = None,
         refresh_token: Optional[str] = None,
         auth_mode: Optional[
             Literal["Internal", "Windows", "LDAP", "SAML", "Auto"]
         ] = None,
         site_name: Optional[str] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.TokenResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.TokenResponse
+    ):
         """Get an access token
 
         Operation to request an access token for one of the following authentication modes. Or, you can request an access token using a refresh token. An API client key is required in both cases, and the authentication mode you use must be the mode used by the CSM Browser Client.
 
         Internal - Use a CSM username and password. If no other mode is specified, Internal mode is used.
 
         Windows - Uses the server variable LOGON_USER to attempt to find a CSM user.  You can also use domain&#92;username and password.
@@ -63,15 +67,15 @@
          :param password: Specify the password assigned to the login ID.
          :param refresh_token: Specify the refresh token used to grant another access token.
          :param auth_mode: Specify the Authentication Mode to use for requesting an access token.
          :param site_name: If for portal specify the Site name to use for requesting an access token.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Security.TokenResponse
         """
         post = {"grant_type": grant_type, "client_id": client_id.get_secret_value()}
-        params = {}
+        params: dict[str, Any] = {}
         if client_secret is not None:
             post["client_secret"] = client_secret.get_secret_value()
         if username is not None:
             post["username"] = username
         if password is not None:
             post["password"] = password.get_secret_value()
         if refresh_token is not None:
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Teams.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class TeamsInterface(GeneratedInterfaceBase):
     async def AddUserToTeamByBatchV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamByBatchRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamByBatchResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamByBatchResponse
+    ):
         """Add users to a team by batch
 
         Operation to add users to a Team by batch. To get internal IDs for users, use “Get User Information in a Batch.” To get a Team's internal ID, use "Get all available Teams."
          :param request: Request object to specify a list of add user to team request objects.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamByBatchResponse
         """
         response = await self.post_body(
@@ -33,20 +35,22 @@
         Operation to add a user to a Team. To get the user's internal ID, use "Get a user by login ID" or "Get a user by public ID." To get a Team's internal ID, use "Get all available Teams."
          :param dataRequest: Request object to specify user and team values.
          :return: None"""
         response = await self.post_body(
             "/api/V1/addusertoteam",
             content=dataRequest.json(exclude_unset=True, by_alias=True),
         )
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def AddUserToTeamV2(
         self,
         dataRequest: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamResponse
+    ):
         """Add a user to a team
 
         Operation to add a user to a Team. To get the user's internal ID, use "Get a user by login ID" or "Get a user by public ID." To get a Team's internal ID, use "Get all available Teams."
          :param dataRequest: Request object to specify user and team values.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.AddUserToTeamResponse
         """
         response = await self.post_body(
@@ -65,48 +69,54 @@
         """Delete a Team
 
         Operation to delete a Team by Team ID.
          :param teamid: Specify the Team ID.
          :return: None"""
         self.validate_path_param(teamid, str)
         response = await self.delete(f"/api/V1/deleteteam/{teamid}")
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def GetTeamsV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse
+    ):
         """Get all available Teams
 
         Operation to get IDs and names for all available Teams.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse
         """
         response = await self.get("/api/V1/getteams")
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse,
         )
 
     async def GetTeamsV2(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response
+    ):
         """Get all available Teams
 
         Operation to get IDs and names for all available Teams.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response
         """
         response = await self.get("/api/V2/getteams")
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response,
         )
 
     async def GetTeamV1(
         self,
         teamid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamResponse
+    ):
         """Get a team by its TeamId
 
         Operation to get Team Info for a  single Team using its Team ID. To get a Team's internal ID, use "Get all available Teams." Note that TeamType has two possible values, where TeamType = 0 for User (CSM Users), or TeamType = 1 for Workgroup (CSM Customers).
          :param teamid: The Team ID of the Team to get.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamResponse
         """
         self.validate_path_param(teamid, str)
@@ -115,15 +125,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamResponse,
         )
 
     async def GetUsersTeamsV1(
         self,
         userRecordId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse
+    ):
         """Get Team assignments for a user
 
         Operation to get Team assignments for a user. To get record IDs, use "Get a user by login ID" or "Get a user by public id."
          :param userRecordId: Specify the user record ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse
         """
         self.validate_path_param(userRecordId, str)
@@ -132,15 +144,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse,
         )
 
     async def GetUsersTeamsV2(
         self,
         userRecordId: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response
+    ):
         """Get Team assignments for a user
 
         Operation to get Team assignments for a user. To get record IDs, use "Get a user by login ID" or "Get a user by public id."
          :param userRecordId: Specify the user record ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response
         """
         self.validate_path_param(userRecordId, str)
@@ -148,29 +162,33 @@
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response,
         )
 
     async def GetWorkgroupsV1(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse
+    ):
         """Get all available Workgroups
 
         Operation to get IDs and names for all available Workgroups.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse
         """
         response = await self.get("/api/V1/getworkgroups")
         return self.parse_response(
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsResponse,
         )
 
     async def GetWorkgroupsV2(
         self,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response
+    ):
         """Get all available Workgroups
 
         Operation to get IDs and names for all available Workgroups.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamsV2Response
         """
         response = await self.get("/api/V2/getworkgroups")
         return self.parse_response(
@@ -190,21 +208,23 @@
          :param userrecordid: Specify the record ID of the User to remove.
          :return: None"""
         self.validate_path_param(teamId, str)
         self.validate_path_param(userrecordid, str)
         response = await self.delete(
             f"/api/V1/removeuserfromteam/teamid/{teamId}/userrecordid/{userrecordid}"
         )
-        return self.parse_response(response, None)
+        self.check_response(response)
 
     async def RemoveUserFromTeamV2(
         self,
         teamId: str,
         userrecordid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveUserFromTeamResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveUserFromTeamResponse
+    ):
         """Operation to remove a User from a Team.
 
         Operation to remove a User from a Team. To get the User's record ID, use "Get a User by login ID" or "Get a User by public ID." To get a Team's internal ID, use "Get all available Teams."
          :param teamId: Specify the internal ID of the Team.
          :param userrecordid: Specify the record ID of the User to remove.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveUserFromTeamResponse
         """
@@ -218,15 +238,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveUserFromTeamResponse,
         )
 
     async def RemoveCustomerFromWorkgroupV1(
         self,
         workgroupid: str,
         customerrecordid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveCustomerFromWorkgroupResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveCustomerFromWorkgroupResponse
+    ):
         """Remove a customer from a Workgroup
 
         Operation to remove a Customer from a Workgroup.  To remove, specify the Workgroup ID and the Customer Record ID.
          :param workgroupid: Specify the Workgroup ID.
          :param customerrecordid: Specify the Customer record ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveCustomerFromWorkgroupResponse
         """
@@ -239,15 +261,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.RemoveCustomerFromWorkgroupResponse,
         )
 
     async def SaveTeamV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamSaveRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamSaveResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamSaveResponse
+    ):
         """Create or update a team
 
         Operation to create or update a Team or Workgroup.
          :param request: Request object to create Teams or Workgroups. To create a Team, use teamType and teamName. To update a team, use teamID. Team type values must be User or CustomerWorkgroup. The teamType cannot be changed for existing Teams or Workgroups.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamSaveResponse
         """
         response = await self.post_body(
@@ -257,15 +281,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.TeamSaveResponse,
         )
 
     async def SaveTeamMemberV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveTeamMemberRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveTeamMemberResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveTeamMemberResponse
+    ):
         """Add or Update a team member
 
         Operation to add or update a Team Member. To add or update, specify User ID, Team ID, and if Team Manager.   Optionally, set the Team as the User's default Team.
          :param request: The request object to add or update a Team Member. User recID specifies the User to add or update. TeamId specifies the Team to update. IsTeamManager specifies whether the User is a Team Manager, and SetAsDefaultTeam specifies whether to set this Team as the User's default team. UserRecId, TeamId, and IsTeamManager are required.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveTeamMemberResponse
         """
         response = await self.post_body(
@@ -276,15 +302,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveTeamMemberResponse,
         )
 
     async def SaveWorkgroupMemberV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveWorkgroupMemberRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveWorkgroupMemberResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveWorkgroupMemberResponse
+    ):
         """Save the membership status of a Workgroup member.
 
         Operation to add or update a Workgroup Member.  To add or update, specify Customer Record ID, Workgroup ID, and if Workgroup Manager.
          :param request: The request object to add or update a Workgroup Member. CustomerRecordId specifies the Customer to add or update. WorkgroupId specifies the Workgroup to update. CustomerIsWorkgroupManager specifies whether the Customer is a Workgroup Manager.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Teams.SaveWorkgroupMemberResponse
         """
         response = await self.post_body(
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/Users.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/Users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Any, Literal, Optional
+from typing import Any, Literal, Optional  # type: ignore
 
 import cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users
 from cherwell_pydantic_api.generated_api_utils import GeneratedInterfaceBase
 
 
 class UsersInterface(GeneratedInterfaceBase):
     async def DeleteUserBatchV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteResponse
+    ):
         """Delete a batch of users
 
         Operation to delete a batch of users. To get record IDs, use "Get a user by login ID" or "Get a user by public id."
          :param request: Request object listing record IDs for users to be deleted and an error flag.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteResponse
         """
         response = await self.post_body(
@@ -23,15 +25,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteResponse,
         )
 
     async def DeleteUserBatchV2(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteV2Response
+    ):
         """Delete a batch of users
 
         Operation to delete a batch of users. To get record IDs, use "Get a user by login ID" or "Get a user by public id."
          :param request: Request object listing record IDs for users to be deleted and an error flag.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteV2Response
         """
         response = await self.post_body(
@@ -42,15 +46,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchDeleteV2Response,
         )
 
     async def DeleteUserV1(
         self,
         userrecordid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteResponse
+    ):
         """Delete a user by record ID
 
         Operation to delete a user by record ID. To get record IDs, use "Get a user by login ID" or "Get a user by public id."
          :param userrecordid: Specify the record ID of the user you want to delete
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteResponse
         """
         self.validate_path_param(userrecordid, str)
@@ -59,15 +65,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteResponse,
         )
 
     async def DeleteUserV2(
         self,
         userrecordid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteV2Response
+    ):
         """Delete a user by record ID
 
         Operation to delete a user by record ID. To get record IDs, use "Get a user by login ID" or "Get a user by public id."
          :param userrecordid: Specify the record ID of the user you want to delete
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteV2Response
         """
         self.validate_path_param(userrecordid, str)
@@ -77,15 +85,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserDeleteV2Response,
         )
 
     async def GetListOfUsers(
         self,
         loginidfilter: Literal["Internal", "Windows", "Both"],
         stoponerror: Optional[bool] = None,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserListResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserListResponse
+    ):
         """Get a list of all system users.
 
         Operation to get a list of all system users.
          :param loginidfilter: Specify the login ID filter to apply to the users list.
          :param stoponerror: Specify whether the operation is interrupted if retrieving any user causes an error.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserListResponse
         """
@@ -97,15 +107,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserListResponse,
         )
 
     async def GetUserBatchV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchReadRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchReadResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchReadResponse
+    ):
         """Get user information in a batch
 
         Operation to get user information in a batch. To get record IDs, use "Get a user by login ID" or "Get a user by public id."
          :param request: Request object that lists user record IDs or public IDs of users and an error flag.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchReadResponse
         """
         response = await self.post_body(
@@ -116,15 +128,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchReadResponse,
         )
 
     async def GetUserByLoginIdV1(
         self,
         loginid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User
+    ):
         """Get a user by login ID
 
         Operation to get detailed user information by login ID. Use to get user record IDs and account settings, for example. This operation has been deprecated by a V2 operation of the same name, but with query string parameters.
          :param loginid: Specify the user's login ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User
         """
         self.validate_path_param(loginid, str)
@@ -134,15 +148,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User,
         )
 
     async def GetUserByLoginIdV2(
         self,
         loginid: str,
         loginidtype: Literal["Internal", "Windows"],
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User
+    ):
         """Get a user by login ID and login ID type
 
         Operation to get detailed user information by login ID. Use to get user record IDs and account settings, for example.
          :param loginid: Specify the user's login ID.
          :param loginidtype: Specify the login ID type.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User
         """
@@ -153,15 +169,17 @@
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.User,
         )
 
     async def GetUserByLoginIdV3(
         self,
         loginid: str,
         loginidtype: Literal["Internal", "Windows"],
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2
+    ):
         """Get a user by login ID and login ID type
 
         Operation to get detailed user information by login ID. Use to get user record IDs and account settings, for example.
          :param loginid: Specify the user's login ID.
          :param loginidtype: Specify the login ID type.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2
         """
@@ -171,15 +189,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2,
         )
 
     async def GetUserByPublicIdV1(
         self,
         publicid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadResponse
+    ):
         """Get a user by public ID
 
         Operation to get detailed user information by public ID. Use to get user record IDs and account settings, for example.
          :param publicid: Specify the user's public ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadResponse
         """
         self.validate_path_param(publicid, str)
@@ -188,15 +208,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadResponse,
         )
 
     async def GetUserByPublicIdV2(
         self,
         publicid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadV2Response
+    ):
         """Get a user by public ID
 
         Operation to get detailed user information by public ID. Use to get user record IDs and account settings, for example.
          :param publicid: Specify the user's public ID.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadV2Response
         """
         self.validate_path_param(publicid, str)
@@ -205,15 +227,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserReadV2Response,
         )
 
     async def GetUserByRecId(
         self,
         recid: str,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2
+    ):
         """Get a user by record ID
 
         Operation to get detailed user information by record ID.  Use to get user public IDs and account settings, for example.
          :param recid: Specify the user's record ID
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2
         """
         self.validate_path_param(recid, str)
@@ -222,15 +246,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserV2,
         )
 
     async def SaveUserBatchV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveResponse
+    ):
         """Create or update users in a batch
 
         Operation to create or update users in a batch. To update, specify record ID. To create, leave record ID empty.
          :param request: Request object listing user record IDs and an error flag.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveResponse
         """
         response = await self.post_body(
@@ -241,15 +267,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveResponse,
         )
 
     async def SaveUserBatchV2(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveV2Request,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveV2Response
+    ):
         """Create or update users in a batch
 
         Operation to create or update users in a batch. To update, specify record ID. To create, leave record ID empty.
          :param request: Request object listing user record IDs and an error flag.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveV2Response
         """
         response = await self.post_body(
@@ -260,15 +288,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserBatchSaveV2Response,
         )
 
     async def SaveUserV1(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveRequest,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveResponse:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveResponse
+    ):
         """Create or update a user
 
         Operation to create or update a user.  The response is a collection because if you use a public ID, more than one user could be updated since public IDs may not be unique.
          :param request: Request object to specify user parameters and fields with values to be created or updated. The loginId and either the Business Object record ID or Public ID are required.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveResponse
         """
         response = await self.post_body(
@@ -278,15 +308,17 @@
             response,
             cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveResponse,
         )
 
     async def SaveUserV2(
         self,
         request: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveV2Request,
-    ) -> cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveV2Response:
+    ) -> (
+        cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveV2Response
+    ):
         """Create or update a user
 
         Operation to create or update a user.  The response is a collection because if you use a public ID, more than one user could be updated since public IDs may not be unique.
          :param request: Request object to specify user parameters and fields with values to be created or updated. The loginId and either the Business Object record ID or Public ID are required.
          :return: cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Users.UserSaveV2Response
         """
         response = await self.post_body(
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/endpoints/__init__.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Approval.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,40 @@
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import ApiBaseModel, HttpStatusCode
 
 from .... import CherwellObjectID
 from . import Core
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class ApprovalReadResponse(ApiBaseModel):
     properties: Optional[Dict[str, CherwellObjectID]] = None
     links: Optional[List[Core.CherwellLink]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class GetApprovalsResponse(ApiBaseModel):
     totalRecords: Optional[int] = None
     approvals: Optional[List[ApprovalReadResponse]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/BusinessObject.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,91 +9,147 @@
 
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import ApiBaseModel, HttpStatusCode
 
 from . import Core
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class FieldValidationError(ApiBaseModel):
     error: Optional[str] = None
     errorCode: Optional[str] = None
     fieldId: Optional[ct.FieldID] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class NotificationTrigger(ApiBaseModel):
     sourceType: Optional[str] = None
     sourceId: Optional[str] = None
     sourceChange: Optional[str] = None
     key: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class DeleteRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class DeleteResponse(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class FieldTemplateItem(ApiBaseModel):
     dirty: Optional[bool] = None
     displayName: Optional[str] = None
     fieldId: Optional[ct.FieldID] = None
     fullFieldId: Optional[ct.FieldID] = None
     html: Optional[str] = None
     name: Optional[str] = None
     value: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class FieldValuesLookupRequest(ApiBaseModel):
     busbPublicId: Optional[str] = None
     busObId: Optional[ct.BusObID] = None
     busObRecId: Optional[ct.BusObRecID] = None
     fieldId: Optional[ct.FieldID] = None
     fieldName: Optional[str] = None
     fields: Optional[List[FieldTemplateItem]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class FieldValuesLookupResponse(ApiBaseModel):
     values: Optional[List[str]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BusObActivity(ApiBaseModel):
     id: Optional[str] = None
     parentBusObDefId: Optional[str] = None
     parentBusObRecId: Optional[ct.BusObRecID] = None
     historyBusObDefId: Optional[str] = None
     historyBusObRecId: Optional[ct.BusObRecID] = None
     type: Optional[str] = None
@@ -139,14 +195,21 @@
     UsedAsSolution = 'UsedAsSolution'
     ExternalSolution = 'ExternalSolution'
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class Attachment(ApiBaseModel):
     attachedBusObId: Optional[ct.BusObID] = None
     attachedBusObRecId: Optional[ct.BusObRecID] = None
     attachmentFileId: Optional[str] = None
     attachmentFileName: Optional[str] = None
     attachmentFileType: Optional[str] = None
     attachmentId: Optional[str] = None
@@ -162,49 +225,77 @@
     scopeOwner: Optional[str] = None
     type: Optional[Type] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class AttachmentsRequest(ApiBaseModel):
     attachmentId: Optional[str] = None
     attachmentTypes: Optional[List[AttachmentType]] = None
     busObId: Optional[ct.BusObID] = None
     busObName: Optional[str] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
     includeLinks: Optional[bool] = None
     types: Optional[List[Type]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class ReadRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BarcodeLookupResponse(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObRecId: Optional[ct.BusObRecID] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class FieldDefinition(ApiBaseModel):
     autoFill: Optional[bool] = None
     calculated: Optional[bool] = None
     category: Optional[str] = None
     decimalDigits: Optional[int] = None
     description: Optional[str] = None
     details: Optional[str] = None
@@ -223,35 +314,56 @@
     validated: Optional[bool] = None
     wholeDigits: Optional[int] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class GridDefinition(ApiBaseModel):
     gridId: Optional[str] = None
     name: Optional[str] = None
     displayName: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class Relationship(ApiBaseModel):
     cardinality: Optional[str] = None
     description: Optional[str] = None
     displayName: Optional[str] = None
     fieldDefinitions: Optional[List[FieldDefinition]] = None
     relationshipId: Optional[ct.RelationshipID] = None
     target: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class Summary(ApiBaseModel):
     firstRecIdField: Optional[str] = None
     groupSummaries: Optional[List[Summary]] = None
     recIdFields: Optional[str] = None
     stateFieldId: Optional[ct.FieldID] = None
     states: Optional[str] = None
     busObId: Optional[ct.BusObID] = None
@@ -262,36 +374,57 @@
     name: Optional[str] = None
     supporting: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class TemplateRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     fieldNames: Optional[List[str]] = None
     fieldIds: Optional[List[str]] = None
     includeAll: Optional[bool] = None
     includeRequired: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class TemplateResponse(ApiBaseModel):
     fields: Optional[List[FieldTemplateItem]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class ViewSummary(ApiBaseModel):
     groupSummaries: Optional[List[ViewSummary]] = None
     image: Optional[str] = None
     isPartOfView: Optional[bool] = None
     busObId: Optional[ct.BusObID] = None
     displayName: Optional[str] = None
     group: Optional[bool] = None
@@ -300,14 +433,21 @@
     name: Optional[str] = None
     supporting: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class SaveBusObAttachmentRequest(ApiBaseModel):
     attachBusObId: Optional[ct.BusObID] = None
     attachBusObName: Optional[str] = None
     attachBusObPublicId: Optional[str] = None
     attachBusObRecId: Optional[ct.BusObRecID] = None
     busObId: Optional[ct.BusObID] = None
     busObName: Optional[str] = None
@@ -316,28 +456,42 @@
     comment: Optional[str] = None
     includeLinks: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class SaveLinkAttachmentRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObName: Optional[str] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
     comment: Optional[str] = None
     displayText: Optional[str] = None
     includeLinks: Optional[bool] = None
     uncFilePath: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class SaveUrlAttachmentRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObName: Optional[str] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
     comment: Optional[str] = None
     displayText: Optional[str] = None
@@ -350,27 +504,41 @@
     User = 'User'
     Session = 'Session'
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class SaveRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
     cacheKey: Optional[str] = None
     cacheScope: Optional[CacheScope] = None
     fields: Optional[List[FieldTemplateItem]] = None
     persist: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class RelatedSaveRequest(ApiBaseModel):
     parentBusObId: Optional[ct.BusObID] = None
     parentBusObPublicId: Optional[str] = None
     parentBusObRecId: Optional[ct.BusObRecID] = None
     relationshipId: Optional[ct.RelationshipID] = None
     busObId: Optional[ct.BusObID] = None
     busObPublicId: Optional[str] = None
@@ -380,14 +548,21 @@
     fields: Optional[List[FieldTemplateItem]] = None
     persist: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class RelatedSaveResponse(ApiBaseModel):
     parentBusObId: Optional[ct.BusObID] = None
     parentBusObPublicId: Optional[str] = None
     parentBusObRecId: Optional[ct.BusObRecID] = None
     relationshipId: Optional[ct.RelationshipID] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
@@ -399,14 +574,21 @@
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class SaveResponse(ApiBaseModel):
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
     cacheKey: Optional[str] = None
     fieldValidationErrors: Optional[List[FieldValidationError]] = None
     notificationTriggers: Optional[List[NotificationTrigger]] = None
     errorCode: Optional[str] = None
@@ -414,29 +596,50 @@
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BatchDeleteRequest(ApiBaseModel):
     deleteRequests: Optional[List[DeleteRequest]] = None
     stopOnError: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BatchDeleteResponse(ApiBaseModel):
     responses: Optional[List[DeleteResponse]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class ReadResponse(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
     fields: Optional[List[FieldTemplateItem]] = None
     links: Optional[List[Core.CherwellLink]] = None
     errorCode: Optional[str] = None
@@ -444,40 +647,68 @@
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class AttachmentsResponse(ApiBaseModel):
     attachments: Optional[List[Attachment]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BatchReadRequest(ApiBaseModel):
     readRequests: Optional[List[ReadRequest]] = None
     stopOnError: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BatchReadResponse(ApiBaseModel):
     responses: Optional[List[ReadResponse]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class SchemaResponse(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     fieldDefinitions: Optional[List[FieldDefinition]] = None
     firstRecIdField: Optional[str] = None
     gridDefinitions: Optional[List[GridDefinition]] = None
     name: Optional[str] = None
     recIdFields: Optional[str] = None
@@ -489,29 +720,50 @@
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BusObsForViewResponse(ApiBaseModel):
     summaries: Optional[List[ViewSummary]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BatchSaveRequest(ApiBaseModel):
     saveRequests: Optional[List[SaveRequest]] = None
     stopOnError: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class BatchSaveResponse(ApiBaseModel):
     responses: Optional[List[SaveResponse]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Core.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Users.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,337 +1,415 @@
 # generated by datamodel-codegen:
 #   filename:  csm_api-swagger.json
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import ApiBaseModel
 
-from .... import CherwellObjectID
-from ... import CherwellNameValuePair
+from . import BusinessObject
 
 
-class CherwellLink(ApiBaseModel):
-    name: Optional[str] = None
-    url: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
 
 
-import cherwell_pydantic_api.types as ct
-from cherwell_pydantic_api.generated_api_utils import HttpStatusCode
+Enum  # type: ignore
 
 
-class ManagerItem(ApiBaseModel):
-    association: Optional[str] = None
-    description: Optional[str] = None
+class User(ApiBaseModel):
+    accountLocked: Optional[bool] = None
+    createDateTime: Optional[datetime] = None
     displayName: Optional[str] = None
-    galleryImage: Optional[str] = None
-    id: Optional[str] = None
-    links: Optional[List[CherwellLink]] = None
-    localizedScopeName: Optional[str] = None
-    name: Optional[str] = None
-    parentFolder: Optional[str] = None
-    parentIsScopeFolder: Optional[bool] = None
-    scope: Optional[str] = None
-    scopeOwner: Optional[str] = None
-    standInKey: Optional[str] = None
-
-
-class StoredValueType(Enum):
-    Text = 'Text'
-    Number = 'Number'
-    DateTime = 'DateTime'
-    Logical = 'Logical'
-    Color = 'Color'
-    Json = 'Json'
-    JsonArray = 'JsonArray'
-    Xml = 'Xml'
-    XmlCollection = 'XmlCollection'
+    error: Optional[str] = None
+    errorCode: Optional[str] = None
+    fields: Optional[List[BusinessObject.FieldTemplateItem]] = None
+    hasError: Optional[bool] = None
+    lastPasswordResetDate: Optional[datetime] = None
+    lastResetDateTime: Optional[datetime] = None
+    ldapRequired: Optional[bool] = None
+    passwordNeverExpires: Optional[bool] = None
+    publicId: Optional[str] = None
+    recordId: Optional[str] = None
+    securityGroupId: Optional[str] = None
+    shortDisplayName: Optional[str] = None
+    userCannotChangePassword: Optional[bool] = None
+    userMustResetPasswordAtNextLogin: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
+from cherwell_pydantic_api.generated_api_utils import HttpStatusCode
+
+
+ct  # type: ignore
+from enum import Enum
+
 
+Enum  # type: ignore
 
-class StoredValueResponse(ApiBaseModel):
-    description: Optional[str] = None
-    folder: Optional[str] = None
-    id: Optional[str] = None
-    name: Optional[str] = None
-    scope: Optional[str] = None
-    scopeOwner: Optional[str] = None
-    standInKey: Optional[str] = None
-    storedValueType: Optional[StoredValueType] = None
-    value: Optional[str] = None
+
+class UserV2(ApiBaseModel):
+    accountLocked: Optional[bool] = None
+    createDateTime: Optional[datetime] = None
+    displayName: Optional[str] = None
+    fields: Optional[List[BusinessObject.FieldTemplateItem]] = None
+    lastPasswordResetDate: Optional[datetime] = None
+    lastResetDateTime: Optional[datetime] = None
+    ldapRequired: Optional[bool] = None
+    passwordNeverExpires: Optional[bool] = None
+    publicId: Optional[str] = None
+    recordId: Optional[str] = None
+    securityGroupId: Optional[str] = None
+    shortDisplayName: Optional[str] = None
+    userCannotChangePassword: Optional[bool] = None
+    userMustResetPasswordAtNextLogin: Optional[bool] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class View(ApiBaseModel):
-    name: Optional[str] = None
-    viewId: Optional[str] = None
-    image: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
 
 
-class Level(Enum):
-    Fatal = 'Fatal'
-    Error = 'Error'
-    Warning = 'Warning'
-    Info = 'Info'
-    Stats = 'Stats'
-    Debug = 'Debug'
+class UserBatchDeleteRequest(ApiBaseModel):
+    stopOnError: Optional[bool] = None
+    userRecordIds: Optional[List[str]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class LogRequest(ApiBaseModel):
-    keyValueProperties: Optional[List[CherwellObjectID]] = None
-    level: Optional[Level] = None
-    message: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
 
 
-class ImageType(Enum):
-    Imported = 'Imported'
-    File = 'File'
-    Url = 'Url'
+class UserDeleteResponse(ApiBaseModel):
+    error: Optional[str] = None
+    errorCode: Optional[str] = None
+    hasError: Optional[bool] = None
+    users: Optional[List[User]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class SaveGalleryImageRequest(ApiBaseModel):
-    base64EncodedImageData: Optional[str] = None
-    description: Optional[str] = None
-    folder: Optional[str] = None
-    imageType: Optional[ImageType] = None
-    name: Optional[str] = None
-    scope: Optional[str] = None
-    scopeOwner: Optional[str] = None
-    standInKey: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserDeleteV2Response(ApiBaseModel):
+    userRecordId: Optional[str] = None
+    errorCode: Optional[str] = None
+    errorMessage: Optional[str] = None
+    hasError: Optional[bool] = None
+    httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class SaveGalleryImageResponse(ApiBaseModel):
-    name: Optional[str] = None
-    standInKey: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserListResponse(ApiBaseModel):
+    users: Optional[List[UserV2]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class SaveStoredValueRequest(ApiBaseModel):
-    description: Optional[str] = None
-    folder: Optional[str] = None
-    name: Optional[str] = None
-    scope: Optional[str] = None
-    scopeOwner: Optional[str] = None
-    standInKey: Optional[str] = None
-    storedValueType: Optional[StoredValueType] = None
-    value: Optional[str] = None
-
-
-class ActionType(Enum):
-    None_ = 'None'
-    OneStep = 'OneStep'
-    Command = 'Command'
-    BuiltIn = 'BuiltIn'
-    Category = 'Category'
-    SearchGrp = 'SearchGrp'
-    Report = 'Report'
-    Dashboard = 'Dashboard'
-    Calendar = 'Calendar'
-    Visualization = 'Visualization'
-    Group = 'Group'
-    Page = 'Page'
-    DocRepository = 'DocRepository'
-    PortalCommand = 'PortalCommand'
-    ActionCatalog = 'ActionCatalog'
-    OneStepForRecord = 'OneStepForRecord'
-
-
-class LoginEnabledMode(Enum):
-    Anonymous = 'Anonymous'
-    LoggedIn = 'LoggedIn'
-    Both = 'Both'
-
-
-class LoginVisibilityMode(Enum):
-    Anonymous = 'Anonymous'
-    LoggedIn = 'LoggedIn'
-    Both = 'Both'
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserReadRequest(ApiBaseModel):
+    loginId: Optional[str] = None
+    publicId: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class Action(ApiBaseModel):
-    actionCommand: Optional[str] = None
-    actionType: Optional[ActionType] = None
-    alwaysTextAndImage: Optional[bool] = None
-    beginGroup: Optional[bool] = None
-    childActions: Optional[List[Action]] = None
-    dependencies: Optional[List[str]] = None
-    displayText: Optional[str] = None
-    enabled: Optional[bool] = None
-    galleryImage: Optional[str] = None
-    helpText: Optional[str] = None
-    loginEnabledMode: Optional[LoginEnabledMode] = None
-    loginVisibilityMode: Optional[LoginVisibilityMode] = None
-    name: Optional[str] = None
-    parameters: Optional[Dict[str, str]] = None
-    visible: Optional[bool] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserReadResponse(ApiBaseModel):
+    error: Optional[str] = None
+    errorCode: Optional[str] = None
+    hasError: Optional[bool] = None
+    users: Optional[List[User]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class Location(ApiBaseModel):
-    altitude: Optional[float] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserSaveRequest(ApiBaseModel):
+    accountLocked: Optional[bool] = None
     busObId: Optional[ct.BusObID] = None
+    busObPublicId: Optional[str] = None
     busObRecId: Optional[ct.BusObRecID] = None
-    latitude: Optional[float] = None
-    longitude: Optional[float] = None
+    displayName: Optional[str] = None
+    error: Optional[str] = None
+    errorCode: Optional[str] = None
+    hasError: Optional[bool] = None
+    ldapRequired: Optional[bool] = None
+    loginId: Optional[str] = None
+    nextPasswordResetDate: Optional[datetime] = None
+    password: Optional[str] = None
+    passwordNeverExpires: Optional[bool] = None
+    securityGroupId: Optional[str] = None
+    userCannotChangePassword: Optional[bool] = None
+    userInfoFields: Optional[List[BusinessObject.FieldTemplateItem]] = None
+    userMustChangePasswordAtNextLogin: Optional[bool] = None
+    windowsUserId: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class SimplePromptValue(ApiBaseModel):
-    promptDefId: Optional[str] = None
-    promptName: Optional[str] = None
-    value: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserSaveResponse(ApiBaseModel):
+    busObPublicId: Optional[str] = None
+    busObRecId: Optional[ct.BusObRecID] = None
+    error: Optional[str] = None
+    errorCode: Optional[str] = None
+    hasError: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class PromptValue(ApiBaseModel):
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserSaveV2Request(ApiBaseModel):
+    accountLocked: Optional[bool] = None
+    allCultures: Optional[bool] = None
     busObId: Optional[ct.BusObID] = None
-    collectionStoreEntireRow: Optional[str] = None
-    collectionValueField: Optional[str] = None
-    fieldId: Optional[ct.FieldID] = None
-    listReturnFieldId: Optional[ct.FieldID] = None
-    promptId: Optional[str] = None
-    value: Optional[CherwellObjectID] = None
-    valueIsRecId: Optional[bool] = None
-
-
-class ListDisplayOption(Enum):
-    Auto = 'Auto'
-    Text = 'Text'
-    Combo = 'Combo'
-    GridList = 'GridList'
-    SimpleList = 'SimpleList'
-    PromptSimpleGrid = 'PromptSimpleGrid'
-
-
-class PromptType(Enum):
-    None_ = 'None'
-    Text = 'Text'
-    Number = 'Number'
-    DateTime = 'DateTime'
-    Logical = 'Logical'
-    Binary = 'Binary'
-    DateOnly = 'DateOnly'
-    TimeOnly = 'TimeOnly'
-    Json = 'Json'
-    JsonArray = 'JsonArray'
-    Xml = 'Xml'
-    XmlCollection = 'XmlCollection'
-    TimeValue = 'TimeValue'
+    busObPublicId: Optional[str] = None
+    busObRecId: Optional[ct.BusObRecID] = None
+    displayName: Optional[str] = None
+    ldapRequired: Optional[bool] = None
+    loginId: Optional[str] = None
+    nextPasswordResetDate: Optional[datetime] = None
+    password: Optional[str] = None
+    passwordNeverExpires: Optional[bool] = None
+    securityGroupId: Optional[str] = None
+    specificCulture: Optional[str] = None
+    userCannotChangePassword: Optional[bool] = None
+    userInfoFields: Optional[List[BusinessObject.FieldTemplateItem]] = None
+    userMustChangePasswordAtNextLogin: Optional[bool] = None
+    windowsUserId: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class Prompt(ApiBaseModel):
-    allowValuesOnly: Optional[bool] = None
-    busObId: Optional[ct.BusObID] = None
-    collectionStoreEntireRow: Optional[str] = None
-    collectionValueField: Optional[str] = None
-    constraintXml: Optional[str] = None
-    contents: Optional[str] = None
-    default: Optional[str] = None
-    fieldId: Optional[ct.FieldID] = None
-    isDateRange: Optional[bool] = None
-    listDisplayOption: Optional[ListDisplayOption] = None
-    listReturnFieldId: Optional[ct.FieldID] = None
-    multiLine: Optional[bool] = None
-    promptId: Optional[str] = None
-    promptType: Optional[PromptType] = None
-    promptTypeName: Optional[str] = None
-    required: Optional[bool] = None
-    text: Optional[str] = None
-    value: Optional[CherwellObjectID] = None
-    values: Optional[List[str]] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserSaveV2Response(ApiBaseModel):
+    busObPublicId: Optional[str] = None
+    busObRecId: Optional[ct.BusObRecID] = None
+    errorCode: Optional[str] = None
+    errorMessage: Optional[str] = None
+    hasError: Optional[bool] = None
+    httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class ServiceInfoResponse(ApiBaseModel):
-    apiVersion: Optional[str] = None
-    csmCulture: Optional[str] = None
-    csmVersion: Optional[str] = None
-    systemDateTime: Optional[datetime] = None
-    timeZone: Optional[CherwellObjectID] = None
-    systemUtcOffset: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserReadV2Response(ApiBaseModel):
+    users: Optional[List[UserV2]] = None
+    errorCode: Optional[str] = None
+    errorMessage: Optional[str] = None
+    hasError: Optional[bool] = None
+    httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class ManagerFolder(ApiBaseModel):
-    association: Optional[str] = None
-    childFolders: Optional[List[ManagerFolder]] = None
-    childItems: Optional[List[ManagerItem]] = None
-    id: Optional[str] = None
-    links: Optional[List[CherwellLink]] = None
-    localizedScopeName: Optional[str] = None
-    name: Optional[str] = None
-    parentId: Optional[str] = None
-    scope: Optional[str] = None
-    scopeOwner: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchDeleteResponse(ApiBaseModel):
+    responses: Optional[List[UserDeleteResponse]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class ViewsResponse(ApiBaseModel):
-    views: Optional[List[View]] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchDeleteV2Response(ApiBaseModel):
+    responses: Optional[List[UserDeleteV2Response]] = None
+    errorCode: Optional[str] = None
+    errorMessage: Optional[str] = None
+    hasError: Optional[bool] = None
+    httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class LogBatchRequest(ApiBaseModel):
-    logRequests: Optional[List[LogRequest]] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchReadRequest(ApiBaseModel):
+    readRequests: Optional[List[UserReadRequest]] = None
+    stopOnError: Optional[bool] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class ManagerData(ApiBaseModel):
-    root: Optional[ManagerFolder] = None
-    supportedAssociations: Optional[List[CherwellNameValuePair]] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchReadResponse(ApiBaseModel):
+    responses: Optional[List[UserReadV2Response]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
-Action.update_forward_refs()
-ManagerFolder.update_forward_refs()
+import cherwell_pydantic_api.types as ct
+
+
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchSaveRequest(ApiBaseModel):
+    saveRequests: Optional[List[UserSaveRequest]] = None
+    stopOnError: Optional[bool] = None
+
+
+import cherwell_pydantic_api.types as ct
+
+
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchSaveResponse(ApiBaseModel):
+    responses: Optional[List[UserSaveResponse]] = None
+
+
+import cherwell_pydantic_api.types as ct
+
+
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchSaveV2Request(ApiBaseModel):
+    saveRequests: Optional[List[UserSaveV2Request]] = None
+    stopOnError: Optional[bool] = None
+
+
+import cherwell_pydantic_api.types as ct
+
+
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class UserBatchSaveV2Response(ApiBaseModel):
+    responses: Optional[List[UserSaveV2Response]] = None
+    errorCode: Optional[str] = None
+    errorMessage: Optional[str] = None
+    hasError: Optional[bool] = None
+    httpStatusCode: Optional[HttpStatusCode] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Forms.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,38 +9,59 @@
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import ApiBaseModel, HttpStatusCode
 
 from .... import CherwellObjectID
 from . import BusinessObject, Core
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class SectionField(ApiBaseModel):
     attributes: Optional[List[CherwellObjectID]] = None
     fieldId: Optional[ct.FieldID] = None
     fieldType: Optional[str] = None
     label: Optional[str] = None
     multiline: Optional[bool] = None
     value: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class Section(ApiBaseModel):
     sectionFields: Optional[List[SectionField]] = None
     galleryImage: Optional[str] = None
     title: Optional[str] = None
     relationshipId: Optional[ct.RelationshipID] = None
     targetBusObId: Optional[ct.BusObID] = None
     targetBusObRecId: Optional[ct.BusObRecID] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class MobileFormResponse(ApiBaseModel):
     actions: Optional[List[Core.Action]] = None
     attachments: Optional[List[BusinessObject.Attachment]] = None
     galleryImage: Optional[str] = None
     locationInformation: Optional[Core.Location] = None
     sections: Optional[List[Section]] = None
     title: Optional[str] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/OneStepActions.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import ApiBaseModel, HttpStatusCode
 
 from . import Core
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class OneStepActionResponse(ApiBaseModel):
     completed: Optional[bool] = None
     currentPrimaryBusObId: Optional[ct.BusObID] = None
     currentPrimaryBusObRecId: Optional[ct.BusObRecID] = None
     hasNewAccessToken: Optional[bool] = None
     newAccessToken: Optional[str] = None
     errorCode: Optional[str] = None
@@ -23,13 +30,20 @@
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class OneStepActionRequest(ApiBaseModel):
     acquireLicense: Optional[bool] = None
     busObId: Optional[ct.BusObID] = None
     busObRecId: Optional[ct.BusObRecID] = None
     oneStepActionStandInKey: Optional[str] = None
     promptValues: Optional[List[Core.SimplePromptValue]] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Queues.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,93 +6,149 @@
 from enum import Enum
 from typing import Optional
 
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import ApiBaseModel
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class AddItemToQueueRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObRecId: Optional[ct.BusObRecID] = None
     queueStandInKey: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import HttpStatusCode
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class AddItemToQueueResponse(ApiBaseModel):
     historyRecId: Optional[str] = None
     historyText: Optional[str] = None
     historyTypeId: Optional[str] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class CheckInQueueItemRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObRecId: Optional[ct.BusObRecID] = None
     historyNotes: Optional[str] = None
     queueStandInKey: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class CheckInQueueItemResponse(ApiBaseModel):
     historyRecId: Optional[str] = None
     historyText: Optional[str] = None
     historyTypeId: Optional[str] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class CheckOutQueueItemRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObRecId: Optional[ct.BusObRecID] = None
     historyNotes: Optional[str] = None
     queueStandInKey: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class CheckOutQueueItemResponse(ApiBaseModel):
     historyRecId: Optional[str] = None
     historyText: Optional[str] = None
     historyTypeId: Optional[str] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class RemoveItemFromQueueRequest(ApiBaseModel):
     busObId: Optional[ct.BusObID] = None
     busObRecId: Optional[ct.BusObRecID] = None
     historyNotes: Optional[str] = None
     queueStandInKey: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class RemoveItemFromQueueResponse(ApiBaseModel):
     historyRecId: Optional[str] = None
     historyText: Optional[str] = None
     historyTypeId: Optional[str] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Teams.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/WebApi/DataContracts/Lifecycle.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,183 +3,177 @@
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import List, Optional
 
 import cherwell_pydantic_api.types as ct
-from cherwell_pydantic_api.generated_api_utils import ApiBaseModel
+from cherwell_pydantic_api.generated_api_utils import ApiBaseModel, HttpStatusCode
 
-from . import BusinessObject
+
+ct  # type: ignore
+from enum import Enum
 
 
-class AddUserToTeamRequest(ApiBaseModel):
-    teamId: Optional[str] = None
-    userIsTeamManager: Optional[bool] = None
-    userRecordId: Optional[str] = None
+Enum  # type: ignore
+
+
+class GetStagesResponseStages(ApiBaseModel):
+    id: Optional[str] = None
+    isFinal: Optional[bool] = None
+    name: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
-from cherwell_pydantic_api.generated_api_utils import HttpStatusCode
 
 
-class AddUserToTeamResponse(ApiBaseModel):
-    errorCode: Optional[str] = None
-    errorMessage: Optional[str] = None
-    hasError: Optional[bool] = None
-    httpStatusCode: Optional[HttpStatusCode] = None
+ct  # type: ignore
+from enum import Enum
 
 
-import cherwell_pydantic_api.types as ct
+Enum  # type: ignore
 
 
-class Team(ApiBaseModel):
-    teamId: Optional[str] = None
-    teamName: Optional[str] = None
+class GetStatusesResponseStatuses(ApiBaseModel):
+    id: Optional[str] = None
+    isInitial: Optional[bool] = None
+    name: Optional[str] = None
+    stageId: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class TeamsV2Response(ApiBaseModel):
-    teams: Optional[List[Team]] = None
-    errorCode: Optional[str] = None
-    errorMessage: Optional[str] = None
-    hasError: Optional[bool] = None
-    httpStatusCode: Optional[HttpStatusCode] = None
+ct  # type: ignore
+from enum import Enum
 
 
-class TeamType(Enum):
-    User = 'User'
-    CustomerWorkgroup = 'CustomerWorkgroup'
+Enum  # type: ignore
+
+
+class GetTransitionsResponseTransition(ApiBaseModel):
+    id: Optional[str] = None
+    name: Optional[str] = None
+    fromStatusId: Optional[str] = None
+    toStatusId: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class TeamResponse(ApiBaseModel):
-    description: Optional[str] = None
-    emailAlias: Optional[str] = None
-    fields: Optional[List[BusinessObject.FieldTemplateItem]] = None
-    image: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class GetRecordStatusResponse(ApiBaseModel):
+    id: Optional[str] = None
     name: Optional[str] = None
-    teamId: Optional[str] = None
-    teamType: Optional[TeamType] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class RemoveUserFromTeamResponse(ApiBaseModel):
-    teamId: Optional[str] = None
-    userRecordId: Optional[str] = None
-    errorCode: Optional[str] = None
-    errorMessage: Optional[str] = None
-    hasError: Optional[bool] = None
-    httpStatusCode: Optional[HttpStatusCode] = None
+ct  # type: ignore
+from enum import Enum
 
 
-import cherwell_pydantic_api.types as ct
+Enum  # type: ignore
 
 
-class RemoveCustomerFromWorkgroupResponse(ApiBaseModel):
-    workgroupId: Optional[str] = None
-    customerRecordId: Optional[str] = None
-    errorCode: Optional[str] = None
-    errorMessage: Optional[str] = None
-    hasError: Optional[bool] = None
-    httpStatusCode: Optional[HttpStatusCode] = None
+class GetTransitionOptionsResponseTransition(ApiBaseModel):
+    name: Optional[str] = None
+    id: Optional[str] = None
+    isAvailable: Optional[bool] = None
+    criteria: Optional[List[str]] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class TeamSaveRequest(ApiBaseModel):
-    description: Optional[str] = None
-    emailAlias: Optional[str] = None
-    image: Optional[str] = None
-    teamId: Optional[str] = None
-    teamName: Optional[str] = None
-    teamType: Optional[TeamType] = None
+ct  # type: ignore
+from enum import Enum
 
 
-import cherwell_pydantic_api.types as ct
+Enum  # type: ignore
 
 
-class TeamSaveResponse(ApiBaseModel):
-    teamId: Optional[str] = None
-    errorCode: Optional[str] = None
-    errorMessage: Optional[str] = None
-    hasError: Optional[bool] = None
-    httpStatusCode: Optional[HttpStatusCode] = None
+class TransitionRecordRequest(ApiBaseModel):
+    transitionOptionId: Optional[str] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class SaveTeamMemberRequest(ApiBaseModel):
-    isTeamManager: Optional[bool] = None
-    setAsDefaultTeam: Optional[bool] = None
-    teamId: Optional[str] = None
-    userRecId: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
 
 
-import cherwell_pydantic_api.types as ct
+Enum  # type: ignore
 
 
-class SaveTeamMemberResponse(ApiBaseModel):
+class GetStagesResponse(ApiBaseModel):
+    stages: Optional[List[GetStagesResponseStages]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class SaveWorkgroupMemberRequest(ApiBaseModel):
-    customerRecordId: Optional[str] = None
-    workgroupId: Optional[str] = None
-    customerIsWorkgroupManager: Optional[bool] = None
+ct  # type: ignore
+from enum import Enum
 
 
-import cherwell_pydantic_api.types as ct
+Enum  # type: ignore
 
 
-class SaveWorkgroupMemberResponse(ApiBaseModel):
+class GetStatusesResponse(ApiBaseModel):
+    statuses: Optional[List[GetStatusesResponseStatuses]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class AddUserToTeamByBatchRequest(ApiBaseModel):
-    addUserToTeamRequests: Optional[List[AddUserToTeamRequest]] = None
-    stopOnError: Optional[bool] = None
+ct  # type: ignore
+from enum import Enum
 
 
-import cherwell_pydantic_api.types as ct
+Enum  # type: ignore
 
 
-class AddUserToTeamByBatchResponse(ApiBaseModel):
-    responses: Optional[List[AddUserToTeamResponse]] = None
+class GetTransitionsResponse(ApiBaseModel):
+    transitions: Optional[List[GetTransitionsResponseTransition]] = None
     errorCode: Optional[str] = None
     errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
     httpStatusCode: Optional[HttpStatusCode] = None
 
 
 import cherwell_pydantic_api.types as ct
 
 
-class TeamsResponse(ApiBaseModel):
-    error: Optional[str] = None
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
+class GetTransitionOptionsResponse(ApiBaseModel):
+    transitions: Optional[List[GetTransitionOptionsResponseTransition]] = None
     errorCode: Optional[str] = None
+    errorMessage: Optional[str] = None
     hasError: Optional[bool] = None
-    teams: Optional[List[Team]] = None
+    httpStatusCode: Optional[HttpStatusCode] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/Trebuchet/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 
 import cherwell_pydantic_api.types as ct
 from cherwell_pydantic_api.generated_api_utils import ApiBaseModel
 
 from .. import CherwellObjectID
 
 
+ct  # type: ignore
+from enum import Enum
+
+
+Enum  # type: ignore
+
+
 class CherwellNameValuePair(ApiBaseModel):
     name: Optional[str] = None
     valueObject: Optional[CherwellObjectID] = None
     valueString: Optional[str] = None
     category: Optional[str] = None
     description: Optional[str] = None
     displayShowsValue: Optional[bool] = None
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/_generated/api/models/__init__.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/_generated/api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48384,12 +48384,18 @@
 000bcff0: 2750 6572 666f 726d 2042 7573 696e 6573  'Perform Busines
 000bd000: 7320 4f62 6a65 6374 204c 6966 6563 7963  s Object Lifecyc
 000bd010: 6c65 206f 7065 7261 7469 6f6e 7327 2c0a  le operations',.
 000bd020: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
 000bd030: 2020 2020 2020 205d 2c0a 2020 2020 290a         ],.    ).
 000bd040: 0a0a 696d 706f 7274 2063 6865 7277 656c  ..import cherwel
 000bd050: 6c5f 7079 6461 6e74 6963 5f61 7069 2e74  l_pydantic_api.t
-000bd060: 7970 6573 2061 7320 6374 0a66 726f 6d20  ypes as ct.from 
-000bd070: 6368 6572 7765 6c6c 5f70 7964 616e 7469  cherwell_pydanti
-000bd080: 635f 6170 692e 7479 7065 7320 696d 706f  c_api.types impo
-000bd090: 7274 2043 6865 7277 656c 6c4f 626a 6563  rt CherwellObjec
-000bd0a0: 7449 440a                                tID.
+000bd060: 7970 6573 2061 7320 6374 0a0a 0a63 7420  ypes as ct...ct 
+000bd070: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+000bd080: 6672 6f6d 2065 6e75 6d20 696d 706f 7274  from enum import
+000bd090: 2045 6e75 6d0a 0a0a 456e 756d 2020 2320   Enum...Enum  # 
+000bd0a0: 7479 7065 3a20 6967 6e6f 7265 0a0a 6672  type: ignore..fr
+000bd0b0: 6f6d 2063 6865 7277 656c 6c5f 7079 6461  om cherwell_pyda
+000bd0c0: 6e74 6963 5f61 7069 2e74 7970 6573 2069  ntic_api.types i
+000bd0d0: 6d70 6f72 7420 4368 6572 7765 6c6c 4f62  mport CherwellOb
+000bd0e0: 6a65 6374 4944 0a0a 0a43 6865 7277 656c  jectID...Cherwel
+000bd0f0: 6c4f 626a 6563 7449 4420 2023 2074 7970  lObjectID  # typ
+000bd100: 653a 2069 676e 6f72 650a                 e: ignore.
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/api.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,36 +20,39 @@
         self._base_url = self._settings.base_url
         self._client_id = self._settings.client_id
         self._username = self._settings.username
         self._password = self._settings.password
         self._client = httpx.AsyncClient(base_url=str(self._base_url),
                                          headers={
                                              'Content-Type': 'application/json'},
-                                         params={'locale': 'en-150'},
+                                         #params={'locale': 'en-US'},
                                          timeout=self._settings.timeout,
                                          verify=self._settings.verify)
         self._token: Optional[str] = None
         # TODO: come up with a better solution for these:
         self.raise_on_error_500 = False
         self.retry_on_error_401 = False
         self.retry_on_error_401_wait = 4.0
         self.reauthentication_counter = 0
+        if self._settings.intercept_path:
+            from .intercept_transport import InterceptTransport
+            self._intercept = InterceptTransport(self._client, self._settings.intercept_path)
 
 
     async def request(self,
                       method: Literal['GET', 'POST', 'PUT', 'DELETE'],
                       url: URLType,
                       *,
                       content: Optional[Union[str, bytes,
                                               Iterable[bytes], AsyncIterable[bytes]]] = None,
                       data: Optional[Mapping[str, Any]] = None,
                       json: Optional[Any] = None,
                       params: Optional[Mapping[str, Any]] = None,
                       content_type: Optional[str] = None,
-                      **kwargs
+                      **kwargs: Any
                       ) -> Response:
         if content_type is not None:
             kwargs.setdefault('headers', {})['Content-Type'] = content_type
         req = self._client.build_request(
             method, url=url, content=content, data=data, json=json, params=params, **kwargs)
         self.last_request = req
         response = await self._client.send(req)
@@ -78,15 +81,15 @@
         return await self.request('POST', url, data=data, params=params)
 
 
     async def post(self, url: URLType) -> Response:
         return await self.request('POST', url)
 
 
-    async def delete(self, url, **kwargs) -> Response:
+    async def delete(self, url: URLType, **kwargs: Any) -> Response:
         return await self.request('DELETE', url, **kwargs)
 
 
     @docwraps(GeneratedInterfaces.Token)
     async def authenticate(self):
         # TODO: support other grant_type values
         response = await self.Token(grant_type='password', client_id=self._client_id, username=self._username, password=self._password)
@@ -124,14 +127,15 @@
 
     @docwraps(GeneratedInterfaces.GetBusinessObjectSummariesV1)
     async def get_bo_summaries(self, type: BusinessObjectType) -> list[Summary]:
         return await self.GetBusinessObjectSummariesV1(type=type)
 
 
     # TODO: legacy, remove
+    __LEGACY = r"""
     bo_name_to_id = get_busobid
 
 
     def get_bo(self, publicId, busObId=None, busObName=None):
         if busObId is None:
             busObId = self.bo_name_to_id(busObName)
         r = self.get(
@@ -189,7 +193,8 @@
         self.last_search = search
         r = self.post('/api/v1/getsearchresults', search)
         return r
 
 
     def get_search_results_eq(self, bo_dict, fields=None):
         return self.get_search_results_operator(bo_dict=bo_dict, op_dict={}, fields=fields)
+"""
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/collector.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/modelgen/collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 from cherwell_pydantic_api.utils import docwraps
 
 
 
 try:
     import click
 except ImportError:
-    click = None
+    click = None  # type: ignore
 
 
-FilterType = Union[Pattern, str, None]
+FilterType = Union[Pattern[str], str, None]
 
 
-def compile_filter(filter: FilterType) -> Optional[Pattern]:
+def compile_filter(filter: FilterType) -> Optional[Pattern[str]]:
     if filter is None:
         return None
     if isinstance(filter, str):
         if filter == '':
             return None
         return re.compile(filter)
     return filter
@@ -67,15 +67,15 @@
     @cached_property
     def valid_schema(self) -> Optional[ValidSchema]:
         if self.schema is None:
             return None
         return ValidSchema.from_schema_response(self.schema)
 
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, Union[str, int, None]]:
         "Convert to dictionary e.g. for DataFrame use"
         return {'name': self.name,
                 'busobid': self.busobid,
                 'verdict': self.verdict,
                 'bo_type': self.bo_type,
                 'num_fields': len(self.schema.fieldDefinitions) if (self.schema and self.schema.fieldDefinitions) else None,
                 'displayName': self.summary.displayName,
@@ -83,106 +83,112 @@
                 'major': self.summary.major,
                 'supporting': self.summary.supporting,
                 'parent_name': self.parent_item.name if self.parent_item else None,
                 }
 
 
 class CollectorSettings(BaseModel):
-    bo_include_filter: Optional[Pattern]
-    bo_exclude_filter: Optional[Pattern]
+    # mypy wants to see Pattern[str] but Pydantic requires Pattern
+    bo_include_filter: Optional[Pattern]  # type: ignore
+    bo_exclude_filter: Optional[Pattern]  # type: ignore
 
 
 class Collector:
     "Collects Business Object summaries and schemas from a Cherwell instance, in order to filter them and generate models."
 
     def __init__(self, instance: Instance, *, bo_include_filter: FilterType = None, bo_exclude_filter: FilterType = None, verbose: bool = False):
         self._instance = instance
         self._bo_include_filter = compile_filter(bo_include_filter)
         self._bo_exclude_filter = compile_filter(bo_exclude_filter)
         self.items: list[CollectorItem] = []
         self.verbose = verbose
 
 
     @property
-    def bo_include_filter(self) -> Optional[Pattern]:
+    def bo_include_filter(self) -> Optional[Pattern[str]]:
         return self._bo_include_filter
 
     @bo_include_filter.setter
     def bo_include_filter(self, value: FilterType):
         self._bo_include_filter = compile_filter(value)
 
     @property
-    def bo_exclude_filter(self) -> Optional[Pattern]:
+    def bo_exclude_filter(self) -> Optional[Pattern[str]]:
         return self._bo_exclude_filter
 
     @bo_exclude_filter.setter
     def bo_exclude_filter(self, value: FilterType):
         self._bo_exclude_filter = compile_filter(value)
 
 
     def filter_bo(self, type: str, summary: Summary) -> bool:
+        if summary.name is None:
+            return False
         if self._bo_exclude_filter is not None:
             if self._bo_exclude_filter.match(summary.name):
                 return False
         if self._bo_include_filter is not None:
             if self._bo_include_filter.match(summary.name):
                 return True
         return False
 
 
     def verbose_report(self, item: CollectorItem):
         icon = "[**]" if item.verdict else "[  ]"
         if item.schema:
-            fields = len(
+            fields: Union[str, int] = len(
                 item.schema.fieldDefinitions) if item.schema.fieldDefinitions else 0
-            rels = len(
+            rels: Union[str, int] = len(
                 item.schema.relationships) if item.schema.relationships else 0
         else:
             fields = rels = '?'
         report = f" {item.bo_type[:3]:3} {item.name:30} {fields:>4} {rels:>4}  {item.busobid:24}"
         if click:
             click.secho(icon, nl=False,
                         bg='green' if item.verdict else 'red', fg='white')
             click.secho(report, fg='cyan')
         else:
             print(icon, report)
 
 
-    @alru_cache
+    @alru_cache()
     @docwraps(Instance.get_bo_summaries)
     async def get_bo_summaries(self, bo_type: BusinessObjectType) -> list[Summary]:
         return await self._instance.get_bo_summaries(bo_type)
 
 
     @alru_cache(maxsize=1024)
     @docwraps(Instance.get_bo_schema)
     async def get_bo_schema(self, busobid: BusObID) -> Optional[SchemaResponse]:
         return await self._instance.get_bo_schema(busobid=busobid)
 
 
     async def select(self) -> list[CollectorItem]:
         "Get all the business object summaries from Cherwell and filter them."
-        items = []
+        items: list[CollectorItem] = []
         for bo_type in cast(list[BusinessObjectType], ['Major', 'Supporting', 'Lookup', 'Groups']):
             for bo_summary in await self.get_bo_summaries(bo_type):
                 verdict = self.filter_bo(bo_type, bo_summary)
-                item = CollectorItem(
-                    bo_type=bo_type, summary=bo_summary, verdict=verdict)
+                item = CollectorItem(bo_type=bo_type, summary=bo_summary, verdict=verdict)
                 items.append(item)
                 # Add group members. There is only one level of groups according to Cherwell docs.
                 if bo_summary.groupSummaries:
                     for group_summary in bo_summary.groupSummaries:
                         verdict = self.filter_bo(bo_type, group_summary)
-                        sub_item = CollectorItem(
-                            bo_type=bo_type, summary=group_summary, verdict=verdict, parent_item=item)
+                        # If a child group is included, then the parent is included too.
+                        if verdict and not item.verdict:
+                            item.verdict = True
+                        sub_item = CollectorItem(bo_type=bo_type, summary=group_summary,
+                                                 verdict=verdict, parent_item=item)
                         items.append(sub_item)
         return items
 
 
     async def collect(self) -> list[CollectorItem]:
+        "Get all the business object summaries from Cherwell, filter them, and fetch the schemas of matching business objects."
         items = await self.select()
         for item in items:
             if item.verdict:
                 schema = await self.get_bo_schema(item.summary.busObId)
             else:
                 schema = None
             item.schema = schema
@@ -190,20 +196,24 @@
                 self.verbose_report(item)
         self.items = items
         return items
 
 
     def generate_models(self) -> FileGenerator:
         yield ('__init__.py', '### autogenerated by cherwell_pydantic_api ###\n')
-        model_generator = PydanticModelGenerator(self._instance.settings)
+        model_generator = PydanticModelGenerator(self._instance)
         yield ('__base.py', model_generator.generate_base())
         for item in self.items:
             if not item.verdict:
                 continue
             schema = self._instance.bo.get_schema(item.busobid)
+            if item.parent_item:
+                schema.parentSchema = self._instance.bo.get_schema(item.parent_item.busobid)
+            else:
+                schema.parentSchema = None
             yield (f"{schema.identifier}.py", model_generator.generate_model(schema))
 
 
     def save_models(self, repo: ModelRepo):
         return repo.save(instance=self._instance, file_type='model', file_generator=self.generate_models())
 
 
@@ -215,17 +225,17 @@
 
     def save_settings(self, repo: ModelRepo):
         return repo.save(instance=self._instance, file_type='registry', file_generator=self.generate_settings())
 
 
     def load_settings(self, repo: ModelRepo):
         collector_settings = CollectorSettings.parse_file(
-            repo._repo_dir / self._instance.settings.get_repo_subpackage() / 'registry/collector_settings.json')
-        self.bo_include_filter = collector_settings.bo_include_filter
-        self.bo_exclude_filter = collector_settings.bo_exclude_filter
+            repo.repo_dir / self._instance.settings.get_repo_subpackage() / 'registry/collector_settings.json')
+        self.bo_include_filter = collector_settings.bo_include_filter  # type: ignore
+        self.bo_exclude_filter = collector_settings.bo_exclude_filter  # type: ignore
 
 
     def clear_caches(self):
         self.get_bo_summaries.cache_clear()
         self.get_bo_schema.cache_clear()
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/modelgen/repo.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/modelgen/repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# pyright: strict, reportUnknownMemberType=false
 import logging
 from pathlib import Path
-from typing import Any, Iterable, Literal, Optional, Union
+from typing import Iterable, Literal, Optional, Union
 
 from dulwich import porcelain
 from dulwich.errors import NotGitRepository
 from dulwich.repo import Repo
 
 from cherwell_pydantic_api.instance import Instance
 from cherwell_pydantic_api.settings import Settings
@@ -15,24 +16,24 @@
 
 
 FileTypeLiteral = Literal['registry', 'model']
 FileGenerator = Iterable[tuple[str, str]]
 
 
 class ModelRepo:
-    _repo: Repo
+    _repo: Optional[Repo]
 
     def __init__(self, *, create: bool = False, permit_missing: bool = False):
         is_new = False
         self._repo_dir = Settings().repo_dir.absolute()
         if not self._repo_dir.exists():
             if create:
                 self._repo_dir.mkdir(parents=True)
             elif permit_missing:
-                self._repo = None  # type: ignore
+                self._repo = None
                 return
             else:
                 raise FileNotFoundError(
                     f'Repo directory {self._repo_dir} does not exist')
         try:
             self._repo = Repo(root=str(self._repo_dir))
         except NotGitRepository:
@@ -48,26 +49,28 @@
             commit = f'cherwell_pydantic_api: initial repo setup'
             author = Settings().repo_author
             self._repo.do_commit(message=commit.encode(),
                                  author=author.encode())
 
 
     def prepare_save(self, *, instance_name: Optional[str] = None, instance: Optional[Instance] = None) -> tuple[Instance, Path]:
+        if self._repo is None:
+            raise ValueError('Repository is missing')
         # ensure repo is clean
-        repo_status = porcelain.status(self._repo)  # type: ignore
+        repo_status = porcelain.status(self._repo) # type: ignore
         if repo_status.unstaged or repo_status.untracked or repo_status.staged['add'] or repo_status.staged['delete'] or repo_status.staged['modify']:
             raise ValueError(
                 'Repo is not clean, please commit or stash your changes before saving')
 
         # resolve arguments
         if instance is None:
             if instance_name is None:
                 raise ValueError(
                     'Either instance_name or instance must be given')
-            instance = Instance._instances[instance_name]
+            instance = Instance.use(instance_name)
         else:
             instance_name = instance.settings.name
 
         instance_dir = self._repo_dir / instance.settings.get_repo_subpackage()
         if not instance_dir.exists():
             logging.info(
                 f'Creating instance directory {instance_dir} for instance {instance_name}')
@@ -77,14 +80,16 @@
 
     def save(self, *,
              instance_name: Optional[str] = None,
              instance: Optional[Instance] = None,
              file_type: FileTypeLiteral = 'registry',
              file_generator: FileGenerator,
              commit: bool = True) -> Optional[bytes]:
+        if self._repo is None:
+            raise ValueError('Repository is missing')
         instance, instance_dir = self.prepare_save(
             instance_name=instance_name, instance=instance)
         file_type_dir = instance_dir / file_type
         if not file_type_dir.exists():
             logging.info(
                 f'Creating {file_type} directory {file_type_dir} for instance {instance_name}')
             file_type_dir.mkdir()
@@ -95,14 +100,16 @@
             self._repo.stage(str(filepath.relative_to(self._repo_dir)))
         if commit:
             return self.commit(instance=instance, file_type=file_type)
         return None
 
 
     def commit(self, *, instance: Instance, file_type: FileTypeLiteral) -> Optional[bytes]:
+        if self._repo is None:
+            raise ValueError('Repository is missing')
         # Check if there are any changes to commit (because dulwich allows empty commits)
         encoding = self._repo.get_config().encoding
         repo_status = porcelain.status(self._repo)  # type: ignore
         if not repo_status.staged['add'] and not repo_status.staged['delete'] and not repo_status.staged['modify']:
             logging.info(
                 f'No {file_type} changes to commit for instance {instance.settings.name}')
             return None
@@ -112,61 +119,68 @@
         if branch.encode(encoding) not in porcelain.branch_list(self._repo):
             porcelain.branch_create(self._repo, branch.encode(encoding))
         ref = f'refs/heads/{branch}'
         porcelain.update_head(self._repo, ref)  # this is like git checkout
         logging.info(
             f'Committing {file_type} to {branch} for instance {instance.settings.name}')
         return self._repo.do_commit(message=commit.encode(),
-                                    author=author.encode(), ref=ref.encode())
+                                    author=author.encode(), ref=ref.encode()) # type: ignore
 
 
     def save_instance(self, instance: Instance) -> Optional[bytes]:
         return self.save(instance=instance, file_generator=instance.bo.marshal())
 
 
     def save_all(self) -> dict[str, Optional[bytes]]:
-        r = {}
-        for instance in Instance._instances.values():
+        r: dict[str, Optional[bytes]] = {}
+        for instance in Instance.all_instances():
             r[instance.settings.name] = self.save_instance(instance)
         return r
 
 
     def get_info(self, *,
                  instance_name: Optional[str] = None,
-                 instance: Optional[Instance] = None) -> dict[str, Union[str, bool, dict[str, Union[str, bool]]]]:
+                 instance: Optional[Instance] = None) -> dict[str, Union[str, bool, dict[str, Union[str, bool, None]]]]:
         # resolve arguments
         if instance is None:
             if instance_name is None:
                 raise ValueError(
                     'Either instance_name or instance must be given')
-            instance = Instance._instances[instance_name]
+            instance = Instance.use(instance_name)
         else:
             instance_name = instance.settings.name
         instance_dir = self._repo_dir / instance.settings.get_repo_subpackage()
-        r = {'instance': {
+        r: dict[str, Union[str, bool, dict[str, Union[str, bool, None]]]] = {'instance': {
             'name': instance.settings.name,
             'repo_subpackage': str(instance.settings.get_repo_subpackage()),
             'repo_branch': instance.settings.get_repo_branch()
         },
             'repo': {
                 'path': self._repo.path if self._repo else None,
                 'settings_path': str(self._repo_dir),
                 'instance_path': str(instance_dir),
                 'instance_path_exists': instance_dir.exists(),
                 'author': Settings().repo_author,
         },
         }
-        if self._repo is not None:
+        if self._repo is not None: # type: ignore # could be None if permit_missing is True
             repo_status = porcelain.status(self._repo)  # type: ignore
             r['status'] = {
                 'dirty': repo_status.unstaged or repo_status.untracked or repo_status.staged['add'] or repo_status.staged['delete'] or repo_status.staged['modify']
             }
             r['ready'] = True
         else:
             r['ready'] = False
         return r
 
 
     @property
     def directory(self) -> str:
         "The absolute path to the repo directory"
+        if self._repo is None:
+            return str(self._repo_dir)
         return self._repo.path
+
+    @property
+    def repo_dir(self) -> Path:
+        "The absolute path to the repo directory as a Path object"
+        return self._repo_dir
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/registry.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from collections import defaultdict
-from typing import Iterable, Mapping, Optional, Union
+from typing import Iterable, Iterator, Mapping, Optional, Union
 from weakref import WeakValueDictionary
 
 from pydantic import AnyHttpUrl, BaseModel
 
 from cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject import (
-    Relationship,
     SchemaResponse,
     Summary,
 )
 from cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core import ServiceInfoResponse
-from cherwell_pydantic_api.bo.valid_schema import ValidSchema
+from cherwell_pydantic_api.bo.valid_schema import ValidRelationship, ValidSchema
 from cherwell_pydantic_api.bo.wrapper import BusinessObjectWrapper, BusinessObjectWrapperBase
 from cherwell_pydantic_api.interfaces import ApiRequesterInterface
 from cherwell_pydantic_api.types import BusObID, BusObIdentifier, RelationshipID
 
 
 
 # Registry of business object schemas.
@@ -33,35 +32,49 @@
     pass
 
 
 class BusinessObjectRegistry(Mapping[str, BusinessObjectWrapperBase]):
     # There is exactly one BusinessObjectRegistry per Instance.
     # There can be more than one wrapper per BO but only one schema or summary.
 
+    _instance: ApiRequesterInterface
+    _wrapper_class: type[BusinessObjectWrapperBase]
+    _schemas: dict[BusObID, ValidSchema]
+    _summaries: dict[BusObID, Summary]
+    _parents: dict[BusObID, BusObID]
+    _name_to_id: dict[BusObIdentifier, BusObID]
+    _relationships: dict[RelationshipID, ValidRelationship]
+    _unresolved_relationships: dict[BusObID, set[RelationshipID]]
+    _bo_rels: defaultdict[BusObID, set[RelationshipID]] = defaultdict(set)
+    _wrappers: WeakValueDictionary[BusObID, BusinessObjectWrapperBase] = WeakValueDictionary()
+    _service_info: Optional[ServiceInfoResponse] = None
+    _models: WeakValueDictionary[BusObID, type[BusinessObjectModelRegistryMixin]] = WeakValueDictionary()
+
+
     def __init__(self, instance: ApiRequesterInterface, wrapper_class: type[BusinessObjectWrapperBase] = BusinessObjectWrapper):
         self._instance = instance
         self._wrapper_class = wrapper_class
-        self._schemas: dict[BusObID, ValidSchema] = {}
-        self._summaries: dict[BusObID, Summary] = {}
-        self._name_to_id: dict[BusObIdentifier, BusObID] = {}
-        self._relationships: dict[RelationshipID, Relationship] = {}
-        self._bo_rels: defaultdict[BusObID,
-                                   set[RelationshipID]] = defaultdict(set)
-        self._wrappers: WeakValueDictionary[BusObID,
-                                            wrapper_class] = WeakValueDictionary()
-        self._service_info: Optional[ServiceInfoResponse] = None
-        self._models: WeakValueDictionary[BusObID,
-                                          type[BusinessObjectModelRegistryMixin]] = WeakValueDictionary()
+        self._schemas = {}
+        self._summaries = {}
+        self._parents = {}
+        self._name_to_id = {}
+        self._relationships = {}
+        self._unresolved_relationships = defaultdict(set)
+        self._bo_rels = defaultdict(set)
+        self._wrappers = WeakValueDictionary()
+        self._service_info = None
+        self._models = WeakValueDictionary()
 
 
     def marshal(self, include_summaries: bool = False) -> Iterable[tuple[str, str]]:
         yield ('instance_name.txt', self._instance.settings.name)
         for busobid, schema in self._schemas.items():
-            yield (f'bo.{busobid}.json', schema.json(indent=2, exclude={'relationships'}, sort_keys=True, exclude_unset=True, exclude_defaults=True))
-        # TODO: include relationships
+            yield (f'bo.{busobid}.json', schema.json(indent=2, sort_keys=True, exclude_unset=True, exclude_defaults=True))
+        for relid, rel in self._relationships.items():
+            yield (f'rel.{relid}.json', rel.json(indent=2, exclude={'target_schema', 'source_schema', 'fieldDefinitions'}, sort_keys=True, exclude_unset=True, exclude_defaults=True))
         if include_summaries:
             for busobid, summary in self._summaries.items():
                 if busobid in self._schemas:
                     continue
                 yield (f'bo_sum.{busobid}.json', summary.json(indent=2, sort_keys=True))
         names_csv = [
             f"{name};{self._name_to_id[name]}\n" for name in self._name_to_id.keys()]
@@ -82,16 +95,16 @@
 
 
     def register(self, schema: SchemaResponse):
         if schema.busObId is None:
             raise ValueError('SchemaResponse.busObId is None')
         if schema.name is None:
             raise ValueError('SchemaResponse.name is None')
-        busobid = BusObID(schema.busObId)
         valid_schema = ValidSchema.from_schema_response(schema)
+        busobid = valid_schema.busObId
         identifier = valid_schema.identifier
         if busobid in self._schemas:
             if self._schemas[busobid] != valid_schema:
                 raise ValueError(
                     f'SchemaResponse busObId {busobid} already registered and new schema is different')
             if identifier in self._name_to_id:
                 if self._name_to_id[identifier] != busobid:
@@ -99,33 +112,57 @@
                         f'SchemaResponse identifier {identifier} already registered and new busObId is different')
         else:
             self._schemas[busobid] = valid_schema
             self._name_to_id[identifier] = busobid
 
         # Register relationships
         if schema.relationships:
+            summary = self._summaries.get(busobid)
+            if summary is None:
+                raise ValueError(
+                    f'busObId {busobid} ({valid_schema.name}) has relationships but no summary was registered')
             for rel in schema.relationships:
-                assert rel.relationshipId is not None
-                relid = RelationshipID(rel.relationshipId)
+                valid_rel = ValidRelationship.from_relationship(
+                    valid_schema, rel)
+                relid = valid_rel.relationshipId
                 assert relid in valid_schema.relationshipIds
+                valid_rel.source_schema = valid_schema
+                valid_schema.relationships[relid] = valid_rel
+                if valid_rel.target in self._schemas:
+                    valid_rel.target_schema = self.get_schema(valid_rel.target)
+                    valid_rel.target_name = valid_rel.target_schema.name
+                else:
+                    self._unresolved_relationships[valid_rel.target].add(relid)
+                    if valid_rel.target in self._summaries:
+                        valid_rel.target_name = self._summaries[valid_rel.target].name
                 if relid in self._relationships:
-                    if self._relationships[relid] != rel:
+                    existing_rel = self._relationships[relid]
+                    if existing_rel.source != busobid:
+                        if self._parents.get(busobid) == existing_rel.source:
+                            # print(f"Skipping child relationship {relid} on {identifier} < {existing_rel.source_schema.identifier}")
+                            continue
+                    if existing_rel != valid_rel:
                         raise ValueError(
-                            f'Relationship {relid} already registered and new relationship is different')
+                            f'Relationship {relid} already registered ({existing_rel.source_schema.name} to {existing_rel.target_schema and existing_rel.target_schema.name}) and new relationship is different ({valid_schema.name} to {valid_rel.target_schema and valid_rel.target_schema.name})')
                     if not relid in self._bo_rels[busobid]:
                         # TODO: This occurs in group summaries
                         continue
                         raise ValueError(
                             f"Relationship {relid} is not in busObId {busobid}")
                 else:
-                    self._relationships[relid] = rel
+                    self._relationships[relid] = valid_rel
                     self._bo_rels[busobid].add(relid)
-                    # TODO: Make a ValidRelationship wrapper like ValidSchema
-                    assert rel.target is not None
-                    self._bo_rels[rel.target].add(relid) # type: ignore
+                    self._bo_rels[valid_rel.target].add(relid)
+
+        # Fixup relationships of which this bo is a target
+        if self._unresolved_relationships[busobid]:
+            for relid in self._unresolved_relationships[busobid]:
+                urel = self._relationships[relid]
+                urel.target_schema = valid_schema
+            del self._unresolved_relationships[busobid]
 
 
     def register_summary(self, summary: Summary):
         # TODO: decide if this is needed, if so make it more useful
         if summary.busObId is None:
             raise ValueError('Summary.busObId is None')
         if summary.name is None:
@@ -140,14 +177,21 @@
             self._name_to_id[identifier] = busobid
         if busobid in self._summaries:
             if self._summaries[busobid] != summary:
                 raise ValueError(
                     f'Summary busObId {summary.busObId} already registered and new summary is different')
             return
         self._summaries[busobid] = summary
+        if summary.groupSummaries:
+            for sub_summary in summary.groupSummaries:
+                if sub_summary.busObId is None:
+                    raise ValueError(
+                        'Summary.busObId is None in groupSummaries')
+                self.register_summary(sub_summary)
+                self._parents[sub_summary.busObId] = busobid
 
 
     def register_model(self, busobid: BusObID, model: type[BusinessObjectModelRegistryMixin]):
         self._models[busobid] = model
 
 
     def get_model(self, busobid: BusObID) -> type[BusinessObjectModelRegistryMixin]:
@@ -181,15 +225,15 @@
             busobid = False
         if not busobid or busobid not in self._schemas:
             busobname = BusObIdentifier(item)
             busobid = self._name_to_id[busobname]
         return self.get_wrapper(busobid)
 
 
-    def __iter__(self) -> Iterable[str]:
+    def __iter__(self) -> Iterator[str]:
         """Iterate over the names of the registered business objects. Don't include summaries. (Not the business object IDs)"""
         return iter([k for k, v in self._name_to_id.items() if v in self._schemas])
 
 
     def __len__(self) -> int:
         """Return the number of registered business objects. Don't include summaries."""
         return len(self._schemas)
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/templates/dot_gitignore` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/templates/dot_gitignore`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/bo/wrapper.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/bo/wrapper.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/__init__.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/env python
+# pyright: reportUnusedImport=false
 
 import sys
 from pathlib import Path
 
+from click import Context
+
 
 
 if sys.version_info < (3, 9):
     sys.stderr.write("Python 3.9 or higher is required.")
     sys.exit(1)
 try:
     import cherwell_pydantic_api
@@ -32,15 +35,15 @@
 or
     poetry add -E all cherwell_pydantic_api
 
 """)
     sys.exit(1)
 
 
-def check_envpath(offer_setup=True):
+def check_envpath(offer_setup: bool = True) -> Path:
     envpath = Path.cwd().joinpath('cherwell.env')
     if not envpath.exists():
         click.secho(
             f"\nNo cherwell.env file found in the current path, {Path.cwd()}.\nYou can now create one, or press Ctrl+C to abort.\n", fg='yellow')
         from .welcome import initial_setup
         initial_setup(envpath)
     return envpath
@@ -86,25 +89,25 @@
 def root():
     "cherwell_pydantic_api CLI"
     pass
 
 
 @root.command(context_settings=dict(ignore_unknown_options=True, allow_extra_args=True))
 @click.pass_context
-def getting_started(ctx):
+def getting_started(ctx: Context):
     "Launch the Getting Started notebook in JupyterLab"
     try:
-        import jupyterlab.labapp
+        import jupyterlab.labapp  # type: ignore
     except:
         click.secho(
             "To use the JupyterLab interface, you must install cherwell_pydantic_api[all].\n", fg='red')
         return
     import os.path
     nb = os.path.dirname(__file__) + '/../examples/GettingStarted.ipynb'
-    jupyterlab.labapp.main(ctx.args + [nb])
+    jupyterlab.labapp.main(ctx.args + [nb]) # type: ignore
 
 
 def cli_normal():
     from . import check
     root.add_command(check.check)
     from . import ipython
     root.add_command(ipython.ipython_shell)
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/check.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/check.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pyright: reportUnusedImport=false, reportUnusedFunction=false, reportUntypedFunctionDecorator=false
+
 from typing import Optional
 
 import click
 
 from ..instance import Instance
 from .utils import async_command
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/ipython.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/ipython.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
+# pyright: reportUnusedImport=false, reportUnusedFunction=false, reportUntypedFunctionDecorator=false
 
-from typing import TYPE_CHECKING, Optional
+
+from typing import TYPE_CHECKING, Any, Optional
 
 import click
 
 
 
 @click.command('ipython', context_settings={'allow_extra_args': True, 'ignore_unknown_options': True}, epilog="Further arguments will be passed to IPython.")
 @click.option('--instance-name', '-I', help='The name of the instance to use. If not specified, the default instance will be used.')
 @click.option('--quiet', '-q', is_flag=True, help='Suppress most messages')
 @click.pass_context
-def ipython_shell(ctx, instance_name: Optional[str] = None, quiet: bool = False):
+def ipython_shell(ctx: click.Context, instance_name: Optional[str] = None, quiet: bool = False):
     "Start an interactive IPython shell"
     try:
         import IPython
         import traitlets
     except:
         if not quiet:
             click.secho("IPython is not installed", fg='red')
@@ -22,19 +24,22 @@
 
     from cherwell_pydantic_api.bo.modelgen.collector import Collector
     from cherwell_pydantic_api.bo.modelgen.repo import ModelRepo
     from cherwell_pydantic_api.instance import Instance
     from cherwell_pydantic_api.interactive import Interactive
     from cherwell_pydantic_api.settings import Settings
 
-    collector = Collector(Instance.use(instance_name
-                                       ), verbose=True, bo_include_filter=r'(?i)ticket|task|changerequest|conf.*|journal.*|spec.*|.*port*')
+    collector = Collector(Instance.use(instance_name), verbose=True, bo_include_filter=r'(?i)ticket$')
     repo = ModelRepo(create=True)
+    try:
+        collector.load_settings(repo)
+    except:
+        pass
 
-    def startup(objs):
+    def startup(objs: list[str]) -> Interactive:
         cw = Interactive(instance_name=instance_name,
                          waiter=IPython.get_ipython().loop_runner)  # type: ignore
         if not quiet:
             click.secho('\nWelcome to cherwell_pydantic_api!', fg='cyan')
             click.secho(
                 f'Connecting to instance "{cw.instance.settings.name}" at {cw.instance.settings.base_url}...', nl=False, fg='magenta')
         cw.authenticate()
@@ -59,28 +64,28 @@
             def _ipython_display_(self):
                 click.secho('\n'.join(self.msg))
 
         cw.help = help()
         return cw
 
     # Create a namespace for the shell
-    ns = {}
+    ns: dict[str, Any] = {}
     for name, obj in locals().items():
         if not (name.startswith('_') or name in ('ctx', 'IPython', 'traitlets', 'quiet', 'ns')):
             ns[name] = obj
     ns['click'] = click
     ns['object_help'] = [k for k in ns.keys() if k not in ('object_help', 'startup')]
     ns['object_help'].sort()
     config = traitlets.config.Config()  # type: ignore
-    config.InteractiveShellApp.exec_lines = [
+    config.InteractiveShellApp.exec_lines = [  # type: ignore
         "cw = startup(object_help)",
         "del startup",
         "del object_help",
     ]
     if quiet:
-        config.InteractiveShellApp.display_banner = False
-    IPython.start_ipython(config=config, user_ns=ns, argv=ctx.args)
+        config.InteractiveShellApp.display_banner = False  # type: ignore
+    IPython.start_ipython(config=config, user_ns=ns, argv=ctx.args)  # type: ignore
 
 
 
 if __name__ == '__main__':
     ipython_shell()
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/cli/welcome.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/cli/welcome.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Module for the welcoming initial setup CLI"""
+# pyright: reportUnusedImport=false
 
 import time
 from pathlib import Path
+from typing import Optional
 
 import click
 import httpx
 try:
     import readline
 except:
     pass
 
 
-def api_detect(urls):
+def api_detect(urls: list[str]) -> tuple[Optional[str], str, float, bool]:
     "Try to detect the Cherwell API at the given URLs"
     for url in urls:
         try:
             click.secho(
                 f"Trying to detect Cherwell API at {url}...", fg='cyan')
             t1 = time.time()
             verify = True
@@ -30,25 +32,25 @@
             if response.is_success:
                 service_info = response.json()
                 return (url, service_info.get('apiVersion', 'unknown'), t2 - t1, verify)
             click.secho(
                 f"HTTP Error: {response.status_code} {response.reason_phrase}", fg='red')
         except Exception as e:
             click.secho(f"Error: {e}", fg='red')
-    return (None, None, 0.0, False)
+    return (None, '', 0.0, False)
 
 
-def initial_setup(envpath: Path):
+def initial_setup(envpath: Path) -> None:
     "Create a new cherwell.env file from user input"
-    envdict = {}
+    envdict: dict[str, str] = {}
     click.secho("""Enter the API base URL of your Cherwell instance, e.g. https://myinstance.cherwellsoftware.com/CherwellAPI
 You can also just enter the hostname or IP address and I will attempt to guess the rest.
 If you have multiple instances, set up the development instance first. You can add your production instance later.\n""", fg='green')
     while True:
-        api_base_url = click.prompt('API base URL or host', type=str)
+        api_base_url: Optional[str] = click.prompt('API base URL or host', type=str)
         if not api_base_url:
             continue
         if not api_base_url.startswith('http'):
             urls = [f"https://{api_base_url}/CherwellAPI",
                     f"http://{api_base_url}/CherwellAPI"]
         else:
             urls = [api_base_url]
@@ -59,15 +61,15 @@
             f"No API found. Please check your URL and network connectivity.", fg='red')
     click.secho(
         f"Success! Cherwell API version {api_version} found at {api_base_url}", bg='green', fg='black')
     envdict['cherwell_base_url'] = api_base_url
     duration = round(duration, 1)
     if duration > 5.0:
         click.secho(f"Warning: The API took {duration} seconds to respond. I will configure a timeout of {duration*2} seconds.", fg='yellow')
-        envdict['cherwell_timeout'] = duration * 2
+        envdict['cherwell_timeout'] = f"{duration * 2}"
     if not verify:
         click.secho(
             f"Warning: SSL certificate verification failed. Connection will be set up with verify=False", fg='red', bg='yellow')
         envdict['cherwell_verify'] = 'off'
     click.echo(f"""
 You can now enter your client ID, username and password. You can also leave these blank and configure them later,
 however you won't be able to use the API until you do. Contact your Cherwell administrator if you don't have these details.
@@ -80,10 +82,12 @@
         'Password', type=str, default='')
 
     click.echo('Would you like to create the file ', nl=False)
     click.secho(f"{envpath}", fg='cyan', nl=False)
     click.echo(' with the above settings?')
     if click.confirm('Create file?', default=None):
         envpath.write_text(''.join([f"{k}={v}\n" for k, v in envdict.items()]))
-        click.secho(f"{envpath} created successfully:", fg='green')
-
+        click.secho(f"{envpath} created successfully.\n", fg='green')
+        click.secho("If you are a first-time user, I recommend the Getting Started JupyterLab notebook.", bg='green', fg='black')
+        click.secho("Run it with", nl=False, bg='green', fg='black')
+        click.secho(" cwcli getting-started", fg='cyan')
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/examples/GettingStarted.ipynb` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/examples/GettingStarted.ipynb`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/generated_api_utils.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/generated_api_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import re
-from typing import TYPE_CHECKING, Any, AsyncIterable, Iterable, Literal, Mapping, Optional, Type, Union, get_origin
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncIterable,
+    Iterable,
+    Literal,
+    Mapping,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    get_args,
+    get_origin,
+)
 
 import httpx
 import pydantic
 
+from cherwell_pydantic_api.types import CherwellObjectID, FileDownload
+from cherwell_pydantic_api.utils import issubclass_noexcept
+
 
 
 URLType = Union[str, httpx.URL]
 HttpStatusCode = httpx.codes
 Response = httpx.Response
 
-_re_path_param = re.compile(r'^[a-zA-Z0-9_-]+$')
+_re_path_param = re.compile(r'^[a-zA-Z0-9_.-]+$')
 
 
 class ApiBaseModel(pydantic.BaseModel):
     """Base class of all generated API models."""
 
     # Methods to improve IPython experience
 
-    def __dir__(self):
-        return [arg[0] for arg in self.__repr_args__()]
+    def __dir__(self) -> list[str]:
+        return [arg[0] for arg in self.__repr_args__()] # type: ignore # I don't think None will ever be returned
 
-    def _repr_pretty_(self, p, cycle):
+    def _repr_pretty_(self, p: Any, cycle: Any) -> None:
         if cycle:
             p.text(f"{self.__class__.__name__}(...)")
         else:
             p.begin_group(2, f"{self.__class__.__name__}(")
             first = True
             for name, value in self.__repr_args__():
                 if not first:
@@ -59,70 +75,73 @@
         async def delete(self, url: URLType, *, params: Optional[Mapping[str, Any]] = None) -> Response:
             ...
 else:
     class GeneratedInterfaceBaseType:
         pass
 
 
+ApiBaseModel_co = TypeVar('ApiBaseModel_co', bound=ApiBaseModel, covariant=True)
+
 class GeneratedInterfaceBase(GeneratedInterfaceBaseType):
     """Generated Cherwell API interface"""
 
-    def validate_path_param(self, value: str, type: Type = str):
+    def validate_path_param(self, value: str, type: Union[Type[Union[str, int]], object] = str) -> None:
+        # Literal types can be passed in and mypy sees them as object
         if not _re_path_param.match(value):
             raise ValueError(f"Invalid path parameter: {value!r}")
         type_origin = get_origin(type)
         if type_origin is Literal:
-            if value.lower() not in [a.lower() for a in type.__args__]:
+            if value.lower() not in [a.lower() for a in get_args(type)]:
                 raise ValueError(
                     f"Parameter mismatch with literal: {value} not in {type}")
 
 
-    def parse_response(self, response: Response, rtype: Type) -> Any:
+    def parse_response(self, response: Response, rtype: Type[Union[ApiBaseModel, list[ApiBaseModel_co], list[CherwellObjectID], str, bytes]]) -> Any:
         # If the response type has a `httpStatusCode` field, set it to the actual HTTP status code
         # and don't raise an exception if the HTTP request failed
-        try:
-            # issubclass can fail especially with types
-            is_api = issubclass(rtype, ApiBaseModel)
-        except:
-            is_api = False
-
-        if is_api:
+        if issubclass_noexcept(rtype, ApiBaseModel):
+            if TYPE_CHECKING:
+                assert issubclass(rtype, ApiBaseModel)
             status_code = None
             try:
                 # The Cherwell server sends the header: "Content-Type: application/json;charset=UTF-8"
                 obj = rtype.parse_raw(response.content,
                                       content_type=response.headers.get(
                                           'content-type').split(';', 1)[0],
                                       encoding=response.encoding or 'utf-8')
                 if hasattr(obj, 'httpStatusCode'):
                     obj.httpStatusCode = response.status_code  # type: ignore
                     status_code = response.status_code
             except pydantic.ValidationError:
                 # Maybe the pydantic validation failed because the HTTP request failed
-                if not response.is_success:
-                    response.raise_for_status()
+                response.raise_for_status()
                 raise
             # HTTP error: if we can respond with a httpStatusCode in the response, do so, otherwise raise an exception
             if not response.is_success:
                 if status_code:
                     return obj
                 response.raise_for_status()
             # HTTP success and pydantic validation succeeded
             return obj
 
         # Reach here if the type isn't a pydantic model
-        if not response.is_success:
-            response.raise_for_status()
+        response.raise_for_status()
 
         if rtype is str:
             return response.text
         if rtype is bytes:
             return response.content
-        if rtype is None:
-            return None
 
         return pydantic.parse_raw_as(rtype,
                                      response.content,
                                      content_type=response.headers.get(
                                          'content-type').split(';', 1)[0],
                                      encoding=response.encoding or 'utf-8')
 
+
+    def download_response(self, response: Response) -> FileDownload:
+        response.raise_for_status()
+        return response.aiter_bytes()
+
+    def check_response(self, response: Response) -> None:
+        "Raise an exception if the HTTP request failed"
+        response.raise_for_status()
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/instance.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from typing import Any, ClassVar, Optional
+from typing import Any, ClassVar, Iterator, Optional
 
 from cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.BusinessObject import (
     ReadResponse,
     SchemaResponse,
     Summary,
 )
 from cherwell_pydantic_api._generated.api.models.Trebuchet.WebApi.DataContracts.Core import ServiceInfoResponse
@@ -30,14 +30,18 @@
         self._connection = Connection(instance_settings)
 
 
     @property
     def settings(self) -> InstanceSettingsBase:
         return self._settings
 
+    @property
+    def connection(self) -> Connection:
+        return self._connection
+
 
     @docwraps(Connection.authenticate)
     async def authenticate(self):
         return await self._connection.authenticate()
 
 
     @docwraps(Connection.logout)
@@ -102,7 +106,13 @@
             instance_settings = settings.get_instance(name)
         if instance_settings is None:
             raise ValueError(f"Instance {name} not found in settings")
         name = instance_settings.name
         if name not in cls._instances:
             cls._instances[name] = cls(instance_settings, cls.__call_token)
         return cls._instances[name]
+
+
+    @classmethod
+    def all_instances(cls) -> Iterator["Instance"]:
+        """Return an iterator over all existing Instance objects."""
+        return iter(cls._instances.values())
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interactive.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,56 +15,61 @@
 
 
 __all__ = ['Interactive']
 
 
 _ReturnType = TypeVar("_ReturnType")
 _WaiterType = Callable[[Coroutine[Any, Any, _ReturnType]], _ReturnType]
+_Waiter = _WaiterType[Any]
 
 
 class RestaurantInterface:
     "A restaurant contains a waiter."
-    _waiter: _WaiterType
+    _waiter: _Waiter
+
+    @property
+    def waiter(self) -> _Waiter:
+        return self._waiter
 
 
 def wait(amethod: Callable[..., Coroutine[Any, Any, _ReturnType]]) -> Callable[..., _ReturnType]:
     """Decorator to convert an async method into a sync method, using the waiter method of the Interactive instance.
     """
 
     @wraps(amethod)
-    def wrapper(self: RestaurantInterface, *args, **kwargs):
-        return self._waiter(amethod(self, *args, **kwargs))
+    def wrapper(self: RestaurantInterface, *args: Any, **kwargs: Any) -> _ReturnType:
+        return self.waiter(amethod(self, *args, **kwargs))
     return wrapper
 
 
 class WaiterProxy(RestaurantInterface):
     """A proxy around an object with async methods that uses the waiter method to make all public methods sync."""
 
-    def __init__(self, async_obj: object, waiter: _WaiterType):
+    def __init__(self, async_obj: object, waiter: _Waiter):
         self._async_obj = async_obj
         self._waiter = waiter
         self.__doc__ = async_obj.__doc__
         self.__wrapped__ = async_obj
 
     def __getattr__(self, name: str) -> Any:
         if name.startswith('_'):
             raise AttributeError(name)
         amethod = getattr(self._async_obj, name)
         if not callable(amethod):
             return amethod
 
         @wraps(amethod)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any):
             r = amethod(*args, **kwargs)
             if isinstance(r, types.CoroutineType):
-                return self._waiter(r)
+                return self._waiter(r) # type: ignore
             return r
         return wrapper
 
-    def __setattr__(self, name: str, value) -> None:
+    def __setattr__(self, name: str, value: Any) -> None:
         if not name.startswith('_') and hasattr(self._async_obj, name):
             setattr(self._async_obj, name, value)
         else:
             super().__setattr__(name, value)
 
     def __delattr__(self, name: str) -> None:
         if not name.startswith('_') and hasattr(self._async_obj, name):
@@ -76,54 +81,54 @@
         return dir(self._async_obj)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._async_obj!r})"
 
 
 @wraps(BusinessObjectWrapper)
-def create_bo_wrapper_class(waiter: _WaiterType) -> type[BusinessObjectWrapper]:
+def create_bo_wrapper_class(waiter: _Waiter) -> type[BusinessObjectWrapper]:
     class InteractiveBusinessObjectWrapper(BusinessObjectWrapper, RestaurantInterface):
         _waiter = waiter
 
         @wait
-        async def get(self, publicid: str) -> ReadResponse:
+        async def get(self, publicid: str) -> ReadResponse: # type: ignore
             return await super().get(publicid=publicid)
 
     return InteractiveBusinessObjectWrapper
 
 
 
 class Interactive(RestaurantInterface):
     """A wrapper around various cherwell_pydantic_api objects, using the waiter method to make all methods sync (no await needed).
     Each instance of Interactive wraps a specific Instance and indirectly the Connection object.
     It also wraps the BusinessObjectRegistry, so that all BusinessObjectWrapper objects created by it can be accessed with using await.
     """
 
-    def __init__(self, *, instance_name: Optional[str] = None, waiter: Optional[_WaiterType] = None):
+    def __init__(self, *, instance_name: Optional[str] = None, waiter: Optional[_Waiter] = None):
         self._instance = Instance.use(name=instance_name)
         if waiter is None:
             import asyncio
             waiter = asyncio.run
         self._waiter = waiter
         self._instance_proxy = WaiterProxy(self._instance, self._waiter)
         self._connection_proxy = WaiterProxy(
-            self._instance._connection, self._waiter)
+            self._instance.connection, self._waiter)
         self.help: Any = ''
 
     @property
     def connection(self) -> WaiterProxy:
         "WaiterProxy wrapper around the Connection object."
         return self._connection_proxy
 
     @property
     def instance(self) -> WaiterProxy:
         "WaiterProxy wrapper around the Instance object."
         return self._instance_proxy
 
-    def async_wrap(self, **kwargs) -> "Interactive":
+    def async_wrap(self, **kwargs: object) -> "Interactive":
         "Wrap the given objects with WaiterProxy and add them as attributes to the Interactive instance."
         # TODO: restrict attribute name
         for attr, obj in kwargs.items():
             setattr(self, attr, WaiterProxy(obj, self._waiter))
         return self
 
     @wait
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/interfaces.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/interfaces.py`

 * *Files identical despite different names*

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/__init__.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/schema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-
+# pyright: basic, reportMissingImports=false, reportGeneralTypeIssues=false
+# mypy: ignore-errors
 import sys
 import importlib.abc
 import importlib.machinery
 import types
 from typing import Any, Callable, List, Optional, Sequence, Tuple, Union
 from marshmallow import Schema, pre_load, post_load, post_dump, fields as marshmallow_fields
 import pprint
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/schema/fields.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/schema/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# pyright: basic, reportMissingImports=false, reportGeneralTypeIssues=false
+# mypy: ignore-errors
+
 from marshmallow import fields
 import datetime
 import re
 
 
 def from_cw_datetime(value):
     value = value.replace('/', '.')
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/settings.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import keyword
 import re
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-from pydantic import AnyHttpUrl, BaseSettings, Field, SecretStr, validator
+from pydantic import validator  # type: ignore # pylance doesn't like it
+from pydantic import AnyHttpUrl, BaseSettings, Field, SecretStr
 
 
 
 class InstanceSettingsBase(BaseSettings):
     name: str = Field(default='_unset')
     base_url: Optional[AnyHttpUrl] = Field(default=None)
-    client_id: SecretStr = Field(default='')
+    client_id: SecretStr = Field(default=SecretStr(''))
     username: str = Field(default='')
-    password: SecretStr = Field(default='')
+    password: SecretStr = Field(default=SecretStr(''))
     timeout: float = Field(default=5.0)
     verify: Union[str, bool] = Field(default='on')
     subpackage: Optional[Path] = Field(
         description='Subpackage name, corresponds to subdirectory name within repo_dir, if unset default to instance name')
     repo_branch: Optional[str] = Field(
         description='Branch to use for this instance, if unset default to main')
+    intercept_path: Optional[Path] = Field(description='If set, intercept HTTP requests and responses and save to files here (internal use)')
 
     @validator('verify')
-    def validate_verify(cls, v):
+    def validate_verify(cls, v: str) -> Union[str, bool]:
         if v.lower() in ('off', 'false', 'no'):
             return False
         if v.lower() in ('', 'on', 'true', 'yes'):
             return True
         return v
 
     def get_repo_subpackage(self) -> Path:
@@ -40,34 +42,34 @@
 class InstanceSettings(InstanceSettingsBase):
     pass
 
 
 class Settings(InstanceSettingsBase):
     name: str = Field('default', const=True)
     inst: dict[str, InstanceSettings] = Field(default={})
-    repo_dir: Path = Field(default='repo')
+    repo_dir: Path = Field(default=Path('repo'))
     repo_author: str = 'cherwell_pydantic_api <noreply@cherwell-pydantic-api.nonexistent.anthonyuk.dev>'
     suppress_banner: bool = Field(default=False, description='Suppress the CLI welcome banner')
 
     _re_inst_name = re.compile(r'^[a-z][a-z0-9]+$')
 
     def get_instance(self, instance_name: Optional[str] = None) -> Optional[InstanceSettingsBase]:
         """Return the instance settings for the given instance, or the default settings if instance_name is None or 'default'"""
         if instance_name is None or instance_name == self.name:
             return self
         return self.inst.get(instance_name, None)
 
     @validator('inst')
-    def validate_inst(cls, v):
-        for inst_name, inst in v.items():
+    def validate_inst(cls, v: dict[str, InstanceSettings]) -> dict[str, InstanceSettings]:
+        for inst_name in v:
             if not cls._re_inst_name.match(inst_name) or inst_name == 'default' or keyword.iskeyword(inst_name):
                 raise ValueError(f"Invalid instance name: {inst_name}")
         return v
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._fixup()
 
     def _fixup(self):
         #TODO: Use pydantic's built-in support for this
         """After instantiation, propagate the default values to the instances."""
         for inst_name, inst in self.inst.items():
@@ -83,15 +85,15 @@
                 inst.username = self.username
             if not inst.password:
                 inst.password = self.password
             if not inst.timeout:
                 inst.timeout = self.timeout
 
 
-    class Config:
+    class Config: # type: ignore
         env_file = ['cherwell.env']
         env_file_encoding = 'utf-8'
         env_prefix = 'cherwell_'
         env_nested_delimiter = '__'
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/types.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import keyword
 import re
 from typing import TYPE_CHECKING, Annotated, Any, AsyncIterable, Iterable, Literal, NewType, Optional, Union
 
 
 
+# TODO: There must be a better solution here
 if TYPE_CHECKING:
     IDType = NewType
     IdentifierType = NewType
     LCIdentifierType = NewType
 else:
     def IDType(name, tp):
         """Create a subtype of str with a constructor that converts identifiers to lower case. Non-hex characters
@@ -23,41 +24,42 @@
 
     def IdentifierType(name, tp):
         """Create a subtype of str with a constructor that converts field names, etc. to a string
         that can be used as a Python identifier, except python keywords and fields that begin with a digit,
         in which case a prefix of I_ will be added (capitals). For the type checker it is the same as NewType"""
         def identifier_type(x):
             x = re.sub(r'[^0-9A-Za-z_]', '_', x)
-            if x[0].isdigit() or keyword.iskeyword(x):
+            if x[0].isdigit() or x[0] == '_' or keyword.iskeyword(x):
                 x = 'I_' + x
             return x
         identifier_type.__name__ = name
         identifier_type.__supertype__ = tp
         return identifier_type
 
     def LCIdentifierType(name, tp):
         """Create a subtype of str with a constructor that converts field names, etc. to a _lowercase_ string
         that can be used as a Python identifier, except python keywords and fields that begin with a digit,
         in which case a prefix of I_ will be added (capitals). For the type checker it is the same as NewType"""
         def identifier_type(x):
             x = re.sub(r'[^0-9a-z_]', '_', x.lower())
-            if x[0].isdigit() or keyword.iskeyword(x):
+            if x[0].isdigit() or x[0] == '_' or keyword.iskeyword(x):
                 x = 'I_' + x
             return x
         identifier_type.__name__ = name
         identifier_type.__supertype__ = tp
         return identifier_type
 
 
 CherwellObjectID = dict[str, Any]
 BusObID = IDType("BusObID", str)
 BusObRecID = IDType("BusObRecID", str)
 BusObIDParamType = BusObID
 BusObIdentifier = LCIdentifierType("BusObIdentifier", str)
-FieldID = IDType("FieldID", str)
+FieldID = NewType("FieldID", str)
+ShortFieldID = IDType("ShortFieldID", str)
 FieldIdentifier = IdentifierType("FieldIdentifier", str)
 RelationshipID = IDType("RelationshipID", str)
 FileType = Union[str, bytes, Iterable[bytes], AsyncIterable[bytes]]
 FileUpload = Annotated[FileType, "FileUpload"]
 FileDownload = Annotated[FileType, "FileDownload"]
 StringResponse = NewType("StringResponse", str)
 
@@ -86,12 +88,23 @@
 AttachmentType.__doc__ = """For file types, select the type of attachment:
         Imported - Attachment was imported into database.
         Linked - Attachment is linked to an external file.
         URL - Attachment is a URL."""
 
 
 class CherwellAPIError(Exception):
+    extras: dict[str, Any]
+
     def __init__(self, msg: str = "Cherwell API error", *, errorCode: Optional[str] = None,
                  errorMessage: Optional[str] = None,
-                 httpStatusCode: Optional[Any] = None):
+                 httpStatusCode: Optional[Any] = None,
+                 **kwargs: Any):
         message = f"{msg}: {errorCode=} {errorMessage=} {httpStatusCode=}"
+        self.errorCode = errorCode
+        self.errorMessage = errorMessage
+        self.httpStatusCode = httpStatusCode
+        self.extras = kwargs
         super().__init__(message)
+
+
+class SaveBusinessObjectError(CherwellAPIError):
+    pass
```

### Comparing `cherwell_pydantic_api-0.0.3/cherwell_pydantic_api/utils.py` & `cherwell_pydantic_api-0.0.4/cherwell_pydantic_api/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-from typing import Any, Callable
-from cherwell_pydantic_api.types import FieldID
+from typing import Any, Callable, TypeVar
 
+from cherwell_pydantic_api.types import FieldID, ShortFieldID
 
 
-def fieldid_parts(field_id: str) -> dict[str, str]:
+
+def fieldid_parts(field_id: FieldID) -> dict[str, str]:
     """The fieldId has the format: 'BO:947dfef9ae6b072ca567a444dca79d9f9ea47a112f,FI:9492462c89a8f7785f1537412ca51a2f218293edb0,RE:9492535dfbf4286b49047f45bab2f201737e739a46'
     This method returns a dict with the keys 'BO', 'FI', 'RE', etc. and the values are the corresponding IDs."""
-    r = {}
+    r: dict[str, str] = {}
     for part in field_id.split(','):
         k, v = part.split(':', 1)
         assert k in ('BO', 'FI', 'RE')
-        r[k.upper()] = FieldID(v)
+        r[k.upper()] = ShortFieldID(v)
     return r
 
 
-def docwraps(func: Callable[..., Any]) -> Callable[..., Any]:
+_R = TypeVar('_R')
+
+def docwraps(func: Any) -> Callable[[Callable[..., _R]], Callable[..., _R]]:
     """Decorator to copy the docstring from the wrapped function to the wrapper function."""
-    def wrapper(wrapper_func: Callable[..., Any]) -> Callable[..., Any]:
+    def wrapper(wrapper_func: Callable[..., _R]) -> Callable[..., _R]:
         if wrapper_func.__doc__ is None:
             wrapper_func.__doc__ = f"Wraps {func.__qualname__}"
         else:
             wrapper_func.__doc__ += f"\nWraps {func.__qualname__}"
         if func.__doc__ is not None:
             wrapper_func.__doc__ += ":\n" + func.__doc__
         return wrapper_func
     return wrapper
+
+
+def issubclass_noexcept(cls: type, classinfo: Any) -> bool:
+    try:
+        return issubclass(cls, classinfo)
+    except TypeError:
+        return False
```

### Comparing `cherwell_pydantic_api-0.0.3/pyproject.toml` & `cherwell_pydantic_api-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cherwell_pydantic_api"
-version = "0.0.3"
+version = "0.0.4"
 description = "A pythonic, asyncio connector for the Cherwell CSM API with full usage of Pydantic types"
 authors = ["Anthony Uk <uk@anthonyuk.dev>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/dataway/cherwell_pydantic_api"
 homepage = "https://github.com/dataway/cherwell_pydantic_api"
 
@@ -24,36 +24,41 @@
 ]
 keywords = ["cherwell", "pydantic"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pydantic = {extras = ["dotenv"], version = "^1.10.6"}
+pydantic-changedetect = "^0.2.5"
 httpx = "^0.24.0"
 async-lru = "^2.0.2"
 click = "^8.1.3"
 black = { version = "^23.1.0", optional = true }
 dulwich = { version = "^0.21.3", optional = true }
 jupyter = { version = "^1.0.0", optional = true }
 nest-asyncio = { version = "^1.5.6", optional = true }
 ipywidgets = { version = "^8.0.5", optional = true }
-jupyterlab = { version = "^3.6.2", optional = true }
+jupyterlab = { version = "^4.0.0", optional = true }
 ipyaggrid = { version = "^0.4.0", optional = true }
 jinja2 = { version = "^3.1.2", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-ipython = "^8.11.0"
+ipython = ">=8.11.0"
 dulwich = "^0.21.3"
-datamodel-code-generator = "^0.17.2"
+datamodel-code-generator = ">=0.17.2"
 black = "^23.1.0"
-pdoc = "^13.0.0"
-rich = "^13.3.2"
+pdoc = ">=13.0.0"
+rich = ">=13.3.2"
 pre-commit = "^3.2.2"
-cherwell_pydantic_api = {path = ".", extras = ["modelgen", "jupyter"]}
-autopep8 = "^2.0.2"
+autopep8 = ">=2.0.2"
+pytest = ">=7.3.0"
+mypy = ">=1.2.0"
+pytest-httpx = "^0.22.0"
+hypothesis = {extras = ["cli"], version = "^6.72.0"}
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry.extras]
 modelgen = ["black", "dulwich", "click", "jinja2"]
 jupyter = ["jupyter", "ipywidgets", "jupyterlab", "ipyaggrid", "nest-asyncio"]
 all = ["modelgen", "jupyter"]
 
 [tool.poetry.scripts]
@@ -62,14 +67,24 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.autopep8]
 ignore = ['E303']
-line-length = 120
+max-line-length = 120
 
 [tool.isort]
 profile = "hug"
 line_length = 120
 lines_after_imports = 3
 
+[tool.pyright]
+#reportUnknownArgumentType = false
+#reportUnknownParameterType = false
+#reportMissingParameterType = false
+pythonVersion = "3.9"
+
+[tool.mypy]
+plugins = "pydantic.mypy"
+#ignore_missing_imports = true
+exclude = ['repo/']
```

### Comparing `cherwell_pydantic_api-0.0.3/PKG-INFO` & `cherwell_pydantic_api-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cherwell-pydantic-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pythonic, asyncio connector for the Cherwell CSM API with full usage of Pydantic types
 Home-page: https://github.com/dataway/cherwell_pydantic_api
 License: MIT
 Keywords: cherwell,pydantic
 Author: Anthony Uk
 Author-email: uk@anthonyuk.dev
 Requires-Python: >=3.9,<4.0
@@ -16,32 +16,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Provides-Extra: all
 Provides-Extra: jupyter
 Provides-Extra: modelgen
 Requires-Dist: async-lru (>=2.0.2,<3.0.0)
 Requires-Dist: black (>=23.1.0,<24.0.0) ; extra == "modelgen"
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "modelgen"
 Requires-Dist: dulwich (>=0.21.3,<0.22.0) ; extra == "modelgen"
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: ipyaggrid (>=0.4.0,<0.5.0) ; extra == "jupyter"
 Requires-Dist: ipywidgets (>=8.0.5,<9.0.0) ; extra == "jupyter"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "modelgen"
 Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "jupyter" or extra == "all"
-Requires-Dist: jupyterlab (>=3.6.2,<4.0.0) ; extra == "jupyter"
+Requires-Dist: jupyterlab (>=4.0.0,<5.0.0) ; extra == "jupyter"
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0) ; extra == "jupyter"
+Requires-Dist: pydantic-changedetect (>=0.2.5,<0.3.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.6,<2.0.0)
 Project-URL: Repository, https://github.com/dataway/cherwell_pydantic_api
 Description-Content-Type: text/markdown
 
 # cherwell_pydantic_api
 ## a pythonic, asyncio connector for the Cherwell CSM API with full usage of Pydantic types
```


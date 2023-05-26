# Comparing `tmp/frequenz-api-microgrid-0.13.0.tar.gz` & `tmp/frequenz-api-microgrid-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-microgrid-0.13.0.tar", last modified: Tue May 23 12:21:43 2023, max compression
+gzip compressed data, was "frequenz-api-microgrid-0.14.0.tar", last modified: Fri May 26 15:15:09 2023, max compression
```

## Comparing `frequenz-api-microgrid-0.13.0.tar` & `frequenz-api-microgrid-0.14.0.tar`

### file list

```diff
@@ -1,106 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.688909 frequenz-api-microgrid-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/minimum-requirements-ci.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.652907 frequenz-api-microgrid-0.13.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.652907 frequenz-api-microgrid-0.13.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.656908 frequenz-api-microgrid-0.13.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.668908 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/battery.proto
--rw-r--r--   0 runner    (1001) docker     (122)    13408 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/common.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/grid.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/meter.proto
--rw-r--r--   0 runner    (1001) docker     (122)    17865 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/microgrid.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/sensor.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.656908 frequenz-api-microgrid-0.13.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.656908 frequenz-api-microgrid-0.13.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.656908 frequenz-api-microgrid-0.13.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.668908 frequenz-api-microgrid-0.13.0/py/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/py/frequenz/api/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/py/frequenz/api/microgrid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.668908 frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-23 12:21:43.000000 frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3917 2023-05-23 12:21:43.000000 frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:21:43.000000 frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-23 12:21:43.000000 frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 12:21:43.000000 frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 12:21:43.688909 frequenz-api-microgrid-0.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.656908 frequenz-api-microgrid-0.13.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.656908 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.660908 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.680909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.680909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.660908 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.656908 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.680909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.660908 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:21:43.684909 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-05-23 12:21:26.000000 frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3304 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/minimum-requirements-ci.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.926161 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     5331 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     4475 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/common.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/meter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    17754 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/microgrid.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/sensor.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.926161 frequenz-api-microgrid-0.14.0/py/frequenz/api/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/py/frequenz/api/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/py/frequenz/api/microgrid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.926161 frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-26 15:15:09.000000 frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4144 2023-05-26 15:15:09.000000 frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 15:15:09.000000 frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-26 15:15:09.000000 frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-26 15:15:09.000000 frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-05-26 15:14:47.000000 frequenz-api-microgrid-0.14.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.930161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.930161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.930161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.930161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-05-26 15:14:48.000000 frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.922160 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.926161 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-26 15:14:49.000000 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:15:09.934161 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-05-26 15:14:49.000000 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-05-26 15:14:49.000000 frequenz-api-microgrid-0.14.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
```

### Comparing `frequenz-api-microgrid-0.13.0/CONTRIBUTING.md` & `frequenz-api-microgrid-0.14.0/CONTRIBUTING.md`

 * *Files 24% similar despite different names*

```diff
@@ -35,14 +35,41 @@
 python setup.py compile_proto
 ```
 
 If you have any issues with these dependencies, please check the
 `pyproject.toml` file and try installing the exact supported versions instead.
 
 
+Upgrading dependencies
+======================
+
+If you want to update the dependency `frequenz-api-common`, then you need to
+* update the submodule `frequenz-api-common`
+* update the version of the `frequenz-api-common` package in `pyproject.toml`
+* update the version of the `frequenz-api-common` package in
+`minimum-requirements-ci.txt`
+
+The version of `frequenz-api-common` used in all the three places mentioned
+above should be the same.
+
+Here is an example of upgrading the `frequenz-api-common` dependency to version
+`v0.2.0`:
+```sh
+ver="0.2.0"
+
+cd submodules/frequenz-api-common
+git remote update
+git checkout v${ver}
+cd ../..
+
+sed s/"frequenz-api-common == [0-9]\.[0-9]\.[0-9]"/"frequenz-api-common == ${ver}"/g -i pyproject.toml
+
+sed s/"frequenz-api-common == .*"/"frequenz-api-common == ${ver}"/g -i minimum-requirements-ci.txt
+```
+
 Releasing
 =========
 
 These are the steps to create a new release:
 
 1. Get the latest head you want to create a release from.
```

### Comparing `frequenz-api-microgrid-0.13.0/LICENSE` & `frequenz-api-microgrid-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/PKG-INFO` & `frequenz-api-microgrid-0.14.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.13.0
+Version: 0.14.0
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
 Keywords: frequenz,api,microgrid,grpc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Frequenz Microgrid API
 ======================
 
 Microgrid is a gRPC API used to provide monitoring and control over the
```

### Comparing `frequenz-api-microgrid-0.13.0/README.md` & `frequenz-api-microgrid-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/battery.proto` & `frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/battery.proto`

 * *Files 9% similar despite different names*

```diff
@@ -8,37 +8,26 @@
 
 syntax = "proto3";
 
 package frequenz.api.microgrid.battery;
 
 import "frequenz/api/microgrid/common.proto";
 
-// Enumerated battery types.
-enum Type {
-  // Unspecified.
-  TYPE_UNSPECIFIED = 0;
-
-  // Li-ion batteries.
-  TYPE_LI_ION = 1;
-
-  // Lithium-Iron-Phosphate batteries.
-  TYPE_LI_FE_PO = 2;
-
-  // Sodium-ion batteries
-  TYPE_NA_ION = 3;
-}
+import "frequenz/api/common/components.proto";
+import "frequenz/api/common/metrics/electrical.proto";
 
 // The battery metadata.
 message Metadata {
   // The battery type.
-  Type type = 1;
+  frequenz.api.common.components.BatteryType type = 1;
 }
 
 enum ComponentState {
   // Default value.
+  // This value is used only when the state information is not available.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
   // The battery is switched off.
   COMPONENT_STATE_OFF = 1;
 
   // The battery is idle.
   COMPONENT_STATE_IDLE = 2;
@@ -51,14 +40,24 @@
 
   // The battery is in a faulty state.
   COMPONENT_STATE_ERROR = 5;
 
   // The battery is online, but currently unavailable, possibly due to
   // a pre-scheduled maintenance, or waiting for a resource to be loaded.
   COMPONENT_STATE_LOCKED = 6;
+
+  // The battery is starting up and needs some time to become fully operational.
+  COMPONENT_STATE_SWITCHING_ON = 7;
+
+  // The battery is switching off and needs some time to fully shut down.
+  COMPONENT_STATE_SWITCHING_OFF = 8;
+
+  // The state is provided by the device, but it can not be parsed as any of the
+  // above (known) states.
+  COMPONENT_STATE_UNKNOWN = 9;
 }
 
 enum RelayState {
   // Default value.
   RELAY_STATE_UNSPECIFIED = 0;
 
   // The relays are open, and the DC power line to the inverter is
@@ -171,15 +170,15 @@
   // The error message.
   string msg = 3;
 }
 
 // Battery data.
 message Data {
   // DC electricity metrics.
-  common.DC dc = 1;
+  frequenz.api.common.metrics.electrical.DC dc = 1;
 
   // Battery's overall SoC.
   // In percent (%).
   common.MetricAggregation soc = 2;
 
   // The aggregated values of all the temperature measurements of a battery.
   // In degree Celsius (°C).
```

### Comparing `frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/ev_charger.proto` & `frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/ev_charger.proto`

 * *Files 9% similar despite different names*

```diff
@@ -8,39 +8,28 @@
 
 syntax = "proto3";
 
 package frequenz.api.microgrid.ev_charger;
 
 import "frequenz/api/microgrid/common.proto";
 
-
-// The possible types of an EV charging station.
-enum Type {
-  // Default type.
-  TYPE_UNSPECIFIED = 0;
-
-  // The EV charging station supports AC charging only.
-  TYPE_AC = 1;
-
-  // The EV charging station supports DC charging only.
-  TYPE_DC = 2;
-
-  // The EV charging station supports both AC and DC.
-  TYPE_HYBRID = 3;
-}
+import "frequenz/api/common/components.proto";
+import "frequenz/api/common/metrics.proto";
+import "frequenz/api/common/metrics/electrical.proto";
 
 // The EV charger metadata.
 message Metadata {
   // The EV charger type.
-  Type type = 1;
+  frequenz.api.common.components.EVChargerType type = 1;
 }
 
 // The possible states of an EV charging station.
 enum ComponentState {
   // Default state.
+  // This value is used only when the state information is not available.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
   // The EV charging station is starting up.
   COMPONENT_STATE_STARTING = 1;
 
   // The EV charging station is unplugged or RFID is not working.
   COMPONENT_STATE_NOT_READY = 2;
@@ -59,14 +48,18 @@
   COMPONENT_STATE_ERROR = 6;
 
   // The EV charging station rejected the last authorization.
   COMPONENT_STATE_AUTHORIZATION_REJECTED = 7;
 
   // The EV charging process hes been temporarily interrupted.
   COMPONENT_STATE_INTERRUPTED = 8;
+
+  // The state is provided by the device, but it can not be parsed as any of the
+  // above (known) states.
+  COMPONENT_STATE_UNKNOWN = 9;
 }
 
 // The possible states of the cable connecting an EV charging station and an
 // EV.
 enum CableState {
   // Default state.
   CABLE_STATE_UNSPECIFIED = 0;
@@ -170,25 +163,25 @@
 
 // EV charger data.
 message Data {
   // DC metrics of the EV charging station.
   // Contains data only if DC charging is supported by the EV charging station.
   // (in which case, the type of the EV charging station is TYPE_DC or
   // TYPE_HYBRID)
-  common.DC dc = 1;
+  frequenz.api.common.metrics.electrical.DC dc = 1;
 
   // AC metrics of the EV charging station.
   // Contains data only if AC charging is supported by the EV charging station.
   // (in which case, the type of the EV charging station is TYPE_AC or
   // TYPE_HYBRID)
-  common.AC ac = 2;
+  frequenz.api.common.metrics.electrical.AC ac = 2;
 
   // The overall temperature of the EV charger.
   // In degree Celsius (°C).
-  common.Metric temperature = 3;
+  frequenz.api.common.metrics.Metric temperature = 3;
 }
 
 // EV charger properties.
 message Properties {
   // The firmware version of the component.
   string firmware_ver = 1;
 }
```

### Comparing `frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/grid.proto` & `frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/inverter.proto` & `frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/inverter.proto`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 
 syntax = "proto3";
 
 package frequenz.api.microgrid.inverter;
 
 import "frequenz/api/microgrid/common.proto";
 
+import "frequenz/api/common/components.proto";
+import "frequenz/api/common/metrics.proto";
+import "frequenz/api/common/metrics/electrical.proto";
+
 // Enumerated inverter types.
 enum Type {
   TYPE_UNSPECIFIED = 0;
   TYPE_BATTERY = 1;
   TYPE_SOLAR = 2;
   TYPE_HYBRID = 3;
 }
 
 // The inverter metadata.
 message Metadata {
   // The inverter type.
-  Type type = 1;
+  frequenz.api.common.components.InverterType type = 1;
 }
 
 // Enumerated inverter states.
 enum ComponentState {
   // Default value.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
@@ -58,14 +62,18 @@
 
   // The inverter is in a faulty state.
   COMPONENT_STATE_ERROR = 14;
 
   // The inverter is online, but currently unavailable, possibly due to
   // a pre-scheduled maintenance.
   COMPONENT_STATE_UNAVAILABLE = 15;
+
+  // The state is provided by the device, but it can not be parsed as any of the
+  // above (known) states.
+  COMPONENT_STATE_UNKNOWN = 16;
 }
 
 // Enumerated inverter error codes.
 enum ErrorCode {
   // Unspecified.
   ERROR_CODE_UNSPECIFIED = 0;
 }
@@ -88,26 +96,26 @@
   string msg = 3;
 }
 
 // Inverter data.
 message Data {
   // DC metrics for the inverter-battery linkage.
   // This is applicable to `BATTERY` and `HYBRID` inverters only.
-  common.DC dc_battery = 4;
+  frequenz.api.common.metrics.electrical.DC dc_battery = 4;
 
   // DC metrics for the inverter-PV linkage.
   // This is applicable to `SOLAR` and `HYBRID` inverters only.
-  common.DC dc_solar = 5;
+  frequenz.api.common.metrics.electrical.DC dc_solar = 5;
 
   // AC metrics of the inverter.
-  common.AC ac = 2;
+  frequenz.api.common.metrics.electrical.AC ac = 2;
 
   // The verall temperature of the inverter.
   // In degree Celsius (°C).
-  common.Metric temperature = 3;
+  frequenz.api.common.metrics.Metric temperature = 3;
 }
 
 // Inverter properties.
 message Properties {
   // The firmware version of the component.
   string firmware_ver = 1;
 }
```

### Comparing `frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/meter.proto` & `frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/meter.proto`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 syntax = "proto3";
 
 package frequenz.api.microgrid.meter;
 
 import "frequenz/api/microgrid/common.proto";
 
+import "frequenz/api/common/metrics/electrical.proto";
+
 // Enumerated meter types.
 enum Type {
   TYPE_UNSPECIFIED = 0;
 
   // AC production power meter / inverter production AC power (fallback)
   TYPE_PRODUCTION = 1;
 
@@ -70,15 +72,15 @@
   // The error message.
   string msg = 3;
 }
 
 // Meter data.
 message Data {
   // AC metrics of the inverter.
-  common.AC ac = 1;
+  frequenz.api.common.metrics.electrical.AC ac = 1;
 }
 
 // Meter properties.
 message Properties {
   // The firmware version of the component.
   string firmware_ver = 1;
 }
```

### Comparing `frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/microgrid.proto` & `frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/microgrid.proto`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 // MIT
 
 syntax = "proto3";
 
 package frequenz.api.microgrid;
 
 import "frequenz/api/microgrid/battery.proto";
-import "frequenz/api/microgrid/common.proto";
 import "frequenz/api/microgrid/ev_charger.proto";
 import "frequenz/api/microgrid/grid.proto";
 import "frequenz/api/microgrid/inverter.proto";
 import "frequenz/api/microgrid/meter.proto";
 import "frequenz/api/microgrid/sensor.proto";
 
+import "frequenz/api/common/components.proto";
+import "frequenz/api/common/metrics.proto";
+
 import "google/api/annotations.proto";
 import "google/protobuf/empty.proto";
 import "google/protobuf/timestamp.proto";
 import "google/protobuf/wrappers.proto";
 
 service Microgrid {
   /// Returns the microgrid metadata
@@ -173,15 +175,15 @@
   // <-------|============|------------------|============|--------->
   //                exclusion.lower    exclusion.upper
   // ```
   // ---- values here are disallowed and wil be rejected
   // ==== vales here are allowed and will be accepted
   rpc AddInclusionBounds(SetBoundsParam) returns (google.protobuf.Timestamp);
 
-  // Sets the power output of a component with a given ID, provided the
+  // Sets the active power output of a component with a given ID, provided the
   // component supports it.
   //
   // Note that the target component may have a resolution of more than 1 W.
   // E.g., an inverter may have a resolution of 88 W.
   // In such cases, the magnitude of power will be floored to the nearest
   // multiple of the resolution.
   //
@@ -192,14 +194,27 @@
   //  AC power.
   rpc SetPowerActive(SetPowerActiveParam) returns (google.protobuf.Empty) {
     option (google.api.http) = {
       get : "/v1/components/{component_id}/setPowerActive/{power}"
     };
   }
 
+  // Sets the reactive power output of a component with a given ID, provided the
+  // component supports it.
+  //
+  // Note that the target component may have a resolution of more than 1 VAr.
+  // E.g., an inverter may have a resolution of 88 VAr.
+  // In such cases, the magnitude of power will be floored to the nearest
+  // multiple of the resolution.
+  rpc SetPowerReactive(SetPowerReactiveParam) returns (google.protobuf.Empty) {
+    option (google.api.http) = {
+      get : "/v1/components/{component_id}/setPowerReactive/{power}"
+    };
+  }
+
   // Starts the component, and brings it into a state where it is immediately
   // operational.
   //
   // Performs the following sequence of actions for the following component
   // categories:
   //
   // * Inverter:
@@ -313,58 +328,21 @@
   // This is a natural number that uniquely identifies a given microgrid.
   uint64 microgrid_id = 1;
 
   // The location of the microgrid, in geographical co-ordinates.
   Location location = 2;
 }
 
-// Enumrated component categories.
-enum ComponentCategory {
-  // An unknown component categories, useful for error handling, and marking
-  // unknown components in a list of components with otherwise known categories.
-  COMPONENT_CATEGORY_UNSPECIFIED = 0;
-
-  // The point where the local microgrid is connected to the grid.
-  COMPONENT_CATEGORY_GRID = 1;
-
-  // A meter, for measuring electrical metrics, e.g., current, voltage, etc.
-  COMPONENT_CATEGORY_METER = 2;
-
-  // An electricity generator, with batteries or solar energy.
-  COMPONENT_CATEGORY_INVERTER = 3;
-
-  // A DC-DC converter.
-  COMPONENT_CATEGORY_CONVERTER = 4;
-
-  // A storage system for electrical energy, used by inverters.
-  COMPONENT_CATEGORY_BATTERY = 5;
-
-  // A station for charging electrical vehicles.
-  COMPONENT_CATEGORY_EV_CHARGER = 6;
-
-  // A sensor for measuring ambient metrics, e.g., temperature, humidity, etc.
-  COMPONENT_CATEGORY_SENSOR = 7;
-
-  // A crypto miner.
-  COMPONENT_CATEGORY_CRYPTO_MINER = 8;
-
-  // An electrolyzer for converting water into hydrogen and oxygen.
-  COMPONENT_CATEGORY_ELECTROLYZER = 9;
-
-  // A heat and power combustion plant (CHP stands for combined heat and power).
-  COMPONENT_CATEGORY_CHP = 10;
-}
-
 // Parameters for filtering the components.
 message ComponentFilter {
   // Return components that have the specified IDs only.
   repeated uint64 ids = 1;
 
   // Return components that have the specified categories only.
-  repeated ComponentCategory categories = 2;
+  repeated frequenz.api.common.components.ComponentCategory categories = 2;
 }
 
 // Encapsulation of a component ID, intended to be used as a parameter for rpc
 // methods.
 message ComponentIdParam {
   uint64 id = 1;
 }
@@ -399,14 +377,26 @@
   uint64 component_id = 1;
 
   // The output active power level, in watts.
   // -ve values are for discharging, and +ve values are for charging.
   float power = 2;
 }
 
+// Parameters for setting the reactive power of an appropriate component using
+// the `SetPowerReactive` RPC.
+message SetPowerReactiveParam {
+  // The ID of the component to set the output reactive power of.
+  uint64 component_id = 1;
+
+  // The output reactive power level, in VAr.
+  // -ve values are for inductive (lagging) power , and +ve values are for
+  //  capacitive (leading) power.
+  float power = 2;
+}
+
 // Parameters for setting bounds of a given metric of a given component.
 message SetBoundsParam {
   // An enumerated list of metrics whose bounds can be set.
   enum TargetMetric {
     TARGET_METRIC_UNSPECIFIED = 0;
     TARGET_METRIC_POWER_ACTIVE = 1;
     TARGET_METRIC_CURRENT = 2;
@@ -419,28 +409,28 @@
   // The ID of the target component.
   uint64 component_id = 1;
 
   // The target metric whose bounds have to be set.
   TargetMetric target_metric = 2;
 
   // The bounds for the target metric.
-  common.Bounds bounds = 3;
+  frequenz.api.common.metrics.Bounds bounds = 3;
 }
 
 // A generic message for components. It is used to represent any category of
 // component, with its static parameters.
 message Component {
   // A unique identifier for the component.
   uint64 id = 1;
 
   // An optional name for the component.
   string name = 2;
 
   // The category of the component.
-  ComponentCategory category = 3;
+  frequenz.api.common.components.ComponentCategory category = 3;
 
   // The component manufacturer.
   string manufacturer = 4;
 
   // The model name of the component.
   string model_name = 5;
```

### Comparing `frequenz-api-microgrid-0.13.0/proto/frequenz/api/microgrid/sensor.proto` & `frequenz-api-microgrid-0.14.0/proto/frequenz/api/microgrid/sensor.proto`

 * *Files 8% similar despite different names*

```diff
@@ -8,45 +8,20 @@
 
 syntax = "proto3";
 
 package frequenz.api.microgrid.sensor;
 
 import "frequenz/api/microgrid/common.proto";
 
-// Enumerated sensor types.
-enum Type {
-  // Unspecified
-  TYPE_UNSPECIFIED = 0;
-
-  // Thermometer (temperature sensor)
-  TYPE_THERMOMETER = 1;
-
-  // Hygrometer (humidity sensor)
-  TYPE_HYGROMETER = 2;
-
-  // Barometer (pressure sensor).
-  TYPE_BAROMETER = 3;
-
-  // Pyranometer (solar irradiance sensor).
-  TYPE_PYRANOMETER = 4;
-
-  // Anemometer (wind velocity and direction sensor).
-  TYPE_ANEMOMETER = 5;
-
-  // Accelerometers (acceleration sensor).
-  TYPE_ACCELEROMETER = 6;
-
-  // General sensors, which do not fall in any of the above categories
-  TYPE_GENERAL = 7;
-}
+import "frequenz/api/common/components.proto";
 
 // The sensor metadata.
 message Metadata {
   // The sensor type.
-  Type type = 1;
+  frequenz.api.common.components.SensorType type = 1;
 }
 
 // Enumerated sensor states.
 enum ComponentState {
   // Unspecified state.
   COMPONENT_STATE_UNSPECIFIED = 0;
```

### Comparing `frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/PKG-INFO` & `frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.13.0
+Version: 0.14.0
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
 Keywords: frequenz,api,microgrid,grpc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Frequenz Microgrid API
 ======================
 
 Microgrid is a gRPC API used to provide monitoring and control over the
```

### Comparing `frequenz-api-microgrid-0.13.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt` & `frequenz-api-microgrid-0.14.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -71,8 +71,11 @@
 submodules/api-common-protos/google/type/expr.proto
 submodules/api-common-protos/google/type/fraction.proto
 submodules/api-common-protos/google/type/latlng.proto
 submodules/api-common-protos/google/type/money.proto
 submodules/api-common-protos/google/type/month.proto
 submodules/api-common-protos/google/type/postal_address.proto
 submodules/api-common-protos/google/type/quaternion.proto
-submodules/api-common-protos/google/type/timeofday.proto
+submodules/api-common-protos/google/type/timeofday.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
```

### Comparing `frequenz-api-microgrid-0.13.0/pyproject.toml` & `frequenz-api-microgrid-0.14.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,19 @@
 keywords = [ "frequenz", "api", "microgrid", "grpc" ]
 classifiers = [
    "Development Status :: 3 - Alpha",
    "Intended Audience :: Developers",
    "License :: OSI Approved :: MIT License",
    "Programming Language :: Python :: 3",
    "Programming Language :: Python :: 3 :: Only",
-   "Programming Language :: Python :: 3.7",
-   "Programming Language :: Python :: 3.8",
-   "Programming Language :: Python :: 3.9",
-   "Programming Language :: Python :: 3.10",
    "Topic :: Software Development :: Libraries",
 ]
-requires-python = ">= 3.7, < 4"
+requires-python = ">= 3.11, < 4"
 dependencies = [
+    "frequenz-api-common == 0.2.0",
     "googleapis-common-protos >= 1.56.2, < 2",
     "grpcio >= 1.47.0, < 2",
 ]
 dynamic = [ "version" ]
 
 [[project.authors]]
 name ="Frequenz Energy-as-a-Service GmbH"
```

### Comparing `frequenz-api-microgrid-0.13.0/setup.py` & `frequenz-api-microgrid-0.14.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         """Compile the Python protobuf files."""
         proto_files = [str(p) for p in pathlib.Path("proto").rglob("*.proto")]
         protoc_cmd = (
             [sys.executable]
             + """-m grpc_tools.protoc
                     -I proto
                     -I submodules/api-common-protos
+                    -I submodules/frequenz-api-common/proto
                     --python_out=py
                     --grpc_python_out=py
                     --mypy_out=py
                     --mypy_grpc_out=py
                     """.split()
             + proto_files
         )
```

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.13.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-microgrid-0.14.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*


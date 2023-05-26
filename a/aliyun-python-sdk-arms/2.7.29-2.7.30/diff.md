# Comparing `tmp/aliyun-python-sdk-arms-2.7.29.tar.gz` & `tmp/aliyun-python-sdk-arms-2.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-arms-2.7.29.tar", last modified: Tue Mar 14 02:05:26 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-arms-2.7.30.tar", last modified: Fri May 26 09:55:27 2023, max compression
```

## Comparing `aliyun-python-sdk-arms-2.7.29.tar` & `aliyun-python-sdk-arms-2.7.30.tar`

### file list

```diff
@@ -1,184 +1,191 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1543 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1543 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10740 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2625 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/
--rw-r--r--   0 root         (0) root         (0)     1942 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddAliClusterIdsToPrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddGrafanaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewByAliClusterIdsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusRemoteWriteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1641 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddRecordingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1928 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AppendInstancesToPrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     2999 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ApplyScenarioRequest.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/BindPrometheusGrafanaInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CheckServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ConfigAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateAlertContactGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateAlertContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateDispatchRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateAlertRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1923 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateContactGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateEventBridgeIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3151 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateIMRobotRequest.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateNotificationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateSilencePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateWebhookContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreatePrometheusAlertRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3544 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreatePrometheusInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateRetcodeAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateSyntheticTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateWebhookRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DelAuthTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertContactGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1462 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteCmsExporterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteContactGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1424 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteDispatchRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteEventBridgeIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteGrafanaResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteIMRobotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteIntegrationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteNotificationPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusAlertRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusRemoteWriteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteRetcodeAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteScenarioRequest.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteSilencePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteSourceMapRequest.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteSyntheticTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1738 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteTraceAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteWebhookContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeContactGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeContactsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeDispatchRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeIMRobotsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribePrometheusAlertRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1291 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeTraceLicenseKeyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeWebhookContactsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAgentDownloadUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAlertRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAppApiByPageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAuthTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetCloudClusterAllUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1462 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetClusterAllUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetExploreUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetIntegrationStateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetManagedPrometheusStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetMultipleTraceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetOnCallSchedulesDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1287 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusApiTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusRemoteWriteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1462 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRecordingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeAppByPidRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeDataByQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeLogstoreRequest.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeShareUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSourceMapInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetStackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSyntheticTaskDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSyntheticTaskListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1293 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSyntheticTaskMonitorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetTraceAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetTraceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ImportAppAlertRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/InstallCmsExporterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/InstallManagedPrometheusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListActivatedAlertsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListAlertEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListAlertsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListClusterFromGrafanaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListCmsInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2887 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListDashboardsByNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListDashboardsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListDispatchRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListEscalationPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListEventBridgeIntegrationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListInsightsEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListNotificationPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1739 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListOnCallSchedulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusAlertRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusAlertTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1293 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusInstanceByTagAndResourceGroupIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusRemoteWritesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListRetcodeAppsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListScenarioRequest.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListSilencePoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListTraceAppsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ManageGetRecordingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ManageRecordingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenArmsDefaultSLRRequest.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenArmsServiceSecondVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenVClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenXtraceDefaultSLRRequest.py
--rw-r--r--   0 root         (0) root         (0)     4001 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/QueryMetricByPageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/QueryPromInstallStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/QueryReleaseMetricRequest.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/RemoveAliClusterIdsFromPrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/RemoveSourcesFromPrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     1904 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SaveTraceAppConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertContactGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertHistoriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchRetcodeAppByPageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTraceAppByNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTraceAppByPageRequest.py
--rw-r--r--   0 root         (0) root         (0)     4280 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTracesByPageRequest.py
--rw-r--r--   0 root         (0) root         (0)     3708 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTracesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SendTTSVerifyLinkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SetRetcodeShareStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/StartAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/StopAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SwitchSyntheticTaskStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SyncRecordingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UninstallManagedPrometheusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UninstallPromClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateAlertContactGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateAlertContactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateAlertRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateDispatchRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     4681 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3298 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusAlertRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusGlobalViewRequest.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusIntegrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusRemoteWriteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateWebhookRequest.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UploadRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-03-14 02:05:26.000000 aliyun-python-sdk-arms-2.7.29/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11210 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddAliClusterIdsToPrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddGrafanaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewByAliClusterIdsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusRemoteWriteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddRecordingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AppendInstancesToPrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ApplyScenarioRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/BindPrometheusGrafanaInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CheckServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ConfigAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateAlertContactGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateAlertContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateDispatchRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5480 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateAlertRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateContactGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateEventBridgeIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateIMRobotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateNotificationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateSilencePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateWebhookContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3559 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreatePrometheusAlertRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreatePrometheusInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreatePrometheusMonitoringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateRetcodeAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateSyntheticTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DelAuthTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertContactGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteCmsExporterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteContactGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteDispatchRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteEventBridgeIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteGrafanaResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteIMRobotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteIntegrationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteNotificationPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusAlertRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusMonitoringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusRemoteWriteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteRetcodeAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteScenarioRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteSilencePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteSourceMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteSyntheticTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteTraceAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteWebhookContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeContactGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeContactsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeDispatchRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeIMRobotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribePrometheusAlertRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeTraceLicenseKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeWebhookContactsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/EnableMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAgentDownloadUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAlertRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAppApiByPageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAuthTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetCloudClusterAllUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetClusterAllUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetExploreUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetIntegrationStateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetManagedPrometheusStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetMultipleTraceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetOnCallSchedulesDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusApiTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusMonitoringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusRemoteWriteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRecordingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeAppByPidRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeDataByQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeLogstoreRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeShareUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSourceMapInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetStackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSyntheticTaskDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSyntheticTaskListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSyntheticTaskMonitorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetTraceAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetTraceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ImportAppAlertRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/InstallCmsExporterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/InstallManagedPrometheusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListActivatedAlertsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListAlertEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListAlertsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListClusterFromGrafanaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListCmsInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListDashboardsByNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListDashboardsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListDispatchRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListEscalationPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListEventBridgeIntegrationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListInsightsEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListNotificationPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListOnCallSchedulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusAlertRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusAlertTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusInstanceByTagAndResourceGroupIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusMonitoringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusRemoteWritesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListRetcodeAppsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListScenarioRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListSilencePoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListTraceAppsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ManageGetRecordingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ManageRecordingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenArmsDefaultSLRRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenArmsServiceSecondVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenVClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenXtraceDefaultSLRRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/QueryMetricByPageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/QueryPromInstallStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/QueryReleaseMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/RemoveAliClusterIdsFromPrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/RemoveSourcesFromPrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SaveTraceAppConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertContactGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertHistoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchRetcodeAppByPageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTraceAppByNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTraceAppByPageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4280 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTracesByPageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTracesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SendTTSVerifyLinkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SetRetcodeShareStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/StartAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/StopAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SwitchSyntheticTaskStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SyncRecordingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UninstallManagedPrometheusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UninstallPromClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateAlertContactGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateAlertContactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateAlertRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateDispatchRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3728 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusAlertRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusGlobalViewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusIntegrationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusMonitoringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusMonitoringStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusRemoteWriteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UploadRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-05-26 09:55:27.000000 aliyun-python-sdk-arms-2.7.30/setup.py
```

### Comparing `aliyun-python-sdk-arms-2.7.29/LICENSE` & `aliyun-python-sdk-arms-2.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/PKG-INFO` & `aliyun-python-sdk-arms-2.7.30/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-arms
-Version: 2.7.29
+Version: 2.7.30
 Summary: The arms module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-arms
```

### Comparing `aliyun-python-sdk-arms-2.7.29/README.rst` & `aliyun-python-sdk-arms-2.7.30/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/PKG-INFO` & `aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-arms
-Version: 2.7.29
+Version: 2.7.30
 Summary: The arms module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-arms
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyun_python_sdk_arms.egg-info/SOURCES.txt` & `aliyun-python-sdk-arms-2.7.30/aliyun_python_sdk_arms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 aliyunsdkarms/request/v20190808/CreateOrUpdateEventBridgeIntegrationRequest.py
 aliyunsdkarms/request/v20190808/CreateOrUpdateIMRobotRequest.py
 aliyunsdkarms/request/v20190808/CreateOrUpdateNotificationPolicyRequest.py
 aliyunsdkarms/request/v20190808/CreateOrUpdateSilencePolicyRequest.py
 aliyunsdkarms/request/v20190808/CreateOrUpdateWebhookContactRequest.py
 aliyunsdkarms/request/v20190808/CreatePrometheusAlertRuleRequest.py
 aliyunsdkarms/request/v20190808/CreatePrometheusInstanceRequest.py
+aliyunsdkarms/request/v20190808/CreatePrometheusMonitoringRequest.py
 aliyunsdkarms/request/v20190808/CreateRetcodeAppRequest.py
 aliyunsdkarms/request/v20190808/CreateSyntheticTaskRequest.py
 aliyunsdkarms/request/v20190808/CreateWebhookRequest.py
 aliyunsdkarms/request/v20190808/DelAuthTokenRequest.py
 aliyunsdkarms/request/v20190808/DeleteAlertContactGroupRequest.py
 aliyunsdkarms/request/v20190808/DeleteAlertContactRequest.py
 aliyunsdkarms/request/v20190808/DeleteAlertRuleRequest.py
@@ -57,14 +58,15 @@
 aliyunsdkarms/request/v20190808/DeleteIMRobotRequest.py
 aliyunsdkarms/request/v20190808/DeleteIntegrationRequest.py
 aliyunsdkarms/request/v20190808/DeleteIntegrationsRequest.py
 aliyunsdkarms/request/v20190808/DeleteNotificationPolicyRequest.py
 aliyunsdkarms/request/v20190808/DeletePrometheusAlertRuleRequest.py
 aliyunsdkarms/request/v20190808/DeletePrometheusGlobalViewRequest.py
 aliyunsdkarms/request/v20190808/DeletePrometheusIntegrationRequest.py
+aliyunsdkarms/request/v20190808/DeletePrometheusMonitoringRequest.py
 aliyunsdkarms/request/v20190808/DeletePrometheusRemoteWriteRequest.py
 aliyunsdkarms/request/v20190808/DeleteRetcodeAppRequest.py
 aliyunsdkarms/request/v20190808/DeleteScenarioRequest.py
 aliyunsdkarms/request/v20190808/DeleteSilencePolicyRequest.py
 aliyunsdkarms/request/v20190808/DeleteSourceMapRequest.py
 aliyunsdkarms/request/v20190808/DeleteSyntheticTaskRequest.py
 aliyunsdkarms/request/v20190808/DeleteTraceAppRequest.py
@@ -72,14 +74,15 @@
 aliyunsdkarms/request/v20190808/DescribeContactGroupsRequest.py
 aliyunsdkarms/request/v20190808/DescribeContactsRequest.py
 aliyunsdkarms/request/v20190808/DescribeDispatchRuleRequest.py
 aliyunsdkarms/request/v20190808/DescribeIMRobotsRequest.py
 aliyunsdkarms/request/v20190808/DescribePrometheusAlertRuleRequest.py
 aliyunsdkarms/request/v20190808/DescribeTraceLicenseKeyRequest.py
 aliyunsdkarms/request/v20190808/DescribeWebhookContactsRequest.py
+aliyunsdkarms/request/v20190808/EnableMetricRequest.py
 aliyunsdkarms/request/v20190808/GetAgentDownloadUrlRequest.py
 aliyunsdkarms/request/v20190808/GetAlertRulesRequest.py
 aliyunsdkarms/request/v20190808/GetAppApiByPageRequest.py
 aliyunsdkarms/request/v20190808/GetAuthTokenRequest.py
 aliyunsdkarms/request/v20190808/GetCloudClusterAllUrlRequest.py
 aliyunsdkarms/request/v20190808/GetClusterAllUrlRequest.py
 aliyunsdkarms/request/v20190808/GetExploreUrlRequest.py
@@ -87,14 +90,15 @@
 aliyunsdkarms/request/v20190808/GetManagedPrometheusStatusRequest.py
 aliyunsdkarms/request/v20190808/GetMultipleTraceRequest.py
 aliyunsdkarms/request/v20190808/GetOnCallSchedulesDetailRequest.py
 aliyunsdkarms/request/v20190808/GetPrometheusApiTokenRequest.py
 aliyunsdkarms/request/v20190808/GetPrometheusGlobalViewRequest.py
 aliyunsdkarms/request/v20190808/GetPrometheusInstanceRequest.py
 aliyunsdkarms/request/v20190808/GetPrometheusIntegrationRequest.py
+aliyunsdkarms/request/v20190808/GetPrometheusMonitoringRequest.py
 aliyunsdkarms/request/v20190808/GetPrometheusRemoteWriteRequest.py
 aliyunsdkarms/request/v20190808/GetRecordingRuleRequest.py
 aliyunsdkarms/request/v20190808/GetRetcodeAppByPidRequest.py
 aliyunsdkarms/request/v20190808/GetRetcodeDataByQueryRequest.py
 aliyunsdkarms/request/v20190808/GetRetcodeLogstoreRequest.py
 aliyunsdkarms/request/v20190808/GetRetcodeShareUrlRequest.py
 aliyunsdkarms/request/v20190808/GetSourceMapInfoRequest.py
@@ -123,14 +127,15 @@
 aliyunsdkarms/request/v20190808/ListOnCallSchedulesRequest.py
 aliyunsdkarms/request/v20190808/ListPrometheusAlertRulesRequest.py
 aliyunsdkarms/request/v20190808/ListPrometheusAlertTemplatesRequest.py
 aliyunsdkarms/request/v20190808/ListPrometheusGlobalViewRequest.py
 aliyunsdkarms/request/v20190808/ListPrometheusInstanceByTagAndResourceGroupIdRequest.py
 aliyunsdkarms/request/v20190808/ListPrometheusInstancesRequest.py
 aliyunsdkarms/request/v20190808/ListPrometheusIntegrationRequest.py
+aliyunsdkarms/request/v20190808/ListPrometheusMonitoringRequest.py
 aliyunsdkarms/request/v20190808/ListPrometheusRemoteWritesRequest.py
 aliyunsdkarms/request/v20190808/ListRetcodeAppsRequest.py
 aliyunsdkarms/request/v20190808/ListScenarioRequest.py
 aliyunsdkarms/request/v20190808/ListSilencePoliciesRequest.py
 aliyunsdkarms/request/v20190808/ListTraceAppsRequest.py
 aliyunsdkarms/request/v20190808/ManageGetRecordingRuleRequest.py
 aliyunsdkarms/request/v20190808/ManageRecordingRuleRequest.py
@@ -168,11 +173,13 @@
 aliyunsdkarms/request/v20190808/UpdateAlertContactRequest.py
 aliyunsdkarms/request/v20190808/UpdateAlertRuleRequest.py
 aliyunsdkarms/request/v20190808/UpdateDispatchRuleRequest.py
 aliyunsdkarms/request/v20190808/UpdateIntegrationRequest.py
 aliyunsdkarms/request/v20190808/UpdatePrometheusAlertRuleRequest.py
 aliyunsdkarms/request/v20190808/UpdatePrometheusGlobalViewRequest.py
 aliyunsdkarms/request/v20190808/UpdatePrometheusIntegrationRequest.py
+aliyunsdkarms/request/v20190808/UpdatePrometheusMonitoringRequest.py
+aliyunsdkarms/request/v20190808/UpdatePrometheusMonitoringStatusRequest.py
 aliyunsdkarms/request/v20190808/UpdatePrometheusRemoteWriteRequest.py
 aliyunsdkarms/request/v20190808/UpdateWebhookRequest.py
 aliyunsdkarms/request/v20190808/UploadRequest.py
 aliyunsdkarms/request/v20190808/__init__.py
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/endpoint.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddAliClusterIdsToPrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddAliClusterIdsToPrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddGrafanaRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddGrafanaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewByAliClusterIdsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewByAliClusterIdsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusInstanceRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddPrometheusRemoteWriteRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddPrometheusRemoteWriteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AddRecordingRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AddRecordingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/AppendInstancesToPrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/AppendInstancesToPrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ApplyScenarioRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ApplyScenarioRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/BindPrometheusGrafanaInstanceRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/BindPrometheusGrafanaInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ChangeResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CheckServiceStatusRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CheckServiceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ConfigAppRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ConfigAppRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateAlertContactGroupRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateAlertContactGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateAlertContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateAlertContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateDispatchRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateDispatchRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateAlertRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateAlertRuleRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,23 @@
 	def set_NotifyStrategy(self, NotifyStrategy):  # String
 		self.add_body_params('NotifyStrategy', NotifyStrategy)
 	def get_Labels(self): # String
 		return self.get_body_params().get('Labels')
 
 	def set_Labels(self, Labels):  # String
 		self.add_body_params('Labels', Labels)
+	def get_Tagss(self): # RepeatList
+		return self.get_body_params().get('Tags')
+
+	def set_Tagss(self, Tags):  # RepeatList
+		for depth1 in range(len(Tags)):
+			if Tags[depth1].get('Value') is not None:
+				self.add_body_params('Tags.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
+			if Tags[depth1].get('Key') is not None:
+				self.add_body_params('Tags.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
 	def get_AlertType(self): # String
 		return self.get_body_params().get('AlertType')
 
 	def set_AlertType(self, AlertType):  # String
 		self.add_body_params('AlertType', AlertType)
 	def get_AlertCheckType(self): # String
 		return self.get_body_params().get('AlertCheckType')
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateContactGroupRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateContactGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateEventBridgeIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateEventBridgeIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateIMRobotRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateIMRobotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateNotificationPolicyRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateNotificationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateSilencePolicyRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateSilencePolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateOrUpdateWebhookContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateOrUpdateWebhookContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreatePrometheusAlertRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusAlertRuleRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class CreatePrometheusAlertRuleRequest(RpcRequest):
+class UpdatePrometheusAlertRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'CreatePrometheusAlertRule','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'UpdatePrometheusAlertRule','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -67,17 +67,31 @@
 	def set_Message(self, Message):  # String
 		self.add_query_param('Message', Message)
 	def get_Labels(self): # String
 		return self.get_query_params().get('Labels')
 
 	def set_Labels(self, Labels):  # String
 		self.add_query_param('Labels', Labels)
+	def get_Tagss(self): # RepeatList
+		return self.get_query_params().get('Tags')
+
+	def set_Tagss(self, Tags):  # RepeatList
+		for depth1 in range(len(Tags)):
+			if Tags[depth1].get('Value') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
+			if Tags[depth1].get('Key') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
 	def get_Duration(self): # String
 		return self.get_query_params().get('Duration')
 
 	def set_Duration(self, Duration):  # String
 		self.add_query_param('Duration', Duration)
+	def get_AlertId(self): # Long
+		return self.get_query_params().get('AlertId')
+
+	def set_AlertId(self, AlertId):  # Long
+		self.add_query_param('AlertId', AlertId)
 	def get_NotifyType(self): # String
 		return self.get_query_params().get('NotifyType')
 
 	def set_NotifyType(self, NotifyType):  # String
 		self.add_query_param('NotifyType', NotifyType)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreatePrometheusInstanceRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreatePrometheusInstanceRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_GrafanaInstanceId(self): # String
 		return self.get_query_params().get('GrafanaInstanceId')
 
 	def set_GrafanaInstanceId(self, GrafanaInstanceId):  # String
 		self.add_query_param('GrafanaInstanceId', GrafanaInstanceId)
+	def get_AllSubClustersSuccess(self): # Boolean
+		return self.get_query_params().get('AllSubClustersSuccess')
+
+	def set_AllSubClustersSuccess(self, AllSubClustersSuccess):  # Boolean
+		self.add_query_param('AllSubClustersSuccess', AllSubClustersSuccess)
 	def get_ClusterName(self): # String
 		return self.get_query_params().get('ClusterName')
 
 	def set_ClusterName(self, ClusterName):  # String
 		self.add_query_param('ClusterName', ClusterName)
 	def get_SecurityGroupId(self): # String
 		return self.get_query_params().get('SecurityGroupId')
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateRetcodeAppRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateRetcodeAppRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateSyntheticTaskRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateSyntheticTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/CreateWebhookRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreateWebhookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DelAuthTokenRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DelAuthTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertContactGroupRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertContactGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteAlertRulesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteAlertRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteCmsExporterRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteCmsExporterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteContactGroupRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteContactGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteDispatchRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteDispatchRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteEventBridgeIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteEventBridgeIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteGrafanaResourceRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteGrafanaResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteIMRobotRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteIMRobotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteIntegrationsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteIntegrationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteNotificationPolicyRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteNotificationPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusAlertRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusAlertRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeletePrometheusRemoteWriteRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeletePrometheusRemoteWriteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteRetcodeAppRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteRetcodeAppRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteScenarioRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteScenarioRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteSilencePolicyRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteSilencePolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteSourceMapRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteSourceMapRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteSyntheticTaskRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteSyntheticTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteTraceAppRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteTraceAppRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DeleteWebhookContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DeleteWebhookContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeContactGroupsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeContactGroupsRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,32 +27,32 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_IsDetail(self): # Boolean
+		return self.get_query_params().get('IsDetail')
+
+	def set_IsDetail(self, IsDetail):  # Boolean
+		self.add_query_param('IsDetail', IsDetail)
+	def get_ContactGroupName(self): # String
+		return self.get_query_params().get('ContactGroupName')
+
+	def set_ContactGroupName(self, ContactGroupName):  # String
+		self.add_query_param('ContactGroupName', ContactGroupName)
 	def get_Size(self): # Long
 		return self.get_query_params().get('Size')
 
 	def set_Size(self, Size):  # Long
 		self.add_query_param('Size', Size)
 	def get_GroupIds(self): # String
 		return self.get_query_params().get('GroupIds')
 
 	def set_GroupIds(self, GroupIds):  # String
 		self.add_query_param('GroupIds', GroupIds)
-	def get_IsDetail(self): # Boolean
-		return self.get_query_params().get('IsDetail')
-
-	def set_IsDetail(self, IsDetail):  # Boolean
-		self.add_query_param('IsDetail', IsDetail)
 	def get_Page(self): # Long
 		return self.get_query_params().get('Page')
 
 	def set_Page(self, Page):  # Long
 		self.add_query_param('Page', Page)
-	def get_ContactGroupName(self): # String
-		return self.get_query_params().get('ContactGroupName')
-
-	def set_ContactGroupName(self, ContactGroupName):  # String
-		self.add_query_param('ContactGroupName', ContactGroupName)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeContactsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeContactsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeDispatchRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeDispatchRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeIMRobotsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeIMRobotsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribePrometheusAlertRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribePrometheusAlertRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeTraceLicenseKeyRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeTraceLicenseKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/DescribeWebhookContactsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/DescribeWebhookContactsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAgentDownloadUrlRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAgentDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAlertRulesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAlertRulesRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,23 @@
 	def set_AlertStatus(self, AlertStatus):  # String
 		self.add_query_param('AlertStatus', AlertStatus)
 	def get_ClusterId(self): # String
 		return self.get_query_params().get('ClusterId')
 
 	def set_ClusterId(self, ClusterId):  # String
 		self.add_query_param('ClusterId', ClusterId)
+	def get_Tagss(self): # RepeatList
+		return self.get_query_params().get('Tags')
+
+	def set_Tagss(self, Tags):  # RepeatList
+		for depth1 in range(len(Tags)):
+			if Tags[depth1].get('Value') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
+			if Tags[depth1].get('Key') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
 	def get_AlertNames(self): # String
 		return self.get_query_params().get('AlertNames')
 
 	def set_AlertNames(self, AlertNames):  # String
 		self.add_query_param('AlertNames', AlertNames)
 	def get_AlertType(self): # String
 		return self.get_query_params().get('AlertType')
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAppApiByPageRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAppApiByPageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetAuthTokenRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetAuthTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetCloudClusterAllUrlRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetCloudClusterAllUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetClusterAllUrlRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetClusterAllUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetExploreUrlRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetExploreUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetIntegrationStateRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetIntegrationStateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetManagedPrometheusStatusRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetManagedPrometheusStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetMultipleTraceRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetMultipleTraceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetOnCallSchedulesDetailRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetOnCallSchedulesDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusApiTokenRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusApiTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusInstanceRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetPrometheusRemoteWriteRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetPrometheusRemoteWriteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRecordingRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRecordingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeAppByPidRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeAppByPidRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeDataByQueryRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeDataByQueryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeLogstoreRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeLogstoreRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetRetcodeShareUrlRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetRetcodeShareUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSourceMapInfoRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSourceMapInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetStackRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetStackRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSyntheticTaskDetailRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSyntheticTaskDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSyntheticTaskListRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSyntheticTaskListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetSyntheticTaskMonitorsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetSyntheticTaskMonitorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetTraceAppRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetTraceAppRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/GetTraceRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/GetTraceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ImportAppAlertRulesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ImportAppAlertRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/InstallCmsExporterRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/InstallCmsExporterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/InstallManagedPrometheusRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/InstallManagedPrometheusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListActivatedAlertsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListActivatedAlertsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListAlertEventsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListAlertEventsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListAlertsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListAlertsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListClusterFromGrafanaRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListClusterFromGrafanaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListCmsInstancesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListCmsInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListDashboardsByNameRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListDashboardsByNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListDashboardsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListDashboardsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListDispatchRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListDispatchRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListEscalationPoliciesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListEscalationPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListEventBridgeIntegrationsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListEventBridgeIntegrationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListInsightsEventsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListInsightsEventsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListNotificationPoliciesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListNotificationPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListOnCallSchedulesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListOnCallSchedulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusAlertRulesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreatePrometheusMonitoringRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,43 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class ListPrometheusAlertRulesRequest(RpcRequest):
+class CreatePrometheusMonitoringRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'ListPrometheusAlertRules','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'CreatePrometheusMonitoring','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ConfigYaml(self): # String
+		return self.get_body_params().get('ConfigYaml')
+
+	def set_ConfigYaml(self, ConfigYaml):  # String
+		self.add_body_params('ConfigYaml', ConfigYaml)
 	def get_ClusterId(self): # String
 		return self.get_query_params().get('ClusterId')
 
 	def set_ClusterId(self, ClusterId):  # String
 		self.add_query_param('ClusterId', ClusterId)
 	def get_Type(self): # String
 		return self.get_query_params().get('Type')
 
 	def set_Type(self, Type):  # String
 		self.add_query_param('Type', Type)
-	def get_Name(self): # String
-		return self.get_query_params().get('Name')
-
-	def set_Name(self, Name):  # String
-		self.add_query_param('Name', Name)
-	def get_MatchExpressions(self): # String
-		return self.get_query_params().get('MatchExpressions')
-
-	def set_MatchExpressions(self, MatchExpressions):  # String
-		self.add_query_param('MatchExpressions', MatchExpressions)
-	def get_Status(self): # Integer
+	def get_Status(self): # String
 		return self.get_query_params().get('Status')
 
-	def set_Status(self, Status):  # Integer
+	def set_Status(self, Status):  # String
 		self.add_query_param('Status', Status)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusAlertTemplatesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusAlertTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusInstanceByTagAndResourceGroupIdRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListTraceAppsRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class ListPrometheusInstanceByTagAndResourceGroupIdRequest(RpcRequest):
+class ListTraceAppsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'ListPrometheusInstanceByTagAndResourceGroupId','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'ListTraceApps','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Tags(self): # RepeatList
-		return self.get_query_params().get('Tag')
+	def get_Tagss(self): # RepeatList
+		return self.get_query_params().get('Tags')
 
-	def set_Tags(self, Tag):  # RepeatList
-		for depth1 in range(len(Tag)):
-			if Tag[depth1].get('Value') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
-			if Tag[depth1].get('Key') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+	def set_Tagss(self, Tags):  # RepeatList
+		for depth1 in range(len(Tags)):
+			if Tags[depth1].get('Value') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
+			if Tags[depth1].get('Key') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusInstancesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/StartAlertRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class ListPrometheusInstancesRequest(RpcRequest):
+class StartAlertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'ListPrometheusInstances','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'StartAlert','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ShowGlobalView(self): # Boolean
-		return self.get_query_params().get('ShowGlobalView')
+	def get_AlertId(self): # String
+		return self.get_query_params().get('AlertId')
 
-	def set_ShowGlobalView(self, ShowGlobalView):  # Boolean
-		self.add_query_param('ShowGlobalView', ShowGlobalView)
+	def set_AlertId(self, AlertId):  # String
+		self.add_query_param('AlertId', AlertId)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListPrometheusRemoteWritesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusRemoteWritesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListRetcodeAppsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListRetcodeAppsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListScenarioRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListScenarioRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListSilencePoliciesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListSilencePoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ListTraceAppsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/TagResourcesRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,32 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class ListTraceAppsRequest(RpcRequest):
+class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'ListTraceApps','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'TagResources','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
+	def get_ResourceIds(self): # RepeatList
+		return self.get_query_params().get('ResourceId')
 
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_Tagss(self): # RepeatList
-		return self.get_query_params().get('Tags')
+	def set_ResourceIds(self, ResourceId):  # RepeatList
+		for depth1 in range(len(ResourceId)):
+			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
 
-	def set_Tagss(self, Tags):  # RepeatList
-		for depth1 in range(len(Tags)):
-			if Tags[depth1].get('Value') is not None:
-				self.add_query_param('Tags.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
-			if Tags[depth1].get('Key') is not None:
-				self.add_query_param('Tags.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+	def get_ResourceType(self): # String
+		return self.get_query_params().get('ResourceType')
+
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ManageGetRecordingRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ManageGetRecordingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/ManageRecordingRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ManageRecordingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenArmsDefaultSLRRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenArmsDefaultSLRRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenArmsServiceSecondVersionRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenArmsServiceSecondVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenVClusterRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenVClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/OpenXtraceDefaultSLRRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/OpenXtraceDefaultSLRRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/QueryMetricByPageRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/QueryMetricByPageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/QueryPromInstallStatusRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/QueryPromInstallStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/QueryReleaseMetricRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/QueryReleaseMetricRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/RemoveAliClusterIdsFromPrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/RemoveAliClusterIdsFromPrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/RemoveSourcesFromPrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/RemoveSourcesFromPrometheusGlobalViewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SaveTraceAppConfigRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SaveTraceAppConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertContactGroupRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertContactGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertHistoriesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertHistoriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchAlertRulesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchAlertRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchEventsRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchEventsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchRetcodeAppByPageRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchRetcodeAppByPageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTraceAppByNameRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTraceAppByNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTraceAppByPageRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTraceAppByPageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTracesByPageRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTracesByPageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SearchTracesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SearchTracesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SendTTSVerifyLinkRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SendTTSVerifyLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SetRetcodeShareStatusRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SetRetcodeShareStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/StartAlertRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/StopAlertRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class StartAlertRequest(RpcRequest):
+class StopAlertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'StartAlert','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'StopAlert','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/StopAlertRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateDispatchRuleRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class StopAlertRequest(RpcRequest):
+class UpdateDispatchRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'StopAlert','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'UpdateDispatchRule','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AlertId(self): # String
-		return self.get_query_params().get('AlertId')
+	def get_DispatchRule(self): # String
+		return self.get_query_params().get('DispatchRule')
 
-	def set_AlertId(self, AlertId):  # String
-		self.add_query_param('AlertId', AlertId)
+	def set_DispatchRule(self, DispatchRule):  # String
+		self.add_query_param('DispatchRule', DispatchRule)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SwitchSyntheticTaskStatusRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SwitchSyntheticTaskStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/SyncRecordingRulesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/SyncRecordingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/TagResourcesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusInstanceByTagAndResourceGroupIdRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,38 +16,37 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class TagResourcesRequest(RpcRequest):
+class ListPrometheusInstanceByTagAndResourceGroupIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'TagResources','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'ListPrometheusInstanceByTagAndResourceGroupId','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceIds(self): # RepeatList
-		return self.get_query_params().get('ResourceId')
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
 
-	def set_ResourceIds(self, ResourceId):  # RepeatList
-		for depth1 in range(len(ResourceId)):
-			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_ListAsConsole(self): # Boolean
+		return self.get_query_params().get('ListAsConsole')
+
+	def set_ListAsConsole(self, ListAsConsole):  # Boolean
+		self.add_query_param('ListAsConsole', ListAsConsole)
 	def get_Tags(self): # RepeatList
 		return self.get_query_params().get('Tag')
 
 	def set_Tags(self, Tag):  # RepeatList
 		for depth1 in range(len(Tag)):
 			if Tag[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 			if Tag[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
-	def get_ResourceType(self): # String
-		return self.get_query_params().get('ResourceType')
-
-	def set_ResourceType(self, ResourceType):  # String
-		self.add_query_param('ResourceType', ResourceType)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UninstallManagedPrometheusRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UninstallManagedPrometheusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UninstallPromClusterRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UninstallPromClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UntagResourcesRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateAlertContactGroupRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateAlertContactGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateAlertContactRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateAlertContactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateAlertRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateAlertRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateDispatchRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/ListPrometheusInstancesRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class UpdateDispatchRuleRequest(RpcRequest):
+class ListPrometheusInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'UpdateDispatchRule','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'ListPrometheusInstances','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DispatchRule(self): # String
-		return self.get_query_params().get('DispatchRule')
+	def get_ClusterType(self): # String
+		return self.get_query_params().get('ClusterType')
 
-	def set_DispatchRule(self, DispatchRule):  # String
-		self.add_query_param('DispatchRule', DispatchRule)
+	def set_ClusterType(self, ClusterType):  # String
+		self.add_query_param('ClusterType', ClusterType)
+	def get_ShowGlobalView(self): # Boolean
+		return self.get_query_params().get('ShowGlobalView')
+
+	def set_ShowGlobalView(self, ShowGlobalView):  # Boolean
+		self.add_query_param('ShowGlobalView', ShowGlobalView)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusAlertRuleRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/CreatePrometheusAlertRuleRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkarms.endpoint import endpoint_data
 
-class UpdatePrometheusAlertRuleRequest(RpcRequest):
+class CreatePrometheusAlertRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'UpdatePrometheusAlertRule','arms')
+		RpcRequest.__init__(self, 'ARMS', '2019-08-08', 'CreatePrometheusAlertRule','arms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -67,22 +67,26 @@
 	def set_Message(self, Message):  # String
 		self.add_query_param('Message', Message)
 	def get_Labels(self): # String
 		return self.get_query_params().get('Labels')
 
 	def set_Labels(self, Labels):  # String
 		self.add_query_param('Labels', Labels)
+	def get_Tagss(self): # RepeatList
+		return self.get_query_params().get('Tags')
+
+	def set_Tagss(self, Tags):  # RepeatList
+		for depth1 in range(len(Tags)):
+			if Tags[depth1].get('Value') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
+			if Tags[depth1].get('Key') is not None:
+				self.add_query_param('Tags.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
 	def get_Duration(self): # String
 		return self.get_query_params().get('Duration')
 
 	def set_Duration(self, Duration):  # String
 		self.add_query_param('Duration', Duration)
-	def get_AlertId(self): # Long
-		return self.get_query_params().get('AlertId')
-
-	def set_AlertId(self, AlertId):  # Long
-		self.add_query_param('AlertId', AlertId)
 	def get_NotifyType(self): # String
 		return self.get_query_params().get('NotifyType')
 
 	def set_NotifyType(self, NotifyType):  # String
 		self.add_query_param('NotifyType', NotifyType)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusGlobalViewRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusGlobalViewRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,22 +27,27 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
+	def get_AllSubClustersSuccess(self): # Boolean
+		return self.get_query_params().get('AllSubClustersSuccess')
 
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def set_AllSubClustersSuccess(self, AllSubClustersSuccess):  # Boolean
+		self.add_query_param('AllSubClustersSuccess', AllSubClustersSuccess)
 	def get_ClusterId(self): # String
 		return self.get_query_params().get('ClusterId')
 
 	def set_ClusterId(self, ClusterId):  # String
 		self.add_query_param('ClusterId', ClusterId)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_SubClustersJson(self): # String
 		return self.get_query_params().get('SubClustersJson')
 
 	def set_SubClustersJson(self, SubClustersJson):  # String
 		self.add_query_param('SubClustersJson', SubClustersJson)
```

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusIntegrationRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusIntegrationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdatePrometheusRemoteWriteRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdatePrometheusRemoteWriteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UpdateWebhookRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UpdateWebhookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/aliyunsdkarms/request/v20190808/UploadRequest.py` & `aliyun-python-sdk-arms-2.7.30/aliyunsdkarms/request/v20190808/UploadRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-arms-2.7.29/setup.py` & `aliyun-python-sdk-arms-2.7.30/setup.py`

 * *Files identical despite different names*


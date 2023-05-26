# Comparing `tmp/RobertCommonDriver-0.1.40.tar.gz` & `tmp/RobertCommonDriver-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.40.tar", last modified: Tue May 16 09:48:36 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.41.tar", last modified: Fri May 26 06:57:25 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.40.tar` & `RobertCommonDriver-0.1.41.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.756651 RobertCommonDriver-0.1.40/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.40/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.40/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2023-05-16 09:48:36.756651 RobertCommonDriver-0.1.40/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.40/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.681626 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.40/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.681626 RobertCommonDriver-0.1.40/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.40/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.682664 RobertCommonDriver-0.1.40/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.697671 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87343 2023-03-23 08:25:35.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6025 2023-05-09 08:30:24.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38296 2022-12-01 08:59:47.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.714684 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    67007 2023-05-09 13:35:59.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    62759 2023-05-12 07:35:58.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566042 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46969 2023-04-14 08:33:27.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    33838 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18368 2023-04-27 02:18:02.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    62003 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24929 2023-05-16 07:04:43.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43449 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51679 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41574 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32863 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44698 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-05-16 09:48:36.758043 RobertCommonDriver-0.1.40/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-05-16 08:13:01.000000 RobertCommonDriver-0.1.40/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.715690 RobertCommonDriver-0.1.40/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.40/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.716692 RobertCommonDriver-0.1.40/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.40/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.730853 RobertCommonDriver-0.1.40/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.755300 RobertCommonDriver-0.1.40/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22764 2023-04-27 08:47:35.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15871 2023-05-08 12:34:54.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     8219 2023-05-16 07:37:56.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.583469 RobertCommonDriver-0.1.41/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.41/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.41/MANIFEST.in
+-rw-rw-rw-   0        0        0     1744 2023-05-26 06:57:25.582466 RobertCommonDriver-0.1.41/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.41/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.499331 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0     1744 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-26 06:57:25.000000 RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.41/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.500330 RobertCommonDriver-0.1.41/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.41/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.501331 RobertCommonDriver-0.1.41/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.516494 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87350 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6025 2023-05-09 08:30:24.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38314 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.538701 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    67070 2023-05-23 12:30:50.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65934 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566090 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46987 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34343 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18368 2023-04-27 02:18:02.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    62043 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24991 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43449 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51679 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41711 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32984 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44835 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:57:25.583469 RobertCommonDriver-0.1.41/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-05-26 02:15:16.000000 RobertCommonDriver-0.1.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.540697 RobertCommonDriver-0.1.41/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.41/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.541696 RobertCommonDriver-0.1.41/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.41/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.556396 RobertCommonDriver-0.1.41/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:25.580030 RobertCommonDriver-0.1.41/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.40/LICENSE` & `RobertCommonDriver-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/PKG-INFO` & `RobertCommonDriver-0.1.41/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.40
+Version: 0.1.41
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.40/README.md` & `RobertCommonDriver-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.40
+Version: 0.1.41
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.41/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1311,16 +1311,15 @@
 
         if self.bacnet_device:
             del self.bacnet_device
 
         self.bacnet_application = None
         self.bacnet_device = None
 
-        self._release_bacnet_application_v1(self.bacnet_readwrite_application)
-        self.bacnet_readwrite_application = None
+        self.bacnet_readwrite_application = self._release_bacnet_application_v1(self.bacnet_readwrite_application)
 
     # get local bacnet ip (192.168.1.0/24)
     def _get_local_bacnet_ip(self, ip: str, net: str):
         ip_start = ip_address(str(ip_network(ip, False)).split('/')[0])
         ip_end = ip_network(ip, False).broadcast_address
 
         addrs = net_if_addrs().items()
@@ -1600,15 +1599,15 @@
 
         if bacnet_device:
             bacnet_application = bacnet_app_class(bacnet_device, self.bacnet_server_ip, self)
             self.set_call_result('debug_log', content=f"bacnet({self}) get app: {bacnet_application}")
             if bacnet_application is not None:
                 if bacnet_application.bacnet_init_status is False:
                     logging.error(f'bacnet({self}) get application({self.bacnet_server_ip}) fail {bacnet_application.bacnet_exception}')
-                    self._release_bacnet_application_v1(bacnet_application)
+                    bacnet_application = self._release_bacnet_application_v1(bacnet_application)
                 else:
                     BaseCommon.function_thread(self.control_status, False).start()
                     time.sleep(1)
                     return bacnet_application
         return None
 
     def _release_bacnet_application_v1(self, bacnet_application):
@@ -1621,14 +1620,15 @@
                     bacnet_application.close_socket()
         except Exception as e:
             logging.error(f'bacnet({self}) release {self.bacnet_server_ip} fail {e}')
         finally:
             if bacnet_application:
                 del bacnet_application
             bacnet_application = None
+        return None
 
     def _search_bacnet_device_list_v1(self) -> list:
         self.bacnet_device_list = []
         bacnet_whois_application = None
         try:
             bacnet_whois_application = self._get_bacnet_application_v1(BacnetWhoIsIAmApplication)
             if bacnet_whois_application is not None:
@@ -1636,15 +1636,15 @@
                 BaseCommon.function_thread(fn=self._end_search_bacnet_device_v1, daemon=True, bacnet_application=bacnet_whois_application).start()
 
                 bacnet_whois_application.discover_bacnet_device()
 
                 run(spin=0.1)
             return self.bacnet_device_list
         finally:
-            self._release_bacnet_application_v1(bacnet_whois_application)
+            bacnet_whois_application = self._release_bacnet_application_v1(bacnet_whois_application)
 
     def _read_bacnet_obj_v1(self, bacnet_scan_application, bacnet_address, bacnet_id, obj_type, obj_inst, prop_id, index=None):
         request = ReadPropertyRequest(objectIdentifier=(obj_type, obj_inst), propertyIdentifier=prop_id, propertyArrayIndex=index)
         request.pduDestination = bacnet_address
 
         result = bacnet_scan_application.make_request_iocb(request).ioResponse
         if isinstance(result, ReadPropertyACK):
@@ -1740,15 +1740,15 @@
                         obj_result = self._read_bacnet_obj_v1(bacnet_scan_application, bacnet_address, bacnet_id, "device", bacnet_id, 'objectList', index=array_index)
                         if obj_result is not None:
                             obj_type, obj_index = obj_result
                             bacnet_point_dict.update(self._read_bacnet_prop_v1(bacnet_scan_application, bacnet_address, bacnet_id, obj_type, obj_index, array_index, bacnet_property_reference_list))
                             self.set_call_result('debug_log', content=f"bacnet({self}) read ({bacnet_current}) object: {array_index}/{object_count} address: {bacnet_device_address}/{bacnet_device_id}")
             return bacnet_point_dict
         finally:
-            self._release_bacnet_application_v1(bacnet_scan_application)
+            bacnet_scan_application = self._release_bacnet_application_v1(bacnet_scan_application)
 
     def _format_name_v1(self, device_address: str, device_id: str, type: str, address: str):
         return '%s_%s_%s_%s' % (device_address.replace('.', '_').replace(':', '_'), device_id, type, address)
 
     def _read_bacnet_values_v1(self, bacnet_point_dict: dict, auto_release=True) -> dict:
         result_dict = {}
         try:
@@ -1756,31 +1756,28 @@
                 self.bacnet_readwrite_application = self._get_bacnet_application_v1(BacnetReadWriteApplication)
             if self.bacnet_readwrite_application is not None:
                 result_dict = self.bacnet_readwrite_application._read_values(bacnet_point_dict, self.bacnet_cmd_interval, self.bacnet_multi_read)
             return result_dict
         finally:
             if self.bacnet_readwrite_application is not None:
                 if auto_release is True:
-                    self._release_bacnet_application_v1(self.bacnet_readwrite_application)
-                    self.bacnet_readwrite_application = None
+                    self.bacnet_readwrite_application = self._release_bacnet_application_v1(self.bacnet_readwrite_application)
                 elif len(bacnet_point_dict) > 0 >= len(result_dict):
-                    self._release_bacnet_application_v1(self.bacnet_readwrite_application)
-                    self.bacnet_readwrite_application = None
+                    self.bacnet_readwrite_application = self._release_bacnet_application_v1(self.bacnet_readwrite_application)
 
     def _write_bacnet_value_v1(self, bacnet_point, bacnet_value, auto_release=True) -> bool:
         try:
             if self.bacnet_readwrite_application is None:
                 self.bacnet_readwrite_application = self._get_bacnet_application_v1(BacnetReadWriteApplication)
             if self.bacnet_readwrite_application is not None:
                 return self.bacnet_readwrite_application.write_single_value(bacnet_point, bacnet_value)
             return False
         finally:
             if auto_release is True:
-                self._release_bacnet_application_v1(self.bacnet_readwrite_application)
-                self.bacnet_readwrite_application = None
+                self.bacnet_readwrite_application = self._release_bacnet_application_v1(self.bacnet_readwrite_application)
 
     def control_status(self, status: bool = True):
         if status is True:
             enable_sleeping()
             run(spin=0.1)
         else:
             stop()
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/modbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,17 +240,18 @@
             raise e
         return self.modbus_client
 
     def _release_modbus_client(self):
         try:
             if self.modbus_client:
                 self.modbus_client.close()
-            self.modbus_client = None
         except Exception as e:
             raise e
+        finally:
+            self.modbus_client = None
 
     def _sort_point_by_device(self):
         try:
             if len(self.dict_point) > 0:
                 self.new_point_list = []
 
                 # First create a new point by type and number of bits
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
                     values = [values]
                 if type in [IOTBaseCommon.DataTransform.TypeFormat.BOOL, IOTBaseCommon.DataTransform.TypeFormat.BOOL_ARRAY]:
                     buffer = IOTBaseCommon.DataTransform.convert_bool_array_to_byte(values)
                 else:
                     type_size, type_fmt = IOTBaseCommon.DataTransform.get_type_size_fmt(type, little_endian)
                     buffer = bytearray(len(values) * type_size)
                     for i in range(len(values)):
-                        buffer[(i * type_size): (i + 1) * type_size] = pack(type_fmt, values[i])
+                        buffer[(i * type_size): (i + 1) * type_size] = pack(type_fmt, values[i] if type_fmt[-1:] in ['f', 'd'] else int(float(str(values[i]))))
             return buffer
 
         @staticmethod
         def format_bytes(data: bytes) -> str:
             return ''.join(["%02X " % x for x in data]).strip()
 
         @staticmethod
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from threading import Lock, Event
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Callable, Tuple
 from queue import Queue
 from inspect import stack
+from concurrent.futures import ThreadPoolExecutor
 
 from .base import IOTBaseCommon, IOTDriver, IOTSimulateObject, FunctionTimedOut, func_timeout
 
 # bacnet
-from bacpypes.apdu import AbortReason, RejectReason, ReadAccessSpecification, ConfirmedRequestSequence, ConfirmedCOVNotificationRequest, PropertyReference, ReadPropertyMultipleRequest, ReadPropertyMultipleACK, ReadPropertyRequest, ReadPropertyACK, WritePropertyRequest, SimpleAckPDU, WhoIsRequest, IAmRequest, AbortPDU, RejectPDU, SubscribeCOVRequest
+from bacpypes.apdu import APDU, AbortReason, RejectReason, ReadAccessSpecification, ConfirmedRequestSequence, ConfirmedCOVNotificationRequest, PropertyReference, ReadPropertyMultipleRequest, ReadPropertyMultipleACK, ReadPropertyRequest, ReadPropertyACK, WritePropertyRequest, SimpleAckPDU, WhoIsRequest, IAmRequest, AbortPDU, RejectPDU, SubscribeCOVRequest
 from bacpypes.app import BIPSimpleApplication
 from bacpypes.basetypes import ServicesSupported, StatusFlags
 from bacpypes.constructeddata import Array, Any, Choice
 from bacpypes.core import run, stop, deferred, enable_sleeping
 from bacpypes.iocb import IOCB
 from bacpypes.local.device import LocalDeviceObject
 from bacpypes.npdu import WhoIsRouterToNetwork, WhatIsNetworkNumber
@@ -37,14 +38,92 @@
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def update(self, **kwargs):
         self.kwargs.update(kwargs)
 
 
+class IOCBHelper:
+
+    def __init__(self, iocb: IOCB, request_io: Callable[[IOCB], Any]):
+        self.iocb = iocb
+        self.request_io = request_io
+
+    def __enter__(self):
+        deferred(self.request_io, self.iocb)
+        self.iocb.wait()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        deferred(stop)
+
+
+class BacnetClientSample(BIPSimpleApplication):
+
+    def __init__(self, local_address: Address):
+        super(BacnetClientSample, self).__init__(LocalDeviceObject(
+            objectName="BACpypes Client",
+            objectIdentifier=("device", 1),
+            maxApduLengthAccepted=1024,
+            segmentationSupported="segmentedBoth",
+            vendorIdentifier=15,
+        ), local_address)
+
+    def _init_iocb(self, iocb: IOCB, successful_callback: Callable[[APDU], Any]) -> Any:
+        with IOCBHelper(iocb, self.request_io):
+            if iocb.ioError:
+                raise Exception(f"something error({iocb.ioError})")
+            elif iocb.ioResponse:
+                return successful_callback(iocb.ioResponse)
+            else:
+                raise Exception(f"something wrong")
+            return None
+
+    def _do_read_property(self, read_property_request: ReadPropertyRequest, property_identifier: str):
+
+        def callback(apdu: APDU) -> Any:
+            datatype = get_datatype(apdu.objectIdentifier[0], property_identifier)
+            if not datatype:
+                raise TypeError("unknown datatype")
+            # special case for array parts, others are managed by cast_out
+            value = apdu.propertyValue.cast_out(datatype)
+            return value
+
+        return self._init_iocb(IOCB(read_property_request), callback)
+
+    def _do_read_property_multiple(self, read_property_multiple_request: ReadPropertyMultipleRequest):
+        def callback(apdu: APDU) -> Any:
+            return None
+
+        return self._init_iocb(IOCB(read_property_multiple_request), callback)
+
+    def make_request_read_property(self, device_address: Address, object_identifier: Tuple[str, int],
+                                   property_identifier: str):
+        # Create a BACnet ReadPropertyRequest
+        request = ReadPropertyRequest(
+            objectIdentifier=object_identifier,
+            propertyIdentifier=property_identifier,
+        )
+        request.pduDestination = device_address
+
+        with ThreadPoolExecutor() as executor:
+            future = executor.submit(self._do_read_property, request, property_identifier)
+            run()
+            return future.result()
+
+    def make_request_read_property_multiple(self, device_address: Address):
+        # Create a BACnet ReadPropertyMultipleRequest
+        request = ReadPropertyMultipleRequest()
+        request.pduDestination = device_address
+
+        with ThreadPoolExecutor() as executor:
+            future = executor.submit(self._do_read_property, request)
+            run()
+            return future.result()
+
+
 class BacnetSimulateObject:
 
     class BacnetObject:
         presentValue = None
 
         def set_value(self, name, value):
             pass  # print(f"set value ({name}:{value})")
@@ -287,15 +366,15 @@
             iocb.wait()
         return iocb
 
     def send_request(self, request, wait: bool = True, context: Optional[IOCBContext] = None, process: Optional[str] = ''):
         with self.read_write_lock:
             self.process = process
             iocb = IOCB(request)
-            iocb.set_timeout(self.kwargs.get('timeout', 3000), err=TimeoutError)
+            iocb.set_timeout(self.kwargs.get('timeout', 3000) * (self.kwargs.get('retry', 0) + 1) * 1.2, err=TimeoutError)
             if request.apduInvokeID is None:
                 request.apduInvokeID = self.get_next_invoke_id(request.pduDestination)
             if context is None:
                 context = IOCBContext(invoke_id=request.apduInvokeID)
             else:
                 context.update(invoke_id=request.apduInvokeID)
             iocb.context = context
@@ -1120,28 +1199,30 @@
 
     def _release_client(self):
         try:
             if self.client is not None:
                 self.client.exit()
         except:
             pass
-        self.client = None
+        finally:
+            self.client = None
 
     def _get_server(self):
         if self.server is None:
             self.server = BacnetClient(False, self, **self.configs)
         return self.server
 
     def _release_server(self):
         try:
             if self.server is not None:
                 self.server.exit()
         except:
             pass
-        self.server = None
+        finally:
+            self.server = None
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
             if self._get_client():
                 for target_address, objct_propertys in read_items.items():
                     self.client.read(target_address=target_address, objct_propertys=objct_propertys, max_per_request=self.configs.get('multi_read'), use_read_multiple=self.configs.get('multi_read') > 1, ping_check=False)
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files 0% similar despite different names*

```diff
@@ -12058,15 +12058,15 @@
             if mode == 0:
                 templates.append({'required': False, 'name': '逻辑点名' if lan == 'ch' else 'name alias'.upper(), 'code': 'point_name_alias', 'type': 'string', 'default': 'Chiller_1_CHW_ENT1', 'enum': [], 'tip': ''})
             else:
                 templates.append({'required': True, 'name': '点值' if lan == 'ch' else 'value'.upper(), 'code': 'point_value', 'type': 'int', 'default': 0, 'enum': [], 'tip': ''})
             templates.append({'required': True, 'name': '是否启用' if lan == 'ch' else 'enable'.upper(), 'code': 'point_enabled', 'type': 'bool', 'default': 'TRUE', 'enum': [], 'tip': ''})
             templates.append({'required': True, 'name': '倍率' if lan == 'ch' else 'scale'.upper(), 'code': 'point_scale', 'type': 'string', 'default': '1', 'enum': [], 'tip': ''})
         elif type == 'config':
-            templates.append({'name': '端口' if lan == 'ch' else 'Bacnet Port', 'required': True, 'code': 'address', 'type': 'string', 'default': 'COM2/38400', 'enum': [], 'tip': ''})
+            templates.append({'name': '端口' if lan == 'ch' else 'Bacnet Port', 'required': True, 'code': 'address', 'type': 'string', 'default': 'COM2|38400', 'enum': [], 'tip': ''})
             templates.append({'name': '设备MAC' if lan == 'ch' else 'Bacnet MAC Address', 'required': True, 'code': 'identifier', 'type': 'int', 'default': 5555, 'enum': [], 'tip': ''})
             templates.append({'name': '设备重试' if lan == 'ch' else 'Bacnet Retries', 'required': True, 'code': 'retry', 'type': 'int', 'default': 2, 'enum': [], 'tip': ''})
             templates.append({'name': '设备segmentation' if lan == 'ch' else 'Bacnet Sever segmentation', 'required': True, 'code': 'segmentation', 'type': 'int', 'default': 65, 'enum': [], 'tip': ''})
             templates.append({'name': '设备vendor' if lan == 'ch' else 'Bacnet Sever vendor', 'required': True, 'code': 'vendor_identifier', 'type': 'int', 'default': 15, 'enum': [], 'tip': ''})
 
             if mode == 0:
                 templates.append({'name': '批量读取个数' if lan == 'ch' else 'Multi Read', 'required': True, 'code': 'multi_read', 'type': 'int', 'default': 20, 'enum': [], 'tip': ''})
@@ -12202,17 +12202,17 @@
                 bacnet_type = BACnetDefine.BACnetAddressTypes.IP
                 [ip, port] = IOTBaseCommon.change_local_ip(address).split(':')
                 ip_list = ip.split('/')
                 if len(ip_list) >= 2:
                     bacnet_params.update({'ip': ip_list[1], 'port': int(str(port))})
                 else:
                     bacnet_params.update({'ip': ip, 'port': int(str(port))})
-            else:  # COM/Baud
+            else:  # COM|Baud
                 bacnet_type = BACnetDefine.BACnetAddressTypes.MSTP
-                ip_list = address_list[0].split('/')
+                ip_list = address_list[0].split('|')
                 if len(ip_list) >= 2:
                     bacnet_params.update({'port_name': ip_list[0], 'baud_rate': int(str(ip_list[1]))})
         return bacnet_type, bacnet_params
 
     def _get_client(self):
         if self.client is None:
             bacnet_type, bacnet_params = self._change_bacnet_address(self.configs.get('address'))
@@ -12225,29 +12225,31 @@
 
     def _release_client(self):
         try:
             if self.application is not None:
                 self.application.exit()
         except:
             pass
-        self.application = None
-        self.client = None
+        finally:
+            self.application = None
+            self.client = None
 
     def _get_server(self):
         if self.server is None:
             self.server = None
         return self.server
 
     def _release_server(self):
         try:
             if self.server is not None:
                 self.server.exit()
         except:
             pass
-        self.server = None
+        finally:
+            self.server = None
 
     def _read(self, read_items: dict):
         if len(read_items) > 0:
             if self._get_client():
                 for target_address, objct_propertys in read_items.items():
                     self.application.read(self.client, target_address, objct_propertys)
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_iec104.py`

 * *Files 0% similar despite different names*

```diff
@@ -1083,17 +1083,18 @@
     def _write(self, type: int, address: int, value):
         raise NotImplementedError()
 
     def _release_client(self):
         try:
             if self.client:
                 self.client.exit()
-            self.client = None
         except Exception as e:
             pass
+        finally:
+            self.client = None
 
     def _get_client(self):
         if self.client is not None and self.client.check_invalid() is False:
             self._release_client()
 
         if self.client is None:
             client = IOTBaseCommon.IECSocketClient(self.configs.get('host'), self.configs.get('port'), self.configs.get('timeout', 4), callbacks={'handle_data': self.handle_data, 'handle_connect': self.handle_connect, 'handle_close': self.handle_close, 'handle_error': self.handle_error})
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_modbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                 fun_code = point.get('point_fun_code')
                 address = point.get('point_address')
                 data_type = point.get('point_data_type')
                 data_length = point.get('point_data_length')
                 data_order = point.get('point_data_order', 0)
                 if device_address is not None and slave_id is not None and fun_code is not None and address is not None and data_type is not None and data_length is not None:
                     self._write(device_address, slave_id, fun_code, address, data_type, data_length, data_order, value)
-                    result = self.get_device_property(device_address, self._gen_key(slave_id, fun_code, address), [self.get_write_quality, self.get_write_result])
+                    result = self.get_device_property(device_address, IOTModbus.gen_key(slave_id, fun_code, address), [self.get_write_quality, self.get_write_result])
                 else:
                     result = [False, 'Invalid Params']
             else:
                 result = [False, 'Point UnExist']
             results[name] = result
             if result[0] is not True:
                 self.logging(content=f"write value({name}) fail({result[1]})", level='ERROR', source=name, pos=self.stack_pos)
@@ -315,15 +315,16 @@
                 for id, codes in slaves.items():
                     for code, objects in codes.items():
                         if self._get_server(address) is not None:
                             self._create_objects(address, id, code, objects)
 
                             self._refresh_objects(address, id, code, objects)
 
-    def _gen_key(self, slave_id: int, fun_code: int, address: int) -> str:
+    @staticmethod
+    def gen_key(slave_id: int, fun_code: int, address: int) -> str:
         return f"{slave_id}_{fun_code}_{address}"
 
     def _combine_read_unit(self, modbus_unit, modbus_read_units: dict):
         read_units = modbus_read_units.get(modbus_unit.__str__())
         if read_units is not None:
             if modbus_unit.get_modbus_start == (read_units[-1].get_modbus_end + 1):
                 if read_units[-1].get_modbus_end - read_units[-1].get_modbus_start + 1 >= self.configs.get('multi_read', 100):  # 超过连读上限
@@ -434,25 +435,25 @@
         try:
             self.pending()
             fun_code = self._change_fun_code(fun_code)
             if self._get_client(address) is not None:
                 self.logging(content=f"modbus({address}) read ({slave_id}-{fun_code}-[{add_start}-{add_end}])", pos=self.stack_pos)
                 value_list = self._get_client(address).execute(slave_id, fun_code, add_start, add_end - add_start + 1)
                 for index in range(0, len(value_list)):
-                    self.update_device(address, self._gen_key(slave_id, fun_code, add_start + index), **self.gen_read_write_result(True, value_list[index]))
+                    self.update_device(address, IOTModbus.gen_key(slave_id, fun_code, add_start + index), **self.gen_read_write_result(True, value_list[index]))
         except (socket_timeout, ConnectionRefusedError, ConnectionResetError) as e:  # connect
             err_msg = f"connect fail: {e.__str__()}"
             self._release_client(address)
         except Exception as e:  # other
             err_msg = e.__str__()
         finally:
             if err_msg is not None:
                 self.logging(content=f"modbus({address}) read ({slave_id}-{fun_code}-[{add_start}-{add_end}]) fail({err_msg})", level='ERROR', pos=self.stack_pos)
                 for i in range(add_start, add_end + 1):
-                    self.update_device(address, self._gen_key(slave_id, fun_code, i), **self.gen_read_write_result(False, err_msg))
+                    self.update_device(address, IOTModbus.gen_key(slave_id, fun_code, i), **self.gen_read_write_result(False, err_msg))
 
     def _read_address(self, *args, **kwargs) -> dict:
         (address, slave_items) = args
         results = {}
         read_units = self.cread_read_units(address, slave_items)
         for k, modbus_units in read_units.items():
             for modbus_unit in modbus_units:
@@ -464,34 +465,43 @@
     def _read(self, read_items: dict) -> dict:
         if len(read_items) > 0:
             jobs = IOTBaseCommon.SimpleThreadPool(len(read_items))
             for address, slaves in read_items.items():
                 jobs.submit_task(self._read_address, address, slaves)
             return jobs.done()
         return {}
+    
+    @staticmethod
+    def convert_value(length: int, type: int, order: int, values: list = []):
+        pos = 0
+        if type == IOTBaseCommon.DataTransform.TypeFormat.BOOL_ARRAY.value:
+            pos = length
+        length = IOTBaseCommon.DataTransform.get_type_word_size(type, length)
+        if len(values) == length:
+            return IOTBaseCommon.DataTransform.convert_value(values, IOTBaseCommon.DataTransform.TypeFormat.UINT16, IOTBaseCommon.DataTransform.TypeFormat(type), pos=pos, format=IOTBaseCommon.DataTransform.DataFormat(order))
+        return None
+    
+    @staticmethod
+    def get_type_size(type: int, length: int = 0):
+        return IOTBaseCommon.DataTransform.get_type_word_size(type, length)
 
     def get_value(self, name: str, address: str, slave_id: int, fun_code: int, start: int, length: int, type: int, order: int):
         try:
             values = []
-            pos = 0
-            if type == IOTBaseCommon.DataTransform.TypeFormat.BOOL_ARRAY.value:
-                pos = length
-            length = IOTBaseCommon.DataTransform.get_type_word_size(type, length)
-            for i in range(length):
-                key = self._gen_key(slave_id, fun_code, start+i)
+            for i in range(IOTModbus.get_type_size(type, length)):
+                key = IOTModbus.gen_key(slave_id, fun_code, start+i)
                 [result, value] = self.get_device_property(address, key, [self.get_read_quality, self.get_read_result])
                 if result is True:
                     if value is not None:
                         values.append(value)
                     else:
                         raise Exception(f"({key}) is none")
                 else:
                     raise Exception(str(value))
-            if len(values) == length:
-                return IOTBaseCommon.DataTransform.convert_value(values, IOTBaseCommon.DataTransform.TypeFormat.UINT16, IOTBaseCommon.DataTransform.TypeFormat(type), pos=pos, format=IOTBaseCommon.DataTransform.DataFormat(order))
+            return IOTModbus.convert_value(length, type, order, values)
         except Exception as e:
             self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
         return None
 
     def _convert_value_to_vector(self, src_type: int, src_order: int, dst_type: int, value):
         if src_type == IOTBaseCommon.DataTransform.TypeFormat.BOOL_ARRAY.value:
             return value
@@ -514,26 +524,26 @@
                 else:
                     set_size = 1
 
                 fun_write_code = self._change_fun_code(fun_code, mode=1, length=set_size)
                 self.logging(content=f"modbus({address}) write ({slave_id}-{fun_write_code}-[{start}-{start + set_size}])-({value})", pos=self.stack_pos)
                 value_list = self._get_client(address).execute(slave_id, fun_write_code, start, output_value=set_values)
                 if len(value_list) == 2 and value_list[0] == start:
-                    return self.update_device(address, self._gen_key(slave_id, fun_code, start), **self.gen_read_write_result(True, None, False))
+                    return self.update_device(address, IOTModbus.gen_key(slave_id, fun_code, start), **self.gen_read_write_result(True, None, False))
 
             err_msg = 'Unknown'
         except (socket_timeout, ConnectionRefusedError, ConnectionResetError) as e:  # connect
             err_msg = f"connect fail: {e.__str__()}"
             self._release_client(address)
         except Exception as e:  # other
             err_msg = e.__str__()
         finally:
             if err_msg is not None:
                 self.logging(content=f"modbus({address}) write ({slave_id}-{fun_code}-{start}) fail({err_msg})", level='ERROR', pos=self.stack_pos)
-                self.update_device(address, self._gen_key(slave_id, fun_code, start), **self.gen_read_write_result(False, err_msg, False))
+                self.update_device(address, IOTModbus.gen_key(slave_id, fun_code, start), **self.gen_read_write_result(False, err_msg, False))
 
     def _get_server(self, address: str):
         server = self.servers.get(address, {}).get('server')
         if server is None:
             modbus_info = self._get_address_info(address)
             if 'type' in modbus_info.keys():
                 modbus_type = modbus_info['type']
@@ -553,17 +563,19 @@
         return server
 
     def _release_server(self, address: str):
         try:
             server = self.servers.get(address, {}).get('server')
             if server is not None:
                 server.stop()
-            server = None
         except:
             pass
+        finally:
+            if 'server' in self.servers.get(address, {}).keys():
+                del self.servers[address]['server']
 
     def _get_slave(self, server, cache: dict, id: int):
         slave = cache.get('slaves', {}).get(id)
         if slave is None:
             slave = server.add_slave(id)
             cache['slaves'][id] = {'slave': slave, 'blocks': {}}
         return slave
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import time
 
 from datetime import datetime
 from inspect import stack
 from os import getenv as os_getenv
 from platform import system as platform_system
 from Pyro4 import Proxy, expose as pyro4_expose
@@ -1188,17 +1189,18 @@
         return None
 
     def _release_client(self, client):
         try:
             if client:
                 client.close()
         except Exception as e:
-            print(f'release client fail({e.__str__()})')
+            logging.error(f'release client fail({e.__str__()})')
         finally:
             client = None
+        return None
 
     def _get_client(self, auto_connect: bool = True):
         if self.client is None:
             info = self._get_host_info()
             if isinstance(info, dict):
                 client = None
                 try:
@@ -1210,15 +1212,15 @@
                     if auto_connect is True:
                         client.connect(info.get('server'), info.get('host'))
                         self.logging(content=f"connect opc({info.get('host')}-{info.get('server')})", pos=self.stack_pos)
 
                         client.add_group(self.configs.get('group'), self.configs.get('update_rate'))
                         self.logging(content=f"add opc group({self.configs.get('group')})", pos=self.stack_pos)
                 except Exception as e:
-                    self._release_client(client)
+                    client = self._release_client(client)
                     raise e
                 self.client = client
         return self.client
 
     def pump_wait_msg(self):
         while self.exit_flag is False:
             try:
@@ -1273,13 +1275,12 @@
         except Exception as e:
             for tag in set_values.keys():
                 self.update_device(self.configs.get('server'), tag, **self.gen_read_write_result(False, e.__str__(), False))
             self.logging(content=f"opcda read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def close(self):
         if self.client is not None:
-            self._release_client(self.client)
-        self.client = None
+            self.client = self._release_client(self.client)
 
     def info(self, **kwargs):
         if self._get_client():
             return self._get_client().get_info()
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_opcua.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,23 +251,25 @@
             if self.client is not None:
                 if self.sub is not None:
                     for sub in self.subs:
                         self.sub.unsubscribe(sub)
                     self.sub.delete()
         except:
             pass
+
         try:
             if self.client:
                 self.client.disconnect()
         except:
             pass
-        self.subs = []
-        self.sub = None
-        self.client = None
-        self.devices = {}
+        finally:
+            self.subs = []
+            self.sub = None
+            self.client = None
+            self.devices = {}
 
     def _get_sub(self):
         if self.sub is None:
             sub = self._get_client().create_subscription(self.configs.get('subscript_interval', 500), self.SubHandler(callbacks={'datachange_notification': self._datachange_notification, 'event_notification': self._event_notification, 'status_change_notification': self._status_change_notification}))
             self.sub = sub
         return self.sub
 
@@ -401,16 +403,17 @@
 
     def _release_server(self):
         try:
             if self.server is not None:
                 self.server.stop()
         except Exception as e:
             pass
-        self.server = None
-        self.server_node_folder = {}
+        finally:
+            self.server = None
+            self.server_node_folder = {}
 
     def _create_folder(self, server, paths: Union[str, list]):
         root_folder = self.server_node_folder[self.configs.get('root', 'Robert')]
         if isinstance(paths, list):
             for index, folder in enumerate(paths):
                 self._create_folder(server, '/'.join(paths[:index+1]))
         elif isinstance(paths, str):
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,14 +824,17 @@
         try:
             server = self.servers.get(address, {}).get('server')
             if server is not None:
                 server.stop_server()
             server = None
         except:
             pass
+        finally:
+            if 'server' in self.servers.get(address, {}).keys():
+                del self.servers[address]['server']
 
     def _refresh_objects(self, address: str, objects: list):
         server_cache = self.servers.get(address, {})
         server = server_cache.get('server')
         if server is not None and len(objects) > 0:
             units = IOTBaseCommon.chunk_list(objects, self.configs.get('multi_read'))
             for unit in units:
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,15 @@
                     if pos >= 4:
                         start = int(float(infos[1][4:pos]))
                         addr = int(float(infos[1][pos + 1:]))
                 elif infos[1].startswith('X'):
                     type = IOTBaseCommon.DataTransform.TypeFormat.BOOL
                     length = 1
                     pos = infos[1].find('.')
-                    if pos >= 4:
+                    if pos >= 1:
                         start = int(float(infos[1][1:pos]))
                         addr = int(float(infos[1][pos + 1:]))
 
         else:   # I2.0 VD200
             db = 1 if area == 'V' else 0
             if address[1] == 'B':   # BYTE
                 type = IOTBaseCommon.DataTransform.TypeFormat.INT8
@@ -615,14 +615,17 @@
             server = self.servers.get(port, {}).get('server')
             if server is not None:
                 server.stop()
                 server.destroy()
             server = None
         except:
             pass
+        finally:
+            if 'server' in self.servers.get(port, {}).keys():
+                del self.servers[port]['server']
 
     # 合并生成地址块单元
     def _combine_unit(self, block_unit, block_units: dict):
         units = block_units.get(block_unit.__str__())
         if units is not None:
             if block_unit.get_size > units.get_size:
                 units.set_size(block_unit.get_size)
@@ -663,15 +666,15 @@
                         blocks[key] = block
             except Exception as e:
                 self.logging(content=f"create object({port}) fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _update_value(self, server, block, area, db, start: int, addr: int, type, value):
         if server is not None and isinstance(block, dict):
             index = start
-            if server and index >= 0 and index < block.get('size'):
+            if server and 0 <= index < block.get('size'):
                 if type == IOTBaseCommon.DataTransform.TypeFormat.BOOL:
                     server.lock_area(area, db)
                     snap7_util.set_bool(block.get('buffer'), index, addr, bool(int(float(value))))
                     server.unlock_area(area, db)
                 elif type == IOTBaseCommon.DataTransform.TypeFormat.INT16:
                     server.lock_area(area, db)
                     snap7_util.set_int(block.get('buffer'), index, int(float(value)))
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files 0% similar despite different names*

```diff
@@ -890,14 +890,17 @@
         try:
             server = self.servers.get(address, {}).get('server')
             if server is not None:
                 server.stop_server()
             server = None
         except:
             pass
+        finally:
+            if 'server' in self.servers.get(address, {}).keys():
+                del self.servers[address]['server']
 
     def _refresh_objects(self, address: str, objects: list):
         server_cache = self.servers.get(address, {})
         server = server_cache.get('server')
         if server is not None and len(objects) > 0:
             units = IOTBaseCommon.chunk_list(objects, self.configs.get('multi_read'))
             for unit in units:
```

### Comparing `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.41/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/setup.py` & `RobertCommonDriver-0.1.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.40'
-DATE = '2023-05-16'
+VERSION = '0.1.41'
+DATE = '2023-05-26'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     dict_config = {
         'address': '192.168.1.17/24:47808',  # bacnet server ip(绑定网卡)
         'identifier': 555,  # bacnet server identifier
         'name': 'BacnetDriver',  # bacnet server name
         'max_apdu': 1024,  # bacnet server max apdu
         'segmentation': 'segmentedBoth',  # bacnet server segmentation
         'vendor_identifier': 15,  # bacnet server vendor
-        'multi_read': 20,  # bacnet 批量读取个数
+        'multi_read': 40,  # bacnet 批量读取个数
         'cmd_interval': 0.3,  # bacnet命令间隔
         'time_out': 5000  # 超时时间
     }
 
     dict_point = {'6_4_1_analogValue_1': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True',
                                           'point_device_address': '6:4/604/192.168.1.184', 'point_type': 'analogValue',
                                           'point_property': 'presentValue', 'point_address': 1,
                                           'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
                   '6_4_2_analogValue_2': {'point_name': '6_4_2_analogValue_2', 'index': 3, 'point_writable': 'True',
-                                          'point_device_address': '192.168.1.172', 'point_type': 'analogInput',
+                                          'point_device_address': '192.168.1.184', 'point_type': 'analogInput',
                                           'point_property': 'presentValue', 'point_address': 3,
                                           'point_description': '', 'objectName': 'Random-604-2', 'presentValue': '2.0'},
                   }
 
     dict_point1 = {'192_168_1_184_47808_6_2_602_2_1': {'point_name': '192_168_1_184_47808_6_2_602_2_1', 'index': 0,
                                                        'point_writable': 'True',
                                                        'point_device_address': '6:2/602/192.168.1.184',
@@ -46,59 +46,59 @@
                                                        'point_writable': 'True',
                                                        'point_device_address': '6:2/612/192.168.1.184',
                                                        'point_type': 'analogValue', 'point_property': 'presentValue',
                                                        'point_address': 1233, 'description': 'None', 'point_value': '1.0',
                                                        'object_name': 'Random-602-1'}
                    }
 
-    points = {'6_4_1_analogValue_1': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.171', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_12': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_13': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 2, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_14': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 3, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_15': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_16': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 5, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_17': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 6, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_18': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 7, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_19': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 8, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_110': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 9, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_111': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 10, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_112': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 11, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_113': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 12, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_114': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 13, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_115': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 14, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_116': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 15, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_117': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 16, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_118': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 17, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_119': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 18, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_120': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 19, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_121': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_122': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_123': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 2, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_124': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_125': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 6, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_126': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 17, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_127': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_128': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 2, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_129': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 3, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_130': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_131': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 5, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_132': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 7, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_133': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_134': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 3, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_135': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_136': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 5, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_137': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 7, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_138': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 11, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_139': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 13, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_140': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 14, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_141': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'multiStateInput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
-              '6_4_1_analogValue_142': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.172', 'point_type': 'multiStateOutput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+    points = {'6_4_1_analogValue_1': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_12': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_13': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 2, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_14': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 3, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_15': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_16': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 5, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_17': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 6, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_18': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 7, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_19': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 8, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_110': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 9, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_111': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 10, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_112': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 11, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_113': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 12, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_114': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 13, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_115': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 14, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_116': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 15, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_117': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 16, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_118': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 17, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_119': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 18, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_120': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogInput', 'point_property': 'presentValue', 'point_address': 19, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_121': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_122': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_123': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 2, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_124': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_125': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 6, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_126': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'analogOutput', 'point_property': 'presentValue', 'point_address': 17, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_127': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_128': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 2, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_129': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 3, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_130': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_131': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 5, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_132': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryInput', 'point_property': 'presentValue', 'point_address': 7, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_133': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 1, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_134': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 3, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_135': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 4, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_136': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 5, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_137': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 7, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_138': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 11, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_139': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 13, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_140': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'binaryOutput', 'point_property': 'presentValue', 'point_address': 14, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_141': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'multiStateInput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
+              '6_4_1_analogValue_142': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True', 'point_device_address': '192.168.1.184', 'point_type': 'multiStateOutput', 'point_property': 'presentValue', 'point_address': 0, 'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
               }
 
-    client = IOTBacnet(tag='192.168.1.17/24:47808', configs=dict_config, points= dict_point1)
+    client = IOTBacnet(tag='192.168.1.19/24:47808', configs=dict_config, points= points)
     client.logging(call_logging=logging_print)
     while True:
         try:
             # results = client.discover(retries=2)
 
             #results = client.scan(address='6:4/604/192.168.1.184')
             # results = client.scan()
@@ -162,15 +162,15 @@
     }
 
     dict_point = {'6_4_1_analogValue_1': {'point_name': '6_4_1_analogValue_1', 'index': 2, 'point_writable': 'True',
                                           'point_device_address': '6:2/602/192.168.1.184', 'point_type': 'analogValue',
                                           'point_property': 'presentValue', 'point_address': 1,
                                           'point_description': '', 'objectName': 'Random-604-1', 'presentValue': '1.0'},
                   '6_4_2_analogValue_2': {'point_name': '6_4_2_analogValue_2', 'index': 3, 'point_writable': 'True',
-                                          'point_device_address': '192.168.1.172', 'point_type': 'analogInput',
+                                          'point_device_address': '192.168.1.184', 'point_type': 'analogInput',
                                           'point_property': 'presentValue', 'point_address': 3,
                                           'point_description': '', 'objectName': 'Random-604-2', 'presentValue': '2.0'},
                   }
 
     client = IOTBacnet(configs=dict_config, points=dict_point)
     while True:
         try:
@@ -246,8 +246,8 @@
             time.sleep(1)
         count = len(results)
         results = client.discover()
 
     print('finish')
 
 
-test_address()
+test_driver()
```

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,29 +102,29 @@
     dict_config = {
         'multi_read': 100,  # 批量读取个数
         'cmd_interval': 0.3,  # 命令间隔
         'time_out': 5  # 超时时间
     }
     # 点表
     dict_point = {}
-    dict_point['signed'] = {'point_writable': True, 'point_name': 'signed', 'point_device_address': '192.168.1.184/502',  'point_slave_id': 2, 'point_fun_code': 3, 'point_address': 0, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
-    dict_point['unsigned'] = {'point_writable': True, 'point_name': 'unsigned', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 1, 'point_data_type': 6, 'point_data_length': 1, 'point_scale': '1'}
-    dict_point['bit'] = {'point_writable': True, 'point_name': 'bit', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 2, 'point_data_type': 8, 'point_data_length': 1, 'point_scale': '1'}
-    dict_point['long'] = {'point_writable': True, 'point_name': 'long', 'point_device_address': '192.168.1.184/502',  'point_slave_id': 2, 'point_fun_code': 3, 'point_address': 4, 'point_data_type': 12, 'point_data_length': 2, 'point_scale':'1'}
-    dict_point['long_rev'] = {'point_writable': True, 'point_name': 'long_rev', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 6, 'point_data_type': 12, 'point_data_order': 2, 'point_data_length': 2, 'point_scale': '1'}
-    dict_point['float'] = {'point_writable': True, 'point_name': 'float', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 10, 'point_data_type': 18, 'point_data_length': 2, 'point_scale': '1'}
-    dict_point['float_rev'] = {'point_writable': True, 'point_name': 'float_rev', 'point_device_address': '192.168.1.184/502',  'point_slave_id': 2, 'point_fun_code': 3, 'point_address': 12, 'point_data_type': 18, 'point_data_order': 2, 'point_data_length': 2, 'point_scale':'1'}
-    dict_point['double'] = {'point_writable': True, 'point_name': 'double', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 16, 'point_data_type': 20, 'point_data_length': 4, 'point_scale': '1'}
-    dict_point['double_rev'] = {'point_writable': True, 'point_name': 'double_rev', 'point_device_address': '192.168.1.184/502', 'point_slave_id': 2,'point_fun_code': 3, 'point_address': 24, 'point_data_type': 20, 'point_data_order': 2, 'point_data_length': 4, 'point_scale': '1'}
+    dict_point['signed'] = {'point_writable': True, 'point_name': 'signed', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 1, 'point_fun_code': 3, 'point_address': 0, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'v+3'}
+    dict_point['unsigned'] = {'point_writable': True, 'point_name': 'unsigned', 'point_device_address': '127.0.0.1/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 1, 'point_data_type': 6, 'point_data_length': 1, 'point_scale': '1'}
+    dict_point['bit'] = {'point_writable': True, 'point_name': 'bit', 'point_device_address': '127.0.0.1/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 2, 'point_data_type': 8, 'point_data_length': 1, 'point_scale': '1'}
+    dict_point['long'] = {'point_writable': True, 'point_name': 'long', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 1, 'point_fun_code': 3, 'point_address': 4, 'point_data_type': 12, 'point_data_length': 2, 'point_scale':'1'}
+    dict_point['long_rev'] = {'point_writable': True, 'point_name': 'long_rev', 'point_device_address': '127.0.0.1/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 6, 'point_data_type': 12, 'point_data_order': 2, 'point_data_length': 2, 'point_scale': '1'}
+    dict_point['float'] = {'point_writable': True, 'point_name': 'float', 'point_device_address': '127.0.0.1/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 10, 'point_data_type': 18, 'point_data_length': 2, 'point_scale': '1'}
+    dict_point['float_rev'] = {'point_writable': True, 'point_name': 'float_rev', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 1, 'point_fun_code': 3, 'point_address': 12, 'point_data_type': 18, 'point_data_order': 2, 'point_data_length': 2, 'point_scale':'1'}
+    dict_point['double'] = {'point_writable': True, 'point_name': 'double', 'point_device_address': '127.0.0.1/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 16, 'point_data_type': 20, 'point_data_length': 4, 'point_scale': '1'}
+    dict_point['double_rev'] = {'point_writable': True, 'point_name': 'double_rev', 'point_device_address': '127.0.0.1/502', 'point_slave_id': 1,'point_fun_code': 3, 'point_address': 24, 'point_data_type': 20, 'point_data_order': 2, 'point_data_length': 4, 'point_scale': '1'}
 
     modbus_driver = IOTModbus(configs=dict_config, points=dict_point)
     modbus_driver.logging(call_logging=logging_print)
     # 轮询全部
     while True:
-        dict_result_scrap = modbus_driver.write(values={'double_rev': -123.45, 'double': 1})
+        dict_result_scrap = modbus_driver.write(values={'signed': 1.0})
         time.sleep(2)
 
 
 def test_smiluate():
     #配置项
     dict_config = {
                         'cmd_interval': 0.3,                         # 命令间隔
@@ -148,9 +148,9 @@
     while True:
         #for name, point in dict_point.items():
         #    point['point_value'] = random.randint(1, 100)
         client.simulate(points=dict_point)
         time.sleep(10)
 
 
-test_read2()
+test_write()
```

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,30 @@
             re = client.read()
             print(re)
         except Exception as e:
             print(f"error: {e.__str__()}")
         time.sleep(4)
 
 
-test_read1()
+def test_read2():
+    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'send_timeout': 15, 'rec_timeout': 3500, 'library': r'D:\UM\code\core\snap7.dll'}
+    dict_point = {}
+    dict_point['plc1'] = {'point_writable': True, 'point_name': 'plc1', 'point_device_address': '127.0.0.1/102/0/1', 'point_address': 'DB1,BYTE24', 'point_scale': '1'}
+    dict_point['plc11'] = {'point_writable': True, 'point_name': 'plc11', 'point_device_address': '127.0.0.1/102/0/1', 'point_address': 'DB1,BYTE25', 'point_scale': '1'}
+    dict_point['plc2'] = {'point_writable': True, 'point_name': 'plc2', 'point_device_address': '127.0.0.1/102/0/1', 'point_address': 'DB1,INT24', 'point_scale': '1'}
+    dict_point['plc31'] = {'point_writable': True, 'point_name': 'plc31', 'point_device_address': '127.0.0.1/102/0/1', 'point_address': 'DB1,X24.1', 'point_scale': '1'}
+    dict_point['plc3'] = {'point_writable': True, 'point_name': 'plc3', 'point_device_address': '127.0.0.1/102/0/1', 'point_address': 'DB1,X24.2', 'point_scale': '1'}
+
+    client = IOTPlcS7(configs=dict_config, points=dict_point)
+    client.logging(call_logging=logging_print)
+    while True:
+        try:
+            re = client.read()
+            print(re)
+            client.write(values={'plc3': 1})
+            print(client.read())
+        except Exception as e:
+            print(f"error: {e.__str__()}")
+        time.sleep(4)
+
+
+test_read2()
```

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.41/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*


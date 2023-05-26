# Comparing `tmp/tb-paho-mqtt-client-1.6.2.tar.gz` & `tmp/tb-paho-mqtt-client-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb-paho-mqtt-client-1.6.2.tar", last modified: Thu Mar 23 13:17:10 2023, max compression
+gzip compressed data, was "tb-paho-mqtt-client-1.6.3.tar", last modified: Fri May 26 13:35:43 2023, max compression
```

## Comparing `tb-paho-mqtt-client-1.6.2.tar` & `tb-paho-mqtt-client-1.6.3.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-03-23 13:17:10.763092 tb-paho-mqtt-client-1.6.2/
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     4006 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/CONTRIBUTING.md
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)      156 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/LICENSE.txt
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)      203 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/MANIFEST.in
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1219 2023-03-23 13:17:10.763167 tb-paho-mqtt-client-1.6.2/PKG-INFO
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)    46471 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/README.rst
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     2030 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/about.html
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1569 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/edl-v10
-drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-03-23 13:17:10.758484 tb-paho-mqtt-client-1.6.2/examples/
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     4247 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/aws_iot.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1087 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_logger.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3118 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_mqtt_clear_retain.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1753 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_pub-wait.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     4153 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_pub_opts.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     2968 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_rpc_math.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1692 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_session_present.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1642 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_sub-class.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1827 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_sub-multiple-callback.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1689 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_sub-srv.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1610 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_sub-ws.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1605 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_sub.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3659 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/client_sub_opts.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      657 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/context.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3454 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/loop_asyncio.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     2484 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/loop_select.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3001 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/loop_trio.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      781 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/publish_multiple.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      684 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/publish_single.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      754 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/publish_utf8-27.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      793 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/publish_utf8-3.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     2870 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/server_rpc_math.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      785 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/subscribe_callback.py
--rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      774 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/examples/subscribe_simple.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     9230 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/notice.html
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1340 2023-03-23 13:17:07.000000 tb-paho-mqtt-client-1.6.2/pyproject.toml
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)      160 2023-03-23 13:17:10.763393 tb-paho-mqtt-client-1.6.2/setup.cfg
-drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-03-23 13:17:10.752583 tb-paho-mqtt-client-1.6.2/src/
-drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-03-23 13:17:10.758620 tb-paho-mqtt-client-1.6.2/src/paho/
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)        0 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/__init__.py
-drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-03-23 13:17:10.760427 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)       65 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/__init__.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)   154674 2023-03-15 07:59:20.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/client.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     2771 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/matcher.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1453 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/packettypes.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)    17815 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/properties.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     9624 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/publish.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     8591 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/reasoncodes.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)    11382 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/subscribe.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     4616 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.2/src/paho/mqtt/subscribeoptions.py
-drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-03-23 13:17:10.760978 tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1219 2023-03-23 13:17:10.000000 tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/PKG-INFO
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1399 2023-03-23 13:17:10.000000 tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/SOURCES.txt
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)        1 2023-03-23 13:17:10.000000 tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/dependency_links.txt
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)       45 2023-03-23 13:17:10.000000 tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/requires.txt
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)        5 2023-03-23 13:17:10.000000 tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/top_level.txt
-drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-03-23 13:17:10.762859 tb-paho-mqtt-client-1.6.2/tests/
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)    11537 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.2/tests/test_client.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1006 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.2/tests/test_matcher.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)    57457 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.2/tests/test_mqttv5.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     8534 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.2/tests/test_websocket_integration.py
--rw-r--r--   0 vitaliibidochka   (501) staff       (20)     2160 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.2/tests/test_websockets.py
+drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-05-26 13:35:43.664730 tb-paho-mqtt-client-1.6.3/
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     4006 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/CONTRIBUTING.md
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)      156 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/LICENSE.txt
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)      203 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/MANIFEST.in
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1144 2023-05-26 13:35:43.664792 tb-paho-mqtt-client-1.6.3/PKG-INFO
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)    46471 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/README.rst
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     2030 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/about.html
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1569 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/edl-v10
+drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-05-26 13:35:43.660281 tb-paho-mqtt-client-1.6.3/examples/
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     4247 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/aws_iot.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1087 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_logger.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3118 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_mqtt_clear_retain.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1753 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_pub-wait.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     4153 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_pub_opts.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     2968 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_rpc_math.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1692 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_session_present.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1642 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_sub-class.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1827 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_sub-multiple-callback.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1689 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_sub-srv.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1610 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_sub-ws.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     1605 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_sub.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3659 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/client_sub_opts.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      657 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/context.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3454 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/loop_asyncio.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     2484 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/loop_select.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     3001 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/loop_trio.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      781 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/publish_multiple.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      684 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/publish_single.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      754 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/publish_utf8-27.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      793 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/publish_utf8-3.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)     2870 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/server_rpc_math.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      849 2023-05-26 13:11:57.000000 tb-paho-mqtt-client-1.6.3/examples/subscribe_callback.py
+-rwxr-xr-x   0 vitaliibidochka   (501) staff       (20)      774 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/examples/subscribe_simple.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     9230 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/notice.html
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)      160 2023-05-26 13:35:43.665184 tb-paho-mqtt-client-1.6.3/setup.cfg
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1897 2023-05-26 13:35:08.000000 tb-paho-mqtt-client-1.6.3/setup.py
+drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-05-26 13:35:43.654287 tb-paho-mqtt-client-1.6.3/src/
+drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-05-26 13:35:43.660419 tb-paho-mqtt-client-1.6.3/src/paho/
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)        0 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/src/paho/__init__.py
+drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-05-26 13:35:43.662517 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)       65 2023-05-26 13:35:40.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/__init__.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)   154710 2023-05-26 13:11:53.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/client.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     2771 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/matcher.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1453 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/packettypes.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)    17815 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/properties.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     9624 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/publish.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     8591 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/reasoncodes.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)    11382 2023-03-15 07:47:32.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/subscribe.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     4616 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.3/src/paho/mqtt/subscribeoptions.py
+drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-05-26 13:35:43.663314 tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1144 2023-05-26 13:35:43.000000 tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/PKG-INFO
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1439 2023-05-26 13:35:43.000000 tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)        1 2023-05-26 13:35:43.000000 tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)        1 2023-05-26 13:23:18.000000 tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/not-zip-safe
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)       17 2023-05-26 13:35:43.000000 tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/requires.txt
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)        5 2023-05-26 13:35:43.000000 tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/top_level.txt
+drwxr-xr-x   0 vitaliibidochka   (501) staff       (20)        0 2023-05-26 13:35:43.664596 tb-paho-mqtt-client-1.6.3/tests/
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)    11537 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.3/tests/test_client.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     1006 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.3/tests/test_matcher.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)    57457 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.3/tests/test_mqttv5.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     8534 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.3/tests/test_websocket_integration.py
+-rw-r--r--   0 vitaliibidochka   (501) staff       (20)     2160 2023-03-15 07:47:33.000000 tb-paho-mqtt-client-1.6.3/tests/test_websockets.py
```

### Comparing `tb-paho-mqtt-client-1.6.2/CONTRIBUTING.md` & `tb-paho-mqtt-client-1.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/PKG-INFO` & `tb-paho-mqtt-client-1.6.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: tb-paho-mqtt-client
-Version: 1.6.2
-Summary: Fork of with critical bug fixed.
-Author-email: Samsonov <vbidochka@thingsboard.io>
-Project-URL: Homepage, https://github.com/samson0v/paho.mqtt.python
-Project-URL: Bug Tracker, https://github.com/eclipse/paho.mqtt.python/issues
+Version: 1.6.3
+Summary: MQTT version 5.0/3.1.1 client class
+Home-page: http://eclipse.org/paho
+Author: Samsonov
+Author-email: vbidochka@thingsboard.io
+License: Eclipse Public License v2.0 / Eclipse Distribution License v1.0
+Keywords: paho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
@@ -19,11 +21,9 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: proxy
 License-File: LICENSE.txt
```

### Comparing `tb-paho-mqtt-client-1.6.2/README.rst` & `tb-paho-mqtt-client-1.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/about.html` & `tb-paho-mqtt-client-1.6.3/about.html`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/edl-v10` & `tb-paho-mqtt-client-1.6.3/edl-v10`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/aws_iot.py` & `tb-paho-mqtt-client-1.6.3/examples/aws_iot.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_logger.py` & `tb-paho-mqtt-client-1.6.3/examples/client_logger.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_mqtt_clear_retain.py` & `tb-paho-mqtt-client-1.6.3/examples/client_mqtt_clear_retain.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_pub-wait.py` & `tb-paho-mqtt-client-1.6.3/examples/client_pub-wait.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_pub_opts.py` & `tb-paho-mqtt-client-1.6.3/examples/client_pub_opts.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_rpc_math.py` & `tb-paho-mqtt-client-1.6.3/examples/client_rpc_math.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_session_present.py` & `tb-paho-mqtt-client-1.6.3/examples/client_session_present.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_sub-class.py` & `tb-paho-mqtt-client-1.6.3/examples/client_sub-class.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_sub-multiple-callback.py` & `tb-paho-mqtt-client-1.6.3/examples/client_sub-multiple-callback.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_sub-srv.py` & `tb-paho-mqtt-client-1.6.3/examples/client_sub-srv.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_sub-ws.py` & `tb-paho-mqtt-client-1.6.3/examples/client_sub-ws.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_sub.py` & `tb-paho-mqtt-client-1.6.3/examples/client_sub.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/client_sub_opts.py` & `tb-paho-mqtt-client-1.6.3/examples/client_sub_opts.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/context.py` & `tb-paho-mqtt-client-1.6.3/examples/context.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/loop_asyncio.py` & `tb-paho-mqtt-client-1.6.3/examples/loop_asyncio.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/loop_select.py` & `tb-paho-mqtt-client-1.6.3/examples/loop_select.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/loop_trio.py` & `tb-paho-mqtt-client-1.6.3/examples/loop_trio.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/publish_multiple.py` & `tb-paho-mqtt-client-1.6.3/examples/publish_multiple.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/publish_single.py` & `tb-paho-mqtt-client-1.6.3/examples/publish_single.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/publish_utf8-27.py` & `tb-paho-mqtt-client-1.6.3/examples/publish_utf8-27.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/publish_utf8-3.py` & `tb-paho-mqtt-client-1.6.3/examples/publish_utf8-3.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/server_rpc_math.py` & `tb-paho-mqtt-client-1.6.3/examples/server_rpc_math.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/examples/subscribe_callback.py` & `tb-paho-mqtt-client-1.6.3/examples/subscribe_callback.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,11 +16,16 @@
 # This shows an example of using the subscribe.callback helper function.
 
 import context  # Ensures paho is in PYTHONPATH
 
 import paho.mqtt.subscribe as subscribe
 
 
-def print_msg(client, userdata, message):
-    print("%s : %s" % (message.topic, message.payload))
+def main():
+    def print_msg(client, userdata, message):
+        print("%s : %s" % (message.topic, message.payload))
 
-subscribe.callback(print_msg, "#", hostname="mqtt.eclipseprojects.io")
+    subscribe.callback(print_msg, "#", hostname="mqtt.eclipseprojects.io")
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `tb-paho-mqtt-client-1.6.2/examples/subscribe_simple.py` & `tb-paho-mqtt-client-1.6.3/examples/subscribe_simple.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/notice.html` & `tb-paho-mqtt-client-1.6.3/notice.html`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/client.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -622,14 +622,15 @@
         self._on_publish = None
         self._on_unsubscribe = None
         self._on_disconnect = None
         self._on_socket_open = None
         self._on_socket_close = None
         self._on_socket_register_write = None
         self._on_socket_unregister_write = None
+        self._on_pre_connect = None
         self._websocket_path = "/mqtt"
         self._websocket_extra_headers = None
         # for clean_start == MQTT_CLEAN_START_FIRST_ONLY
         self._mqttv5_first_connect = True
         self.suppress_exceptions = False # For callbacks
 
     def __del__(self):
```

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/matcher.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/matcher.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/packettypes.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/packettypes.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/properties.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/properties.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/publish.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/publish.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/reasoncodes.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/reasoncodes.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/subscribe.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/subscribe.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/paho/mqtt/subscribeoptions.py` & `tb-paho-mqtt-client-1.6.3/src/paho/mqtt/subscribeoptions.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/PKG-INFO` & `tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: tb-paho-mqtt-client
-Version: 1.6.2
-Summary: Fork of with critical bug fixed.
-Author-email: Samsonov <vbidochka@thingsboard.io>
-Project-URL: Homepage, https://github.com/samson0v/paho.mqtt.python
-Project-URL: Bug Tracker, https://github.com/eclipse/paho.mqtt.python/issues
+Version: 1.6.3
+Summary: MQTT version 5.0/3.1.1 client class
+Home-page: http://eclipse.org/paho
+Author: Samsonov
+Author-email: vbidochka@thingsboard.io
+License: Eclipse Public License v2.0 / Eclipse Distribution License v1.0
+Keywords: paho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
@@ -19,11 +21,9 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: proxy
 License-File: LICENSE.txt
```

### Comparing `tb-paho-mqtt-client-1.6.2/src/tb_paho_mqtt_client.egg-info/SOURCES.txt` & `tb-paho-mqtt-client-1.6.3/src/tb_paho_mqtt_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 README.rst
 about.html
 edl-v10
 notice.html
-pyproject.toml
 setup.cfg
+setup.py
 examples/aws_iot.py
 examples/client_logger.py
 examples/client_mqtt_clear_retain.py
 examples/client_pub-wait.py
 examples/client_pub_opts.py
 examples/client_rpc_math.py
 examples/client_session_present.py
@@ -40,14 +40,15 @@
 src/paho/mqtt/publish.py
 src/paho/mqtt/reasoncodes.py
 src/paho/mqtt/subscribe.py
 src/paho/mqtt/subscribeoptions.py
 src/tb_paho_mqtt_client.egg-info/PKG-INFO
 src/tb_paho_mqtt_client.egg-info/SOURCES.txt
 src/tb_paho_mqtt_client.egg-info/dependency_links.txt
+src/tb_paho_mqtt_client.egg-info/not-zip-safe
 src/tb_paho_mqtt_client.egg-info/requires.txt
 src/tb_paho_mqtt_client.egg-info/top_level.txt
 tests/test_client.py
 tests/test_matcher.py
 tests/test_mqttv5.py
 tests/test_websocket_integration.py
 tests/test_websockets.py
```

### Comparing `tb-paho-mqtt-client-1.6.2/tests/test_client.py` & `tb-paho-mqtt-client-1.6.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/tests/test_matcher.py` & `tb-paho-mqtt-client-1.6.3/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/tests/test_mqttv5.py` & `tb-paho-mqtt-client-1.6.3/tests/test_mqttv5.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/tests/test_websocket_integration.py` & `tb-paho-mqtt-client-1.6.3/tests/test_websocket_integration.py`

 * *Files identical despite different names*

### Comparing `tb-paho-mqtt-client-1.6.2/tests/test_websockets.py` & `tb-paho-mqtt-client-1.6.3/tests/test_websockets.py`

 * *Files identical despite different names*


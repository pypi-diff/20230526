# Comparing `tmp/rosrestpy-0.6.1.tar.gz` & `tmp/rosrestpy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosrestpy-0.6.1.tar", max compression
+gzip compressed data, was "rosrestpy-0.7.0.tar", max compression
```

## Comparing `rosrestpy-0.6.1.tar` & `rosrestpy-0.7.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
--rw-r--r--   0        0        0    35149 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/LICENSE
--rw-r--r--   0        0        0     2269 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/README.md
--rw-r--r--   0        0        0     1221 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      553 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/__init__.py
--rw-r--r--   0        0        0     2605 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/_base.py
--rw-r--r--   0        0        0     4631 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/_literals.py
--rw-r--r--   0        0        0     1290 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/_utils.py
--rw-r--r--   0        0        0      301 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/error.py
--rw-r--r--   0        0        0     1617 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/__init__.py
--rw-r--r--   0        0        0     1002 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/bridge/__init__.py
--rw-r--r--   0        0        0      686 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/bridge/bridge.py
--rw-r--r--   0        0        0      262 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/bridge/msti.py
--rw-r--r--   0        0        0      763 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/bridge/port.py
--rw-r--r--   0        0        0      322 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/bridge/vlan.py
--rw-r--r--   0        0        0     1931 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/ethernet.py
--rw-r--r--   0        0        0      754 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/interface.py
--rw-r--r--   0        0        0      572 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/list/__init__.py
--rw-r--r--   0        0        0      244 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/list/list.py
--rw-r--r--   0        0        0      246 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/inteface/list/member.py
--rw-r--r--   0        0        0     2477 2023-04-04 17:33:29.128167 rosrestpy-0.6.1/ros/ip/__init__.py
--rw-r--r--   0        0        0      392 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/address.py
--rw-r--r--   0        0        0      544 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/arp.py
--rw-r--r--   0        0        0      278 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/cloud.py
--rw-r--r--   0        0        0     1245 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dhcp_client.py
--rw-r--r--   0        0        0      470 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dhcp_relay.py
--rw-r--r--   0        0        0      771 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dhcp_server/__init__.py
--rw-r--r--   0        0        0      153 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dhcp_server/_literals.py
--rw-r--r--   0        0        0     1100 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dhcp_server/dhcp_server.py
--rw-r--r--   0        0        0     1383 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dhcp_server/lease.py
--rw-r--r--   0        0        0      423 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dhcp_server/network.py
--rw-r--r--   0        0        0     1032 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dns/__init__.py
--rw-r--r--   0        0        0      126 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dns/_literals.py
--rw-r--r--   0        0        0      195 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dns/cache.py
--rw-r--r--   0        0        0      626 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/dns/static.py
--rw-r--r--   0        0        0     1472 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/firewall/__init__.py
--rw-r--r--   0        0        0      282 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/firewall/_literals.py
--rw-r--r--   0        0        0      748 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/firewall/connection.py
--rw-r--r--   0        0        0     2703 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/firewall/filter.py
--rw-r--r--   0        0        0     2978 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/firewall/mangle.py
--rw-r--r--   0        0        0     2381 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/firewall/nat.py
--rw-r--r--   0        0        0     1042 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/route.py
--rw-r--r--   0        0        0      565 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ip/setting.py
--rw-r--r--   0        0        0      181 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/log.py
--rw-r--r--   0        0        0      744 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ppp/__init__.py
--rw-r--r--   0        0        0      220 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ppp/_literals.py
--rw-r--r--   0        0        0      160 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ppp/aaa.py
--rw-r--r--   0        0        0     1147 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ppp/profile.py
--rw-r--r--   0        0        0      640 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ppp/secret.py
--rw-r--r--   0        0        0      826 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/queue/__init__.py
--rw-r--r--   0        0        0      153 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/queue/interface.py
--rw-r--r--   0        0        0     2076 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/queue/simple.py
--rw-r--r--   0        0        0      726 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/queue/tree.py
--rw-r--r--   0        0        0     7146 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/ros.py
--rw-r--r--   0        0        0      604 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/routing/__init__.py
--rw-r--r--   0        0        0      467 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/routing/rule.py
--rw-r--r--   0        0        0      334 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/routing/table.py
--rw-r--r--   0        0        0     2407 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/__init__.py
--rw-r--r--   0        0        0      123 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/health.py
--rw-r--r--   0        0        0      214 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/history.py
--rw-r--r--   0        0        0      126 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/identity.py
--rw-r--r--   0        0        0      122 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/license.py
--rw-r--r--   0        0        0      248 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/logging.py
--rw-r--r--   0        0        0      146 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/note.py
--rw-r--r--   0        0        0      580 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/package/__init__.py
--rw-r--r--   0        0        0      101 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/package/_literals.py
--rw-r--r--   0        0        0      297 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/package/package.py
--rw-r--r--   0        0        0      774 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/package/update.py
--rw-r--r--   0        0        0      460 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/resource.py
--rw-r--r--   0        0        0      232 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/system/routerboard.py
--rw-r--r--   0        0        0     6460 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/tool/__init__.py
--rw-r--r--   0        0        0      223 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/tool/bandwith_server.py
--rw-r--r--   0        0        0      546 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/tool/bandwith_test.py
--rw-r--r--   0        0        0      158 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/tool/ip_scan.py
--rw-r--r--   0        0        0      236 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/tool/ping.py
--rw-r--r--   0        0        0      416 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/tool/torch.py
--rw-r--r--   0        0        0      290 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/tool/traceroute.py
--rw-r--r--   0        0        0     1746 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/user/__init__.py
--rw-r--r--   0        0        0      168 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/user/aaa.py
--rw-r--r--   0        0        0      167 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/user/active.py
--rw-r--r--   0        0        0      188 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/user/group.py
--rw-r--r--   0        0        0      129 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/user/settings.py
--rw-r--r--   0        0        0      205 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/user/ssh_keys.py
--rw-r--r--   0        0        0      249 2023-04-04 17:33:29.132167 rosrestpy-0.6.1/ros/user/user.py
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 rosrestpy-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2269 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/README.md
+-rw-r--r--   0        0        0     1222 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      553 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/__init__.py
+-rw-r--r--   0        0        0     2605 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/_base.py
+-rw-r--r--   0        0        0     4631 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/_literals.py
+-rw-r--r--   0        0        0     1290 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/_utils.py
+-rw-r--r--   0        0        0      301 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/error.py
+-rw-r--r--   0        0        0     1617 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/__init__.py
+-rw-r--r--   0        0        0     1002 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/bridge/__init__.py
+-rw-r--r--   0        0        0      686 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/bridge/bridge.py
+-rw-r--r--   0        0        0      262 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/bridge/msti.py
+-rw-r--r--   0        0        0      763 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/bridge/port.py
+-rw-r--r--   0        0        0      322 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/bridge/vlan.py
+-rw-r--r--   0        0        0     1931 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/ethernet.py
+-rw-r--r--   0        0        0      754 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/interface.py
+-rw-r--r--   0        0        0      572 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/list/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/list/list.py
+-rw-r--r--   0        0        0      246 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/inteface/list/member.py
+-rw-r--r--   0        0        0     2477 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/address.py
+-rw-r--r--   0        0        0      544 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/arp.py
+-rw-r--r--   0        0        0      278 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/cloud.py
+-rw-r--r--   0        0        0     1245 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dhcp_client.py
+-rw-r--r--   0        0        0      470 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dhcp_relay.py
+-rw-r--r--   0        0        0      771 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dhcp_server/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dhcp_server/_literals.py
+-rw-r--r--   0        0        0     1100 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dhcp_server/dhcp_server.py
+-rw-r--r--   0        0        0     1383 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dhcp_server/lease.py
+-rw-r--r--   0        0        0      423 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dhcp_server/network.py
+-rw-r--r--   0        0        0     1032 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dns/__init__.py
+-rw-r--r--   0        0        0      126 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dns/_literals.py
+-rw-r--r--   0        0        0      195 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dns/cache.py
+-rw-r--r--   0        0        0      626 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/dns/static.py
+-rw-r--r--   0        0        0     1472 2023-05-26 08:10:07.129279 rosrestpy-0.7.0/ros/ip/firewall/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ip/firewall/_literals.py
+-rw-r--r--   0        0        0      748 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ip/firewall/connection.py
+-rw-r--r--   0        0        0     2703 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ip/firewall/filter.py
+-rw-r--r--   0        0        0     2978 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ip/firewall/mangle.py
+-rw-r--r--   0        0        0     2381 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ip/firewall/nat.py
+-rw-r--r--   0        0        0     1042 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ip/route.py
+-rw-r--r--   0        0        0      565 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ip/setting.py
+-rw-r--r--   0        0        0      181 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/log.py
+-rw-r--r--   0        0        0      744 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ppp/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ppp/_literals.py
+-rw-r--r--   0        0        0      160 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ppp/aaa.py
+-rw-r--r--   0        0        0     1147 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ppp/profile.py
+-rw-r--r--   0        0        0      640 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ppp/secret.py
+-rw-r--r--   0        0        0      826 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/queue/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/queue/interface.py
+-rw-r--r--   0        0        0     2076 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/queue/simple.py
+-rw-r--r--   0        0        0      726 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/queue/tree.py
+-rw-r--r--   0        0        0     7146 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/ros.py
+-rw-r--r--   0        0        0      604 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/routing/__init__.py
+-rw-r--r--   0        0        0      467 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/routing/rule.py
+-rw-r--r--   0        0        0      334 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/routing/table.py
+-rw-r--r--   0        0        0     2407 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/health.py
+-rw-r--r--   0        0        0      214 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/history.py
+-rw-r--r--   0        0        0      126 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/identity.py
+-rw-r--r--   0        0        0      122 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/license.py
+-rw-r--r--   0        0        0      248 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/logging.py
+-rw-r--r--   0        0        0      146 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/note.py
+-rw-r--r--   0        0        0      580 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/package/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/package/_literals.py
+-rw-r--r--   0        0        0      297 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/package/package.py
+-rw-r--r--   0        0        0      774 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/package/update.py
+-rw-r--r--   0        0        0      460 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/resource.py
+-rw-r--r--   0        0        0      232 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/system/routerboard.py
+-rw-r--r--   0        0        0     6722 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/bandwith_server.py
+-rw-r--r--   0        0        0      546 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/bandwith_test.py
+-rw-r--r--   0        0        0      158 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/ip_scan.py
+-rw-r--r--   0        0        0     1042 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/netwatch.py
+-rw-r--r--   0        0        0      236 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/ping.py
+-rw-r--r--   0        0        0      416 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/torch.py
+-rw-r--r--   0        0        0      290 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/tool/traceroute.py
+-rw-r--r--   0        0        0     1746 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/user/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/user/aaa.py
+-rw-r--r--   0        0        0      167 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/user/active.py
+-rw-r--r--   0        0        0      188 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/user/group.py
+-rw-r--r--   0        0        0      129 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/user/settings.py
+-rw-r--r--   0        0        0      205 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/user/ssh_keys.py
+-rw-r--r--   0        0        0      249 2023-05-26 08:10:07.133278 rosrestpy-0.7.0/ros/user/user.py
+-rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 rosrestpy-0.7.0/PKG-INFO
```

### Comparing `rosrestpy-0.6.1/LICENSE` & `rosrestpy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/README.md` & `rosrestpy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/pyproject.toml` & `rosrestpy-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rosrestpy"
-version = "0.6.1"
+version = "0.7.0"
 description = "RouterOS v7 REST API python module"
 authors = ["hexatester <hexatester@protonmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/hexatester/rosrestpy"
 packages = [
     { include = "ros" },
@@ -21,17 +21,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 attrs = ">=21.0.0,<=23.0.0"
-requests = "^2.28.1"
 cattrs = ">=21.0.0,<=23.0.0"
 ujson = {version = "^5.5.0", optional = true}
+requests = ">=2.31.0"
 
 [tool.poetry.extras]
 ujson = ["ujson"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 mypy = "^0.961"
```

### Comparing `rosrestpy-0.6.1/ros/__init__.py` & `rosrestpy-0.7.0/ros/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 from .inteface import InterfaceModule
 from .ip import IPModule
 from .ppp import PPPModule
 from .queue import QueueModule
 from .routing import RoutingModule
 from .system import SystemModule
 from .tool import ToolModule
```

### Comparing `rosrestpy-0.6.1/ros/_base.py` & `rosrestpy-0.7.0/ros/_base.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/_literals.py` & `rosrestpy-0.7.0/ros/_literals.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/_utils.py` & `rosrestpy-0.7.0/ros/_utils.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/inteface/__init__.py` & `rosrestpy-0.7.0/ros/inteface/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/inteface/bridge/__init__.py` & `rosrestpy-0.7.0/ros/inteface/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/inteface/bridge/bridge.py` & `rosrestpy-0.7.0/ros/inteface/bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/inteface/bridge/port.py` & `rosrestpy-0.7.0/ros/inteface/bridge/port.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/inteface/ethernet.py` & `rosrestpy-0.7.0/ros/inteface/ethernet.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/inteface/interface.py` & `rosrestpy-0.7.0/ros/inteface/interface.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/inteface/list/__init__.py` & `rosrestpy-0.7.0/ros/inteface/list/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/__init__.py` & `rosrestpy-0.7.0/ros/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/arp.py` & `rosrestpy-0.7.0/ros/ip/arp.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/dhcp_client.py` & `rosrestpy-0.7.0/ros/ip/dhcp_client.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/dhcp_server/__init__.py` & `rosrestpy-0.7.0/ros/ip/dhcp_server/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/dhcp_server/dhcp_server.py` & `rosrestpy-0.7.0/ros/ip/dhcp_server/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/dhcp_server/lease.py` & `rosrestpy-0.7.0/ros/ip/dhcp_server/lease.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/dns/__init__.py` & `rosrestpy-0.7.0/ros/ip/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/dns/static.py` & `rosrestpy-0.7.0/ros/ip/dns/static.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/firewall/__init__.py` & `rosrestpy-0.7.0/ros/ip/firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/firewall/connection.py` & `rosrestpy-0.7.0/ros/ip/firewall/connection.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/firewall/filter.py` & `rosrestpy-0.7.0/ros/ip/firewall/filter.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/firewall/mangle.py` & `rosrestpy-0.7.0/ros/ip/firewall/mangle.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/firewall/nat.py` & `rosrestpy-0.7.0/ros/ip/firewall/nat.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/route.py` & `rosrestpy-0.7.0/ros/ip/route.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ip/setting.py` & `rosrestpy-0.7.0/ros/ip/setting.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ppp/__init__.py` & `rosrestpy-0.7.0/ros/ppp/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ppp/profile.py` & `rosrestpy-0.7.0/ros/ppp/profile.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ppp/secret.py` & `rosrestpy-0.7.0/ros/ppp/secret.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/queue/__init__.py` & `rosrestpy-0.7.0/ros/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/queue/simple.py` & `rosrestpy-0.7.0/ros/queue/simple.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/queue/tree.py` & `rosrestpy-0.7.0/ros/queue/tree.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/ros.py` & `rosrestpy-0.7.0/ros/ros.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/routing/__init__.py` & `rosrestpy-0.7.0/ros/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/system/__init__.py` & `rosrestpy-0.7.0/ros/system/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/system/package/__init__.py` & `rosrestpy-0.7.0/ros/system/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/system/package/update.py` & `rosrestpy-0.7.0/ros/system/package/update.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/tool/__init__.py` & `rosrestpy-0.7.0/ros/tool/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import List, Literal, Union
 
-from ros._base import BaseModule
+from ros._base import BaseModule, BaseProps
 from ros._literals import AnyLiteral, IPProtocol, MACProtocol, PortLiteral
 
 from .bandwith_server import BandwithServer
 from .bandwith_test import BandwithTest
 from .ip_scan import IPScan
+from .netwatch import Netwatch
 from .ping import Ping
 from .torch import Torch
 from .traceroute import Traceroute
 
 
 class ToolModule(BaseModule):
+    _netwatch: BaseProps[Netwatch] = None
+
     @property
     def bandwith_server(self) -> BandwithServer:
         return self.ros.get_as(self.url + "/bandwidth-server", BandwithServer)
 
     def ping(
         self,
         address: str,
@@ -75,14 +78,20 @@
         data = {"interface": interface, "duration": duration}
         if address_range:
             data["address-range"] = address_range
         if freeze_frame_interval:
             data["freeze-frame-interval"] = freeze_frame_interval
         return self.ros.post_as(self.url + "/ip-scan", List[IPScan], data)
 
+    @property
+    def netwatch(self):
+        if not self._netwatch:
+            self._netwatch = BaseProps(self.ros, "/tool/netwatch", Netwatch)
+        return self._netwatch
+
     def torch(
         self,
         interface: str,
         duration: str = "5s",
         src_address: str = "0.0.0.0/0",
         dst_address: str = "0.0.0.0/0",
         src_address6: str = "::/0",
```

### Comparing `rosrestpy-0.6.1/ros/tool/bandwith_test.py` & `rosrestpy-0.7.0/ros/tool/bandwith_test.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/ros/user/__init__.py` & `rosrestpy-0.7.0/ros/user/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.6.1/PKG-INFO` & `rosrestpy-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosrestpy
-Version: 0.6.1
+Version: 0.7.0
 Summary: RouterOS v7 REST API python module
 Home-page: https://github.com/hexatester/rosrestpy
 License: GPL-3.0-only
 Author: hexatester
 Author-email: hexatester@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,23 +13,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Provides-Extra: ujson
 Requires-Dist: attrs (>=21.0.0,<=23.0.0)
 Requires-Dist: cattrs (>=21.0.0,<=23.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0)
 Requires-Dist: ujson (>=5.5.0,<6.0.0) ; extra == "ujson"
 Project-URL: Repository, https://github.com/hexatester/rosrestpy
 Description-Content-Type: text/markdown
 
 # RosRestPy
 
 [![PyPi Package Version](https://img.shields.io/pypi/v/rosrestpy)](https://pypi.org/project/rosrestpy/)
```


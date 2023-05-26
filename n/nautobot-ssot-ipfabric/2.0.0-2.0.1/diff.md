# Comparing `tmp/nautobot_ssot_ipfabric-2.0.0.tar.gz` & `tmp/nautobot_ssot_ipfabric-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_ssot_ipfabric-2.0.0.tar", max compression
+gzip compressed data, was "nautobot_ssot_ipfabric-2.0.1.tar", max compression
```

## Comparing `nautobot_ssot_ipfabric-2.0.0.tar` & `nautobot_ssot_ipfabric-2.0.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      591 2023-01-26 22:29:23.217019 nautobot_ssot_ipfabric-2.0.0/LICENSE
--rw-r--r--   0        0        0    12814 2023-01-26 22:29:23.217019 nautobot_ssot_ipfabric-2.0.0/README.md
--rw-r--r--   0        0        0     1348 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/__init__.py
--rw-r--r--   0        0        0      136 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/__init__.py
--rw-r--r--   0        0        0     7481 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py
--rw-r--r--   0        0        0    10108 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py
--rw-r--r--   0        0        0      522 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/adapters_shared.py
--rw-r--r--   0        0        0    19626 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/diffsync_models.py
--rw-r--r--   0        0        0    10597 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/jobs.py
--rw-r--r--   0        0        0     3063 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/signals.py
--rw-r--r--   0        0        0     4216 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric.png
--rw-r--r--   0        0        0    15558 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric_logo.png
--rw-r--r--   0        0        0       52 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/__init__.py
--rw-r--r--   0        0        0      477 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1545 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json
--rw-r--r--   0        0        0      985 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json
--rw-r--r--   0        0        0     1876 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json
--rw-r--r--   0        0        0     1639 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json
--rw-r--r--   0        0        0     3964 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py
--rw-r--r--   0        0        0     2989 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_jobs.py
--rw-r--r--   0        0        0     3522 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py
--rw-r--r--   0        0        0     5458 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_nbutils.py
--rw-r--r--   0        0        0      516 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/utilities/__init__.py
--rw-r--r--   0        0        0     9436 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/utilities/nbutils.py
--rw-r--r--   0        0        0      508 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/utilities/test_utils.py
--rw-r--r--   0        0        0     5361 2023-01-26 22:29:23.233020 nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/workers.py
--rw-r--r--   0        0        0     3177 2023-01-26 22:29:33.213149 nautobot_ssot_ipfabric-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    14321 1970-01-01 00:00:00.000000 nautobot_ssot_ipfabric-2.0.0/setup.py
--rw-r--r--   0        0        0    13854 1970-01-01 00:00:00.000000 nautobot_ssot_ipfabric-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-26 15:57:01.327861 nautobot_ssot_ipfabric-2.0.1/LICENSE
+-rw-r--r--   0        0        0    12814 2023-05-26 15:57:01.327861 nautobot_ssot_ipfabric-2.0.1/README.md
+-rw-r--r--   0        0        0     1348 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/__init__.py
+-rw-r--r--   0        0        0     7485 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py
+-rw-r--r--   0        0        0    10106 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py
+-rw-r--r--   0        0        0      522 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapters_shared.py
+-rw-r--r--   0        0        0    19626 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/diffsync_models.py
+-rw-r--r--   0        0        0    10621 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/jobs.py
+-rw-r--r--   0        0        0     3063 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/signals.py
+-rw-r--r--   0        0        0     8451 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric.png
+-rw-r--r--   0        0        0    11662 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/static/nautobot_ssot_ipfabric/ipfabric_logo.png
+-rw-r--r--   0        0        0       52 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/__init__.py
+-rw-r--r--   0        0        0      477 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1545 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json
+-rw-r--r--   0        0        0      985 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json
+-rw-r--r--   0        0        0     1876 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json
+-rw-r--r--   0        0        0     1639 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json
+-rw-r--r--   0        0        0     3964 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py
+-rw-r--r--   0        0        0     2989 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_jobs.py
+-rw-r--r--   0        0        0     3522 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py
+-rw-r--r--   0        0        0     5458 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nbutils.py
+-rw-r--r--   0        0        0      516 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/__init__.py
+-rw-r--r--   0        0        0     9440 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/nbutils.py
+-rw-r--r--   0        0        0      508 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/test_utils.py
+-rw-r--r--   0        0        0     5361 2023-05-26 15:57:01.343861 nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/workers.py
+-rw-r--r--   0        0        0     3177 2023-05-26 15:57:14.003926 nautobot_ssot_ipfabric-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13854 1970-01-01 00:00:00.000000 nautobot_ssot_ipfabric-2.0.1/PKG-INFO
```

### Comparing `nautobot_ssot_ipfabric-2.0.0/LICENSE` & `nautobot_ssot_ipfabric-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/README.md` & `nautobot_ssot_ipfabric-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/__init__.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_ipfabric.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         for iface in device_interfaces:
             ip_address = iface.get("primaryIp")
             try:
                 interface = self.interface(
                     diffsync=self,
                     name=iface.get("intName"),
                     device_name=iface.get("hostname"),
-                    description=iface.get("dscr"),
+                    description=iface.get("dscr", ""),
                     enabled=True,
                     mac_address=mac_to_format(iface.get("mac"), "MAC_COLON_TWO").upper()
                     if iface.get("mac")
                     else DEFAULT_INTERFACE_MAC,
                     mtu=iface.get("mtu") if iface.get("mtu") else DEFAULT_INTERFACE_MTU,
                     type=DEFAULT_INTERFACE_TYPE,
                     mgmt_only=iface.get("mgmt_only", False),
```

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapter_nautobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         for interface_record in device_record.interfaces.all():
             interface = self.interface(
                 diffsync=self,
                 status=device_record.status.name,
                 name=interface_record.name,
                 device_name=device_record.name,
-                description=interface_record.description if interface_record.description else None,
+                description=interface_record.description if interface_record.description else "",
                 enabled=True,
                 mac_address=mac_to_format(str(interface_record.mac_address), "MAC_COLON_TWO").upper()
                 if interface_record.mac_address
                 else DEFAULT_INTERFACE_MAC,
                 subnet_mask="255.255.255.255",
                 mtu=interface_record.mtu if interface_record.mtu else DEFAULT_INTERFACE_MTU,
                 type=DEFAULT_INTERFACE_TYPE,
```

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/adapters_shared.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/adapters_shared.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/diffsync/diffsync_models.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/diffsync/diffsync_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/jobs.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     Returns:
         dict: Snapshot objects as dict of tuples {snapshot_ref: (description, snapshot_id)}
     """
     formatted_snapshots = {}
     snapshot_refs = []
     if client:
+        client.update()
         for snapshot_ref, snapshot in client.snapshots.items():
             description = ""
             if snapshot_ref in [LAST, PREV, LAST_LOCKED]:
                 description += f"{snapshot_ref}: "
                 snapshot_refs.append(snapshot_ref)
             if snapshot.name:
                 description += snapshot.name + " - " + snapshot.end.strftime("%d-%b-%y %H:%M:%S")
```

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/signals.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_device_inventory.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_interface_inventory.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_sites.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/fixtures/get_vlans.json`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_ipfabric_adapter.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_jobs.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nautobot_adapter.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/tests/test_nbutils.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/tests/test_nbutils.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/utilities/__init__.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/utilities/nbutils.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/utilities/nbutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         "mgmt_only",
     )
     fields = {k: v for k, v in interface_details.items() if k in interface_fields and v}
     try:
         interface_obj, _ = device_obj.interfaces.get_or_create(**fields)
     except IntegrityError:
         interface_obj, _ = device_obj.interfaces.get_or_create(name=fields["name"])
-        interface_obj.description = fields.get("description")
+        interface_obj.description = fields.get("description", "")
         interface_obj.enabled = fields.get("enabled")
         interface_obj.mac_address = fields.get("mac_address")
         interface_obj.mtu = fields.get("mtu")
         interface_obj.type = fields.get("type")
         interface_obj.mgmt_only = fields.get("mgmt_only", False)
         interface_obj.validated_save()
     tag_object(nautobot_object=interface_obj, custom_field="ssot-synced-from-ipfabric")
```

### Comparing `nautobot_ssot_ipfabric-2.0.0/nautobot_ssot_ipfabric/workers.py` & `nautobot_ssot_ipfabric-2.0.1/nautobot_ssot_ipfabric/workers.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot_ipfabric-2.0.0/pyproject.toml` & `nautobot_ssot_ipfabric-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-ssot-ipfabric"
-version = "v2.0.0"
+version = "v2.0.1"
 description = "Nautobot SSoT IPFabric"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/networktocode-llc/nautobot-plugin-ssot-ipfabric"
 repository = "https://github.com/networktocode-llc/nautobot-plugin-ssot-ipfabric"
 keywords = ["nautobot", "nautobot-plugin"]
```

### Comparing `nautobot_ssot_ipfabric-2.0.0/PKG-INFO` & `nautobot_ssot_ipfabric-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-ssot-ipfabric
-Version: 2.0.0
+Version: 2.0.1
 Summary: Nautobot SSoT IPFabric
 Home-page: https://github.com/networktocode-llc/nautobot-plugin-ssot-ipfabric
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7.1,<4.0
```


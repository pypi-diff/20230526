# Comparing `tmp/python_omnilogic_local-0.2.0.tar.gz` & `tmp/python_omnilogic_local-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.2.0.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.2.1.tar", max compression
```

## Comparing `python_omnilogic_local-0.2.0.tar` & `python_omnilogic_local-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    18677 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3633 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7641 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     8961 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     7903 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6054 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-26 19:56:30.200637 python_omnilogic_local-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    18696 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3633 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7641 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     8961 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     7903 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6119 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-26 20:08:11.310222 python_omnilogic_local-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.2.1/PKG-INFO
```

### Comparing `python_omnilogic_local-0.2.0/README.md` & `python_omnilogic_local-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/api.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         parameter = ET.SubElement(parameters_element, "Parameter", name="HeaterID", dataType="int", alias="EquipmentID")
         parameter.text = str(equipment_id)
         parameter = ET.SubElement(parameters_element, "Parameter", name="Temp", dataType="int", unit=unit, alias="Data")
         parameter.text = str(temperature)
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
-        return await self.async_send_message(MessageType.SET_EQUIPMENT, req_body, False)
+        return await self.async_send_message(MessageType.SET_HEATER_COMMAND, req_body, False)
 
     async def async_set_solar_heater(self, pool_id: int, equipment_id: int, temperature: int, unit: str) -> None:
         """async_set_heater handles sending a SetUIHeaterCmd XML API call to the Hayward Omni pool controller
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
@@ -159,15 +159,15 @@
         parameter = ET.SubElement(parameters_element, "Parameter", name="HeaterID", dataType="int", alias="EquipmentID")
         parameter.text = str(equipment_id)
         parameter = ET.SubElement(parameters_element, "Parameter", name="Temp", dataType="int", unit=unit, alias="Data")
         parameter.text = str(temperature)
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
-        return await self.async_send_message(MessageType.SET_EQUIPMENT, req_body, False)
+        return await self.async_send_message(MessageType.SET_SOLAR_SET_POINT_COMMAND, req_body, False)
 
     async def async_set_heater_enable(self, pool_id: int, equipment_id: int, enabled: int | bool) -> None:
         """async_set_heater_enable handles sending a SetHeaterEnable XML API call to the Hayward Omni pool controller
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
```

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/models/mspconfig.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.0/pyomnilogic_local/types.py` & `python_omnilogic_local-0.2.1/pyomnilogic_local/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 
 # OmniAPI Enums
 class MessageType(Enum):
     XML_ACK = 0000
     REQUEST_CONFIGURATION = 1
     SET_FILTER_SPEED = 9
+    SET_HEATER_COMMAND = 11
     REQUEST_LOG_CONFIG = 31
+    SET_SOLAR_SET_POINT_COMMAND = 40
     SET_HEATER_ENABLED = 147
     SET_EQUIPMENT = 164
     CREATE_SCHEDULE = 230
     DELETE_SCHEDULE = 231
     GET_TELEMETRY = 300
     GET_ALARM_LIST = 304
     SET_STANDALONE_LIGHT_SHOW = 308
```

### Comparing `python_omnilogic_local-0.2.0/pyproject.toml` & `python_omnilogic_local-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.2.0"
+version = "0.2.1"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.2.0/PKG-INFO` & `python_omnilogic_local-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.2.0 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.2.1 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```


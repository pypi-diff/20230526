# Comparing `tmp/python_omnilogic_local-0.1.0.tar.gz` & `tmp/python_omnilogic_local-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.1.0.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.2.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.1.0.tar` & `python_omnilogic_local-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    17176 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3517 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7641 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     8961 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     7903 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6054 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-26 15:57:45.017633 python_omnilogic_local-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    18677 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3633 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7641 2023-05-26 19:56:29.296631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     8961 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     7903 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6054 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-26 19:56:29.300631 python_omnilogic_local-0.2.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-26 19:56:30.200637 python_omnilogic_local-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.2.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.1.0/README.md` & `python_omnilogic_local-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/api.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,43 @@
         parameter = ET.SubElement(parameters_element, "Parameter", name="Temp", dataType="int", unit=unit, alias="Data")
         parameter.text = str(temperature)
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.SET_EQUIPMENT, req_body, False)
 
+    async def async_set_solar_heater(self, pool_id: int, equipment_id: int, temperature: int, unit: str) -> None:
+        """async_set_heater handles sending a SetUIHeaterCmd XML API call to the Hayward Omni pool controller
+
+        Args:
+            pool_id (int): The Pool/BodyOfWater ID that you want to address
+            equipment_id (int): Which equipment_id within that Pool to address
+            temperature (int): What temperature to request
+            unit (str): The temperature unit to use (either F or C)
+
+        Returns:
+            _type_: _description_
+        """
+        body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
+
+        name_element = ET.SubElement(body_element, "Name")
+        name_element.text = "SetUISolarSetPointCmd"
+
+        parameters_element = ET.SubElement(body_element, "Parameters")
+        parameter = ET.SubElement(parameters_element, "Parameter", name="poolId", dataType="int")
+        parameter.text = str(pool_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="HeaterID", dataType="int", alias="EquipmentID")
+        parameter.text = str(equipment_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="Temp", dataType="int", unit=unit, alias="Data")
+        parameter.text = str(temperature)
+
+        req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
+
+        return await self.async_send_message(MessageType.SET_EQUIPMENT, req_body, False)
+
     async def async_set_heater_enable(self, pool_id: int, equipment_id: int, enabled: int | bool) -> None:
         """async_set_heater_enable handles sending a SetHeaterEnable XML API call to the Hayward Omni pool controller
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             enabled (bool, optional): Turn the heater on (True) or off (False)
```

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,17 @@
     # Adjust the heater temperature
     # await omni.async_set_heater(POOL_ID, HEATER_EQUIPMENT_ID, 85, "F")
 
     # Turn the heater on and off
     # await omni.async_set_heater_enable(POOL_ID, HEATER_EQUIPMENT_ID, True)
     # await omni.async_set_heater_enable(POOL_ID, HEATER_EQUIPMENT_ID, False)
 
+    # Adjust solar heater set point
+    # await omni.async_set_solar_heater(POOL_ID, HEATER_EQUIPMENT_ID, 90, "F")
+
     # Turn a variable speed pump on to 50%
     # await omni.async_set_filter_speed(POOL_ID, PUMP_EQUIPMENT_ID, 50)
     # Turn the pump off
     # await omni.async_set_equipment(POOL_ID, PUMP_EQUIPMENT_ID, False)
 
     # Activate a light show
     # await omni.async_set_light_show(
```

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/models/mspconfig.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.1.0/pyomnilogic_local/types.py` & `python_omnilogic_local-0.2.0/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.1.0/pyproject.toml` & `python_omnilogic_local-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.1.0"
+version = "0.2.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.1.0/PKG-INFO` & `python_omnilogic_local-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.1.0
+Version: 0.2.0
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
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.2.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```


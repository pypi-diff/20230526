# Comparing `tmp/python_omnilogic_local-0.0.6.tar.gz` & `tmp/python_omnilogic_local-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.0.6.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.1.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.0.6.tar` & `python_omnilogic_local-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1697 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.6/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    16868 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     2108 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0      407 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     5747 2023-05-25 01:43:01.066838 python_omnilogic_local-0.0.6/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     7770 2023-05-25 01:43:01.066838 python_omnilogic_local-0.0.6/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0      337 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     7262 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     5160 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      361 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     4902 2023-05-25 01:43:10.350956 python_omnilogic_local-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 python_omnilogic_local-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    17176 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3517 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7641 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     8961 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     7903 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6054 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-26 15:57:44.041622 python_omnilogic_local-0.1.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-26 15:57:45.017633 python_omnilogic_local-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.1.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.0.6/README.md` & `python_omnilogic_local-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Pyomnilogic Local
 
-
 <p align="center">
   <a href="https://pypi.org/project/python-omnilogic-local/">
     <img src="https://img.shields.io/pypi/v/python-omnilogic-local.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
   </a>
   <img src="https://img.shields.io/pypi/pyversions/python-omnilogic-local.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/python-omnilogic-local.svg?style=flat-square" alt="License">
 </p>
```

### Comparing `python_omnilogic_local-0.0.6/pyomnilogic_local/api.py` & `python_omnilogic_local-0.1.0/pyomnilogic_local/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import Literal, overload
 import xml.etree.ElementTree as ET
 
+from .models.filter_diagnostics import FilterDiagnostics
+from .models.mspconfig import MSPConfig
+from .models.telemetry import Telemetry
+from .models.util import to_pydantic
 from .protocol import OmniLogicProtocol
 from .types import ColorLogicBrightness, ColorLogicShow, ColorLogicSpeed, MessageType
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class OmniLogicAPI:
@@ -48,24 +52,26 @@
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "GetAllAlarmList"
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.GET_ALARM_LIST, req_body, True)
 
+    @to_pydantic(pydantic_type=MSPConfig)
     async def async_get_config(self) -> str:
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "RequestConfiguration"
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.REQUEST_CONFIGURATION, req_body, True)
 
+    @to_pydantic(pydantic_type=FilterDiagnostics)
     async def async_get_filter_diagnostics(self, pool_id: int, equipment_id: int) -> str:
         """async_get_filter_diagnostics handles sending a GetUIFilterDiagnosticInfo XML API call to the Hayward Omni pool controller
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
 
@@ -86,14 +92,15 @@
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.GET_FILTER_DIAGNOSTIC_INFO, req_body, True)
 
     async def async_get_log_config(self) -> str:
         return await self.async_send_message(MessageType.REQUEST_LOG_CONFIG, None, True)
 
+    @to_pydantic(pydantic_type=Telemetry)
     async def async_get_telemetry(self) -> str:
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "RequestTelemetryData"
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
```

### Comparing `python_omnilogic_local-0.0.6/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.1.0/pyomnilogic_local/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,42 +2,66 @@
 
 import asyncio
 import logging
 import os
 
 from pyomnilogic_local.api import OmniLogicAPI
 
-# from pyomnilogic_local.models.telemetry import Telemetry
-
+from .models.filter_diagnostics import FilterDiagnostics
+from .models.mspconfig import MSPConfig
+from .models.telemetry import Telemetry
 
 POOL_ID = 7
 PUMP_EQUIPMENT_ID = 8
 LIGHT_EQUIPMENT_ID = 10
 HEATER_EQUIPMENT_ID = 18
+RELAY_SYSTEM_ID = 13
 
 
 async def async_main() -> None:
+    diags: FilterDiagnostics  # noqa: F842
+    mspconfig: MSPConfig  # noqa: F842
+    telem: Telemetry  # noqa: F842
+
     omni = OmniLogicAPI(os.environ.get("OMNILOGIC_HOST", "127.0.0.1"), 10444, 5.0)
 
     # Some basic calls to run some testing against the library
-    # Fetch the MSPConfig data
-    config = await omni.async_get_config()
-    print(config)
-    # parsed_config = MSPConfig.load_xml(config)
 
-    # Fetch the current telemetry data
+    # Fetch the MSPConfig data parsed into a model
+    mspconfig = await omni.async_get_config()
+    # Fetch the MSPConfig data as the raw XML
+    # mspconfig = await omni.async_get_config(raw=True)
+    print(mspconfig)
+
+    # Fetch the current telemetry data parsed into a model
     telem = await omni.async_get_telemetry()
+    # Fetch the current telemetry data as the raw XML
+    # telem = await omni.async_get_telemetry(raw=True)
     print(telem)
-    # parsed_telem = Telemetry.load_xml(xml=telem)
 
     # Fetch a list of current alarms
     # print(await omni.async_get_alarm_list())
 
     # Fetch diagnostic data for a filter pump
-    # print(await omni.async_get_filter_diagnostics(POOL_ID, PUMP_EQUIPMENT_ID))
+    diags = await omni.async_get_filter_diagnostics(POOL_ID, PUMP_EQUIPMENT_ID)
+    print(diags)
+    # Decode the filter display revision
+    # b1=chr(diags.get_param_by_name("DisplayFWRevisionB1"))
+    # b2=chr(diags.get_param_by_name("DisplayFWRevisionB2"))
+    # b3=chr(diags.get_param_by_name("DisplayFWRevisionB3"))
+    # b4=chr(diags.get_param_by_name("DisplayFWRevisionB4"))
+    # # b5 and b6 are whitespace and a null terminator
+    # # b5=chr(diags.get_param_by_name("DisplayFWRevisionB5"))
+    # # b6=chr(diags.get_param_by_name("DisplayFWRevisionB6"))
+    # print(f"{b1}{b2}.{b3}.{b4}")
+    # # Decode the filter power consumption (don't do this, it's returned already decoded in the telemetry)
+    # p1=diags.get_param_by_name("PowerMSB")
+    # p2=diags.get_param_by_name("PowerLSB")
+    # # The f-string below converts the bytes to hex and displays them.  Just get this value from the telemetry, it's easier
+    # print(f"{p1:x}{p2:x}")
 
     # Fetch logging configuration
     # print(await omni.async_get_log_config())
 
     # Adjust the heater temperature
     # await omni.async_set_heater(POOL_ID, HEATER_EQUIPMENT_ID, 85, "F")
 
@@ -54,14 +78,18 @@
     # await omni.async_set_light_show(
     #     POOL_ID, LIGHT_EQUIPMENT_ID, ColorLogicShow.TRANQUILITY, ColorLogicSpeed.ONE_TIMES, ColorLogicBrightness.ONE_HUNDRED_PERCENT
     # )
     # Turn the light on/off
     # await omni.async_set_equipment(POOL_ID, LIGHT_EQUIPMENT_ID, True)
     # await omni.async_set_equipment(POOL_ID, LIGHT_EQUIPMENT_ID, False)
 
+    # Turn a relay on/off
+    # await omni.async_set_equipment(POOL_ID, RELAY_SYSTEM_ID, True)
+    # await omni.async_set_equipment(POOL_ID, RELAY_SYSTEM_ID, False)
+
 
 def main() -> None:
     logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=logging.DEBUG)
     asyncio.run(async_main())
 
 
 if __name__ == "__main__":
```

### Comparing `python_omnilogic_local-0.0.6/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.1.0/pyomnilogic_local/models/telemetry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
-from typing import cast
+from typing import Any, SupportsInt, TypeAlias, TypeVar, cast, overload
 
 from pydantic import BaseModel, Field
 from xmltodict import parse as xml_parse
 
 from ..types import (
     BackyardState,
     ChlorinatorOperatingMode,
     ColorLogicBrightness,
-    ColorLogicPowerStates,
+    ColorLogicPowerState,
     ColorLogicShow,
     ColorLogicSpeed,
     FilterState,
     FilterValvePosition,
     FilterWhyOn,
-    HeaterStatus,
-    PumpStatus,
-    RelayStatus,
-    ValveActuatorStatus,
+    HeaterState,
+    OmniType,
+    PumpState,
+    RelayState,
+    ValveActuatorState,
 )
 
 # Example telemetry XML data:
 #
 # <?xml version="1.0" encoding="UTF-8" ?>
 # <STATUS version="1.11">
 #     <Backyard systemId="0" statusVersion="11" airTemp="77" state="1" ConfigChksum="2211028" mspVersion="R0408000" />
@@ -35,175 +36,202 @@
 #     <VirtualHeater systemId="18" Current-Set-Point="85" enable="1" SolarSetPoint="90" Mode="0" SilentMode="0" whyHeaterIsOn="1" />
 #     <Heater systemId="19" heaterState="0" temp="74" enable="1" priority="254" maintainFor="24" />
 #     <Group systemId="21" groupState="0" />
 # </STATUS>
 
 
 class TelemetryBackyard(BaseModel):
-    omni_type = "Backyard"
+    omni_type: OmniType = OmniType.BACKYARD
     system_id: int = Field(alias="@systemId")
     status_version: int = Field(alias="@statusVersion")
     air_temp: int = Field(alias="@airTemp")
     state: BackyardState = Field(alias="@state")
     config_checksum: int = Field(alias="@ConfigChksum")
     msp_version: str = Field(alias="@mspVersion")
 
 
-class TelemetryBOW(BaseModel):
-    omni_type = "BodyOfWater"
+class TelemetryBoW(BaseModel):
+    omni_type: OmniType = OmniType.BOW
     system_id: int = Field(alias="@systemId")
     water_temp: int = Field(alias="@waterTemp")
     flow: int = Field(alias="@flow")
 
 
 class TelemetryChlorinator(BaseModel):
-    omni_type = "Chlorinator"
+    omni_type: OmniType = OmniType.CHLORINATOR
     system_id: int = Field(alias="@systemId")
     status: int = Field(alias="@status")
     instant_salt_level: int = Field(alias="@instantSaltLevel")
     avg_salt_level: int = Field(alias="@avgSaltLevel")
     chlr_alert: int = Field(alias="@chlrAlert")
     chlr_error: int = Field(alias="@chlrError")
     sc_mode: int = Field(alias="@scMode")
     operating_state: int = Field(alias="@operatingState")
     timed_percent: int = Field(alias="@Timed-Percent")
     operating_mode: ChlorinatorOperatingMode = Field(alias="@operatingMode")
     enable: bool
 
 
 class TelemetryColorLogicLight(BaseModel):
-    omni_type = "ColorLogic-Light"
+    omni_type: OmniType = OmniType.CL_LIGHT
     system_id: int = Field(alias="@systemId")
-    state: ColorLogicPowerStates = Field(alias="@lightState")
+    state: ColorLogicPowerState = Field(alias="@lightState")
     show: ColorLogicShow = Field(alias="@currentShow")
     speed: ColorLogicSpeed = Field(alias="@speed")
     brightness: ColorLogicBrightness = Field(alias="@brightness")
     special_effect: int = Field(alias="@specialEffect")
 
 
 class TelemetryFilter(BaseModel):
-    omni_type = "Filter"
+    omni_type: OmniType = OmniType.FILTER
     system_id: int = Field(alias="@systemId")
     state: FilterState = Field(alias="@filterState")
     speed: int = Field(alias="@filterSpeed")
     valve_position: FilterValvePosition = Field(alias="@valvePosition")
     why_on: FilterWhyOn = Field(alias="@whyFilterIsOn")
     reported_speed: int = Field(alias="@reportedFilterSpeed")
     power: int = Field(alias="@power")
     last_speed: int = Field(alias="@lastSpeed")
 
 
 class TelemetryGroup(BaseModel):
-    omni_type = "Group"
+    omni_type: OmniType = OmniType.GROUP
     system_id: int = Field(alias="@systemId")
     state: int = Field(alias="@groupState")
 
 
 class TelemetryHeater(BaseModel):
-    omni_type = "Heater"
+    omni_type: OmniType = OmniType.HEATER
     system_id: int = Field(alias="@systemId")
-    state: HeaterStatus = Field(alias="@heaterState")
+    state: HeaterState = Field(alias="@heaterState")
     temp: int = Field(alias="@temp")
     enabled: bool = Field(alias="@enable")
     priority: int = Field(alias="@priority")
     maintain_for: int = Field(alias="@maintainFor")
 
 
 class TelemetryPump(BaseModel):
-    omni_type = "Pump"
+    omni_type: OmniType = OmniType.PUMP
     system_id: int = Field(alias="@systemId")
-    state: PumpStatus = Field(alias="@pumpState")
+    state: PumpState = Field(alias="@pumpState")
     speed: int = Field(alias="@pummpSpeed")
     last_speed: int = Field(alias="@lastSpeed")
     why_on: int = Field(alias="@whyOn")
 
 
 class TelemetryRelay(BaseModel):
-    omni_type = "Relay"
+    omni_type: OmniType = OmniType.RELAY
     system_id: int = Field(alias="@systemId")
-    state: RelayStatus = Field(alias="@relayState")
+    state: RelayState = Field(alias="@relayState")
     why_on: int = Field(alias="@whyOn")
 
 
 class TelemetryValveActuator(BaseModel):
-    omni_type = "ValveActuator"
+    omni_type: OmniType = OmniType.VALVE_ACTUATOR
     system_id: int = Field(alias="@systemId")
-    state: ValveActuatorStatus = Field(alias="@valveActuatorState")
+    state: ValveActuatorState = Field(alias="@valveActuatorState")
     why_on: int = Field(alias="@whyOn")
 
 
 class TelemetryVirtualHeater(BaseModel):
-    omni_type = "VirtualHeater"
+    omni_type: OmniType = OmniType.VIRT_HEATER
     system_id: int = Field(alias="@systemId")
     current_set_point: int = Field(alias="@Current-Set-Point")
     enabled: bool = Field(alias="@enable")
     solar_set_point: int = Field(alias="@SolarSetPoint")
     mode: int = Field(alias="@Mode")
     silent_mode: int = Field(alias="@SilentMode")
     why_on: int = Field(alias="@whyHeaterIsOn")
 
 
-TTelemetry = (
+TelemetryType: TypeAlias = (
     TelemetryBackyard
-    | TelemetryBOW
+    | TelemetryBoW
     | TelemetryChlorinator
     | TelemetryColorLogicLight
     | TelemetryFilter
     | TelemetryGroup
     | TelemetryHeater
     | TelemetryPump
     | TelemetryRelay
     | TelemetryValveActuator
     | TelemetryVirtualHeater
 )
 
 
 class Telemetry(BaseModel):
     version: str = Field(alias="@version")
-    backyard: list[TelemetryBackyard] = Field(alias="Backyard")
-    bow: list[TelemetryBOW] = Field(alias="BodyOfWater")
+    backyard: TelemetryBackyard = Field(alias="Backyard")
+    bow: list[TelemetryBoW] = Field(alias="BodyOfWater")
     chlorinator: list[TelemetryChlorinator] | None = Field(alias="Chlorinator")
     colorlogic_light: list[TelemetryColorLogicLight] | None = Field(alias="ColorLogic-Light")
     filter: list[TelemetryFilter] | None = Field(alias="Filter")
     group: list[TelemetryGroup] | None = Field(alias="Group")
     heater: list[TelemetryHeater] | None = Field(alias="Heater")
     pump: list[TelemetryPump] | None = Field(alias="Pump")
     relay: list[TelemetryRelay] | None = Field(alias="Relay")
     valve_actuator: list[TelemetryValveActuator] | None = Field(alias="ValveActuator")
-    virtual_heater: list[TelemetryVirtualHeater] | None = Field(alias="VirtualHeater")
+    virtual_heater: TelemetryVirtualHeater | None = Field(alias="VirtualHeater")
 
     class Config:
         orm_mode = True
 
     @staticmethod
     def load_xml(xml: str) -> Telemetry:
+
+        TypeVar("KT")
+        TypeVar("VT", SupportsInt, Any)
+
+        @overload
+        def xml_postprocessor(path: Any, key: Any, value: SupportsInt) -> tuple[Any, SupportsInt]:
+            ...
+
+        @overload
+        def xml_postprocessor(path: Any, key: Any, value: Any) -> tuple[Any, Any]:
+            ...
+
+        def xml_postprocessor(path: Any, key: Any, value: SupportsInt | Any) -> tuple[Any, SupportsInt | Any]:
+            """Post process XML to attempt to convert values to int."""
+            newvalue: SupportsInt | Any
+
+            try:
+                newvalue = int(value)
+            except (ValueError, TypeError):
+                newvalue = value
+
+            return key, newvalue
+
         data = xml_parse(
             xml,
+            postprocessor=xml_postprocessor,
             # Some things will be lists or not depending on if a pool has more than one of that piece of equipment.  Here we are coercing
             # everything into lists to make the parsing more consistent. This does mean that some things that would normally never be lists
             # will become lists (I.E.: Backyard, VirtualHeater), but the upside is that we need far less conditional code to deal with the
             # "maybe list maybe not" devices.
             force_list=(
-                "Backyard",
-                "BodyOfWater",
-                "Chlorinator",
-                "ColorLogic-Light",
-                "Filter",
-                "Group",
-                "Heater",
-                "Pump",
-                "Relay",
-                "ValveActuator",
-                "VirtualHeater",
+                OmniType.BOW,
+                OmniType.CHLORINATOR,
+                OmniType.CL_LIGHT,
+                OmniType.FILTER,
+                OmniType.GROUP,
+                OmniType.HEATER,
+                OmniType.PUMP,
+                OmniType.RELAY,
+                OmniType.VALVE_ACTUATOR,
             ),
         )
         return Telemetry.parse_obj(data["STATUS"])
 
-    def get_telem_by_systemid(self, system_id: int) -> TTelemetry | None:
+    def get_telem_by_systemid(self, system_id: int) -> TelemetryType | None:
         for field_name, value in self:
             if field_name == "version" or value is None:
                 continue
-            for model in value:
-                cast_model = cast(TTelemetry, model)
+            if isinstance(value, list):
+                for model in value:
+                    cast_model = cast(TelemetryType, model)
+                    if cast_model.system_id == system_id:
+                        return cast_model
+            else:
+                cast_model = cast(TelemetryType, value)
                 if cast_model.system_id == system_id:
                     return cast_model
         return None
```

### Comparing `python_omnilogic_local-0.0.6/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.1.0/pyomnilogic_local/protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
             # If the message that we just sent is an ACK, we do not need to wait to receive an ACK, we are done
             if message.type in [MessageType.XML_ACK, MessageType.ACK]:
                 return
 
             # Wait for a bit to either receive an ACK for our message, otherwise, we retry delivery
             try:
-                await asyncio.wait_for(self._wait_for_ack(message.id), 0.5)
+                await asyncio.wait_for(self._wait_for_ack(message.id), 1)
                 delivered = True
             except TimeoutError:
                 _LOGGER.debug("ACK not received, re-attempting delivery")
 
     async def send_and_receive(self, msg_type: MessageType, payload: str | None, msg_id: int | None = None) -> str:
         await self.send_message(msg_type, payload, msg_id)
         return await self._receive_file()
@@ -142,27 +142,35 @@
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
         await self.send_message(MessageType.XML_ACK, req_body, msg_id)
 
     async def _receive_file(self) -> str:
         # wait for the initial packet.
         message = await self.data_queue.get()
 
+        # If messages have to be re-transmitted, we can sometimes receive multiple ACKs.  The first one would be handled by
+        # self._ensure_sent, but if any subsequent ACKs are sent to us, we need to dump them and wait for a "real" message.
+        while message.type in [MessageType.ACK, MessageType.XML_ACK]:
+            message = await self.data_queue.get()
+
         await self._send_ack(message.id)
 
         # If the response is too large, the controller will send a LeadMessage indicating how many follow-up messages will be sent
         if message.type == MessageType.MSP_LEADMESSAGE:
             leadmsg = LeadMessage.from_orm(ET.fromstring(message.payload[:-1]))
 
             # Wait for the block data data
             retval: bytes = b""
             # If we received a LeadMessage, continue to receive messages until we have all of our data
             # Fragments of data may arrive out of order, so we store them in a buffer as they arrive and sort them after
             data_fragments: dict[int, bytes] = {}
             while len(data_fragments) < leadmsg.msg_block_count:
                 resp = await self.data_queue.get()
+                # We only want to collect blockmessages here
+                if resp.type is not MessageType.MSP_BLOCKMESSAGE:
+                    continue
                 await self._send_ack(resp.id)
                 # remove an 8 byte header to get to the payload data
                 data_fragments[resp.id] = resp.payload[8:]
 
             # Reassemble the fragmets in order
             for _, data in sorted(data_fragments.items()):
                 retval += data
@@ -175,9 +183,9 @@
             retval = message.payload[8:]
 
         # Decompress the returned data if necessary
         if message.compressed:
             comp_bytes = bytes.fromhex(retval.hex())
             retval = zlib.decompress(comp_bytes)
 
-        # return retval
-        return retval.decode("utf-8")
+        # For some API calls, the Omni null terminates the response, we are stripping that here to make parsing it later easier
+        return retval.decode("utf-8").strip("\x00")
```

### Comparing `python_omnilogic_local-0.0.6/pyomnilogic_local/types.py` & `python_omnilogic_local-0.1.0/pyomnilogic_local/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,61 +27,84 @@
 
 
 class ClientType(Enum):
     XML = 0
     SIMPLE = 1
 
 
-class BackyardState(str, PrettyEnum):
+class OmniType(str, Enum):
+    BACKYARD = "Backyard"
+    BOW = "BodyOfWater"
+    BOW_MSP = "Body-of-water"
+    CHLORINATOR = "Chlorinator"
+    CHLORINATOR_EQUIP = "Chlorinator-Equipment"
+    CL_LIGHT = "ColorLogic-Light"
+    FAVORITES = "Favorites"
+    FILTER = "Filter"
+    GROUP = "Group"
+    GROUPS = "Groups"
+    HEATER = "Heater"
+    HEATER_EQUIP = "Heater-Equipment"
+    PUMP = "Pump"
+    RELAY = "Relay"
+    SCHE = "sche"
+    SCHEDULE = "Schedule"
+    SENSOR = "Sensor"
+    SYSTEM = "System"
+    VALVE_ACTUATOR = "ValveActuator"
+    VIRT_HEATER = "VirtualHeater"
+
+
+class BackyardState(PrettyEnum):
     OFF = 0
     ON = 1
     SERVICE_MODE = 2
     CONFIG_MODE = 3
     TIMED_SERVICE_MODE = 4
 
 
-class BodyOfWaterStatus(str, PrettyEnum):
+class BodyOfWaterState(PrettyEnum):
     NO_FLOW = 0
     FLOW = 1
 
 
 class BodyOfWaterType(str, PrettyEnum):
     POOL = "BOW_POOL"
     SPA = "BOW_SPA"
 
 
 # Chlorinator status is a bitmask that we still need to figure out
 # class ChlorinatorStatus(str,Enum):
 #     pass
-class ChlorinatorOperatingMode(str, PrettyEnum):
+class ChlorinatorOperatingMode(PrettyEnum):
     TIMED = 1
     ORP = 2
 
 
-class ColorLogicSpeed(str, PrettyEnum):
+class ColorLogicSpeed(PrettyEnum):
     ONE_SIXTEENTH = 0
     ONE_EIGHTH = 1
     ONE_QUARTER = 2
     ONE_HALF = 3
     ONE_TIMES = 4
     TWO_TIMES = 5
     FOUR_TIMES = 6
     EIGHT_TIMES = 7
     SIXTEEN_TIMES = 8
 
 
-class ColorLogicBrightness(str, PrettyEnum):
+class ColorLogicBrightness(PrettyEnum):
     TWENTY_PERCENT = 0
     FOURTY_PERCENT = 1
     SIXTY_PERCENT = 2
     EIGHTY_PERCENT = 3
     ONE_HUNDRED_PERCENT = 4
 
 
-class ColorLogicShow(str, PrettyEnum):
+class ColorLogicShow(PrettyEnum):
     VOODOO_LOUNGE = 0
     DEEP_BLUE_SEA = 1
     ROYAL_BLUE = 2
     AFTERNOON_SKY = 3
     AQUA_GREEN = 4
     EMERALD = 5
     CLOUD_WHITE = 6
@@ -104,37 +127,43 @@
     BURNT_ORANGE = 22
     PURE_WHITE = 23
     CRISP_WHITE = 24
     WARM_WHITE = 25
     BRIGHT_YELLOW = 26
 
 
-class ColorLogicPowerStates(str, PrettyEnum):
+class ColorLogicPowerState(PrettyEnum):
     OFF = 0
     POWERING_OFF = 1
     CHANGING_SHOW = 3
     FIFTEEN_SECONDS_WHITE = 4
     ACTIVE = 6
     COOLDOWN = 7
 
 
-class CSADStatus(str, PrettyEnum):
+class ColorLogicLightType(str, PrettyEnum):
+    UCL = "COLOR_LOGIC_UCL"
+    FOUR_ZERO = "COLOR_LOGIC_4_0"
+    TWO_FIVE = "COLOR_LOGIC_2_5"
+
+
+class CSADStatus(PrettyEnum):
     NOT_DISPENSING = 0
     DISPENSING = 1
 
 
-class CSADMode(str, PrettyEnum):
+class CSADMode(PrettyEnum):
     OFF = 0
     AUTO = 1
     FORCE_ON = 2
     MONITORING = 3
     DISPENSING_OFF = 4
 
 
-class FilterState(str, PrettyEnum):
+class FilterState(PrettyEnum):
     OFF = 0
     ON = 1
     PRIMING = 2
     WAITING_TURN_OFF = 3
     WAITING_TURN_OFF_MANUAL = 4
     HEATER_EXTEND = 5
     COOLDOWN = 6
@@ -147,23 +176,23 @@
 
 class FilterType(str, PrettyEnum):
     VARIABLE_SPEED = "FMT_VARIABLE_SPEED_PUMP"
     DUAL_SPEED = "FMT_DUAL_SPEED"
     SINGLE_SPEED = "FMT_SINGLE_SPEED"
 
 
-class FilterValvePosition(str, PrettyEnum):
+class FilterValvePosition(PrettyEnum):
     POOL_ONLY = 1
     SPA_ONLY = 2
     SPILLOVER = 3
     LOW_PRIO_HEAT = 4
     HIGH_PRIO_HEAT = 5
 
 
-class FilterWhyOn(str, PrettyEnum):
+class FilterWhyOn(PrettyEnum):
     OFF = 0
     NO_WATER_FLOW = 1
     COOLDOWN = 2
     PH_REDUCE_EXTEND = 3
     HEATER_EXTEND = 4
     PAUSED = 5
     VALVE_CHANGING = 6
@@ -174,32 +203,44 @@
     MANUAL_ON = 11
     MANUAL_SPILLOVER = 12
     TIMER_SPILLOVER = 13
     TIMER_ON = 14
     FREEZE_PROTECT = 15
 
 
-class HeaterStatus(str, PrettyEnum):
+class HeaterState(PrettyEnum):
     OFF = 0
     ON = 1
     PAUSE = 2
 
 
 class HeaterType(str, PrettyEnum):
     GAS = "HTR_GAS"
     HEAT_PUMP = "HTR_HEAT_PUMP"
     SOLAR = "HTR_SOLAR"
     ELECTRIC = "HTR_ELECTRIC"
     GEOTHERMAL = "HTR_GEOTHERMAL"
     SMART = "HTR_SMART"
 
 
-class PumpStatus(str, PrettyEnum):
+class PumpState(PrettyEnum):
     OFF = 0
-    ON = 0
+    ON = 1
+
+
+class PumpType(str, PrettyEnum):
+    SINGLE_SPEED = "PMP_SINGLE_SPEED"
+    VARIABLE_SPEED = "PMP_VARIABLE_SPEED_PUMP"
+
+
+class PumpFunction(str, PrettyEnum):
+    WATERFALL = "PMP_WATERFALL"
+    BLOWER = "PMP_BLOWER"
+    JETS = "PMP_JETS"
+    CLEANER = "PMP_CLEANER"
 
 
 class RelayFunction(str, PrettyEnum):
     WATER_FEATURE = "RLY_WATER_FEATURE"
     LIGHT = "RLY_LIGHT"
     BACKYARD_LIGHT = "RLY_BACKYARD_LIGHT"
     POOL_LIGHT = "RLY_POOL_LIGHT"
@@ -214,15 +255,15 @@
     ACCESSORY = "RLY_ACCESSORY"
     CLEANER_PRESSURE = "RLY_CLEANER_PRESSURE"
     CLEANER_SUCTION = "RLY_CLEANER_SUCTION"
     CLEANER_ROBOTIC = "RLY_CLEANER_ROBOTIC"
     CLEANER_IN_FLOOR = "RLY_CLEANER_IN_FLOOR"
 
 
-class RelayStatus(str, PrettyEnum):
+class RelayState(PrettyEnum):
     OFF = 0
     ON = 1
 
 
 class RelayType(str, PrettyEnum):
     VALVE_ACTUATOR = "RLY_VALVE_ACTUATOR"
     HIGH_VOLTAGE = "RLY_HIGH_VOLTAGE_RELAY"
@@ -241,10 +282,10 @@
     CELSIUS = "UNITS_CELSIUS"
     PPM = "UNITS_PPM"
     GRAMS_PER_LITER = "UNITS_GRAMS_PER_LITER"
     MILLIVOLTS = "UNITS_MILLIVOLTS"
     NO_UNITS = "UNITS_NO_UNITS"
 
 
-class ValveActuatorStatus(str, PrettyEnum):
+class ValveActuatorState(PrettyEnum):
     OFF = 0
     ON = 1
```

### Comparing `python_omnilogic_local-0.0.6/pyproject.toml` & `python_omnilogic_local-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.0.6"
+version = "0.1.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -52,35 +52,42 @@
 ]
 combine_as_imports = true
 
 [tool.mypy]
 python_version = "3.10"
 plugins = "pydantic.mypy"
 follow_imports = "silent"
+strict = true
 ignore_missing_imports = true
-local_partial_types = true
-strict_equality = true
-no_implicit_optional = true
-warn_incomplete_stub = true
-warn_redundant_casts = true
-warn_unused_configs = true
-warn_unused_ignores = true
-enable_error_code = "ignore-without-code, redundant-self, truthy-iterable"
-disable_error_code = "annotation-unchecked"
-strict_concatenate = false
-check_untyped_defs = true
-disallow_incomplete_defs = true
-# disallow_subclassing_any = true
-disallow_untyped_calls = true
-disallow_untyped_decorators = true
-disallow_untyped_defs = true
-warn_return_any = true
-warn_unreachable = true
-no_implicit_reexport = true
-disallow_any_generics = true
+disallow_subclassing_any = false
+warn_return_any = false
+# local_partial_types = true
+# strict_equality = true
+# no_implicit_optional = true
+# warn_incomplete_stub = true
+# warn_redundant_casts = true
+# warn_unused_configs = true
+# warn_unused_ignores = true
+# enable_error_code = "ignore-without-code, redundant-self, truthy-iterable"
+# disable_error_code = "annotation-unchecked"
+# strict_concatenate = false
+# check_untyped_defs = true
+# disallow_incomplete_defs = true
+# disallow_untyped_calls = true
+# disallow_untyped_decorators = true
+# disallow_untyped_defs = true
+# warn_unreachable = true
+# no_implicit_reexport = true
+# disallow_any_generics = true
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
 
 [tool.pylint.MAIN]
 py-version = "3.10"
 ignore = [
     "tests",
 ]
 # Use a conservative default here; 2 should speed up most setups and not hurt
@@ -181,7 +188,12 @@
 ]
 
 [tool.pylint.REPORTS]
 score = false
 
 [tool.ruff]
 line-length = 140
+
+[tool.semantic_release]
+branch = "main"
+version_toml = "pyproject.toml:tool.poetry.version"
+build_command = "pip install poetry && poetry build"
```

### Comparing `python_omnilogic_local-0.0.6/PKG-INFO` & `python_omnilogic_local-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.0.6
+Version: 0.1.0
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,14 @@
 Requires-Dist: pydantic-xml (>=0.6.1,<0.7.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/cryptk/python-omnilogic-local
 Description-Content-Type: text/markdown
 
 # Pyomnilogic Local
 
-
 <p align="center">
   <a href="https://pypi.org/project/python-omnilogic-local/">
     <img src="https://img.shields.io/pypi/v/python-omnilogic-local.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
   </a>
   <img src="https://img.shields.io/pypi/pyversions/python-omnilogic-local.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/python-omnilogic-local.svg?style=flat-square" alt="License">
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.0.6 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.1.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```


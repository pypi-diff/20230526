# Comparing `tmp/aioairzone-0.5.6.tar.gz` & `tmp/aioairzone-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-0.5.6.tar", last modified: Tue May 16 06:48:09 2023, max compression
+gzip compressed data, was "aioairzone-0.6.0.tar", last modified: Fri May 26 14:19:50 2023, max compression
```

## Comparing `aioairzone-0.5.6.tar` & `aioairzone-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-16 06:48:09.646561 aioairzone-0.5.6/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.5.6/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.5.6/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-16 06:48:09.646561 aioairzone-0.5.6/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.5.6/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-16 06:48:09.642562 aioairzone-0.5.6/aioairzone/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.5.6/aioairzone/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4509 2023-05-09 19:13:01.000000 aioairzone-0.5.6/aioairzone/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4721 2023-05-16 06:31:23.000000 aioairzone-0.5.6/aioairzone/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    31713 2023-05-16 06:43:17.000000 aioairzone-0.5.6/aioairzone/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.5.6/aioairzone/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    14150 2023-05-12 18:16:45.000000 aioairzone-0.5.6/aioairzone/localapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.5.6/aioairzone/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.5.6/aioairzone/webserver.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-16 06:48:09.646561 aioairzone-0.5.6/aioairzone.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      450 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      930 2023-05-16 06:45:08.000000 aioairzone-0.5.6/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.5.6/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-16 06:48:09.646561 aioairzone-0.5.6/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 14:19:50.424091 aioairzone-0.6.0/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.6.0/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.6.0/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 14:19:50.424091 aioairzone-0.6.0/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.6.0/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 14:19:50.424091 aioairzone-0.6.0/aioairzone/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.6.0/aioairzone/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4647 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6978 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.6.0/aioairzone/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16904 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/localapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.6.0/aioairzone/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     7683 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1565 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/thermostat.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.6.0/aioairzone/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    25111 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 14:19:50.424091 aioairzone-0.6.0/aioairzone.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      494 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      996 2023-05-26 14:19:20.000000 aioairzone-0.6.0/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.6.0/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-26 14:19:50.424091 aioairzone-0.6.0/setup.cfg
```

### Comparing `aioairzone-0.5.6/LICENSE` & `aioairzone-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.6/PKG-INFO` & `aioairzone-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.5.6
+Version: 0.6.0
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.5.6/README.md` & `aioairzone-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.6/aioairzone/common.py` & `aioairzone-0.6.0/aioairzone/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,7 +210,12 @@
         """Convert WebServerType value to string."""
         models: dict[int, str] = {
             self.UNKNOWN: "Unknown",
             self.AIRZONE: "Airzone WebServer",
             self.AIDOO: "Aidoo WebServer",
         }
         return models[self.value]
+
+
+def get_system_zone_id(system_id: int, zone_id: int) -> str:
+    """Combine system and zone IDs."""
+    return f"{system_id}:{zone_id}"
```

### Comparing `aioairzone-0.5.6/aioairzone/device.py` & `aioairzone-0.6.0/aioairzone/zone.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,104 +1,92 @@
 """Airzone Local API Device."""
 from __future__ import annotations
 
-import logging
 from typing import Any
 
 from .common import (
     AirzoneStages,
     EcoAdapt,
     GrilleAngle,
     OperationAction,
     OperationMode,
     SleepTimeout,
-    SystemType,
     TemperatureUnit,
-    ThermostatType,
+    get_system_zone_id,
 )
 from .const import (
     API_AIR_DEMAND,
     API_ANTI_FREEZE,
     API_COLD_ANGLE,
+    API_COLD_DEMAND,
     API_COLD_STAGE,
     API_COLD_STAGES,
     API_COOL_MAX_TEMP,
     API_COOL_MIN_TEMP,
     API_COOL_SET_POINT,
     API_DOUBLE_SET_POINT,
     API_DOUBLE_SET_POINT_PARAMS,
     API_ECO_ADAPT,
     API_ERROR_LOW_BATTERY,
     API_ERRORS,
     API_FLOOR_DEMAND,
     API_HEAT_ANGLE,
+    API_HEAT_DEMAND,
     API_HEAT_MAX_TEMP,
     API_HEAT_MIN_TEMP,
     API_HEAT_SET_POINT,
     API_HEAT_STAGE,
     API_HEAT_STAGES,
     API_HUMIDITY,
-    API_MANUFACTURER,
     API_MASTER_ZONE_ID,
     API_MAX_TEMP,
-    API_MC_CONNECTED,
     API_MIN_TEMP,
     API_MODE,
     API_MODES,
     API_NAME,
     API_ON,
-    API_POWER,
     API_ROOM_TEMP,
     API_SET_POINT,
     API_SLEEP,
     API_SPEED,
     API_SPEEDS,
-    API_SYSTEM_FIRMWARE,
-    API_SYSTEM_ID,
-    API_SYSTEM_TYPE,
     API_TEMP_STEP,
-    API_THERMOS_FIRMWARE,
-    API_THERMOS_RADIO,
-    API_THERMOS_TYPE,
     API_UNITS,
-    API_ZONE_ID,
     AZD_ABS_TEMP_MAX,
     AZD_ABS_TEMP_MIN,
     AZD_ACTION,
     AZD_AIR_DEMAND,
     AZD_ANTI_FREEZE,
+    AZD_AVAILABLE,
     AZD_BATTERY_LOW,
-    AZD_CLAMP_METER,
     AZD_COLD_ANGLE,
+    AZD_COLD_DEMAND,
     AZD_COLD_STAGE,
     AZD_COLD_STAGES,
     AZD_COOL_TEMP_MAX,
     AZD_COOL_TEMP_MIN,
     AZD_COOL_TEMP_SET,
     AZD_DEMAND,
     AZD_DOUBLE_SET_POINT,
     AZD_ECO_ADAPT,
-    AZD_ENERGY,
     AZD_ERRORS,
-    AZD_FIRMWARE,
     AZD_FLOOR_DEMAND,
     AZD_FULL_NAME,
     AZD_HEAT_ANGLE,
+    AZD_HEAT_DEMAND,
     AZD_HEAT_STAGE,
     AZD_HEAT_STAGES,
     AZD_HEAT_TEMP_MAX,
     AZD_HEAT_TEMP_MIN,
     AZD_HEAT_TEMP_SET,
     AZD_HUMIDITY,
     AZD_ID,
-    AZD_MANUFACTURER,
     AZD_MASTER,
     AZD_MASTER_ZONE,
     AZD_MODE,
-    AZD_MODEL,
     AZD_MODES,
     AZD_NAME,
     AZD_ON,
     AZD_PROBLEMS,
     AZD_SLEEP,
     AZD_SPEED,
     AZD_SPEEDS,
@@ -108,411 +96,188 @@
     AZD_TEMP_MIN,
     AZD_TEMP_SET,
     AZD_TEMP_STEP,
     AZD_TEMP_UNIT,
     AZD_THERMOSTAT_FW,
     AZD_THERMOSTAT_MODEL,
     AZD_THERMOSTAT_RADIO,
-    AZD_ZONES_NUM,
-    ERROR_SYSTEM,
+    DEFAULT_TEMP_STEP_CELSIUS,
+    DEFAULT_TEMP_STEP_FAHRENHEIT,
     ERROR_ZONE,
-    THERMOSTAT_RADIO,
-    THERMOSTAT_WIRED,
 )
-from .exceptions import InvalidZone
-
-_LOGGER = logging.getLogger(__name__)
-
-
-class System:
-    """Airzone System."""
-
-    def __init__(self, airzone_system: list[dict[str, Any]]):
-        """System init."""
-        self.clamp_meter: bool | None = None
-        self.eco_adapt: EcoAdapt | None = None
-        self.energy: int | None = None
-        self.errors: list[str] = []
-        self.id: int | None = None
-        self.firmware: str | None = None
-        self.manufacturer: str | None = None
-        self.mode: OperationMode | None = None
-        self.modes: list[OperationMode] = []
-        self.type: SystemType | None = None
-        self.zones: dict[int, Zone] = {}
-
-        for airzone_zone in airzone_system:
-            zone = Zone(self, airzone_zone)
-            if zone:
-                _id = int(airzone_zone[API_SYSTEM_ID])
-                if not self.id:
-                    self.id = _id
-                elif self.id != _id:
-                    _LOGGER.error("System ID mismatch across zones")
-
-                self.zones[zone.get_id()] = zone
-
-    def data(self) -> dict[str, Any]:
-        """Return Airzone system data."""
-        data: dict[str, Any] = {
-            AZD_ID: self.get_id(),
-            AZD_PROBLEMS: self.get_problems(),
-            AZD_ZONES_NUM: self.num_zones(),
-        }
-
-        clamp_meter = self.get_clamp_meter()
-        if clamp_meter is not None:
-            data[AZD_CLAMP_METER] = clamp_meter
-
-            if clamp_meter:
-                energy = self.get_energy()
-                if energy is not None:
-                    data[AZD_ENERGY] = energy
-
-        eco_adapt = self.get_eco_adapt()
-        if eco_adapt is not None:
-            data[AZD_ECO_ADAPT] = eco_adapt
-
-        errors = self.get_errors()
-        if len(errors) > 0:
-            data[AZD_ERRORS] = errors
-
-        firmware = self.get_firmware()
-        if firmware is not None:
-            data[AZD_FIRMWARE] = firmware
-
-        full_name = self.get_full_name()
-        if full_name is not None:
-            data[AZD_FULL_NAME] = full_name
-
-        manufacturer = self.get_manufacturer()
-        if manufacturer is not None:
-            data[AZD_MANUFACTURER] = manufacturer
-
-        mode = self.get_mode()
-        if mode is not None:
-            data[AZD_MODE] = mode
-
-        model = self.get_model()
-        if self.type is not None:
-            data[AZD_MODEL] = model
-
-        modes = self.get_modes()
-        if modes is not None:
-            data[AZD_MODES] = modes
-
-        return data
-
-    def add_error(self, val: str) -> None:
-        """Add system error."""
-        if val not in self.errors:
-            self.errors.append(val)
-
-    def get_clamp_meter(self) -> bool | None:
-        """Return system clamp meter connection."""
-        return self.clamp_meter
-
-    def get_eco_adapt(self) -> EcoAdapt | None:
-        """Return system Eco Adapt."""
-        return self.eco_adapt
-
-    def get_energy(self) -> int | None:
-        """Return system energy consumption."""
-        return self.energy
-
-    def get_errors(self) -> list[str]:
-        """Return system errors."""
-        return self.errors
-
-    def get_id(self) -> int | None:
-        """Return system ID."""
-        return self.id
-
-    def get_firmware(self) -> str | None:
-        """Return system firmware."""
-        if self.firmware and "." not in self.firmware and len(self.firmware) > 2:
-            return f"{self.firmware[0:1]}.{self.firmware[1:]}"
-        return self.firmware
-
-    def get_full_name(self) -> str:
-        """Return full name."""
-        return f"Airzone [{self.get_id()}] System"
-
-    def get_manufacturer(self) -> str | None:
-        """Return system manufacturer."""
-        return self.manufacturer
-
-    def get_model(self) -> str | None:
-        """Return system model."""
-        if self.type:
-            return str(self.type)
-        return None
-
-    def get_mode(self) -> OperationMode | None:
-        """Return system mode."""
-        return self.mode
-
-    def get_modes(self) -> list[OperationMode] | None:
-        """Return system modes."""
-        if len(self.modes) > 0:
-            return self.modes
-        if self.mode is not None:
-            return [self.mode]
-        return None
-
-    def get_problems(self) -> bool:
-        """Return system problems."""
-        return bool(self.errors)
-
-    def get_zone(self, zone_id: int) -> Zone:
-        """Return Airzone zone."""
-        for zone in self.zones.values():
-            if zone.get_id() == zone_id:
-                return zone
-        raise InvalidZone(f"Zone {zone_id} not present in System {self.id}")
-
-    def num_zones(self) -> int:
-        """Return number of system zones."""
-        return len(self.zones)
-
-    def set_eco_adapt(self, eco_adapt: EcoAdapt) -> None:
-        """Set system Eco Adapt."""
-        self.eco_adapt = eco_adapt
-
-    def set_mode(self, mode: OperationMode) -> None:
-        """Set system mode."""
-        self.mode = mode
-
-    def set_modes(self, modes: list[OperationMode]) -> None:
-        """Set system modes."""
-        self.modes = modes
-
-    def set_param(self, key: str, value: Any) -> None:
-        """Update parameters by key and value."""
-        if key == API_ECO_ADAPT:
-            self.eco_adapt = EcoAdapt(value)
-        elif key == API_MODE:
-            self.mode = OperationMode(value)
-
-        for zone in self.zones.values():
-            zone.set_param(key, value)
-
-    def update_data(self, data: dict[str, Any]) -> None:
-        """Update system parameters by dict."""
-
-        if API_MC_CONNECTED in data:
-            self.clamp_meter = bool(data[API_MC_CONNECTED])
-
-        if API_ERRORS in data:
-            errors: list[dict[str, str]] = data[API_ERRORS]
-            for error in errors:
-                for val in error.values():
-                    self.add_error(val)
-
-        if API_MANUFACTURER in data:
-            self.manufacturer = str(data[API_MANUFACTURER])
-
-        if API_POWER in data:
-            self.energy = int(data[API_POWER])
-
-        if API_SYSTEM_FIRMWARE in data:
-            self.firmware = str(data[API_SYSTEM_FIRMWARE])
-
-        if API_SYSTEM_TYPE in data:
-            self.type = SystemType(data[API_SYSTEM_TYPE])
-
-
-class Thermostat:
-    """Airzone Thermostat."""
-
-    def __init__(self, data: dict[str, Any]):
-        """Thermostat init."""
-        self.firmware: str | None = None
-        self.radio: bool | None = None
-        self.type: ThermostatType | None = None
-
-        if API_THERMOS_FIRMWARE in data:
-            self.firmware = str(data[API_THERMOS_FIRMWARE])
-        if API_THERMOS_RADIO in data:
-            self.radio = bool(data[API_THERMOS_RADIO])
-        if API_THERMOS_TYPE in data:
-            self.type = ThermostatType(data[API_THERMOS_TYPE])
-
-    def get_firmware(self) -> str | None:
-        """Return Airzone Thermostat firmware."""
-        if self.firmware and "." not in self.firmware and len(self.firmware) > 2:
-            return f"{self.firmware[0:1]}.{self.firmware[1:]}"
-        return self.firmware
-
-    def get_model(self) -> str | None:
-        """Return Airzone Thermostat model."""
-        if self.type:
-            name = str(self.type)
-            if self.type.exists_radio():
-                sfx = f" ({THERMOSTAT_RADIO if self.radio else THERMOSTAT_WIRED})"
-            else:
-                sfx = ""
-            return f"{name}{sfx}"
-        return None
-
-    def get_radio(self) -> bool | None:
-        """Return Airzone Thermostat radio."""
-        return self.radio
+from .thermostat import Thermostat
 
 
 class Zone:
     """Airzone Zone."""
 
-    def __init__(self, system: System, zone: dict[str, Any]):
+    def __init__(self, system_id: int, zone_id: int, zone_data: dict[str, Any]):
         """Zone init."""
         self.air_demand: bool | None = None
         self.anti_freeze: bool | None = None
+        self.available: bool = True
         self.cold_angle: GrilleAngle | None = None
+        self.cold_demand: bool | None = None
         self.cold_stage: AirzoneStages | None = None
         self.cold_stages: list[AirzoneStages] = []
         self.cool_temp_max: float | None = None
         self.cool_temp_min: float | None = None
         self.cool_temp_set: float | None = None
         self.double_set_point: bool | None = None
-        self.double_set_point_params: bool = zone.keys() >= API_DOUBLE_SET_POINT_PARAMS
         self.eco_adapt: EcoAdapt | None = None
         self.errors: list[str] = []
         self.floor_demand: bool | None = None
         self.heat_angle: GrilleAngle | None = None
+        self.heat_demand: bool | None = None
         self.heat_temp_max: float | None = None
         self.heat_temp_min: float | None = None
         self.heat_temp_set: float | None = None
         self.heat_stage: AirzoneStages | None = None
         self.heat_stages: list[AirzoneStages] = []
         self.humidity: int | None = None
-        self.id = int(zone[API_ZONE_ID])
-        self.master = bool(API_MODES in zone)
+        self.id = zone_id
         self.master_zone: int | None = None
+        self.mode: OperationMode
         self.modes: list[OperationMode] = []
-        self.on = bool(zone[API_ON])
+        self.on: bool
         self.sleep: SleepTimeout | None = None
         self.speed: int | None = None
         self.speeds: list[int] = []
-        self.temp = float(zone[API_ROOM_TEMP])
-        self.temp_max = float(zone[API_MAX_TEMP])
-        self.temp_min = float(zone[API_MIN_TEMP])
-        self.temp_set = float(zone[API_SET_POINT])
+        self.system_id: int = system_id
+        self.system_zone_id: str = get_system_zone_id(system_id, zone_id)
+        self.temp_set: float
+
+        self.name: str = f"Airzone {self.get_system_zone_id()}"
+
+        self.update_data(zone_data)
+
+    def update_data(self, zone_data: dict[str, Any]) -> None:
+        """Update Zone data."""
+        self.set_available(True)
+
+        self.double_set_point_params: bool = (
+            list(zone_data) >= API_DOUBLE_SET_POINT_PARAMS
+        )
+        self.master = bool(API_MODES in zone_data)
+        self.on = bool(zone_data[API_ON])
+        self.temp = float(zone_data[API_ROOM_TEMP])
+        self.temp_max = float(zone_data[API_MAX_TEMP])
+        self.temp_min = float(zone_data[API_MIN_TEMP])
+        self.temp_set = float(zone_data[API_SET_POINT])
         self.temp_step: float | None = None
-        self.temp_unit = TemperatureUnit(zone[API_UNITS])
-        self.thermostat = Thermostat(zone)
-        self.system = system
+        self.temp_unit = TemperatureUnit(zone_data[API_UNITS])
+        self.thermostat = Thermostat(zone_data)
 
-        if API_MASTER_ZONE_ID in zone:
-            master_zone_id = int(zone[API_MASTER_ZONE_ID])
+        if API_MASTER_ZONE_ID in zone_data:
+            master_zone_id = int(zone_data[API_MASTER_ZONE_ID])
             if master_zone_id != self.id:
                 self.master_zone = master_zone_id
 
-        if API_AIR_DEMAND in zone:
-            self.air_demand = bool(zone[API_AIR_DEMAND])
-        if API_FLOOR_DEMAND in zone:
-            self.floor_demand = bool(zone[API_FLOOR_DEMAND])
-
-        if API_ANTI_FREEZE in zone:
-            self.anti_freeze = bool(zone[API_ANTI_FREEZE])
-
-        if API_DOUBLE_SET_POINT in zone:
-            self.double_set_point = bool(zone[API_DOUBLE_SET_POINT])
-
-        if API_ECO_ADAPT in zone:
-            self.eco_adapt = EcoAdapt(zone[API_ECO_ADAPT])
-
-        if API_HUMIDITY in zone:
-            self.humidity = int(zone[API_HUMIDITY])
-
-        if API_COLD_ANGLE in zone:
-            self.cold_angle = GrilleAngle(zone[API_COLD_ANGLE])
-        if API_HEAT_ANGLE in zone:
-            self.heat_angle = GrilleAngle(zone[API_HEAT_ANGLE])
-
-        if API_COLD_STAGE in zone:
-            self.cold_stage = AirzoneStages(zone[API_COLD_STAGE])
-        if API_COLD_STAGES in zone:
-            cold_stages = AirzoneStages(zone[API_COLD_STAGES])
+        if API_AIR_DEMAND in zone_data:
+            self.air_demand = bool(zone_data[API_AIR_DEMAND])
+        if API_FLOOR_DEMAND in zone_data:
+            self.floor_demand = bool(zone_data[API_FLOOR_DEMAND])
+
+        if API_ANTI_FREEZE in zone_data:
+            self.anti_freeze = bool(zone_data[API_ANTI_FREEZE])
+
+        if API_COLD_DEMAND in zone_data:
+            self.cold_demand = bool(zone_data[API_COLD_DEMAND])
+        if API_HEAT_DEMAND in zone_data:
+            self.heat_demand = bool(zone_data[API_HEAT_DEMAND])
+
+        if API_DOUBLE_SET_POINT in zone_data:
+            self.double_set_point = bool(zone_data[API_DOUBLE_SET_POINT])
+
+        if API_ECO_ADAPT in zone_data:
+            self.eco_adapt = EcoAdapt(zone_data[API_ECO_ADAPT])
+
+        if API_HUMIDITY in zone_data:
+            self.humidity = int(zone_data[API_HUMIDITY])
+
+        if API_COLD_ANGLE in zone_data:
+            self.cold_angle = GrilleAngle(zone_data[API_COLD_ANGLE])
+        if API_HEAT_ANGLE in zone_data:
+            self.heat_angle = GrilleAngle(zone_data[API_HEAT_ANGLE])
+
+        if API_COLD_STAGE in zone_data:
+            self.cold_stage = AirzoneStages(zone_data[API_COLD_STAGE])
+        if API_COLD_STAGES in zone_data:
+            cold_stages = AirzoneStages(zone_data[API_COLD_STAGES])
             self.cold_stages = cold_stages.to_list()
         elif self.cold_stage and self.cold_stage.exists():
             self.cold_stages = [self.cold_stage]
 
-        if API_HEAT_STAGE in zone:
-            self.heat_stage = AirzoneStages(zone[API_HEAT_STAGE])
-        if API_HEAT_STAGES in zone:
-            heat_stages = AirzoneStages(zone[API_HEAT_STAGES])
+        if API_HEAT_STAGE in zone_data:
+            self.heat_stage = AirzoneStages(zone_data[API_HEAT_STAGE])
+        if API_HEAT_STAGES in zone_data:
+            heat_stages = AirzoneStages(zone_data[API_HEAT_STAGES])
             self.heat_stages = heat_stages.to_list()
         elif self.heat_stage and self.heat_stage.exists():
             self.heat_stages = [self.heat_stage]
 
-        if API_COOL_MAX_TEMP in zone:
-            self.cool_temp_max = float(zone[API_COOL_MAX_TEMP])
-        if API_COOL_MIN_TEMP in zone:
-            self.cool_temp_min = float(zone[API_COOL_MIN_TEMP])
-        if API_COOL_SET_POINT in zone:
-            self.cool_temp_set = float(zone[API_COOL_SET_POINT])
-        if API_HEAT_MAX_TEMP in zone:
-            self.heat_temp_max = float(zone[API_HEAT_MAX_TEMP])
-        if API_HEAT_MIN_TEMP in zone:
-            self.heat_temp_min = float(zone[API_HEAT_MIN_TEMP])
-        if API_HEAT_SET_POINT in zone:
-            self.heat_temp_set = float(zone[API_HEAT_SET_POINT])
+        if API_COOL_MAX_TEMP in zone_data:
+            self.cool_temp_max = float(zone_data[API_COOL_MAX_TEMP])
+        if API_COOL_MIN_TEMP in zone_data:
+            self.cool_temp_min = float(zone_data[API_COOL_MIN_TEMP])
+        if API_COOL_SET_POINT in zone_data:
+            self.cool_temp_set = float(zone_data[API_COOL_SET_POINT])
+        if API_HEAT_MAX_TEMP in zone_data:
+            self.heat_temp_max = float(zone_data[API_HEAT_MAX_TEMP])
+        if API_HEAT_MIN_TEMP in zone_data:
+            self.heat_temp_min = float(zone_data[API_HEAT_MIN_TEMP])
+        if API_HEAT_SET_POINT in zone_data:
+            self.heat_temp_set = float(zone_data[API_HEAT_SET_POINT])
 
-        if API_ERRORS in zone:
-            errors: list[dict[str, str]] = zone[API_ERRORS]
+        if API_ERRORS in zone_data:
+            errors: list[dict[str, str]] = zone_data[API_ERRORS]
             for error in errors:
                 for key, val in error.items():
                     self.add_error(key, val)
 
-        if API_MODE in zone:
-            self.mode = OperationMode(zone[API_MODE])
+        if API_MODE in zone_data:
+            self.mode = OperationMode(zone_data[API_MODE])
         else:
             self.master = True
             self.mode = OperationMode.AUTO
-            self.modes.append(self.mode)
-
-        if API_NAME in zone:
-            self.name = str(zone[API_NAME])
-        else:
-            self.name = f"Airzone {zone[API_SYSTEM_ID]}:{zone[API_ZONE_ID]}"
-
-        if API_SLEEP in zone:
-            self.sleep = SleepTimeout(zone[API_SLEEP])
+            self.modes = [self.mode]
 
-        if API_SPEED in zone:
-            self.speed = int(zone[API_SPEED])
-        if API_SPEEDS in zone:
-            speeds = int(zone[API_SPEEDS])
+        if self.master:
+            if API_MODES in zone_data:
+                self.modes = []
+                for mode in zone_data[API_MODES]:
+                    self.modes += [OperationMode(mode)]
+
+        if API_NAME in zone_data:
+            self.name = str(zone_data[API_NAME])
+
+        if API_SLEEP in zone_data:
+            self.sleep = SleepTimeout(zone_data[API_SLEEP])
+
+        if API_SPEED in zone_data:
+            self.speed = int(zone_data[API_SPEED])
+        if API_SPEEDS in zone_data:
+            speeds = int(zone_data[API_SPEEDS])
             self.speeds = list(range(0, speeds + 1))
 
-        if API_TEMP_STEP in zone:
-            self.temp_step = float(zone[API_TEMP_STEP])
-
-        if self.master:
-            if API_MODES in zone:
-                for mode in zone[API_MODES]:
-                    self.modes.append(OperationMode(mode))
-            if self.eco_adapt:
-                self.system.set_eco_adapt(self.eco_adapt)
-            self.system.set_mode(self.mode)
-            self.system.set_modes(self.modes)
-            if OperationMode.STOP not in self.modes:
-                self.modes.append(OperationMode.STOP)
+        if API_TEMP_STEP in zone_data:
+            self.temp_step = float(zone_data[API_TEMP_STEP])
         else:
-            if self.eco_adapt and self.system.get_eco_adapt() is None:
-                self.system.set_eco_adapt(self.eco_adapt)
-            if self.system.get_mode() is None:
-                self.system.set_mode(self.mode)
+            if self.temp_unit == TemperatureUnit.FAHRENHEIT:
+                self.temp_step = DEFAULT_TEMP_STEP_FAHRENHEIT
+            else:
+                self.temp_step = DEFAULT_TEMP_STEP_CELSIUS
 
     def data(self) -> dict[str, Any]:
         """Return Airzone zone data."""
         data = {
             AZD_ABS_TEMP_MAX: self.get_abs_temp_max(),
             AZD_ABS_TEMP_MIN: self.get_abs_temp_min(),
             AZD_ACTION: self.get_action(),
+            AZD_AVAILABLE: self.get_available(),
             AZD_DEMAND: self.get_demand(),
             AZD_DOUBLE_SET_POINT: self.get_double_set_point(),
             AZD_ID: self.get_id(),
             AZD_MASTER: self.get_master(),
             AZD_MODE: self.get_mode(),
             AZD_NAME: self.get_name(),
             AZD_ON: self.get_on(),
@@ -571,14 +336,21 @@
         cold_angle = self.get_cold_angle()
         if cold_angle is not None:
             data[AZD_COLD_ANGLE] = cold_angle
         heat_angle = self.get_heat_angle()
         if heat_angle is not None:
             data[AZD_HEAT_ANGLE] = heat_angle
 
+        cold_demand = self.get_cold_demand()
+        if cold_demand is not None:
+            data[AZD_COLD_DEMAND] = cold_demand
+        heat_demand = self.get_heat_demand()
+        if heat_demand is not None:
+            data[AZD_HEAT_DEMAND] = heat_demand
+
         cold_stage = self.get_cold_stage()
         if cold_stage is not None:
             data[AZD_COLD_STAGE] = cold_stage
         cold_stages = self.get_cold_stages()
         if cold_stages is not None:
             data[AZD_COLD_STAGES] = cold_stages
 
@@ -629,21 +401,18 @@
         battery_low = self.get_battery_low()
         if battery_low is not None:
             data[AZD_BATTERY_LOW] = battery_low
 
         return data
 
     def add_error(self, key: str, val: str) -> None:
-        """Add system or zone error."""
+        """Add zone error."""
         _key = key.casefold()
-        if _key == ERROR_SYSTEM:
-            self.system.add_error(val)
-        elif _key == ERROR_ZONE:
-            if val not in self.errors:
-                self.errors.append(val)
+        if _key == ERROR_ZONE and val not in self.errors:
+            self.errors += [val]
 
     def get_abs_temp_max(self) -> float:
         """Return absolute max temp."""
         temps = [
             self.get_cool_temp_max(),
             self.get_heat_temp_max(),
             self.get_temp_max(),
@@ -727,24 +496,32 @@
             if cool_match and not heat_match:
                 return OperationAction.COOLING
             if heat_match and not cool_match:
                 return OperationAction.HEATING
 
         return OperationAction.IDLE
 
+    def get_available(self) -> bool:
+        """Return availability."""
+        return self.available
+
     def get_battery_low(self) -> bool | None:
         """Return battery status."""
         if self.thermostat.get_radio():
             return API_ERROR_LOW_BATTERY in self.errors
         return None
 
     def get_cold_angle(self) -> GrilleAngle | None:
         """Return zone cold angle."""
         return self.cold_angle
 
+    def get_cold_demand(self) -> bool | None:
+        """Return zone cold demand."""
+        return self.cold_demand
+
     def get_cold_stage(self) -> AirzoneStages | None:
         """Return zone cold stage."""
         return self.cold_stage
 
     def get_cold_stages(self) -> list[AirzoneStages] | None:
         """Return zone cold stages."""
         if len(self.cold_stages) > 0:
@@ -805,14 +582,18 @@
         """Return zone ID."""
         return self.id
 
     def get_heat_angle(self) -> GrilleAngle | None:
         """Return zone heat angle."""
         return self.heat_angle
 
+    def get_heat_demand(self) -> bool | None:
+        """Return zone heat demand."""
+        return self.heat_demand
+
     def get_heat_stage(self) -> AirzoneStages | None:
         """Return zone heat stage."""
         return self.heat_stage
 
     def get_heat_stages(self) -> list[AirzoneStages] | None:
         """Return zone heat stages."""
         if len(self.heat_stages) > 0:
@@ -853,34 +634,21 @@
 
     def get_mode(self) -> OperationMode:
         """Return zone mode."""
         return self.mode
 
     def get_modes(self) -> list[OperationMode]:
         """Return zone modes."""
-        if self.master:
-            return self.modes
-
-        modes = None
-        master_zone_id = self.get_master_zone()
-        if master_zone_id is not None:
-            try:
-                master_zone = self.system.get_zone(master_zone_id)
-                modes = master_zone.get_modes()
-            except InvalidZone:
-                pass
+        modes = self.modes
 
-        if modes is None:
-            modes = self.system.get_modes()
-
-        if modes is None:
+        if len(modes) == 0 and self.mode is not None:
             modes = [self.mode]
 
         if OperationMode.STOP not in modes:
-            modes.append(OperationMode.STOP)
+            modes += [OperationMode.STOP]
 
         return modes
 
     def get_name(self) -> str:
         """Return zone name."""
         return self.name
 
@@ -904,19 +672,19 @@
         """Return zone speeds."""
         if len(self.speeds) > 0:
             return self.speeds
         return None
 
     def get_system_id(self) -> int | None:
         """Return system ID."""
-        return self.system.get_id()
+        return self.system_id
 
     def get_system_zone_id(self) -> str:
-        """Combine System and Zone IDs into a single ID."""
-        return f"{self.get_system_id()}:{self.get_id()}"
+        """Return combined system and zone ID."""
+        return self.system_zone_id
 
     def get_temp(self) -> float:
         """Return zone temperature."""
         return round(self.temp, 2)
 
     def get_temp_max(self) -> float:
         """Return zone maximum temperature."""
@@ -954,14 +722,22 @@
             if stage in heat_stages:
                 return True
             if len(heat_stages) == 0:
                 return True
 
         return cold_stages is None and heat_stages is None
 
+    def set_available(self, available: bool) -> None:
+        """Set availability."""
+        self.available = available
+
+    def set_modes(self, modes: list[OperationMode]) -> None:
+        """Set zone modes."""
+        self.modes = modes
+
     def set_param(self, key: str, value: Any) -> None:
         """Update zone parameter by key and value."""
         if key == API_ANTI_FREEZE:
             self.anti_freeze = bool(value)
         elif key == API_COOL_SET_POINT:
             self.cool_temp_set = float(value)
         elif key == API_COLD_ANGLE:
```

### Comparing `aioairzone-0.5.6/aioairzone/exceptions.py` & `aioairzone-0.6.0/aioairzone/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.6/aioairzone/localapi.py` & `aioairzone-0.6.0/aioairzone/localapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,39 +7,38 @@
 from enum import IntEnum
 from json import JSONDecodeError
 from typing import Any, cast
 
 from aiohttp import ClientConnectorError, ClientSession
 from aiohttp.client_reqrep import ClientResponse
 
+from .common import OperationMode, get_system_zone_id
 from .const import (
-    API_COOL_SET_POINT,
     API_DATA,
     API_DEMO,
     API_ERROR_METHOD_NOT_SUPPORTED,
     API_ERROR_REQUEST_MALFORMED,
     API_ERROR_SYSTEM_ID_NOT_AVAILABLE,
     API_ERROR_SYSTEM_ID_OUT_RANGE,
     API_ERROR_ZONE_ID_NOT_AVAILABLE,
     API_ERROR_ZONE_ID_NOT_PROVIDED,
     API_ERROR_ZONE_ID_OUT_RANGE,
     API_ERRORS,
-    API_HEAT_SET_POINT,
     API_HVAC,
     API_INTEGRATION,
     API_MAC,
-    API_SET_POINT,
     API_SYSTEM_ID,
     API_SYSTEM_PARAMS,
     API_SYSTEMS,
     API_V1,
     API_VERSION,
     API_WEBSERVER,
     API_ZONE_ID,
     API_ZONE_PARAMS,
+    AZD_NEW_SYSTEMS,
     AZD_NEW_ZONES,
     AZD_SYSTEMS,
     AZD_SYSTEMS_NUM,
     AZD_VERSION,
     AZD_WEBSERVER,
     AZD_ZONES,
     AZD_ZONES_NUM,
@@ -49,31 +48,31 @@
     RAW_DEMO,
     RAW_HVAC,
     RAW_INTEGRATION,
     RAW_SYSTEMS,
     RAW_VERSION,
     RAW_WEBSERVER,
 )
-from .device import System, Zone
 from .exceptions import (
     APIError,
     InvalidHost,
     InvalidMethod,
     InvalidParam,
     InvalidSystem,
     InvalidZone,
-    ParamUpdateFailure,
     RequestMalformed,
     SystemNotAvailable,
     SystemOutOfRange,
     ZoneNotAvailable,
     ZoneNotProvided,
     ZoneOutOfRange,
 )
+from .system import System
 from .webserver import WebServer
+from .zone import Zone
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ApiFeature(IntEnum):
     """Supported features of the Airzone Local API."""
 
@@ -97,24 +96,25 @@
     def __init__(
         self,
         aiohttp_session: ClientSession,
         options: ConnectionOptions,
     ):
         """Device init."""
         self._api_raw_data: dict[str, Any] = {}
-        self._cached_zones: list[str] = []
         self._first_update: bool = True
-        self._new_zones: bool = False
+        self._new_systems: list[str] = []
+        self._new_zones: list[str] = []
         self.aiohttp_session = aiohttp_session
         self.api_features: int = ApiFeature.HVAC
         self.api_features_checked = False
         self.options = options
         self.systems: dict[int, System] = {}
         self.version: str | None = None
         self.webserver: WebServer | None = None
+        self.zones: dict[str, Zone] = {}
 
     @staticmethod
     def handle_errors(errors: list[dict[str, str]]) -> None:
         """Handle API errors."""
         for error in errors:
             for key, val in error.items():
                 if val == API_ERROR_METHOD_NOT_SUPPORTED:
@@ -143,20 +143,20 @@
             resp: ClientResponse = await self.aiohttp_session.request(
                 method,
                 f"http://{self.options.host}:{self.options.port}/{path}",
                 data=json.dumps(data),
                 timeout=HTTP_CALL_TIMEOUT,
             )
         except ClientConnectorError as err:
-            raise InvalidHost from err
+            raise InvalidHost(err) from err
 
         try:
             resp_json = await resp.json(content_type=None)
         except JSONDecodeError as err:
-            raise InvalidHost from err
+            raise InvalidHost(err) from err
 
         _LOGGER.debug("aiohttp response: %s", resp_json)
         if resp.status != 200:
             if API_ERRORS in resp_json:
                 self.handle_errors(resp_json[API_ERRORS])
             raise APIError(f"HTTP status: {resp.status}")
 
@@ -227,54 +227,112 @@
             raise InvalidHost(f"validate: {API_DATA} not in API response")
 
         if self.webserver:
             return self.webserver.get_mac()
 
         return None
 
-    def detect_zones(self) -> bool:
-        """Check if there are new zones in Airzone data."""
-        new_zones = False
-
-        if self.systems:
-            for system in self.systems.values():
-                for zone in system.zones.values():
-                    zone_id = zone.get_system_zone_id()
-                    if zone_id not in self._cached_zones:
-                        new_zones = True
-                    self._cached_zones.append(zone_id)
-
-        if self._first_update:
-            return False
-
-        return new_zones
-
-    async def update(self) -> bool:
+    async def update(self) -> None:
         """Gather Airzone data."""
-        systems: dict[int, System] = {}
+
+        for system in self.systems.values():
+            system.set_available(False)
+        for zone in self.zones.values():
+            zone.set_available(False)
 
         hvac = await self.get_hvac()
         if self.options.system_id == DEFAULT_SYSTEM_ID:
-            for hvac_system in hvac[API_SYSTEMS]:
-                system = System(hvac_system[API_DATA])
-                if system and (_id := system.get_id()):
-                    systems[_id] = system
+            for system_data in hvac[API_SYSTEMS]:
+                self.parse_system_zones(system_data)
         else:
-            system = System(hvac[API_DATA])
-            if system and (_id := system.get_id()):
-                systems[_id] = system
-        self.systems = systems
+            self.parse_system_zones(hvac)
 
         await self.update_features()
 
-        self._new_zones = self.detect_zones()
-
         self._first_update = False
 
-        return bool(systems)
+    def parse_system_zones(self, system_data: dict[str, Any]) -> None:
+        """Parse all zones from system data."""
+        self._new_systems = []
+        self._new_zones = []
+
+        system_zones: list[dict[str, Any]] = system_data.get(API_DATA, [])
+        for zone_data in system_zones:
+            system_id = int(zone_data.get(API_SYSTEM_ID, 0))
+            if system_id > 0:
+                if system_id not in self.systems:
+                    self.systems[system_id] = System(system_id, zone_data)
+                    self._new_systems += [str(system_id)]
+                else:
+                    self.systems[system_id].update_zone_data(zone_data)
+
+                zone_id = int(zone_data.get(API_ZONE_ID, 0))
+                if zone_id > 0:
+                    system_zone_id = get_system_zone_id(system_id, zone_id)
+
+                    if system_zone_id not in self.zones:
+                        self.zones[system_zone_id] = Zone(system_id, zone_id, zone_data)
+                        self._new_zones += [system_zone_id]
+                    else:
+                        self.zones[system_zone_id].update_data(zone_data)
+
+                    self.update_system_from_zone(
+                        self.systems[system_id], self.zones[system_zone_id]
+                    )
+
+        self.update_zones_from_master_zone()
+
+        if self._first_update:
+            self._new_systems = []
+            self._new_zones = []
+        else:
+            if len(self._new_systems) > 0:
+                _LOGGER.debug("New systems detected: %s", self._new_systems)
+            if len(self._new_zones) > 0:
+                _LOGGER.debug("New zones detected: %s", self._new_zones)
+
+    def update_system_from_zone(self, system: System, zone: Zone) -> None:
+        """Update system data from zone."""
+        if zone.get_master():
+            if (eco_adapt := zone.get_eco_adapt()) is not None:
+                system.set_eco_adapt(eco_adapt)
+
+            system.set_master_system_zone(zone.get_system_zone_id())
+            system.set_master_zone(zone.get_id())
+
+            if (mode := zone.get_mode()) is not None:
+                system.set_mode(mode)
+
+            system.set_modes(zone.get_modes())
+        else:
+            if system.get_eco_adapt() is None:
+                system.set_eco_adapt(zone.get_eco_adapt())
+            if system.get_mode() is None:
+                system.set_mode(zone.get_mode())
+            if len(system.get_modes()) == 0:
+                system.set_modes(zone.get_modes())
+
+    def update_zones_from_master_zone(self) -> None:
+        """Update slave zones data with their master zone."""
+        for zone in self.zones.values():
+            system_id = zone.get_system_id()
+
+            if system_id is not None and not zone.get_master():
+                modes: list[OperationMode] = []
+
+                master_id = zone.get_master_zone()
+                if master_id is None:
+                    system = self.get_system(system_id)
+                    modes = system.get_modes()
+                else:
+                    master_zone = self.get_zone(system_id, master_id)
+                    modes = master_zone.get_modes()
+
+                if len(modes) > 0:
+                    zone.set_modes(modes)
 
     async def get_demo(self) -> dict[str, Any]:
         """Return Airzone demo."""
         res = await self.http_request(
             "POST",
             f"{API_V1}/{API_DEMO}",
         )
@@ -354,92 +412,101 @@
         if API_DATA not in res:
             if API_ERRORS in res:
                 self.handle_errors(res[API_ERRORS])
             raise APIError(f"set_hvac: {API_DATA} not in API response")
 
         data: dict[str, Any] = res[API_DATA][0]
         for key, value in params.items():
-            update_fail = key not in data
-
-            if not update_fail:
-                if key not in [API_COOL_SET_POINT, API_HEAT_SET_POINT, API_SET_POINT]:
-                    update_fail = data[key] != value
-
-            if update_fail:
-                if key == API_SYSTEM_ID and value != 0:
+            if (
+                key in [API_SYSTEM_ID, API_ZONE_ID]
+                and value != 0
+                and data.get(key) != value
+            ):
+                if key == API_SYSTEM_ID:
                     raise InvalidSystem(
                         f"set_hvac: System mismatch: {data.get(key)} vs {value}"
                     )
-                if key == API_ZONE_ID and value != 0:
+                if key == API_ZONE_ID:
                     raise InvalidZone(
                         f"set_hvac: Zone mismatch: {data.get(key)} vs {value}"
                     )
-                if key not in data:
-                    raise InvalidParam(f"set_hvac: param not in data: {key}={value}")
-                raise ParamUpdateFailure(
-                    f"set_hvac: {key} update failure: {data.get(key)} vs {value}"
-                )
+
+            if key not in data:
+                raise InvalidParam(f"set_hvac: param not in data: {key}={value}")
 
         system = self.get_system(data[API_SYSTEM_ID])
         zone = self.get_zone(data[API_SYSTEM_ID], data[API_ZONE_ID])
         for key, value in data.items():
             if key in API_SYSTEM_PARAMS:
                 system.set_param(key, value)
+
+                system_id = system.get_id()
+                for cur_zone in self.zones.values():
+                    if cur_zone.get_system_id() == system_id:
+                        cur_zone.set_param(key, value)
             elif key in API_ZONE_PARAMS:
                 zone.set_param(key, value)
 
         return res
 
-    def new_zones(self) -> bool:
-        """Return if there are new zones in Airzone data."""
+    def new_systems(self) -> list[str]:
+        """Return new systems detected in last update."""
+        return self._new_systems
+
+    def new_zones(self) -> list[str]:
+        """Return new zones detected in last update."""
         return self._new_zones
 
     def raw_data(self) -> dict[str, Any]:
         """Return raw Airzone API data."""
         return self._api_raw_data
 
     def data(self) -> dict[str, Any]:
         """Return Airzone device data."""
-        data: dict[str, Any] = {
-            AZD_NEW_ZONES: self.new_zones(),
-            AZD_SYSTEMS_NUM: self.num_systems(),
-            AZD_ZONES_NUM: self.num_zones(),
-        }
+        data: dict[str, Any] = {}
+
+        data[AZD_NEW_SYSTEMS] = self.new_systems()
 
-        if self.systems:
+        data[AZD_SYSTEMS_NUM] = self.num_systems()
+        if len(self.systems):
             systems: dict[int, Any] = {}
-            zones: dict[str, Any] = {}
             for system_id, system in self.systems.items():
                 systems[system_id] = system.data()
-                for zone in system.zones.values():
-                    zones[zone.get_system_zone_id()] = zone.data()
             data[AZD_SYSTEMS] = systems
-            if self.webserver:
-                data[AZD_WEBSERVER] = self.webserver.data()
+
+        if self.webserver is not None:
+            data[AZD_WEBSERVER] = self.webserver.data()
+
+        data[AZD_NEW_ZONES] = self.new_zones()
+
+        data[AZD_ZONES_NUM] = self.num_zones()
+        if len(self.zones):
+            zones: dict[str, Any] = {}
+            for system_zone_id, zone in self.zones.items():
+                zones[system_zone_id] = zone.data()
             data[AZD_ZONES] = zones
 
         if self.version is not None:
             data[AZD_VERSION] = self.version
 
         return data
 
     def get_system(self, system_id: int) -> System:
         """Return Airzone system."""
-        for system in self.systems.values():
-            if system.get_id() == system_id:
-                return system
-        raise InvalidSystem(f"System {system_id} not present")
+        if system_id not in self.systems:
+            raise InvalidSystem(f"System {system_id} not present")
+        return self.systems[system_id]
 
     def get_zone(self, system_id: int, zone_id: int) -> Zone:
-        """Return Airzone system zone."""
-        return self.get_system(system_id).get_zone(zone_id)
+        """Return Airzone zone."""
+        system_zone_id = get_system_zone_id(system_id, zone_id)
+        if system_zone_id not in self.zones:
+            raise InvalidZone(f"Zone {system_zone_id} not present")
+        return self.zones[system_zone_id]
 
     def num_systems(self) -> int:
-        """Return number of airzone systems."""
+        """Return number of systems."""
         return len(self.systems)
 
     def num_zones(self) -> int:
-        """Return total number of zones."""
-        count = 0
-        for system in self.systems.values():
-            count += system.num_zones()
-        return count
+        """Return number of zones."""
+        return len(self.zones)
```

### Comparing `aioairzone-0.5.6/aioairzone/webserver.py` & `aioairzone-0.6.0/aioairzone/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.6/aioairzone.egg-info/PKG-INFO` & `aioairzone-0.6.0/aioairzone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.5.6
+Version: 0.6.0
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.5.6/pyproject.toml` & `aioairzone-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone"
-version = "0.5.6"
+version = "0.6.0"
 description = "Library to control Airzone devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
@@ -27,10 +27,13 @@
 "Bug Tracker" = "https://github.com/Noltari/aioairzone/issues"
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe = false
 include-package-data = true
 
+[tool.setuptools.package-data]
+"aioairzone_cloud" = ["py.typed"]
+
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```


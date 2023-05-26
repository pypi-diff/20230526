# Comparing `tmp/aioairzone-0.6.0.tar.gz` & `tmp/aioairzone-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-0.6.0.tar", last modified: Fri May 26 14:19:50 2023, max compression
+gzip compressed data, was "aioairzone-0.6.1.tar", last modified: Fri May 26 21:30:57 2023, max compression
```

## Comparing `aioairzone-0.6.0.tar` & `aioairzone-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 14:19:50.424091 aioairzone-0.6.0/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.6.0/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.6.0/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 14:19:50.424091 aioairzone-0.6.0/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.6.0/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 14:19:50.424091 aioairzone-0.6.0/aioairzone/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.6.0/aioairzone/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4647 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6978 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.6.0/aioairzone/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16904 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/localapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.6.0/aioairzone/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     7683 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1565 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/thermostat.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.6.0/aioairzone/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    25111 2023-05-26 14:19:03.000000 aioairzone-0.6.0/aioairzone/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 14:19:50.424091 aioairzone-0.6.0/aioairzone.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      494 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-26 14:19:50.000000 aioairzone-0.6.0/aioairzone.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      996 2023-05-26 14:19:20.000000 aioairzone-0.6.0/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.6.0/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-26 14:19:50.424091 aioairzone-0.6.0/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 21:30:57.139387 aioairzone-0.6.1/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.6.1/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.6.1/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 21:30:57.139387 aioairzone-0.6.1/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.6.1/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 21:30:57.139387 aioairzone-0.6.1/aioairzone/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.6.1/aioairzone/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4647 2023-05-26 14:19:03.000000 aioairzone-0.6.1/aioairzone/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6978 2023-05-26 14:19:03.000000 aioairzone-0.6.1/aioairzone/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.6.1/aioairzone/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16799 2023-05-26 15:45:08.000000 aioairzone-0.6.1/aioairzone/localapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.6.1/aioairzone/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8044 2023-05-26 20:19:09.000000 aioairzone-0.6.1/aioairzone/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1565 2023-05-26 14:19:03.000000 aioairzone-0.6.1/aioairzone/thermostat.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.6.1/aioairzone/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    25108 2023-05-26 20:18:51.000000 aioairzone-0.6.1/aioairzone/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-26 21:30:57.139387 aioairzone-0.6.1/aioairzone.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      494 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-26 21:30:56.000000 aioairzone-0.6.1/aioairzone.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-26 21:30:57.000000 aioairzone-0.6.1/aioairzone.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      996 2023-05-26 21:28:12.000000 aioairzone-0.6.1/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.6.1/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-26 21:30:57.139387 aioairzone-0.6.1/setup.cfg
```

### Comparing `aioairzone-0.6.0/LICENSE` & `aioairzone-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.0/PKG-INFO` & `aioairzone-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.6.0
+Version: 0.6.1
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.6.0/README.md` & `aioairzone-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.0/aioairzone/common.py` & `aioairzone-0.6.1/aioairzone/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.0/aioairzone/const.py` & `aioairzone-0.6.1/aioairzone/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.0/aioairzone/exceptions.py` & `aioairzone-0.6.1/aioairzone/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.0/aioairzone/localapi.py` & `aioairzone-0.6.1/aioairzone/localapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,17 @@
                     self.systems[system_id].update_zone_data(zone_data)
 
                 zone_id = int(zone_data.get(API_ZONE_ID, 0))
                 if zone_id > 0:
                     system_zone_id = get_system_zone_id(system_id, zone_id)
 
                     if system_zone_id not in self.zones:
-                        self.zones[system_zone_id] = Zone(system_id, zone_id, zone_data)
+                        _zone = Zone(system_id, zone_id, zone_data)
+                        self.zones[system_zone_id] = _zone
+                        self.systems[system_id].add_zone(_zone)
                         self._new_zones += [system_zone_id]
                     else:
                         self.zones[system_zone_id].update_data(zone_data)
 
                     self.update_system_from_zone(
                         self.systems[system_id], self.zones[system_zone_id]
                     )
@@ -434,19 +436,14 @@
                 raise InvalidParam(f"set_hvac: param not in data: {key}={value}")
 
         system = self.get_system(data[API_SYSTEM_ID])
         zone = self.get_zone(data[API_SYSTEM_ID], data[API_ZONE_ID])
         for key, value in data.items():
             if key in API_SYSTEM_PARAMS:
                 system.set_param(key, value)
-
-                system_id = system.get_id()
-                for cur_zone in self.zones.values():
-                    if cur_zone.get_system_id() == system_id:
-                        cur_zone.set_param(key, value)
             elif key in API_ZONE_PARAMS:
                 zone.set_param(key, value)
 
         return res
 
     def new_systems(self) -> list[str]:
         """Return new systems detected in last update."""
@@ -463,27 +460,27 @@
     def data(self) -> dict[str, Any]:
         """Return Airzone device data."""
         data: dict[str, Any] = {}
 
         data[AZD_NEW_SYSTEMS] = self.new_systems()
 
         data[AZD_SYSTEMS_NUM] = self.num_systems()
-        if len(self.systems):
+        if len(self.systems) > 0:
             systems: dict[int, Any] = {}
             for system_id, system in self.systems.items():
                 systems[system_id] = system.data()
             data[AZD_SYSTEMS] = systems
 
         if self.webserver is not None:
             data[AZD_WEBSERVER] = self.webserver.data()
 
         data[AZD_NEW_ZONES] = self.new_zones()
 
         data[AZD_ZONES_NUM] = self.num_zones()
-        if len(self.zones):
+        if len(self.zones) > 0:
             zones: dict[str, Any] = {}
             for system_zone_id, zone in self.zones.items():
                 zones[system_zone_id] = zone.data()
             data[AZD_ZONES] = zones
 
         if self.version is not None:
             data[AZD_VERSION] = self.version
```

### Comparing `aioairzone-0.6.0/aioairzone/system.py` & `aioairzone-0.6.1/aioairzone/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     AZD_MASTER_ZONE,
     AZD_MODE,
     AZD_MODEL,
     AZD_MODES,
     AZD_PROBLEMS,
     ERROR_SYSTEM,
 )
+from .zone import Zone
 
 
 class System:
     """Airzone System."""
 
     def __init__(self, system_id: int, zone_data: dict[str, Any]):
         """System init."""
@@ -46,20 +47,21 @@
         self.firmware: str | None = None
         self.manufacturer: str | None = None
         self.master_system_zone: str | None = None
         self.master_zone: int | None = None
         self.mode: OperationMode | None = None
         self.modes: list[OperationMode] = []
         self.type: SystemType | None = None
+        self.zones: dict[int, Zone] = {}
 
         self.update_zone_data(zone_data)
 
     def update_zone_data(self, zone_data: dict[str, Any]) -> None:
         """Update System data."""
-        self.set_available(True)
+        self.available = True
 
         errors: list[dict[str, str]] = zone_data.get(API_ERRORS, [])
         for error in errors:
             for key, val in error.items():
                 self.add_error(val, key)
 
     def data(self) -> dict[str, Any]:
@@ -128,14 +130,20 @@
         if error_id is not None:
             if error_id.casefold() == ERROR_SYSTEM and error not in self.errors:
                 self.errors += [error]
         else:
             if error not in self.errors:
                 self.errors += [error]
 
+    def add_zone(self, zone: Zone) -> None:
+        """Add zone to system."""
+        zone_id = zone.get_id()
+        if zone_id not in self.zones:
+            self.zones[zone_id] = zone
+
     def get_available(self) -> bool:
         """Return availability."""
         return self.available
 
     def get_clamp_meter(self) -> bool | None:
         """Return system clamp meter connection."""
         return self.clamp_meter
@@ -231,17 +239,22 @@
     def set_param(self, key: str, value: Any) -> None:
         """Update parameters by key and value."""
         if key == API_ECO_ADAPT:
             self.eco_adapt = EcoAdapt(value)
         elif key == API_MODE:
             self.mode = OperationMode(value)
 
+        for zone in self.zones.values():
+            zone.set_param(key, value)
+
     def update_data(self, data: dict[str, Any]) -> None:
         """Update system parameters by dict."""
 
+        self.available = True
+
         if API_MC_CONNECTED in data:
             self.clamp_meter = bool(data[API_MC_CONNECTED])
 
         if API_ERRORS in data:
             errors: list[dict[str, str]] = data[API_ERRORS]
             for error in errors:
                 for val in error.values():
```

### Comparing `aioairzone-0.6.0/aioairzone/thermostat.py` & `aioairzone-0.6.1/aioairzone/thermostat.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.0/aioairzone/webserver.py` & `aioairzone-0.6.1/aioairzone/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.6.0/aioairzone/zone.py` & `aioairzone-0.6.1/aioairzone/zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
         self.name: str = f"Airzone {self.get_system_zone_id()}"
 
         self.update_data(zone_data)
 
     def update_data(self, zone_data: dict[str, Any]) -> None:
         """Update Zone data."""
-        self.set_available(True)
+        self.available = True
 
         self.double_set_point_params: bool = (
             list(zone_data) >= API_DOUBLE_SET_POINT_PARAMS
         )
         self.master = bool(API_MODES in zone_data)
         self.on = bool(zone_data[API_ON])
         self.temp = float(zone_data[API_ROOM_TEMP])
```

### Comparing `aioairzone-0.6.0/aioairzone.egg-info/PKG-INFO` & `aioairzone-0.6.1/aioairzone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.6.0
+Version: 0.6.1
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
```

### Comparing `aioairzone-0.6.0/pyproject.toml` & `aioairzone-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone"
-version = "0.6.0"
+version = "0.6.1"
 description = "Library to control Airzone devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```


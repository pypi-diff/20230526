# Comparing `tmp/autotraders-1.2.3.tar.gz` & `tmp/autotraders-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.2.3.tar", last modified: Fri May 26 21:21:38 2023, max compression
+gzip compressed data, was "autotraders-1.2.4.tar", last modified: Fri May 26 21:53:51 2023, max compression
```

## Comparing `autotraders-1.2.3.tar` & `autotraders-1.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 21:21:20.000000 autotraders-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:21:38.194998 autotraders-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 21:21:20.000000 autotraders-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.190998 autotraders-1.2.3/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.190998 autotraders-1.2.3/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.190998 autotraders-1.2.3/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 21:21:20.000000 autotraders-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:21:38.194998 autotraders-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 21:53:37.000000 autotraders-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:53:51.442672 autotraders-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 21:53:37.000000 autotraders-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 21:53:37.000000 autotraders-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:53:51.442672 autotraders-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_util.py
```

### Comparing `autotraders-1.2.3/LICENSE` & `autotraders-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/PKG-INFO` & `autotraders-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.3
+Version: 1.2.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.2.3/README.md` & `autotraders-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders/agent.py` & `autotraders-1.2.4/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders/faction/contract.py` & `autotraders-1.2.4/autotraders/faction/contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from typing import Optional
 
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.util import parse_time
 
@@ -11,24 +12,24 @@
         self.trade_symbol = MapSymbol(data["tradeSymbol"])
         self.destination_symbol = MapSymbol(data["destinationSymbol"])
         self.units_required = data["unitsRequired"]
         self.units_fulfilled = data["unitsFulfilled"]
 
 
 class Contract(SpaceTradersEntity):
-    def __init__(self, contract_id, session: AutoTradersSession, update=True):
+    def __init__(self, contract_id: str, session: AutoTradersSession, update=True):
         self.contract_data = None
         self.accepted: Optional[bool] = None
         self.fulfilled: Optional[bool] = None
-        self.deadline = None
-        self.accept_deadline = None
+        self.deadline: Optional[datetime] = None
+        self.accept_deadline: Optional[datetime] = None
         self.contract_type = None
         self.on_fulfilled: Optional[str] = None
         self.on_accepted: Optional[str] = None
-        self.contract_id = contract_id
+        self.contract_id: str = contract_id
         super().__init__(session, update, "my/contracts/" + self.contract_id)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.on_accepted = data["terms"]["payment"]["onAccepted"]
         self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
```

### Comparing `autotraders-1.2.3/autotraders/map/system.py` & `autotraders-1.2.4/autotraders/map/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from autotraders.session import AutoTradersSession
 from autotraders.map.waypoint import Waypoint
 from autotraders.shared_models.map_symbol import MapSymbol
 
 
 class System(SpaceTradersEntity):
     def __init__(self, symbol, session: AutoTradersSession, update=True):
-        self.symbol = MapSymbol(symbol)
+        self.symbol: MapSymbol = MapSymbol(symbol)
         self.x: Optional[int] = None
         self.y: Optional[int] = None
         self.waypoints: Optional[list[Waypoint]] = None
         self.factions: Optional[list[str]] = None
         self.star_type: Optional[str] = None
         super().__init__(session, update, "systems/" + str(self.symbol) + "/")
```

### Comparing `autotraders-1.2.3/autotraders/map/waypoint.py` & `autotraders-1.2.4/autotraders/map/waypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
 
 
 class Waypoint(SpaceTradersEntity):
     def __init__(self, symbol, session: AutoTradersSession, update=True):
         self.waypoint_type: Optional[str] = None
-        self.faction = None
-        self.traits = None
+        self.faction: Optional[str] = None
+        self.traits: Optional[list[Trait]] = []
         self.marketplace: Optional[bool] = None
         self.shipyard: Optional[bool] = None
         self.symbol = MapSymbol(symbol)
         self.x: Optional[int] = None
         self.y: Optional[int] = None
         super().__init__(
             session,
```

### Comparing `autotraders-1.2.3/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.2.4/autotraders/map/waypoint_types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from autotraders.shared_models.map_symbol import MapSymbol
 
 
 class WaypointType(SpaceTradersEntity):
     def __init__(
         self, waypoint: str, trait: str, session: AutoTradersSession, update=True
     ):
-        self.location = MapSymbol(waypoint)
+        self.location: MapSymbol = MapSymbol(waypoint)
         super().__init__(
             session,
             update,
             "systems/"
             + self.location.system
             + "/waypoints/"
             + self.location.waypoint
```

### Comparing `autotraders-1.2.3/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.2.4/autotraders/map/waypoint_types/marketplace.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from typing import Optional
+
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
 
 
 class TradeGood:
     def __init__(self, data):
-        self.symbol = data["symbol"]
-        self.trade_volume = data["tradeVolume"]
-        self.supply = data["supply"]
-        self.purchase_price = data["purchasePrice"]
-        self.sell_price = data["sellPrice"]
+        self.symbol: str = data["symbol"]
+        self.trade_volume: int = data["tradeVolume"]
+        self.supply: str = data["supply"]
+        self.purchase_price: int = data["purchasePrice"]
+        self.sell_price: int = data["sellPrice"]
 
 
 class Marketplace(WaypointType):
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
-        self.imports = None
-        self.exports = None
-        self.exchange = None
-        self.trade_goods = None
+        self.imports: Optional[list[str]] = None
+        self.exports: Optional[list[str]] = None
+        self.exchange: Optional[list[str]] = None
+        self.trade_goods: Optional[list[TradeGood]] = None
         super().__init__(waypoint, "market", session, update)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
```

### Comparing `autotraders-1.2.3/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.2.4/autotraders/map/waypoint_types/shipyard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
 from autotraders.ship import Frame, Reactor, Engine, Module, Mount
 
 
 class ShipyardShip:
     def __init__(self, data):
@@ -14,16 +16,16 @@
         self.engine = Engine(data["engine"])
         self.modules = [Module(d) for d in data["modules"]]
         self.mounts = [Mount(d) for d in data["mounts"]]
 
 
 class Shipyard(WaypointType):
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
-        self.ship_types = None
-        self.ships = None
+        self.ship_types: Optional[list[str]] = None
+        self.ships: Optional[list[ShipyardShip]] = None
         super().__init__(waypoint, "shipyard", session, update)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
```

### Comparing `autotraders-1.2.3/autotraders/session.py` & `autotraders-1.2.4/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders/shared_models/map_symbol.py` & `autotraders-1.2.4/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders/ship/__init__.py` & `autotraders-1.2.4/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders/ship/ship_components.py` & `autotraders-1.2.4/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders/space_traders_entity.py` & `autotraders-1.2.4/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders/status.py` & `autotraders-1.2.4/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/autotraders.egg-info/PKG-INFO` & `autotraders-1.2.4/autotraders.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.3
+Version: 1.2.4
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.2.3/autotraders.egg-info/SOURCES.txt` & `autotraders-1.2.4/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/pyproject.toml` & `autotraders-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.2.3/tests/test_init.py` & `autotraders-1.2.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/tests/test_ship.py` & `autotraders-1.2.4/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.3/tests/test_util.py` & `autotraders-1.2.4/tests/test_util.py`

 * *Files identical despite different names*


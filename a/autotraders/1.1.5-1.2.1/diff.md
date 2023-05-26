# Comparing `tmp/autotraders-1.1.5.tar.gz` & `tmp/autotraders-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.1.5.tar", last modified: Wed May 24 04:56:45 2023, max compression
+gzip compressed data, was "autotraders-1.2.1.tar", last modified: Fri May 26 20:23:02 2023, max compression
```

## Comparing `autotraders-1.1.5.tar` & `autotraders-1.2.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.956564 autotraders-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-24 04:56:33.000000 autotraders-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-24 04:56:45.956564 autotraders-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 04:56:33.000000 autotraders-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.952564 autotraders-1.1.5/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.952564 autotraders-1.1.5/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.952564 autotraders-1.1.5/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.952564 autotraders-1.1.5/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.956564 autotraders-1.1.5/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.956564 autotraders-1.1.5/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 04:56:33.000000 autotraders-1.1.5/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.952564 autotraders-1.1.5/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-24 04:56:45.000000 autotraders-1.1.5/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-24 04:56:45.000000 autotraders-1.1.5/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 04:56:45.000000 autotraders-1.1.5/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 04:56:45.000000 autotraders-1.1.5/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 04:56:33.000000 autotraders-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 04:56:45.956564 autotraders-1.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:45.956564 autotraders-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 04:56:33.000000 autotraders-1.1.5/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-24 04:56:33.000000 autotraders-1.1.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-24 04:56:33.000000 autotraders-1.1.5/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 20:22:45.000000 autotraders-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:23:02.765131 autotraders-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 20:22:45.000000 autotraders-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.761131 autotraders-1.2.1/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.761131 autotraders-1.2.1/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 20:22:45.000000 autotraders-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:23:02.765131 autotraders-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:45.000000 autotraders-1.2.1/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-26 20:22:45.000000 autotraders-1.2.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 20:22:45.000000 autotraders-1.2.1/tests/test_util.py
```

### Comparing `autotraders-1.1.5/LICENSE` & `autotraders-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.5/PKG-INFO` & `autotraders-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.5
+Version: 1.2.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.5/README.md` & `autotraders-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.5/autotraders/agent.py` & `autotraders-1.2.1/autotraders/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.contracts = None
         self.starting_faction = None
         self.symbol = None
         self.account_id = None
         self.credits = None
         self.ships = None
         self.headquarters = None
-        super().__init__(session, update, session.base_url + "my/agent")
+        super().__init__(session, update, "my/agent")
 
     def update(self, data=None):
         """Uses 3 API requests to get all agent details"""
         if data is None:
             data = self.get()["data"]
         self.account_id = data["accountId"]
         self.symbol = data["symbol"]
```

### Comparing `autotraders-1.1.5/autotraders/faction/__init__.py` & `autotraders-1.2.1/autotraders/faction/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, symbol, session: AutoTradersSession, update=True):
         self.is_recruting = None
         self.traits = None
         self.headquarters = None
         self.description = None
         self.name = None
         self.symbol = symbol
-        super().__init__(session, update, session.base_url + "factions/" + self.symbol)
+        super().__init__(session, update, "factions/" + self.symbol)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.name = data["name"]
         self.description = data["description"]
         self.headquarters = MapSymbol(data["headquarters"])
```

### Comparing `autotraders-1.1.5/autotraders/faction/contract.py` & `autotraders-1.2.1/autotraders/faction/contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         self.fulfilled: Optional[bool] = None
         self.deadline = None
         self.accept_deadline = None
         self.contract_type = None
         self.on_fulfilled: Optional[str] = None
         self.on_accepted: Optional[str] = None
         self.contract_id = contract_id
-        super().__init__(
-            session, update, session.base_url + "my/contracts/" + self.contract_id
-        )
+        super().__init__(session, update, "my/contracts/" + self.contract_id)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.on_accepted = data["terms"]["payment"]["onAccepted"]
         self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
         self.accepted = data["accepted"]
@@ -49,30 +47,29 @@
     def deliver(self, symbol, cargo_symbol, amount):
         j = self.post(
             "deliver",
             data={"shipSymbol": symbol, "tradeSymbol": cargo_symbol, "units": amount},
         )
         self.update(j["data"]["contract"])
 
-    def negotiate(self, ship_symbol, session):
+    @staticmethod
+    def negotiate(ship_symbol, session):
         j = session.post(
-            self.session.base_url + "my/ships/" + ship_symbol + "/negotiate/contract"
+            session.base_url + "my/ships/" + ship_symbol + "/negotiate/contract"
         ).json()
         if "error" in j:
             raise IOError(j["error"]["message"])
-        c = Contract(j["data"]["id"], self.session, False)
-        c.update(j["data"])
+        print(j)
+        c = Contract(j["data"]["contract"]["id"], session, False)
+        c.update(j["data"]["contract"])
         return c
 
     def fulfill(self):
-        j = self.session.post(
-            self.session.base_url + "my/contracts/" + self.contract_id + "/fulfill"
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("fulfill")
+        self.update(j["data"]["contract"])
 
     @staticmethod
     def all(session, page: int = 1):
         r = session.get(session.base_url + "my/contracts?page=" + str(page))
         j = r.json()
         contracts = []
         for contract in j["data"]:
```

### Comparing `autotraders-1.1.5/autotraders/map/system.py` & `autotraders-1.2.1/autotraders/map/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,15 @@
     def __init__(self, symbol, session: AutoTradersSession, update=True):
         self.symbol = MapSymbol(symbol)
         self.x: Optional[int] = None
         self.y: Optional[int] = None
         self.waypoints: Optional[list[Waypoint]] = None
         self.factions: Optional[list[str]] = None
         self.star_type: Optional[str] = None
-        super().__init__(
-            session, update, session.base_url + "systems/" + str(self.symbol) + "/"
-        )
+        super().__init__(session, update, "systems/" + str(self.symbol) + "/")
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.waypoints = []
         self.x = data["x"]
         self.y = data["y"]
@@ -43,8 +41,8 @@
         return systems, r.json()["meta"]["total"]
 
     def __eq__(self, other):
         return self.symbol == other.symbol
 
 
 def list_systems(session, page=1) -> (list[System], int):
-    System.all(session, page)
+    return System.all(session, page)
```

### Comparing `autotraders-1.1.5/autotraders/map/waypoint.py` & `autotraders-1.2.1/autotraders/map/waypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         self.faction = None
         self.traits = None
         self.marketplace: Optional[bool] = None
         self.shipyard: Optional[bool] = None
         self.symbol = MapSymbol(symbol)
         self.x: Optional[int] = None
         self.y: Optional[int] = None
-        super().__init__(session, update, session.base_url
-                         + "systems/"
-                         + self.symbol.system
-                         + "/waypoints/"
-                         + self.symbol.waypoint)
+        super().__init__(
+            session,
+            update,
+            "systems/" + self.symbol.system + "/waypoints/" + self.symbol.waypoint,
+        )
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.waypoint_type = data["type"]
         self.x = data["x"]
         self.y = data["y"]
@@ -34,18 +34,18 @@
         else:
             self.faction = None
         self.traits = []
         if "traits" in data:
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
         self.marketplace = (
-                len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
         )
         self.shipyard = (
-                len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
         )
 
     @staticmethod
     def all(system, session) -> (list, int):
         r = session.get(session.base_url + "systems/" + system + "/waypoints?limit=20")
         data = r.json()["data"]
         waypoints = []
```

### Comparing `autotraders-1.1.5/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.2.1/autotraders/map/waypoint_types/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     def __init__(
         self, waypoint: str, trait: str, session: AutoTradersSession, update=True
     ):
         self.location = MapSymbol(waypoint)
         super().__init__(
             session,
             update,
-            session.base_url
-            + "systems/"
+            "systems/"
             + self.location.system
             + "/waypoints/"
             + self.location.waypoint
             + "/"
             + trait
             + "/",
         )
```

### Comparing `autotraders-1.1.5/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.2.1/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.5/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.2.1/autotraders/map/waypoint_types/marketplace.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
         self.supply = data["supply"]
         self.purchase_price = data["purchasePrice"]
         self.sell_price = data["sellPrice"]
 
 
 class Marketplace(WaypointType):
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
-        super().__init__(waypoint, "market", session, update)
         self.imports = None
         self.exports = None
         self.exchange = None
         self.trade_goods = None
+        super().__init__(waypoint, "market", session, update)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
                 + self.location.system
```

### Comparing `autotraders-1.1.5/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.2.1/autotraders/map/waypoint_types/shipyard.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         self.engine = Engine(data["engine"])
         self.modules = [Module(d) for d in data["modules"]]
         self.mounts = [Mount(d) for d in data["mounts"]]
 
 
 class Shipyard(WaypointType):
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
-        super().__init__(waypoint, "shipyard", session, update)
         self.ship_types = None
         self.ships = None
+        super().__init__(waypoint, "shipyard", session, update)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
                 + self.location.system
@@ -35,14 +35,14 @@
         self.ship_types = []
         for ship_type in data["shipTypes"]:
             self.ship_types.append(ship_type["type"])
         self.ships = None
         if "ships" in data:
             self.ships = []
             for ship in data["ships"]:
-                ShipyardShip(ship)
+                self.ships.append(ShipyardShip(ship))
 
     def purchase(self, ship_type: str):
         self.session.post(
             self.session.base_url + "my/ships",
             data={"shipType": ship_type, "waypointSymbol": self.location},
         )
```

### Comparing `autotraders-1.1.5/autotraders/shared_models/map_symbol.py` & `autotraders-1.2.1/autotraders/shared_models/map_symbol.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,37 @@
         """Your input must be a valid symbol for a sector, system, or waypoint. or a value error might be raised.
         :param s: The symbol
         """
         if type(s) is MapSymbol:
             s = str(s)
         split = s.split("-")
         self.sector = split[0]
+        # TODO: Wait till stoplight is fixed
+        # if len(self.sector) != 2:
+        #     raise ValueError("Invalid map symbol")
         self.system = None
         self.waypoint = None
         if len(split) > 1:
             self.system = split[0] + "-" + split[1]
         if len(split) > 2:
             self.waypoint = split[0] + "-" + split[1] + "-" + split[2]
         if len(split) > 3:
             raise ValueError("Invalid map symbol")
         self.raw = s
 
     def __str__(self):
         """Returns the input that was passed as a string."""
         return self.raw
 
-    def __div__(self, other):
+    def __truediv__(self, other):
         """Concatenates with a '-'"""
         assert isinstance(other, str)
         if other[0] == "-":
             other = other[1:]
         return MapSymbol(str(self) + "-" + other)
 
     def __eq__(self, other):
-        return self.sector == other.sector and self.system == other.system and self.waypoint == other.waypoint
+        return (
+            self.sector == other.sector
+            and self.system == other.system
+            and self.waypoint == other.waypoint
+        )
```

### Comparing `autotraders-1.1.5/autotraders/ship/__init__.py` & `autotraders-1.2.1/autotraders/ship/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,15 @@
         self.symbol: str = symbol
         self.frame: Optional[Frame] = None
         self.reactor: Optional[Reactor] = None
         self.engine: Optional[Engine] = None
         self.modules: Optional[list[Module]] = None
         self.mounts: Optional[list[Mount]] = None
         self.crew: Optional[Crew] = None
-        super().__init__(
-            session, update, session.base_url + "my/ships/" + self.symbol + "/"
-        )
+        super().__init__(session, update, "my/ships/" + self.symbol + "/")
 
     def update(self, data: dict = None, hard=False):
         if data is None:
             data = self.get()["data"]
 
         def go_for_update(d, s):
             return s in data and (d is None or hard)
@@ -253,15 +251,15 @@
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return waypoints
 
     def scan_ships(self):
         j = self.post("scan/ships")
         ships = []
         for ship in j["data"]["ships"]:
-            s = Ship(ship["data"], self.session, False)
+            s = Ship(ship, self.session, False)
             s.update(ship)
             ships.append(s)
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return ships
 
     def update_ship_cooldown(self):
         j = self.get("cooldown")
```

### Comparing `autotraders-1.1.5/autotraders/ship/ship_components.py` & `autotraders-1.2.1/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.5/autotraders/space_traders_entity.py` & `autotraders-1.2.1/autotraders/space_traders_entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 from autotraders import AutoTradersSession
 
 
 class SpaceTradersEntity:
     def __init__(self, session: AutoTradersSession, update, action_url):
         self.session: AutoTradersSession = session
-        self.action_url = action_url
+        self.action_url = (
+            session.base_url + action_url
+        )
         if self.action_url[-1] != "/":
             self.action_url += "/"
         if update:
             self.update()
 
     def get(self, action: str = None) -> dict:
         if action is None:
-            r = self.session.get(self.action_url[0 : len(self.action_url) - 1]) # noqa E203
+            r = self.session.get(
+                self.action_url[0 : len(self.action_url) - 1]  # noqa E203
+            )
         else:
             r = self.session.get(
                 self.action_url + action,
             )
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
```

### Comparing `autotraders-1.1.5/autotraders/status.py` & `autotraders-1.2.1/autotraders/status.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime
 
 import requests
 
+from autotraders.util import parse_time
+
 
 class LeaderboardPlayer:
     symbol: str
     value: int
 
 
 class Leaderboard:
@@ -40,25 +42,30 @@
     leaderboards: list[Leaderboard]
     next_reset: datetime
     reset_frequency: str
     announcements: list[Announcement]
     links: list[Link]
 
 
-def get_status() -> Status:
+def get_status(session=None) -> Status:
     """returns the API status, with reset dates, see the Status class for more info."""
-    r = requests.get("https://api.spacetraders.io/v2/")
+    if session is None:
+        r = requests.get("https://api.spacetraders.io/v2/")
+    else:
+        r = session.get("https://api.spacetraders.io/v2/")
     j = r.json()
+    if "error" in j:
+        raise IOError(j["error"]["message"])
     s = Status()
     s.status = j["status"]
     s.version = j["version"]
-    s.reset_date = j["resetDate"]
+    s.reset_date = parse_time(j["resetDate"])
     s.description = j["description"]
     s.stats = j["stats"]
-    s.next_reset = j["serverResets"]["nextReset"]
+    s.next_reset = parse_time(j["serverResets"]["next"])
     s.reset_frequency = j["serverResets"]["frequency"]
     s.announcements = []
     for announcement in j["announcements"]:
         s.announcements.append(
             Announcement(title=announcement["title"], body=announcement["body"])
         )
     s.links = []
```

### Comparing `autotraders-1.1.5/autotraders.egg-info/PKG-INFO` & `autotraders-1.2.1/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.5
+Version: 1.2.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.5/autotraders.egg-info/SOURCES.txt` & `autotraders-1.2.1/autotraders.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 autotraders/space_traders_entity.py
 autotraders/status.py
 autotraders/transaction.py
 autotraders/util.py
 autotraders.egg-info/PKG-INFO
 autotraders.egg-info/SOURCES.txt
 autotraders.egg-info/dependency_links.txt
+autotraders.egg-info/requires.txt
 autotraders.egg-info/top_level.txt
 autotraders/faction/__init__.py
 autotraders/faction/contract.py
 autotraders/map/__init__.py
 autotraders/map/system.py
 autotraders/map/waypoint.py
 autotraders/map/waypoint_types/__init__.py
```

### Comparing `autotraders-1.1.5/pyproject.toml` & `autotraders-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.1.5"
+version = "1.2.1"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "requests>=2.20",
+    "requests-ratelimiter >=0.4"
+]
 
 [tool.setuptools.packages.find]
 include = ["autotraders*"]
 exclude = ["source*", "tests*", "venv*"]
 
 [project.urls]
 "Homepage" = "https://arihant2math.github.io/autotraders/"
```

### Comparing `autotraders-1.1.5/tests/test_init.py` & `autotraders-1.2.1/tests/test_init.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,89 @@
+import time
+
 import pytest
 
+from autotraders import get_status
 from autotraders.agent import Agent
+from autotraders.faction import Faction
 from autotraders.session import get_session
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship import Ship
 from autotraders.faction.contract import Contract
 
 
 @pytest.fixture
 def session():
-    s = get_session("BLANK")
+    s = get_session(None)
     s.base_url = "https://stoplight.io/mocks/spacetraders/spacetraders/96627693/"
     return s
 
 
 def test_invalid_api_key():
     s = get_session("TEST")
     try:
         Agent(s)
         assert False  # shouldn't complete successfully
     except Exception as e:
         assert type(e) is IOError
 
 
+def test_get_status():
+    status = get_status()
+    assert status.version == "v2"
+
+
+def test_rate_limiter(session):
+    t1 = time.time()
+    for i in range(20):
+        get_status(session)
+    t2 = time.time()
+    assert t2-t1 < 100
+
+
 def test_agent(session):
-    a = Agent(session)
-    assert a.credits == 0
-    assert a.symbol == "string"
+    Agent(session)
 
 
 def test_ship(session):
     Ship("TEST", session)
 
 
 def test_ship_functions(session):
     s = Ship("TEST", session)
+    s.update_ship_cooldown()
     s.dock()
     s.orbit()
     s.refuel()
     s.extract()
 
 
 def test_ship_param_functions(session):
     s = Ship("TEST-1", session)
     s.navigate("X1-TEST-TEST")
+    s.patch_navigation("DRIFT")
     s.jump(MapSymbol("X1-TEST-TEST"))
     s.warp("X1-TEST-TEST")
     s.sell("FUEL", 42)
     s.buy("FUEL", 42)
     s.refine("FUEL")
     s.transfer("TEST-2", "FUEL", 42)
+    s.jettison("FUEL", 42)
 
 
 def test_contact(session):
     Contract("blah", session)
 
 
 def test_contact_functions(session):
     c = Contract("blah", session)
     c.accept()
     c.fulfill()
+
+
+def test_contact_param_functions(session):
+    c = Contract.negotiate("TEST-1", session)
     c.deliver("TEST-1", "GOLD", 5)
+
+
+def test_faction(session):
+    Faction.all(session)
```


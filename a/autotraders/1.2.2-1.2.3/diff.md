# Comparing `tmp/autotraders-1.2.2.tar.gz` & `tmp/autotraders-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.2.2.tar", last modified: Fri May 26 20:42:17 2023, max compression
+gzip compressed data, was "autotraders-1.2.3.tar", last modified: Fri May 26 21:21:38 2023, max compression
```

## Comparing `autotraders-1.2.2.tar` & `autotraders-1.2.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 20:41:56.000000 autotraders-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:42:17.412455 autotraders-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 20:41:56.000000 autotraders-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.408455 autotraders-1.2.2/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.408455 autotraders-1.2.2/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.408455 autotraders-1.2.2/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 20:41:56.000000 autotraders-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:42:17.412455 autotraders-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:41:56.000000 autotraders-1.2.2/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-26 20:41:56.000000 autotraders-1.2.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 20:41:56.000000 autotraders-1.2.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 21:21:20.000000 autotraders-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:21:38.194998 autotraders-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 21:21:20.000000 autotraders-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.190998 autotraders-1.2.3/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.190998 autotraders-1.2.3/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 21:21:20.000000 autotraders-1.2.3/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.190998 autotraders-1.2.3/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 21:21:38.000000 autotraders-1.2.3/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 21:21:20.000000 autotraders-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:21:38.194998 autotraders-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:21:38.194998 autotraders-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 21:21:20.000000 autotraders-1.2.3/tests/test_util.py
```

### Comparing `autotraders-1.2.2/LICENSE` & `autotraders-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/PKG-INFO` & `autotraders-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.2
+Version: 1.2.3
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.2.2/README.md` & `autotraders-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/faction/__init__.py` & `autotraders-1.2.3/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/faction/contract.py` & `autotraders-1.2.3/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/map/system.py` & `autotraders-1.2.3/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/map/waypoint.py` & `autotraders-1.2.3/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.2.3/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.2.3/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.2.3/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.2.3/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/session.py` & `autotraders-1.2.3/autotraders/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional
 
 import requests
-from pyrate_limiter import Limiter, RequestRate, Duration
 from requests_ratelimiter import LimiterSession
 
 
 class BearerAuth(requests.auth.AuthBase):
     def __init__(self, token):
         self.token = token
```

### Comparing `autotraders-1.2.2/autotraders/shared_models/map_symbol.py` & `autotraders-1.2.3/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/ship/__init__.py` & `autotraders-1.2.3/autotraders/ship/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from datetime import datetime, timezone
 from typing import Union, Optional
 
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
@@ -31,26 +32,26 @@
             self.current += symbol["units"]
 
 
 class Route:
     def __init__(self, data):
         self.destination = MapSymbol(data["destination"]["symbol"])
         self.departure = MapSymbol(data["departure"]["symbol"])
-        self.moving = self.destination != self.departure
-        if self.moving:
-            self.departure_time = parse_time(data["departureTime"])
-            self.arrival = parse_time(data["arrival"])
+        self.departure_time = parse_time(data["departureTime"])
+        self.arrival = parse_time(data["arrival"])
+        self.moving = self.arrival > datetime.now(timezone.utc)
 
 
 class Nav:
     def __init__(self, data):
         self.status = data["status"]
         self.location = MapSymbol(data["waypointSymbol"])
         self.flight_mode = data["flightMode"]
         self.route = Route(data["route"])
+        self.moving = self.route.moving
 
 
 class Crew:
     def __init__(self, data):
         self.current = data["current"]
         self.required = data["required"]
         self.capacity = data["capacity"]
```

### Comparing `autotraders-1.2.2/autotraders/ship/ship_components.py` & `autotraders-1.2.3/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/space_traders_entity.py` & `autotraders-1.2.3/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders/status.py` & `autotraders-1.2.3/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.2/autotraders.egg-info/PKG-INFO` & `autotraders-1.2.3/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.2
+Version: 1.2.3
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.2.2/autotraders.egg-info/SOURCES.txt` & `autotraders-1.2.3/autotraders.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 autotraders/map/waypoint_types/marketplace.py
 autotraders/map/waypoint_types/shipyard.py
 autotraders/shared_models/map_symbol.py
 autotraders/shared_models/trait.py
 autotraders/ship/__init__.py
 autotraders/ship/ship_components.py
 autotraders/ship/survey.py
-tests/test_agent.py
+tests/test_contract.py
 tests/test_init.py
+tests/test_ship.py
 tests/test_util.py
```

### Comparing `autotraders-1.2.2/pyproject.toml` & `autotraders-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.2.2/tests/test_init.py` & `autotraders-1.2.3/tests/test_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import pytest
 
 from autotraders import get_status
 from autotraders.agent import Agent
 from autotraders.faction import Faction
 from autotraders.session import get_session
-from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.ship import Ship
-from autotraders.faction.contract import Contract
 
 
 @pytest.fixture
 def session():
     s = get_session(None)
     s.base_url = "https://stoplight.io/mocks/spacetraders/spacetraders/96627693/"
     return s
@@ -33,57 +30,16 @@
 
 
 def test_rate_limiter(session):
     t1 = time.time()
     for i in range(20):
         get_status(session)
     t2 = time.time()
-    assert t2-t1 < 100
+    assert t2 - t1 < 100
 
 
 def test_agent(session):
     Agent(session)
 
 
-def test_ship(session):
-    Ship("TEST", session)
-
-
-def test_ship_functions(session):
-    s = Ship("TEST", session)
-    s.update_ship_cooldown()
-    s.dock()
-    s.orbit()
-    s.refuel()
-    s.extract()
-
-
-def test_ship_param_functions(session):
-    s = Ship("TEST-1", session)
-    s.navigate("X1-TEST-TEST")
-    s.patch_navigation("DRIFT")
-    s.jump(MapSymbol("X1-TEST-TEST"))
-    s.warp("X1-TEST-TEST")
-    s.sell("FUEL", 42)
-    s.buy("FUEL", 42)
-    s.refine("FUEL")
-    s.transfer("TEST-2", "FUEL", 42)
-    s.jettison("FUEL", 42)
-
-
-def test_contact(session):
-    Contract("blah", session)
-
-
-def test_contact_functions(session):
-    c = Contract("blah", session)
-    c.accept()
-    c.fulfill()
-
-
-def test_contact_param_functions(session):
-    c = Contract.negotiate("TEST-1", session)
-    c.deliver("TEST-1", "GOLD", 5)
-
-
 def test_faction(session):
     Faction.all(session)
```

### Comparing `autotraders-1.2.2/tests/test_util.py` & `autotraders-1.2.3/tests/test_util.py`

 * *Files identical despite different names*


# Comparing `tmp/autotraders-1.2.1.tar.gz` & `tmp/autotraders-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.2.1.tar", last modified: Fri May 26 20:23:02 2023, max compression
+gzip compressed data, was "autotraders-1.2.2.tar", last modified: Fri May 26 20:42:17 2023, max compression
```

## Comparing `autotraders-1.2.1.tar` & `autotraders-1.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 20:22:45.000000 autotraders-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:23:02.765131 autotraders-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 20:22:45.000000 autotraders-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.761131 autotraders-1.2.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 20:22:45.000000 autotraders-1.2.1/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.761131 autotraders-1.2.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 20:23:02.000000 autotraders-1.2.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 20:22:45.000000 autotraders-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:23:02.765131 autotraders-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:23:02.765131 autotraders-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:22:45.000000 autotraders-1.2.1/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-26 20:22:45.000000 autotraders-1.2.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 20:22:45.000000 autotraders-1.2.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 20:41:56.000000 autotraders-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:42:17.412455 autotraders-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 20:41:56.000000 autotraders-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.408455 autotraders-1.2.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.408455 autotraders-1.2.2/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 20:41:56.000000 autotraders-1.2.2/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.408455 autotraders-1.2.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 20:42:17.000000 autotraders-1.2.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 20:41:56.000000 autotraders-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:42:17.412455 autotraders-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:42:17.412455 autotraders-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:41:56.000000 autotraders-1.2.2/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-26 20:41:56.000000 autotraders-1.2.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 20:41:56.000000 autotraders-1.2.2/tests/test_util.py
```

### Comparing `autotraders-1.2.1/LICENSE` & `autotraders-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/PKG-INFO` & `autotraders-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.1
+Version: 1.2.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.2.1/README.md` & `autotraders-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/agent.py` & `autotraders-1.2.2/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/faction/__init__.py` & `autotraders-1.2.2/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/faction/contract.py` & `autotraders-1.2.2/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/map/system.py` & `autotraders-1.2.2/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/map/waypoint.py` & `autotraders-1.2.2/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.2.2/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.2.2/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.2.2/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.2.2/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/session.py` & `autotraders-1.2.2/autotraders/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,21 +12,18 @@
     def __call__(self, r):
         r.headers["authorization"] = "Bearer " + self.token
         return r
 
 
 class AutoTradersSession(LimiterSession):
     def __init__(self, base_url="https://api.spacetraders.io/v2/"):
-        second_rate = RequestRate(2, Duration.SECOND)
-        burst_rate = RequestRate(10, Duration.SECOND * 10)
-        limiter = Limiter(second_rate, burst_rate)
-        super().__init__(limiter=limiter, limit_statuses=[429, 502])
+        super().__init__(per_second=2, burst_rate=10, limit_statuses=[429, 502])
         self.base_url = base_url
         self.headers.update({"Prefer": "dynamic=true"})
 
 
-def get_session(token: Optional[str]) -> AutoTradersSession:
+def get_session(token: Optional[str] = None) -> AutoTradersSession:
     """Creates a session with the provided token."""
     s = AutoTradersSession()
     if token is not None:
         s.auth = BearerAuth(token)
     return s
```

### Comparing `autotraders-1.2.1/autotraders/shared_models/map_symbol.py` & `autotraders-1.2.2/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/ship/__init__.py` & `autotraders-1.2.2/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/ship/ship_components.py` & `autotraders-1.2.2/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/space_traders_entity.py` & `autotraders-1.2.2/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders/status.py` & `autotraders-1.2.2/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.2.2/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.1
+Version: 1.2.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.2.1/autotraders.egg-info/SOURCES.txt` & `autotraders-1.2.2/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/pyproject.toml` & `autotraders-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.2.1/tests/test_init.py` & `autotraders-1.2.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.1/tests/test_util.py` & `autotraders-1.2.2/tests/test_util.py`

 * *Files identical despite different names*


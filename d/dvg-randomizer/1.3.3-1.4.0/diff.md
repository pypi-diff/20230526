# Comparing `tmp/dvg-randomizer-1.3.3.tar.gz` & `tmp/dvg-randomizer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvg-randomizer-1.3.3.tar", last modified: Sat Dec 10 17:02:03 2022, max compression
+gzip compressed data, was "dvg-randomizer-1.4.0.tar", last modified: Fri May 26 10:30:58 2023, max compression
```

## Comparing `dvg-randomizer-1.3.3.tar` & `dvg-randomizer-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,31 @@
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2022-12-10 17:02:03.340557 dvg-randomizer-1.3.3/
--rw-r--r--   0 jquelin   (5000) users      (100)      716 2022-02-07 14:15:49.000000 dvg-randomizer-1.3.3/LICENSE
--rw-r--r--   0 jquelin   (5000) users      (100)      196 2022-12-10 17:00:59.000000 dvg-randomizer-1.3.3/MANIFEST.in
--rw-r--r--   0 jquelin   (5000) users      (100)     1696 2022-12-10 17:02:03.340557 dvg-randomizer-1.3.3/PKG-INFO
--rw-r--r--   0 jquelin   (5000) users      (100)     1155 2022-12-10 14:59:34.000000 dvg-randomizer-1.3.3/README.md
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2022-12-10 17:02:03.337557 dvg-randomizer-1.3.3/dvg_randomizer/
--rw-r--r--   0 jquelin   (5000) users      (100)      815 2022-12-10 14:56:14.000000 dvg-randomizer-1.3.3/dvg_randomizer/__main__.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1618 2022-12-10 13:08:34.000000 dvg-randomizer-1.3.3/dvg_randomizer/aircraft.py
--rw-r--r--   0 jquelin   (5000) users      (100)     6122 2022-12-10 13:09:47.000000 dvg-randomizer-1.3.3/dvg_randomizer/boardgame.py
--rw-r--r--   0 jquelin   (5000) users      (100)     3866 2022-12-10 13:09:59.000000 dvg-randomizer-1.3.3/dvg_randomizer/campaign.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1512 2022-12-10 12:58:30.000000 dvg-randomizer-1.3.3/dvg_randomizer/config.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2022-12-10 17:02:03.339557 dvg-randomizer-1.3.3/dvg_randomizer/csv/
--rw-r--r--   0 jquelin   (5000) users      (100)     4780 2021-12-07 14:39:10.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/aircrafts.csv
--rw-r--r--   0 jquelin   (5000) users      (100)     7498 2021-11-12 14:27:41.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/allowed.csv
--rw-r--r--   0 jquelin   (5000) users      (100)      137 2021-10-14 13:20:05.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/boardgames.csv
--rw-r--r--   0 jquelin   (5000) users      (100)     1564 2022-01-13 14:06:25.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/campaign_costs.csv
--rw-r--r--   0 jquelin   (5000) users      (100)     6566 2022-01-12 17:06:01.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/campaigns.csv
--rw-r--r--   0 jquelin   (5000) users      (100)       90 2021-11-10 09:20:10.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/forbidden.csv
--rw-r--r--   0 jquelin   (5000) users      (100)    20385 2021-11-16 13:56:25.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/pilots.csv
--rw-r--r--   0 jquelin   (5000) users      (100)     3814 2022-12-06 17:34:49.000000 dvg-randomizer-1.3.3/dvg_randomizer/csv/spruance.csv
--rw-r--r--   0 jquelin   (5000) users      (100)     9397 2022-12-10 13:25:10.000000 dvg-randomizer-1.3.3/dvg_randomizer/data.py
--rwxr-xr-x   0 jquelin   (5000) users      (100)     6111 2022-12-10 13:11:16.000000 dvg-randomizer-1.3.3/dvg_randomizer/game.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2022-12-10 17:02:03.339557 dvg-randomizer-1.3.3/dvg_randomizer/gui/
--rw-r--r--   0 jquelin   (5000) users      (100)     5930 2022-12-10 13:12:48.000000 dvg-randomizer-1.3.3/dvg_randomizer/gui/composition.py
--rw-r--r--   0 jquelin   (5000) users      (100)    14179 2022-12-10 13:27:14.000000 dvg-randomizer-1.3.3/dvg_randomizer/gui/main.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1203 2022-12-10 13:03:44.000000 dvg-randomizer-1.3.3/dvg_randomizer/logger.py
--rw-r--r--   0 jquelin   (5000) users      (100)    16453 2022-12-10 13:30:52.000000 dvg-randomizer-1.3.3/dvg_randomizer/logsheet.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2022-12-10 17:02:03.339557 dvg-randomizer-1.3.3/dvg_randomizer/misc/
--rw-r--r--   0 jquelin   (5000) users      (100)   755124 2021-12-07 18:53:06.000000 dvg-randomizer-1.3.3/dvg_randomizer/misc/DejaVuSansCondensed.ttf
--rw-r--r--   0 jquelin   (5000) users      (100)     2334 2022-12-10 13:11:35.000000 dvg-randomizer-1.3.3/dvg_randomizer/pilot.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2022-12-10 17:02:03.338557 dvg-randomizer-1.3.3/dvg_randomizer.egg-info/
--rw-r--r--   0 jquelin   (5000) users      (100)     1696 2022-12-10 17:02:03.000000 dvg-randomizer-1.3.3/dvg_randomizer.egg-info/PKG-INFO
--rw-r--r--   0 jquelin   (5000) users      (100)      899 2022-12-10 17:02:03.000000 dvg-randomizer-1.3.3/dvg_randomizer.egg-info/SOURCES.txt
--rw-r--r--   0 jquelin   (5000) users      (100)        1 2022-12-10 17:02:03.000000 dvg-randomizer-1.3.3/dvg_randomizer.egg-info/dependency_links.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       63 2022-12-10 17:02:03.000000 dvg-randomizer-1.3.3/dvg_randomizer.egg-info/entry_points.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       22 2022-12-10 17:02:03.000000 dvg-randomizer-1.3.3/dvg_randomizer.egg-info/requires.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       15 2022-12-10 17:02:03.000000 dvg-randomizer-1.3.3/dvg_randomizer.egg-info/top_level.txt
--rw-r--r--   0 jquelin   (5000) users      (100)      744 2022-12-10 16:57:58.000000 dvg-randomizer-1.3.3/pyproject.toml
--rw-r--r--   0 jquelin   (5000) users      (100)       38 2022-12-10 17:02:03.340557 dvg-randomizer-1.3.3/setup.cfg
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:30:58.969581 dvg-randomizer-1.4.0/
+-rw-r--r--   0 jquelin   (5000) users      (100)    35149 2017-09-30 07:16:26.000000 dvg-randomizer-1.4.0/COPYING
+-rw-r--r--   0 jquelin   (5000) users      (100)      716 2022-02-07 14:15:49.000000 dvg-randomizer-1.4.0/LICENSE
+-rw-r--r--   0 jquelin   (5000) users      (100)      196 2022-12-10 17:00:59.000000 dvg-randomizer-1.4.0/MANIFEST.in
+-rw-r--r--   0 jquelin   (5000) users      (100)     1739 2023-05-26 10:30:58.969581 dvg-randomizer-1.4.0/PKG-INFO
+-rw-r--r--   0 jquelin   (5000) users      (100)     1155 2023-05-26 09:56:05.000000 dvg-randomizer-1.4.0/README.md
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:30:58.966581 dvg-randomizer-1.4.0/dvg_randomizer/
+-rw-r--r--   0 jquelin   (5000) users      (100)      815 2022-12-10 14:56:14.000000 dvg-randomizer-1.4.0/dvg_randomizer/__main__.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1712 2023-05-25 12:50:05.000000 dvg-randomizer-1.4.0/dvg_randomizer/aircraft.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     6122 2023-05-25 11:06:48.000000 dvg-randomizer-1.4.0/dvg_randomizer/boardgame.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     3866 2023-05-26 08:56:42.000000 dvg-randomizer-1.4.0/dvg_randomizer/campaign.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1512 2022-12-10 12:58:30.000000 dvg-randomizer-1.4.0/dvg_randomizer/config.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     9179 2023-05-26 08:48:30.000000 dvg-randomizer-1.4.0/dvg_randomizer/data.py
+-rwxr-xr-x   0 jquelin   (5000) users      (100)     6111 2022-12-12 17:02:41.000000 dvg-randomizer-1.4.0/dvg_randomizer/game.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:30:58.968581 dvg-randomizer-1.4.0/dvg_randomizer/gui/
+-rw-r--r--   0 jquelin   (5000) users      (100)     5930 2022-12-10 13:12:48.000000 dvg-randomizer-1.4.0/dvg_randomizer/gui/composition.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    14179 2022-12-10 13:27:14.000000 dvg-randomizer-1.4.0/dvg_randomizer/gui/main.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1203 2022-12-10 13:03:44.000000 dvg-randomizer-1.4.0/dvg_randomizer/logger.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    16460 2023-05-25 14:33:55.000000 dvg-randomizer-1.4.0/dvg_randomizer/logsheet.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:30:58.968581 dvg-randomizer-1.4.0/dvg_randomizer/misc/
+-rw-r--r--   0 jquelin   (5000) users      (100)   755124 2021-12-07 18:53:06.000000 dvg-randomizer-1.4.0/dvg_randomizer/misc/DejaVuSansCondensed.ttf
+-rw-r--r--   0 jquelin   (5000) users      (100)     2425 2023-05-26 08:45:33.000000 dvg-randomizer-1.4.0/dvg_randomizer/pilot.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:30:58.967581 dvg-randomizer-1.4.0/dvg_randomizer.egg-info/
+-rw-r--r--   0 jquelin   (5000) users      (100)     1739 2023-05-26 10:30:58.000000 dvg-randomizer-1.4.0/dvg_randomizer.egg-info/PKG-INFO
+-rw-r--r--   0 jquelin   (5000) users      (100)      643 2023-05-26 10:30:58.000000 dvg-randomizer-1.4.0/dvg_randomizer.egg-info/SOURCES.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)        1 2023-05-26 10:30:58.000000 dvg-randomizer-1.4.0/dvg_randomizer.egg-info/dependency_links.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       63 2023-05-26 10:30:58.000000 dvg-randomizer-1.4.0/dvg_randomizer.egg-info/entry_points.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       34 2023-05-26 10:30:58.000000 dvg-randomizer-1.4.0/dvg_randomizer.egg-info/requires.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       15 2023-05-26 10:30:58.000000 dvg-randomizer-1.4.0/dvg_randomizer.egg-info/top_level.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)      784 2023-05-26 10:30:40.000000 dvg-randomizer-1.4.0/pyproject.toml
+-rw-r--r--   0 jquelin   (5000) users      (100)       38 2023-05-26 10:30:58.969581 dvg-randomizer-1.4.0/setup.cfg
```

### Comparing `dvg-randomizer-1.3.3/LICENSE` & `dvg-randomizer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/PKG-INFO` & `dvg-randomizer-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dvg-randomizer
-Version: 1.3.3
-Summary: classical Risk game
+Version: 1.4.0
+Summary: Randomizer app for DVG Leader boardgames
 Author-email: Jerome Quelin <jquelin@gmail.com>
 Project-URL: Homepage, https://github.com/jquelin/dvg-randomize
 Project-URL: Bug Tracker, https://github.com/jquelin/dvg-randomize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: COPYING
 
 # NAME
 
 dvg-randomizer - gui to randomize your squadron for DVG Air Leader games
 
 
 # DESCRIPTION
```

### Comparing `dvg-randomizer-1.3.3/README.md` & `dvg-randomizer-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/__main__.py` & `dvg-randomizer-1.4.0/dvg_randomizer/__main__.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/aircraft.py` & `dvg-randomizer-1.4.0/dvg_randomizer/aircraft.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 #
 
 
 from dvg_randomizer.logger import log
 
 class Aircraft:
     def __init__(self, bg, box, service, name, year_in:int,
-                 year_out:int, cost, role):
+                 year_out:int, cost_s, cost_m, cost_l, role):
         self.boardgame = bg
         self.box       = box
         self.service   = service
         self.services  = service.split('+')
         self.name      = name
         self.year_in   = int(year_in)
         self.year_out  = int(year_out) if year_out else 9999
-        self.cost      = int(cost)
+        self.cost_s    = int(cost_s)
+        self.cost_m    = int(cost_m)
+        self.cost_l    = int(cost_l)
         self.role      = role
 
     def __lt__(self, a):
         return self.name < a.name
 
     def id(self):
         # box should not be part of id, since a core aircraft can be
```

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/boardgame.py` & `dvg-randomizer-1.4.0/dvg_randomizer/boardgame.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/campaign.py` & `dvg-randomizer-1.4.0/dvg_randomizer/campaign.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/config.py` & `dvg-randomizer-1.4.0/dvg_randomizer/config.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/game.py` & `dvg-randomizer-1.4.0/dvg_randomizer/game.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/gui/composition.py` & `dvg-randomizer-1.4.0/dvg_randomizer/gui/composition.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/gui/main.py` & `dvg-randomizer-1.4.0/dvg_randomizer/gui/main.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/logger.py` & `dvg-randomizer-1.4.0/dvg_randomizer/logger.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/logsheet.py` & `dvg-randomizer-1.4.0/dvg_randomizer/logsheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 BLACK  = 0
 
 def generate_pdf(game):
     bg = game.boardgame
     campaign = game.campaign
     clength  = game.clength
 
-    has_aces = bg.alias in {'CL', 'ZL'}
+    has_aces = bg.alias in {'CL', 'StL', 'ZL'}
 
     margin = 10
     width  = 4  # default cell width
     height = 5  # default row height
     wfull = 297
     hfull = 210
     wreal = wfull - 2 * margin
```

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/misc/DejaVuSansCondensed.ttf` & `dvg-randomizer-1.4.0/dvg_randomizer/misc/DejaVuSansCondensed.ttf`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer/pilot.py` & `dvg-randomizer-1.4.0/dvg_randomizer/pilot.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,26 @@
 # <https://www.gnu.org/licenses/>.
 #
 
 
 from dvg_randomizer.logger import log
 
 class Pilot:
-    def __init__(self, bg, box, service, name, aircraft, elite):
+    def __init__(self, bg, box, service, name, aircraft, elite_s,
+                 elite_m, elite_l):
         self.boardgame = bg
         self.box       = box
         self.service   = service
         self.services  = service.split('+')
         self.name      = name
         self.aircraft  = aircraft
-        if elite != '':
+        if elite_s is not None:
             self.is_elite    = True
             self.elite_name  = f'\u2606 {name} \u2606'
-            if '+' in elite:
-                self.elite   = [int(s) for s in elite.split('+')]
-            else:
-                self.elite   = [0, int(elite)]
+            self.elite = [elite_s, elite_m, elite_l]
         else:
             self.is_elite    = False
             self.elite       = None
             self.elite_name  = name
 
     def id(self):
         id = self.boardgame.alias
@@ -49,17 +47,22 @@
     def __repr__(self):
         return f'{self.id()} ({self.aircraft})'
 
     def so_bonus(self, game):
         special = game.campaign.special_costs
         cl_level = game.clength.level
         if self.is_elite:
-            so_cost = self.elite[0] + self.elite[1]*cl_level
+            so_cost = self.elite[cl_level-1]
         else:
-            so_cost = self.aircraft.cost * cl_level
+            if cl_level == 1:
+                so_cost = self.aircraft.cost_s
+            elif cl_level == 2:
+                so_cost = self.aircraft.cost_m
+            else:
+                so_cost = self.aircraft.cost_l
             if special:
                 for aircraft, cost in special:
                     if self.aircraft.name == aircraft:
                         sp_so_cost = int(cost * cl_level)
                         log.debug(f'aircraft {aircraft} has a special cost {sp_so_cost} (instead of {so_cost} for this campaign')
                         so_cost = sp_so_cost
```

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer.egg-info/PKG-INFO` & `dvg-randomizer-1.4.0/dvg_randomizer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dvg-randomizer
-Version: 1.3.3
-Summary: classical Risk game
+Version: 1.4.0
+Summary: Randomizer app for DVG Leader boardgames
 Author-email: Jerome Quelin <jquelin@gmail.com>
 Project-URL: Homepage, https://github.com/jquelin/dvg-randomize
 Project-URL: Bug Tracker, https://github.com/jquelin/dvg-randomize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: COPYING
 
 # NAME
 
 dvg-randomizer - gui to randomize your squadron for DVG Air Leader games
 
 
 # DESCRIPTION
```

### Comparing `dvg-randomizer-1.3.3/dvg_randomizer.egg-info/SOURCES.txt` & `dvg-randomizer-1.4.0/dvg_randomizer.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+COPYING
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 dvg_randomizer/__main__.py
 dvg_randomizer/aircraft.py
 dvg_randomizer/boardgame.py
@@ -14,18 +15,10 @@
 dvg_randomizer/pilot.py
 dvg_randomizer.egg-info/PKG-INFO
 dvg_randomizer.egg-info/SOURCES.txt
 dvg_randomizer.egg-info/dependency_links.txt
 dvg_randomizer.egg-info/entry_points.txt
 dvg_randomizer.egg-info/requires.txt
 dvg_randomizer.egg-info/top_level.txt
-dvg_randomizer/csv/aircrafts.csv
-dvg_randomizer/csv/allowed.csv
-dvg_randomizer/csv/boardgames.csv
-dvg_randomizer/csv/campaign_costs.csv
-dvg_randomizer/csv/campaigns.csv
-dvg_randomizer/csv/forbidden.csv
-dvg_randomizer/csv/pilots.csv
-dvg_randomizer/csv/spruance.csv
 dvg_randomizer/gui/composition.py
 dvg_randomizer/gui/main.py
 dvg_randomizer/misc/DejaVuSansCondensed.ttf
```


# Comparing `tmp/dvg-randomizer-1.4.1.tar.gz` & `tmp/dvg-randomizer-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvg-randomizer-1.4.1.tar", last modified: Fri May 26 10:42:16 2023, max compression
+gzip compressed data, was "dvg-randomizer-1.4.2.tar", last modified: Fri May 26 10:48:25 2023, max compression
```

## Comparing `dvg-randomizer-1.4.1.tar` & `dvg-randomizer-1.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:42:16.999126 dvg-randomizer-1.4.1/
--rw-r--r--   0 jquelin   (5000) users      (100)    35149 2017-09-30 07:16:26.000000 dvg-randomizer-1.4.1/COPYING
--rw-r--r--   0 jquelin   (5000) users      (100)      716 2022-02-07 14:15:49.000000 dvg-randomizer-1.4.1/LICENSE
--rw-r--r--   0 jquelin   (5000) users      (100)      156 2023-05-26 10:32:26.000000 dvg-randomizer-1.4.1/MANIFEST.in
--rw-r--r--   0 jquelin   (5000) users      (100)     1840 2023-05-26 10:42:16.999126 dvg-randomizer-1.4.1/PKG-INFO
--rw-r--r--   0 jquelin   (5000) users      (100)     1256 2023-05-26 10:34:12.000000 dvg-randomizer-1.4.1/README.md
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:42:16.996126 dvg-randomizer-1.4.1/dvg_randomizer/
--rw-r--r--   0 jquelin   (5000) users      (100)      815 2022-12-10 14:56:14.000000 dvg-randomizer-1.4.1/dvg_randomizer/__main__.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1712 2023-05-25 12:50:05.000000 dvg-randomizer-1.4.1/dvg_randomizer/aircraft.py
--rw-r--r--   0 jquelin   (5000) users      (100)     6122 2023-05-25 11:06:48.000000 dvg-randomizer-1.4.1/dvg_randomizer/boardgame.py
--rw-r--r--   0 jquelin   (5000) users      (100)     3866 2023-05-26 08:56:42.000000 dvg-randomizer-1.4.1/dvg_randomizer/campaign.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1512 2022-12-10 12:58:30.000000 dvg-randomizer-1.4.1/dvg_randomizer/config.py
--rw-r--r--   0 jquelin   (5000) users      (100)     9179 2023-05-26 08:48:30.000000 dvg-randomizer-1.4.1/dvg_randomizer/data.py
--rw-r--r--   0 jquelin   (5000) users      (100)    45175 2023-05-26 09:01:35.000000 dvg-randomizer-1.4.1/dvg_randomizer/dvg.ods
--rwxr-xr-x   0 jquelin   (5000) users      (100)     6111 2022-12-12 17:02:41.000000 dvg-randomizer-1.4.1/dvg_randomizer/game.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:42:16.998126 dvg-randomizer-1.4.1/dvg_randomizer/gui/
--rw-r--r--   0 jquelin   (5000) users      (100)     5930 2022-12-10 13:12:48.000000 dvg-randomizer-1.4.1/dvg_randomizer/gui/composition.py
--rw-r--r--   0 jquelin   (5000) users      (100)    14179 2022-12-10 13:27:14.000000 dvg-randomizer-1.4.1/dvg_randomizer/gui/main.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1203 2022-12-10 13:03:44.000000 dvg-randomizer-1.4.1/dvg_randomizer/logger.py
--rw-r--r--   0 jquelin   (5000) users      (100)    16460 2023-05-25 14:33:55.000000 dvg-randomizer-1.4.1/dvg_randomizer/logsheet.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:42:16.998126 dvg-randomizer-1.4.1/dvg_randomizer/misc/
--rw-r--r--   0 jquelin   (5000) users      (100)   755124 2021-12-07 18:53:06.000000 dvg-randomizer-1.4.1/dvg_randomizer/misc/DejaVuSansCondensed.ttf
--rw-r--r--   0 jquelin   (5000) users      (100)     2425 2023-05-26 08:45:33.000000 dvg-randomizer-1.4.1/dvg_randomizer/pilot.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:42:16.997126 dvg-randomizer-1.4.1/dvg_randomizer.egg-info/
--rw-r--r--   0 jquelin   (5000) users      (100)     1840 2023-05-26 10:42:16.000000 dvg-randomizer-1.4.1/dvg_randomizer.egg-info/PKG-INFO
--rw-r--r--   0 jquelin   (5000) users      (100)      666 2023-05-26 10:42:16.000000 dvg-randomizer-1.4.1/dvg_randomizer.egg-info/SOURCES.txt
--rw-r--r--   0 jquelin   (5000) users      (100)        1 2023-05-26 10:42:16.000000 dvg-randomizer-1.4.1/dvg_randomizer.egg-info/dependency_links.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       63 2023-05-26 10:42:16.000000 dvg-randomizer-1.4.1/dvg_randomizer.egg-info/entry_points.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       34 2023-05-26 10:42:16.000000 dvg-randomizer-1.4.1/dvg_randomizer.egg-info/requires.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       15 2023-05-26 10:42:16.000000 dvg-randomizer-1.4.1/dvg_randomizer.egg-info/top_level.txt
--rw-r--r--   0 jquelin   (5000) users      (100)      784 2023-05-26 10:40:21.000000 dvg-randomizer-1.4.1/pyproject.toml
--rw-r--r--   0 jquelin   (5000) users      (100)       38 2023-05-26 10:42:16.999126 dvg-randomizer-1.4.1/setup.cfg
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.680579 dvg-randomizer-1.4.2/
+-rw-r--r--   0 jquelin   (5000) users      (100)    35149 2017-09-30 07:16:26.000000 dvg-randomizer-1.4.2/COPYING
+-rw-r--r--   0 jquelin   (5000) users      (100)      716 2022-02-07 14:15:49.000000 dvg-randomizer-1.4.2/LICENSE
+-rw-r--r--   0 jquelin   (5000) users      (100)      156 2023-05-26 10:32:26.000000 dvg-randomizer-1.4.2/MANIFEST.in
+-rw-r--r--   0 jquelin   (5000) users      (100)     1970 2023-05-26 10:48:25.679579 dvg-randomizer-1.4.2/PKG-INFO
+-rw-r--r--   0 jquelin   (5000) users      (100)     1386 2023-05-26 10:45:44.000000 dvg-randomizer-1.4.2/README.md
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.677579 dvg-randomizer-1.4.2/dvg_randomizer/
+-rw-r--r--   0 jquelin   (5000) users      (100)      815 2022-12-10 14:56:14.000000 dvg-randomizer-1.4.2/dvg_randomizer/__main__.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1712 2023-05-25 12:50:05.000000 dvg-randomizer-1.4.2/dvg_randomizer/aircraft.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     6122 2023-05-25 11:06:48.000000 dvg-randomizer-1.4.2/dvg_randomizer/boardgame.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     3866 2023-05-26 08:56:42.000000 dvg-randomizer-1.4.2/dvg_randomizer/campaign.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1512 2022-12-10 12:58:30.000000 dvg-randomizer-1.4.2/dvg_randomizer/config.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     9179 2023-05-26 08:48:30.000000 dvg-randomizer-1.4.2/dvg_randomizer/data.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    45175 2023-05-26 09:01:35.000000 dvg-randomizer-1.4.2/dvg_randomizer/dvg.ods
+-rwxr-xr-x   0 jquelin   (5000) users      (100)     6111 2022-12-12 17:02:41.000000 dvg-randomizer-1.4.2/dvg_randomizer/game.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.678578 dvg-randomizer-1.4.2/dvg_randomizer/gui/
+-rw-r--r--   0 jquelin   (5000) users      (100)     5930 2022-12-10 13:12:48.000000 dvg-randomizer-1.4.2/dvg_randomizer/gui/composition.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    14179 2022-12-10 13:27:14.000000 dvg-randomizer-1.4.2/dvg_randomizer/gui/main.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1203 2022-12-10 13:03:44.000000 dvg-randomizer-1.4.2/dvg_randomizer/logger.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    16460 2023-05-25 14:33:55.000000 dvg-randomizer-1.4.2/dvg_randomizer/logsheet.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.679579 dvg-randomizer-1.4.2/dvg_randomizer/misc/
+-rw-r--r--   0 jquelin   (5000) users      (100)   755124 2021-12-07 18:53:06.000000 dvg-randomizer-1.4.2/dvg_randomizer/misc/DejaVuSansCondensed.ttf
+-rw-r--r--   0 jquelin   (5000) users      (100)     2425 2023-05-26 08:45:33.000000 dvg-randomizer-1.4.2/dvg_randomizer/pilot.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.678578 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/
+-rw-r--r--   0 jquelin   (5000) users      (100)     1970 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/PKG-INFO
+-rw-r--r--   0 jquelin   (5000) users      (100)      666 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/SOURCES.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)        1 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/dependency_links.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       63 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/entry_points.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       34 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/requires.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       15 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/top_level.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)      784 2023-05-26 10:47:57.000000 dvg-randomizer-1.4.2/pyproject.toml
+-rw-r--r--   0 jquelin   (5000) users      (100)       38 2023-05-26 10:48:25.680579 dvg-randomizer-1.4.2/setup.cfg
```

### Comparing `dvg-randomizer-1.4.1/COPYING` & `dvg-randomizer-1.4.2/COPYING`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/LICENSE` & `dvg-randomizer-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/PKG-INFO` & `dvg-randomizer-1.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-Metadata-Version: 2.1
-Name: dvg-randomizer
-Version: 1.4.1
-Summary: Randomizer app for DVG Leader boardgames
-Author-email: Jerome Quelin <jquelin@gmail.com>
-Project-URL: Homepage, https://github.com/jquelin/dvg-randomize
-Project-URL: Bug Tracker, https://github.com/jquelin/dvg-randomize/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYING
-
 # NAME
 
 dvg-randomizer - gui to randomize your squadron for DVG Air Leader games
 
 
 # DESCRIPTION
 
-Dan Verssen Games (DVG) publishes awesome boardgames putting you in
-command of a squadron for a given campaign. One of the modes is to have
-a random squadron, and this app just does that: it randomizes 
+Dan Verssen Games (DVG) publishes awesome boardgames putting you in command of
+a squadron for a given campaign. One of the modes is to have a random squadron,
+and this app just does that: it provides a way to easily randomize your
+squadron according to available planes & pilots. It can also generate a
+logsheet to use for the game.
 
 
 As of today, the soft supports:
 - Hornet Leader: Carrier Air Operation, with the Cthulhu conflict
   expansion and the expansion #1
 - Phantom Leader, with the expansion #1
 - Israeli Air Force Leader, with its expansion #1
```

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/__main__.py` & `dvg-randomizer-1.4.2/dvg_randomizer/__main__.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/aircraft.py` & `dvg-randomizer-1.4.2/dvg_randomizer/aircraft.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/boardgame.py` & `dvg-randomizer-1.4.2/dvg_randomizer/boardgame.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/campaign.py` & `dvg-randomizer-1.4.2/dvg_randomizer/campaign.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/config.py` & `dvg-randomizer-1.4.2/dvg_randomizer/config.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/data.py` & `dvg-randomizer-1.4.2/dvg_randomizer/data.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/dvg.ods` & `dvg-randomizer-1.4.2/dvg_randomizer/dvg.ods`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/game.py` & `dvg-randomizer-1.4.2/dvg_randomizer/game.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/gui/composition.py` & `dvg-randomizer-1.4.2/dvg_randomizer/gui/composition.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/gui/main.py` & `dvg-randomizer-1.4.2/dvg_randomizer/gui/main.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/logger.py` & `dvg-randomizer-1.4.2/dvg_randomizer/logger.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/logsheet.py` & `dvg-randomizer-1.4.2/dvg_randomizer/logsheet.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/misc/DejaVuSansCondensed.ttf` & `dvg-randomizer-1.4.2/dvg_randomizer/misc/DejaVuSansCondensed.ttf`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer/pilot.py` & `dvg-randomizer-1.4.2/dvg_randomizer/pilot.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer.egg-info/PKG-INFO` & `dvg-randomizer-1.4.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvg-randomizer
-Version: 1.4.1
+Version: 1.4.2
 Summary: Randomizer app for DVG Leader boardgames
 Author-email: Jerome Quelin <jquelin@gmail.com>
 Project-URL: Homepage, https://github.com/jquelin/dvg-randomize
 Project-URL: Bug Tracker, https://github.com/jquelin/dvg-randomize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -16,17 +16,19 @@
 # NAME
 
 dvg-randomizer - gui to randomize your squadron for DVG Air Leader games
 
 
 # DESCRIPTION
 
-Dan Verssen Games (DVG) publishes awesome boardgames putting you in
-command of a squadron for a given campaign. One of the modes is to have
-a random squadron, and this app just does that: it randomizes 
+Dan Verssen Games (DVG) publishes awesome boardgames putting you in command of
+a squadron for a given campaign. One of the modes is to have a random squadron,
+and this app just does that: it provides a way to easily randomize your
+squadron according to available planes & pilots. It can also generate a
+logsheet to use for the game.
 
 
 As of today, the soft supports:
 - Hornet Leader: Carrier Air Operation, with the Cthulhu conflict
   expansion and the expansion #1
 - Phantom Leader, with the expansion #1
 - Israeli Air Force Leader, with its expansion #1
```

### Comparing `dvg-randomizer-1.4.1/dvg_randomizer.egg-info/SOURCES.txt` & `dvg-randomizer-1.4.2/dvg_randomizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.1/pyproject.toml` & `dvg-randomizer-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dvg-randomizer"
-version = '1.4.1'
+version = '1.4.2'
 authors = [
   { name="Jerome Quelin", email="jquelin@gmail.com" },
 ]
 description = "Randomizer app for DVG Leader boardgames"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


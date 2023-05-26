# Comparing `tmp/simpleupdater-0.1.2.tar.gz` & `tmp/simpleupdater-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleupdater-0.1.2.tar", last modified: Fri May 26 04:25:20 2023, max compression
+gzip compressed data, was "simpleupdater-0.1.3.tar", last modified: Fri May 26 05:18:24 2023, max compression
```

## Comparing `simpleupdater-0.1.2.tar` & `simpleupdater-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.949952 simpleupdater-0.1.2/
--rw-rw-rw-   0        0        0     1086 2023-05-25 14:24:34.000000 simpleupdater-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1912 2023-05-26 04:25:20.950945 simpleupdater-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1314 2023-05-25 18:18:43.000000 simpleupdater-0.1.2/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 15:24:20.000000 simpleupdater-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      722 2023-05-26 04:25:20.967833 simpleupdater-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.828766 simpleupdater-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.888366 simpleupdater-0.1.2/src/SimpleUpdater/
--rw-rw-rw-   0        0        0     1348 2023-05-26 04:16:33.000000 simpleupdater-0.1.2/src/SimpleUpdater/SimpleUpdater.py
--rw-rw-rw-   0        0        0        0 2023-05-25 12:55:01.000000 simpleupdater-0.1.2/src/SimpleUpdater/__init__.py
--rw-rw-rw-   0        0        0      253 2023-05-26 04:18:39.000000 simpleupdater-0.1.2/src/SimpleUpdater/check.py
--rw-rw-rw-   0        0        0      693 2023-05-26 04:18:02.000000 simpleupdater-0.1.2/src/SimpleUpdater/download.py
-drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.947968 simpleupdater-0.1.2/src/simpleupdater.egg-info/
--rw-rw-rw-   0        0        0     1912 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:24.837205 simpleupdater-0.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-05-25 14:24:34.000000 simpleupdater-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5891 2023-05-26 05:18:24.838199 simpleupdater-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5224 2023-05-26 05:03:09.000000 simpleupdater-0.1.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 15:24:20.000000 simpleupdater-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      722 2023-05-26 05:18:24.842172 simpleupdater-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:24.681250 simpleupdater-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:24.738867 simpleupdater-0.1.3/src/SimpleUpdater/
+-rw-rw-rw-   0        0        0     1387 2023-05-26 04:35:12.000000 simpleupdater-0.1.3/src/SimpleUpdater/SimpleUpdater.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 12:55:01.000000 simpleupdater-0.1.3/src/SimpleUpdater/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-05-26 04:18:39.000000 simpleupdater-0.1.3/src/SimpleUpdater/check.py
+-rw-rw-rw-   0        0        0      693 2023-05-26 04:18:02.000000 simpleupdater-0.1.3/src/SimpleUpdater/download.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:24.833232 simpleupdater-0.1.3/src/simpleupdater.egg-info/
+-rw-rw-rw-   0        0        0     5891 2023-05-26 05:18:24.000000 simpleupdater-0.1.3/src/simpleupdater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-05-26 05:18:24.000000 simpleupdater-0.1.3/src/simpleupdater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 05:18:24.000000 simpleupdater-0.1.3/src/simpleupdater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 05:18:24.000000 simpleupdater-0.1.3/src/simpleupdater.egg-info/top_level.txt
```

### Comparing `simpleupdater-0.1.2/LICENSE` & `simpleupdater-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleupdater-0.1.2/setup.cfg` & `simpleupdater-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 696d 706c 6575 7064 6174 6572   = simpleupdater
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 320d 0a61 7574 686f 7220 3d20 5669 7368  2..author = Vish
+00000030: 330d 0a61 7574 686f 7220 3d20 5669 7368  3..author = Vish
 00000040: 6f6b 204d 0d0a 6175 7468 6f72 5f65 6d61  ok M..author_ema
 00000050: 696c 203d 200d 0a64 6573 6372 6970 7469  il = ..descripti
 00000060: 6f6e 203d 2053 6561 6d6c 6573 736c 7920  on = Seamlessly 
 00000070: 7570 6461 7465 2079 6f75 7220 736f 6674  update your soft
 00000080: 7761 7265 2077 6974 6820 6561 7365 2075  ware with ease u
 00000090: 7369 6e67 2074 6869 7320 6c69 6768 7477  sing this lightw
 000000a0: 6569 6768 7420 5079 7468 6f6e 206d 6f64  eight Python mod
```

### Comparing `simpleupdater-0.1.2/src/SimpleUpdater/SimpleUpdater.py` & `simpleupdater-0.1.3/src/SimpleUpdater/SimpleUpdater.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
         if updateType == "normal":
             from easygui import ynbox
             if ynbox('An update for the application is available. Would you like to download and install it?', 'Update Available', ('Yes, Download Now', 'No, Remind Me Later')):
                 Popen(updaterPath)
                 exit()
         elif updateType == "important":
+            from easygui import ynbox
             if ynbox('An important update for the application is available. This update contains critical bug fixes and security enhancements. It is mandatory to download and install the update to ensure the continued functionality and security of the application.', 'Important Update Required', ('Download Now', 'Exit Application')):
                 Popen(updaterPath)
                 exit()
             else:
                 exit()
         elif updateType == "silent":
             Popen(updaterPath)
```

### Comparing `simpleupdater-0.1.2/src/SimpleUpdater/download.py` & `simpleupdater-0.1.3/src/SimpleUpdater/download.py`

 * *Files identical despite different names*


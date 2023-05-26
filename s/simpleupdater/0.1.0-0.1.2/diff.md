# Comparing `tmp/simpleupdater-0.1.0.tar.gz` & `tmp/simpleupdater-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleupdater-0.1.0.tar", last modified: Thu May 25 17:05:27 2023, max compression
+gzip compressed data, was "simpleupdater-0.1.2.tar", last modified: Fri May 26 04:25:20 2023, max compression
```

## Comparing `simpleupdater-0.1.0.tar` & `simpleupdater-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:05:27.836490 simpleupdater-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-05-25 14:24:34.000000 simpleupdater-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1717 2023-05-25 17:05:27.837491 simpleupdater-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-05-25 15:17:14.000000 simpleupdater-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 15:24:20.000000 simpleupdater-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      722 2023-05-25 17:05:27.843492 simpleupdater-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 17:05:27.703490 simpleupdater-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 17:05:27.755492 simpleupdater-0.1.0/src/SimpleUpdater/
--rw-rw-rw-   0        0        0      475 2023-05-25 16:30:09.000000 simpleupdater-0.1.0/src/SimpleUpdater/SimpleUpdater.py
--rw-rw-rw-   0        0        0        0 2023-05-25 12:55:01.000000 simpleupdater-0.1.0/src/SimpleUpdater/__init__.py
--rw-rw-rw-   0        0        0      172 2023-05-25 12:58:55.000000 simpleupdater-0.1.0/src/SimpleUpdater/check.py
--rw-rw-rw-   0        0        0      533 2023-05-25 13:23:00.000000 simpleupdater-0.1.0/src/SimpleUpdater/download.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:05:27.826490 simpleupdater-0.1.0/src/simpleupdater.egg-info/
--rw-rw-rw-   0        0        0     1717 2023-05-25 17:05:27.000000 simpleupdater-0.1.0/src/simpleupdater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-05-25 17:05:27.000000 simpleupdater-0.1.0/src/simpleupdater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 17:05:27.000000 simpleupdater-0.1.0/src/simpleupdater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-25 17:05:27.000000 simpleupdater-0.1.0/src/simpleupdater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.949952 simpleupdater-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-05-25 14:24:34.000000 simpleupdater-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1912 2023-05-26 04:25:20.950945 simpleupdater-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1314 2023-05-25 18:18:43.000000 simpleupdater-0.1.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 15:24:20.000000 simpleupdater-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      722 2023-05-26 04:25:20.967833 simpleupdater-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.828766 simpleupdater-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.888366 simpleupdater-0.1.2/src/SimpleUpdater/
+-rw-rw-rw-   0        0        0     1348 2023-05-26 04:16:33.000000 simpleupdater-0.1.2/src/SimpleUpdater/SimpleUpdater.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 12:55:01.000000 simpleupdater-0.1.2/src/SimpleUpdater/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-05-26 04:18:39.000000 simpleupdater-0.1.2/src/SimpleUpdater/check.py
+-rw-rw-rw-   0        0        0      693 2023-05-26 04:18:02.000000 simpleupdater-0.1.2/src/SimpleUpdater/download.py
+drwxrwxrwx   0        0        0        0 2023-05-26 04:25:20.947968 simpleupdater-0.1.2/src/simpleupdater.egg-info/
+-rw-rw-rw-   0        0        0     1912 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 04:25:20.000000 simpleupdater-0.1.2/src/simpleupdater.egg-info/top_level.txt
```

### Comparing `simpleupdater-0.1.0/LICENSE` & `simpleupdater-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleupdater-0.1.0/setup.cfg` & `simpleupdater-0.1.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 696d 706c 6575 7064 6174 6572   = simpleupdater
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 300d 0a61 7574 686f 7220 3d20 5669 7368  0..author = Vish
+00000030: 320d 0a61 7574 686f 7220 3d20 5669 7368  2..author = Vish
 00000040: 6f6b 204d 0d0a 6175 7468 6f72 5f65 6d61  ok M..author_ema
 00000050: 696c 203d 200d 0a64 6573 6372 6970 7469  il = ..descripti
 00000060: 6f6e 203d 2053 6561 6d6c 6573 736c 7920  on = Seamlessly 
 00000070: 7570 6461 7465 2079 6f75 7220 736f 6674  update your soft
 00000080: 7761 7265 2077 6974 6820 6561 7365 2075  ware with ease u
 00000090: 7369 6e67 2074 6869 7320 6c69 6768 7477  sing this lightw
 000000a0: 6569 6768 7420 5079 7468 6f6e 206d 6f64  eight Python mod
```

### Comparing `simpleupdater-0.1.0/src/SimpleUpdater/download.py` & `simpleupdater-0.1.2/src/SimpleUpdater/download.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 import os.path
 import tempfile
 
 def versionFile(versionUrl):
     print("Checking for updates...")
     tempDir = tempfile.gettempdir()
     downloadPath = os.path.join(tempDir, 'ver.txt')
-    req.urlretrieve(versionUrl, downloadPath)
-    return downloadPath
+    try:
+        req.urlretrieve(versionUrl, downloadPath)
+        return downloadPath
+    except Exception as e:
+        print(e)
+        exit()
 
 def updaterFile(updaterUrl):
     print("Update found, downloading...")
     tempDir = tempfile.gettempdir()
     updaterPath = os.path.join(tempDir, 'updater.exe')
-    req.urlretrieve(updaterUrl, updaterPath)
-    return updaterPath
+    try:
+        req.urlretrieve(updaterUrl, updaterPath)
+        return updaterPath
+    except Exception as e:
+        print(e)
+        exit()
```


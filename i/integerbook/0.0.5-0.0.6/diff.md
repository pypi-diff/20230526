# Comparing `tmp/integerbook-0.0.5.tar.gz` & `tmp/integerbook-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integerbook-0.0.5.tar", last modified: Tue May 23 13:20:14 2023, max compression
+gzip compressed data, was "integerbook-0.0.6.tar", last modified: Fri May 26 14:07:58 2023, max compression
```

## Comparing `integerbook-0.0.5.tar` & `integerbook-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.472965 integerbook-0.0.5/
--rw-r--r--   0 jvo        (501) staff       (20)    35149 2022-03-18 13:05:53.000000 integerbook-0.0.5/LICENSE
--rw-r--r--   0 jvo        (501) staff       (20)       84 2023-04-23 18:25:14.000000 integerbook-0.0.5/MANIFEST.in
--rw-r--r--   0 jvo        (501) staff       (20)    42574 2023-05-23 13:20:14.472283 integerbook-0.0.5/PKG-INFO
--rw-r--r--   0 jvo        (501) staff       (20)     1560 2023-04-25 14:48:32.000000 integerbook-0.0.5/README.md
--rw-r--r--   0 jvo        (501) staff       (20)      645 2023-05-23 13:19:53.000000 integerbook-0.0.5/pyproject.toml
--rw-r--r--   0 jvo        (501) staff       (20)       38 2023-05-23 13:20:14.473153 integerbook-0.0.5/setup.cfg
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.384853 integerbook-0.0.5/src/
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.398044 integerbook-0.0.5/src/integerbook/
--rw-r--r--   0 jvo        (501) staff       (20)     2475 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/CanvasCreator.py
--rw-r--r--   0 jvo        (501) staff       (20)     5918 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/LocationFinder.py
--rw-r--r--   0 jvo        (501) staff       (20)    10412 2023-05-23 09:49:37.000000 integerbook-0.0.5/src/integerbook/Settings.py
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)     1186 2023-04-23 18:31:12.000000 integerbook-0.0.5/src/integerbook/alternativeSymbols.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.418214 integerbook-0.0.5/src/integerbook/auxiliary_scripts/
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)      756 2023-04-23 22:57:26.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/changeNameMxl.py
--rw-r--r--   0 jvo        (501) staff       (20)     6139 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/chordTypes.py
--rw-r--r--   0 jvo        (501) staff       (20)      680 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/createBatchJson.py
--rw-r--r--   0 jvo        (501) staff       (20)      173 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/printSettings.py
--rw-r--r--   0 jvo        (501) staff       (20)     1619 2023-04-23 21:43:41.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/runMultiple.py
--rw-r--r--   0 jvo        (501) staff       (20)     3588 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/separateRealbook.py
--rw-r--r--   0 jvo        (501) staff       (20)      537 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/setMode.py
--rw-r--r--   0 jvo        (501) staff       (20)     1855 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/setModes.py
--rw-r--r--   0 jvo        (501) staff       (20)     1544 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/auxiliary_scripts/writeTexFile.py
--rw-r--r--   0 jvo        (501) staff       (20)      709 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/fontDimensions.json
--rw-r--r--   0 jvo        (501) staff       (20)     1735 2023-04-29 18:11:08.000000 integerbook-0.0.5/src/integerbook/fontSettings.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.421677 integerbook-0.0.5/src/integerbook/fonts/
--rw-r--r--   0 jvo        (501) staff       (20)     6148 2023-04-02 10:13:05.000000 integerbook-0.0.5/src/integerbook/fonts/.DS_Store
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.422668 integerbook-0.0.5/src/integerbook/fonts/Realbook/
--rw-r--r--   0 jvo        (501) staff       (20)    66232 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/fonts/Realbook/Realbook.ttf
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.424768 integerbook-0.0.5/src/integerbook/fonts/symbola/
--rw-r--r--   0 jvo        (501) staff       (20)  2240100 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/fonts/symbola/Symbola.ttf
--rw-r--r--   0 jvo        (501) staff       (20)     2818 2023-05-22 13:36:25.000000 integerbook-0.0.5/src/integerbook/main.py
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.470971 integerbook-0.0.5/src/integerbook/plotter/
--rw-r--r--   0 jvo        (501) staff       (20)    13336 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/plotter/PlotterBarLines.py
--rw-r--r--   0 jvo        (501) staff       (20)     1741 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/plotter/PlotterBase.py
--rw-r--r--   0 jvo        (501) staff       (20)    14658 2023-04-29 17:50:17.000000 integerbook-0.0.5/src/integerbook/plotter/PlotterChords.py
--rw-r--r--   0 jvo        (501) staff       (20)     1367 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/plotter/PlotterMain.py
--rw-r--r--   0 jvo        (501) staff       (20)     3121 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/plotter/PlotterMetadata.py
--rw-r--r--   0 jvo        (501) staff       (20)    23638 2023-04-23 21:51:35.000000 integerbook-0.0.5/src/integerbook/plotter/PlotterNotes.py
--rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/plotter/__init__.py
--rw-r--r--   0 jvo        (501) staff       (20)    10373 2023-04-23 18:25:14.000000 integerbook-0.0.5/src/integerbook/plotter/patches.py
--rw-r--r--   0 jvo        (501) staff       (20)    10761 2023-05-23 13:13:20.000000 integerbook-0.0.5/src/integerbook/runSingle.py
--rw-r--r--   0 jvo        (501) staff       (20)     1603 2023-05-23 09:49:37.000000 integerbook-0.0.5/src/integerbook/settings.json
-drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-23 13:20:14.404295 integerbook-0.0.5/src/integerbook.egg-info/
--rw-r--r--   0 jvo        (501) staff       (20)    42574 2023-05-23 13:20:14.000000 integerbook-0.0.5/src/integerbook.egg-info/PKG-INFO
--rw-r--r--   0 jvo        (501) staff       (20)     1481 2023-05-23 13:20:14.000000 integerbook-0.0.5/src/integerbook.egg-info/SOURCES.txt
--rw-r--r--   0 jvo        (501) staff       (20)        1 2023-05-23 13:20:14.000000 integerbook-0.0.5/src/integerbook.egg-info/dependency_links.txt
--rw-r--r--   0 jvo        (501) staff       (20)       11 2023-05-23 13:20:14.000000 integerbook-0.0.5/src/integerbook.egg-info/requires.txt
--rw-r--r--   0 jvo        (501) staff       (20)       12 2023-05-23 13:20:14.000000 integerbook-0.0.5/src/integerbook.egg-info/top_level.txt
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.419567 integerbook-0.0.6/
+-rw-r--r--   0 jvo        (501) staff       (20)    35149 2022-03-18 13:05:53.000000 integerbook-0.0.6/LICENSE
+-rw-r--r--   0 jvo        (501) staff       (20)       84 2023-04-23 18:25:14.000000 integerbook-0.0.6/MANIFEST.in
+-rw-r--r--   0 jvo        (501) staff       (20)    42574 2023-05-26 14:07:58.419091 integerbook-0.0.6/PKG-INFO
+-rw-r--r--   0 jvo        (501) staff       (20)     1560 2023-04-25 14:48:32.000000 integerbook-0.0.6/README.md
+-rw-r--r--   0 jvo        (501) staff       (20)      645 2023-05-26 14:07:38.000000 integerbook-0.0.6/pyproject.toml
+-rw-r--r--   0 jvo        (501) staff       (20)       38 2023-05-26 14:07:58.419755 integerbook-0.0.6/setup.cfg
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.353792 integerbook-0.0.6/src/
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.365841 integerbook-0.0.6/src/integerbook/
+-rw-r--r--   0 jvo        (501) staff       (20)     2475 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/CanvasCreator.py
+-rw-r--r--   0 jvo        (501) staff       (20)     5918 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/LocationFinder.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10412 2023-05-23 09:49:37.000000 integerbook-0.0.6/src/integerbook/Settings.py
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1186 2023-04-23 18:31:12.000000 integerbook-0.0.6/src/integerbook/alternativeSymbols.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.382001 integerbook-0.0.6/src/integerbook/auxiliary_scripts/
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)      756 2023-04-23 22:57:26.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/changeNameMxl.py
+-rw-r--r--   0 jvo        (501) staff       (20)     6139 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/chordTypes.py
+-rw-r--r--   0 jvo        (501) staff       (20)      680 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/createBatchJson.py
+-rw-r--r--   0 jvo        (501) staff       (20)      173 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/printSettings.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1619 2023-04-23 21:43:41.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/runMultiple.py
+-rw-r--r--   0 jvo        (501) staff       (20)     3588 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/separateRealbook.py
+-rw-r--r--   0 jvo        (501) staff       (20)      537 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/setMode.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1855 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/setModes.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1544 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/auxiliary_scripts/writeTexFile.py
+-rw-r--r--   0 jvo        (501) staff       (20)      709 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/fontDimensions.json
+-rw-r--r--   0 jvo        (501) staff       (20)     1735 2023-04-29 18:11:08.000000 integerbook-0.0.6/src/integerbook/fontSettings.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.382927 integerbook-0.0.6/src/integerbook/fonts/
+-rw-r--r--   0 jvo        (501) staff       (20)     6148 2023-04-02 10:13:05.000000 integerbook-0.0.6/src/integerbook/fonts/.DS_Store
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.383720 integerbook-0.0.6/src/integerbook/fonts/Realbook/
+-rw-r--r--   0 jvo        (501) staff       (20)    66232 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/fonts/Realbook/Realbook.ttf
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.385249 integerbook-0.0.6/src/integerbook/fonts/symbola/
+-rw-r--r--   0 jvo        (501) staff       (20)  2240100 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/fonts/symbola/Symbola.ttf
+-rw-r--r--   0 jvo        (501) staff       (20)     2818 2023-05-22 13:36:25.000000 integerbook-0.0.6/src/integerbook/main.py
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.417870 integerbook-0.0.6/src/integerbook/plotter/
+-rw-r--r--   0 jvo        (501) staff       (20)    13336 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/plotter/PlotterBarLines.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1741 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/plotter/PlotterBase.py
+-rw-r--r--   0 jvo        (501) staff       (20)    14658 2023-04-29 17:50:17.000000 integerbook-0.0.6/src/integerbook/plotter/PlotterChords.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1367 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/plotter/PlotterMain.py
+-rw-r--r--   0 jvo        (501) staff       (20)     3121 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/plotter/PlotterMetadata.py
+-rw-r--r--   0 jvo        (501) staff       (20)    24015 2023-05-26 13:51:29.000000 integerbook-0.0.6/src/integerbook/plotter/PlotterNotes.py
+-rw-r--r--   0 jvo        (501) staff       (20)        0 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/plotter/__init__.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10373 2023-04-23 18:25:14.000000 integerbook-0.0.6/src/integerbook/plotter/patches.py
+-rw-r--r--   0 jvo        (501) staff       (20)    10979 2023-05-26 13:10:42.000000 integerbook-0.0.6/src/integerbook/runSingle.py
+-rw-r--r--   0 jvo        (501) staff       (20)     1603 2023-05-23 09:49:37.000000 integerbook-0.0.6/src/integerbook/settings.json
+drwxr-xr-x   0 jvo        (501) staff       (20)        0 2023-05-26 14:07:58.371133 integerbook-0.0.6/src/integerbook.egg-info/
+-rw-r--r--   0 jvo        (501) staff       (20)    42574 2023-05-26 14:07:58.000000 integerbook-0.0.6/src/integerbook.egg-info/PKG-INFO
+-rw-r--r--   0 jvo        (501) staff       (20)     1481 2023-05-26 14:07:58.000000 integerbook-0.0.6/src/integerbook.egg-info/SOURCES.txt
+-rw-r--r--   0 jvo        (501) staff       (20)        1 2023-05-26 14:07:58.000000 integerbook-0.0.6/src/integerbook.egg-info/dependency_links.txt
+-rw-r--r--   0 jvo        (501) staff       (20)       11 2023-05-26 14:07:58.000000 integerbook-0.0.6/src/integerbook.egg-info/requires.txt
+-rw-r--r--   0 jvo        (501) staff       (20)       12 2023-05-26 14:07:58.000000 integerbook-0.0.6/src/integerbook.egg-info/top_level.txt
```

### Comparing `integerbook-0.0.5/LICENSE` & `integerbook-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/PKG-INFO` & `integerbook-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integerbook
-Version: 0.0.5
+Version: 0.0.6
 Summary: sheet music converter
 Author-email: Jesse van Oostrum <integerbook@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `integerbook-0.0.5/README.md` & `integerbook-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/pyproject.toml` & `integerbook-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integerbook"
-version = "0.0.5"
+version = "0.0.6"
 description = "sheet music converter"
 readme = "README.md"
 authors = [{ name = "Jesse van Oostrum", email = "integerbook@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `integerbook-0.0.5/src/integerbook/CanvasCreator.py` & `integerbook-0.0.6/src/integerbook/CanvasCreator.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/LocationFinder.py` & `integerbook-0.0.6/src/integerbook/LocationFinder.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/Settings.py` & `integerbook-0.0.6/src/integerbook/Settings.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/alternativeSymbols.json` & `integerbook-0.0.6/src/integerbook/alternativeSymbols.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/changeNameMxl.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/changeNameMxl.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/chordTypes.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/chordTypes.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/createBatchJson.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/createBatchJson.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/runMultiple.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/runMultiple.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/separateRealbook.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/separateRealbook.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/setMode.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/setMode.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/setModes.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/setModes.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/auxiliary_scripts/writeTexFile.py` & `integerbook-0.0.6/src/integerbook/auxiliary_scripts/writeTexFile.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/fontDimensions.json` & `integerbook-0.0.6/src/integerbook/fontDimensions.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/fontSettings.json` & `integerbook-0.0.6/src/integerbook/fontSettings.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/fonts/.DS_Store` & `integerbook-0.0.6/src/integerbook/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/fonts/Realbook/Realbook.ttf` & `integerbook-0.0.6/src/integerbook/fonts/Realbook/Realbook.ttf`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/fonts/symbola/Symbola.ttf` & `integerbook-0.0.6/src/integerbook/fonts/symbola/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/main.py` & `integerbook-0.0.6/src/integerbook/main.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/plotter/PlotterBarLines.py` & `integerbook-0.0.6/src/integerbook/plotter/PlotterBarLines.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/plotter/PlotterBase.py` & `integerbook-0.0.6/src/integerbook/plotter/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/plotter/PlotterChords.py` & `integerbook-0.0.6/src/integerbook/plotter/PlotterChords.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/plotter/PlotterMain.py` & `integerbook-0.0.6/src/integerbook/plotter/PlotterMain.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/plotter/PlotterMetadata.py` & `integerbook-0.0.6/src/integerbook/plotter/PlotterMetadata.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/plotter/PlotterNotes.py` & `integerbook-0.0.6/src/integerbook/plotter/PlotterNotes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import json
+import io
 import music21
+from matplotlib.backend_bases import RendererBase
 from matplotlib.patches import FancyBboxPatch, Rectangle, Ellipse
 from itertools import tee, islice, chain
 import numpy as np
 
 from integerbook.plotter.patches import Parallelogram
 from integerbook.plotter.PlotterBase import Plotter
 
@@ -288,27 +290,31 @@
                 sameLineAsLastElement = self.yPosLineBaseLast[strLineNumber] == yPosLineBase
 
                 if xPosLyric < self.xPosLyricEnd[strLineNumber] and sameLineAsLastElement:
                     xPosLyric = self.xPosLyricEnd[strLineNumber] + self.Settings.fontWidthLyric * 0.3
 
                 yPos = yPosLineBase - lineNumber * (1 + marginTop) * self.Settings.capsizeLyric
 
-                if self.Settings.usePlt:
-                    self.renderer = self.axs[page].figure.canvas.get_renderer()
-
                 plottedLyric = self.axs[page].text(xPosLyric, yPos, lyric.text,
                                                    fontsize=self.Settings.fontSizeLyrics,
                                                    va='baseline', ha='left', font='Dejavu Sans', fontstyle='normal')
 
                 if self.Settings.usePlt:
+                    self.renderer = self.axs[page].figure.canvas.get_renderer()
                     bb = plottedLyric.get_window_extent(renderer=self.renderer).transformed(
                         self.axs[page].transData.inverted())
                     lyricWidth = bb.width
                 else:
-                    lyricWidth = self.Settings.fontWidthLyric * len(lyric.text) * 0.7
+                    self.axs[page].figure.canvas.print_pdf(io.BytesIO())
+                    renderer = self.axs[page].figure._cachedRenderer
+                    # renderer = RendererBase()
+                    bb = plottedLyric.get_window_extent(renderer=renderer).transformed(self.axs[page].transData.inverted())
+                    lyricWidth = bb.width
+
+                    # lyricWidth = self.Settings.fontWidthLyric * len(lyric.text) * 0.7
 
                 if self.lastSyllabic[strLineNumber] == 'middle' or self.lastSyllabic[strLineNumber] == 'begin':
                     """note that in musescore export there is often middle and end syllable, after middle there is a hyphen"""
 
                     if sameLineAsLastElement:
                         xPosHyphen = (self.xPosLyricEnd[strLineNumber] + xPosLyric) / 2
                     else:
```

### Comparing `integerbook-0.0.5/src/integerbook/plotter/patches.py` & `integerbook-0.0.6/src/integerbook/plotter/patches.py`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook/runSingle.py` & `integerbook-0.0.6/src/integerbook/runSingle.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,35 +81,37 @@
 song75 = "/Users/jvo/Downloads/tempMxl/2021 -- HALLELUJAH RJS mods.musicxml"
 song76 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/musescore/Think_About_Things_-_Iceland_Eurovision_2020_-_Dai_Freyr-Part.mscz"
 song77 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/All_Of_Me.musicxml"
 song78 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/All_Of_Me-different-key.musicxml"
 song79 = "/Users/jvo/Downloads/favicon.musicxml"
 song80 = '/Users/jvo/Downloads/DickSchmittMxl/2020 --  Home, Sweet Home RJSReformat.musicxml'
 song81 = '/Users/jvo/Downloads/DickSchmittMxl/2022 -- Back Home Again in Indiana RJSMods.musicxml'
+song82 = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/bladmuziek/popular_sheets/Dream_A_Little_Dream_Of_Me.mxl"
+song83 = "/Users/jvo/Downloads/sheets2/Don't Know Why.musicxml"
 
 settings = {}
-settings["measuresPerLine"] = 4
-settings["subdivision"] = 0
-settings["fontSizeNotes"] = 10
-settings["setInMajorKey"] = True
-settings["lyrics"] = False
-settings['coloursVoices'] = False
-settings['coloursCircleOfFifths'] = False
-settings['thickBarlines'] = True
-settings['plotTimeSignature'] = True
-settings['printArranger'] = False
-settings['saveCropped'] = True
-settings['alpha'] = 0.2
-settings['xkcd'] = False
-
-settings['overlapFactor'] = 0.5
-settings["plotChordTones"] = False
-settings["plotMelody"] = True
-settings["forceMinor"] = True
-# settings["usePlt"] = True
+# settings["measuresPerLine"] = 4
+# settings["subdivision"] = 0
+# settings["fontSizeNotes"] = 10
+# settings["setInMajorKey"] = True
+settings["lyrics"] = True
+# settings['coloursVoices'] = False
+# settings['coloursCircleOfFifths'] = False
+# settings['thickBarlines'] = True
+# settings['plotTimeSignature'] = True
+# settings['printArranger'] = False
+# settings['saveCropped'] = True
+# settings['alpha'] = 0.2
+# settings['xkcd'] = False
+#
+# settings['overlapFactor'] = 0.5
+# settings["plotChordTones"] = False
+# settings["plotMelody"] = True
+# settings["forceMinor"] = True
+settings["usePlt"] = True
 
 # settings["alternativeSymbols"] = "SBJ"
 # settings["fontSizeNotes"] = 7
 
 
 # Settings['font'] = 'Sathu'
 # Settings['font'] = 'STIXGeneral'
@@ -123,15 +125,15 @@
 
 # Settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Realbook"
 # Settings['font'] = 'Realbook'
 
 # settings['fontDirectory'] = "/Users/jvo/Library/Mobile Documents/com~apple~CloudDocs/fonts/Humor Sans"
 # settings['font'] = 'Humor Sans'
 
-song = song77
+song = song83
 
 if song[-5:] == ".mscz":
 
     dirSongsMxl = "/Users/jvo/Downloads/tempMxl"
     filename = os.path.basename(song).split("/")[-1]
     outputName = os.path.splitext(filename)[0] + '.musicxml'
```

### Comparing `integerbook-0.0.5/src/integerbook/settings.json` & `integerbook-0.0.6/src/integerbook/settings.json`

 * *Files identical despite different names*

### Comparing `integerbook-0.0.5/src/integerbook.egg-info/PKG-INFO` & `integerbook-0.0.6/src/integerbook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integerbook
-Version: 0.0.5
+Version: 0.0.6
 Summary: sheet music converter
 Author-email: Jesse van Oostrum <integerbook@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `integerbook-0.0.5/src/integerbook.egg-info/SOURCES.txt` & `integerbook-0.0.6/src/integerbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*


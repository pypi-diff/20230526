# Comparing `tmp/OpihiExarata-2023.5.19.tar.gz` & `tmp/OpihiExarata-2023.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpihiExarata-2023.5.19.tar", last modified: Fri May 19 03:05:59 2023, max compression
+gzip compressed data, was "OpihiExarata-2023.5.26.tar", last modified: Fri May 26 05:19:56 2023, max compression
```

## Comparing `OpihiExarata-2023.5.19.tar` & `OpihiExarata-2023.5.26.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.853671 OpihiExarata-2023.5.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-19 03:05:59.849671 OpihiExarata-2023.5.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 03:05:59.853671 OpihiExarata-2023.5.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.833671 OpihiExarata-2023.5.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.833671 OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-19 03:05:59.000000 OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-19 03:05:59.000000 OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:05:59.000000 OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 03:05:59.000000 OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 03:05:59.000000 OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 03:05:59.000000 OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.837671 OpihiExarata-2023.5.19/src/opihiexarata/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.837671 OpihiExarata-2023.5.19/src/opihiexarata/astrometry/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/astrometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/astrometry/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/astrometry/webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/configuration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.837671 OpihiExarata-2023.5.19/src/opihiexarata/ephemeris/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/ephemeris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/ephemeris/jplhorizons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/ephemeris/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.837671 OpihiExarata-2023.5.19/src/opihiexarata/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36468 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)   127424 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.841671 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/automatic.ui
--rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
--rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
--rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/old_manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/qtui_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/qtui_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/qtui_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/selector.ui
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/window_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    50323 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/gui/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.845671 OpihiExarata-2023.5.19/src/opihiexarata/library/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/mpcrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/phototable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/tcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/library/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.845671 OpihiExarata-2023.5.19/src/opihiexarata/opihi/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/opihi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/opihi/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/opihi/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/opihi/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.849671 OpihiExarata-2023.5.19/src/opihiexarata/orbit/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/orbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/orbit/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/orbit/orbfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/orbit/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.849671 OpihiExarata-2023.5.19/src/opihiexarata/photometry/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/photometry/panstarrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33786 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/photometry/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.849671 OpihiExarata-2023.5.19/src/opihiexarata/propagate/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/propagate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/propagate/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/propagate/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/src/opihiexarata/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:05:59.849671 OpihiExarata-2023.5.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 03:05:39.000000 OpihiExarata-2023.5.19/tests/test_global.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 05:19:39.000000 OpihiExarata-2023.5.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-26 05:19:39.000000 OpihiExarata-2023.5.26/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.795427 OpihiExarata-2023.5.26/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.799427 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 05:19:56.000000 OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.799427 OpihiExarata-2023.5.26/src/opihiexarata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.799427 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/astrometry/webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/configuration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.803427 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/jplhorizons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.803427 OpihiExarata-2023.5.26/src/opihiexarata/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37613 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128567 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.807427 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/automatic.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
+-rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/old_manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/selector.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/window_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50479 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/gui/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.807427 OpihiExarata-2023.5.26/src/opihiexarata/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/mpcrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/phototable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/tcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/library/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/opihi/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/opihi/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/orbit/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/orbfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/orbit/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/photometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/photometry/panstarrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/photometry/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/src/opihiexarata/propagate/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/propagate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/propagate/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/propagate/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/src/opihiexarata/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:19:56.811427 OpihiExarata-2023.5.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-26 05:19:40.000000 OpihiExarata-2023.5.26/tests/test_global.py
```

### Comparing `OpihiExarata-2023.5.19/LICENSE` & `OpihiExarata-2023.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/PKG-INFO` & `OpihiExarata-2023.5.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.5.19
+Version: 2023.5.26
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.5.19/README.md` & `OpihiExarata-2023.5.26/README.md`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/setup.py` & `OpihiExarata-2023.5.26/setup.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/PKG-INFO` & `OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.5.19
+Version: 2023.5.26
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.5.19/src/OpihiExarata.egg-info/SOURCES.txt` & `OpihiExarata-2023.5.26/src/OpihiExarata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/__init__.py` & `OpihiExarata-2023.5.26/src/opihiexarata/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/__main__.py` & `OpihiExarata-2023.5.26/src/opihiexarata/__main__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/astrometry/solution.py` & `OpihiExarata-2023.5.26/src/opihiexarata/astrometry/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/astrometry/webclient.py` & `OpihiExarata-2023.5.26/src/opihiexarata/astrometry/webclient.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/configuration.yaml` & `OpihiExarata-2023.5.26/src/opihiexarata/configuration.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -270,19 +270,19 @@
 # detector and so are pixel based and have units of pixels. (For faster 
 # computational speed, the science mask is a box.)
 PHOTOMETRY_SCIENCE_RADIUS_MASK_PIXELS : 500
 PHOTOMETRY_EDGE_WIDTH_MASK_PIXELS : 100
 
 # Photometry does not work well when using highly saturated stars or 
 # under saturated stars in the calculation. As such, we... 
-# ... limit the stars used to those only dimmer than some apparent magnitude;
+# ... limit the stars used to those only those within a magnitude range;
 # ... (others);
+PHOTOMETRY_ZERO_POINT_DIMMEST_MAGNITUDE : 12
 PHOTOMETRY_ZERO_POINT_BRIGHTEST_MAGNITUDE : 6
 
-
 ############################################################
 ##########     API and Engine Services Configuration
 ############################################################
 
 # The maximum number of attempts that will be made when connecting to any API
 # service.
 API_CONNECTION_MAXIMUM_ATTEMPTS : 10
@@ -324,15 +324,15 @@
 ###########
 
 # Which data release should the MAST API use?
 PANSTARRS_MAST_API_DATA_RELEASE_VERSION : 2
 
 # The maximum number of rows to query from the MAST API, use this if the 
 # downloading of the rows is too much.
-PANSTARRS_MAST_API_MAXIMUM_DATA_ROWS : 10000
+PANSTARRS_MAST_API_MAXIMUM_DATA_ROWS : 1000
 
 ###########
 ##### OrbFit Compiled Binaries
 ###########
 
 # The location where OrbFit was installed. These fields should be filled out 
 # with information from the last step of the installation instructions when
```

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/ephemeris/jplhorizons.py` & `OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/jplhorizons.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/ephemeris/solution.py` & `OpihiExarata-2023.5.26/src/opihiexarata/ephemeris/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/__init__.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/automatic.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/automatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,15 +512,15 @@
 
         # Check that the filter compatibility. If the photometry failed, this
         # may be one of the reasons so it is something to warn about.
         if not photometry_solve_status:
             if filter_name not in getattr(
                 opihi_solution.photometrics, "available_filters", []
             ):
-                print("warn")
+                error.warn(warn_class=error.FilterWarning, message="The filter {f} is not within the list of available filters; hence photometry failed.".format(f=filter_name))
 
         # Saving the file.
         # Extracting the entire path from the current name, we are saving it
         # to the same location.
         directory, basename, extension = library.path.split_pathname(pathname=filename)
         # We are just adding the suffix to the filename.
         suffix = str(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX)
@@ -614,47 +614,65 @@
         # A new image is to be solved. We fetch the new image.
         fetched_filename = self.fetch_new_filename()
 
         # Test to see if we have already processed this file and currently
         # have information about it. This prevents doing too much work.
         def _is_same_file(file_1: str, file_2: str) -> bool:
             """A small inner function to see if two files are the same
-            for the purposes of fetching files."""
+            for the purposes of fetching files.
+            
+            Note we also check for the root of the filename so we avoid any 
+            loops with the intermediate files in reduction.
+            """
             # Assume false, they are not the same file.
             file_1 = file_1 if isinstance(file_1, str) else ""
             file_2 = file_2 if isinstance(file_2, str) else ""
             # If they are the same...
             if file_1 == file_2:
                 return True
             # If neither exists...
             if not os.path.isfile(file_1) and not os.path.isfile(file_2):
                 return True
-            # If they are the same file...
+            # If they are the same file in the OS...
             try:
                 return bool(os.path.samefile(file_1, file_2))
             except FileNotFoundError:
                 pass
+            # If their base names are the same; assuming we remove all of the 
+            # reduction tags.
+            base_file_1 = file_1.replace(library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, "").replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
+            base_file_2 = file_2.replace(library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, "").replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
+            if base_file_1 == base_file_2:
+                return True
+
             # All done; as no check says they are the same file, they are not.
             return False
 
         # Checking if the files are the same...
         if _is_same_file(file_1=fetched_filename, file_2=self.results_fits_filename):
             # The new fetched file is the same one that is already solved. It
             # would be silly to solve it again, there is no point in continuing.
+            self.refresh_window()
             return None
         elif _is_same_file(file_1=fetched_filename, file_2=self.working_fits_filename):
             # Same principle, this new file is the same as the working file.
             # We need to be patient.
+            self.refresh_window()
             return None
         else:
             # This new file becomes our working file.
             self.working_fits_filename = fetched_filename
             # Keeping the GUI up to date while in the loop.
             self.refresh_window()
 
+        # We have a new file, however, in the unlikely event that this 
+        # file is still being written and is locked under permissions because
+        # it is mid-write, we wait a little bit.
+        library.http.api_request_sleep(seconds=1)
+
         # With this new working fits file, we attempt to solve it.
         # First preprocessing the file. We desire to reduce the data if a
         # preprocess solution exists to do so.
         if isinstance(self.preprocess_solution, opihiexarata.OpihiPreprocessSolution):
             # We want to check if the FITS file has already been preprocessed.
             raw_fits_filename = self.working_fits_filename
             header, __ = library.fits.read_fits_image_file(filename=raw_fits_filename)
```

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/functions.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/functions.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/manual.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -695,30 +695,30 @@
         -------
         None
         """
         # If there is no astrometric solution, nothing can be done. Exit this
         # early.
         primary_solution = self.opihi_solution_list[self.primary_file_index]
         if not isinstance(primary_solution, opihiexarata.OpihiSolution):
-            print("warn")
+            error.warn(warn_class=error.SequentialOrderWarning, message="The file does not actually have a solution attached to it.")
             return None
         # In order to send the TCS the target's location, it must have been
         # defined already. Otherwise, there is nothing to do.
         if (
             primary_solution.asteroid_location is None
             or primary_solution.asteroid_location == (None, None)
         ):
-            print("warn")
+            error.warn(warn_class=error.SequentialOrderWarning, message="The location of the target has not been provided, we cannot calculate a position and so nothing can be sent to the TCS.")
             return None
         # The astrometric solution itself is also required.
         if not (
             isinstance(primary_solution.astrometrics, astrometry.AstrometricSolution)
             and primary_solution.astrometrics_status
         ):
-            print("warn")
+            error.warn(warn_class="The astrometric solution has not been computed yet. We cannot calculate the position to send to the TCS.")
             return None
 
         # Extracting the needed parameters for the TCS command.
         # Name...
         target_name = primary_solution.asteroid_name
         # On-sky location...
         target_x, target_y = primary_solution.asteroid_location
@@ -979,17 +979,18 @@
                         overwrite=True,
                         raise_on_error=True,
                         vehicle_args=vehicle_args,
                     )
                 except error.InputError:
                     # An input error is typically due to improper filters being
                     # provided
-                    print("warn: bad filter set!")
-                except Exception:
-                    print("warn")
+                    error.warn(warn_class=error.InputWarning,message="An InputError was caught from the photometry solution, this is likely because the filter was incorrect.")
+                except Exception as err:
+                    error.warn(warn_class=error.UnknownWarning, message="The following error was thrown: {e}".format(e=err))
+                    raise err
                 else:
                     # Photometry is special as the data may also be saved to the
                     # zero point database. We attempt to write a zero point record to
                     # the database, the wrapper writing function checks if writing to
                     # the database is a valid operation. We work on a copy of the
                     # solution just in case.
                     opihi_solution_copy = copy.deepcopy(self.opihi_solution_list[index])
@@ -1162,15 +1163,15 @@
         """
         # If there is no ephemeris solution, there is nothing to be done.
         primary_solution = self.opihi_solution_list[self.primary_file_index]
         if not (
             isinstance(primary_solution, opihiexarata.OpihiSolution)
             and isinstance(primary_solution.ephemeritics, ephemeris.EphemeriticSolution)
         ):
-            print("warn")
+            error.warn(warn_class=error.SequentialOrderWarning, message="There is no ephemeris solution and thus no rates to send to update the TCS.")
             return None
 
         # We use the ephemeritic solution rates to update the TCS, the
         # function provided already converts the values as needed
         # so we can provide the units as per convention.
         # We do not care about the response for now.
         __ = library.tcs.t3io_tcs_ns_rate(
@@ -1326,15 +1327,15 @@
         """
         # If there is no propagation solution, there is nothing to be done.
         primary_solution = self.opihi_solution_list[self.primary_file_index]
         if not (
             isinstance(primary_solution, opihiexarata.OpihiSolution)
             and isinstance(primary_solution.propagatives, propagate.PropagativeSolution)
         ):
-            print("warn")
+            error.warn(warn_class=error.SequentialOrderWarning, message="There is no propagation solution and thus no rates to send to update the TCS.")
             return None
 
         # We use the propagative solution rates to update the TCS, the
         # function provided already converts the values as needed
         # so we can provide the units as per convention.
         # We do not care about the response for now.
         __ = library.tcs.t3io_tcs_ns_rate(
@@ -1783,15 +1784,15 @@
             archive_filename = archive_filename
         else:
             archive_filename = self._get_mpcrecord_archive_filename()
 
         # If the file does not exist, there is nothing to load so a blank
         # history is returned.
         if not os.path.isfile(archive_filename):
-            print("warn")
+            error.warn(warn_class=error.InputWarning, message="We cannot find an an archive filename for historical astroid observations. No history is being provided.")
             target_history = []
         else:
             # Read the historical data.
             with open(archive_filename, "r") as mpcfile:
                 raw_lines = mpcfile.readlines()
                 # The files have new line characters on them, they need
                 # to be removed to have the normal 80 characters.
@@ -1817,20 +1818,19 @@
         # Determining the archive filename.
         if archive_filename is not None:
             archive_filename = archive_filename
         else:
             try:
                 archive_filename = self._get_mpcrecord_archive_filename()
             except Exception:
-                print("warn")
                 archive_filename = None
         # An archive filename cannot be determined, we cannot save the
         # observational history. There is no point in continuing.
         if not isinstance(archive_filename, str):
-            print("warn")
+            error.warn(warn_class=error.InputWarning, message="The archive filename cannot be determined, so we cannot save any of the observational data.")
             return None
 
         # Loading the old history.
         archive_history = self.load_target_history_archive(
             archive_filename=archive_filename
         )
```

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/name.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/name.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/automatic.ui` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/automatic.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/manual.ui` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/old_manual.ui` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/old_manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/qtui_automatic.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/qtui_manual.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_manual.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/qtui_selector.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/qtui_selector.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/selector.ui` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/selector.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/qtui/window_icon.png` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/qtui/window_icon.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/gui/selector.py` & `OpihiExarata-2023.5.26/src/opihiexarata/gui/selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1183,15 +1183,15 @@
                 p0=guess_y_gaussian,
                 method="trf",
             )
             # We only need the gaussian centers, the asteroid pixel locations.
             search_x = float(x_gaussian_param[0])
             search_y = float(y_gaussian_param[0])
         except Exception:
-            print("warn")
+            error.warn(warn_class=error.AccuracyWarning, message="The centroid of the star could not be computed using Gaussian cross sections; we are using maximum pixel instead.")
             # Something happened and for some reason the Gaussian method did
             # not work as intended. We fall back to a far more robust but
             # inaccurate approach of determining the center based on the
             # maximum pixel.
             search_y, search_x = np.unravel_index(
                 np.nanargmax(search_array), search_array.shape
             )
```

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/__init__.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/config.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/config.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/conversion.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/conversion.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/engine.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/engine.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/error.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/error.py`

 * *Files 7% similar despite different names*

```diff
@@ -161,14 +161,30 @@
 ####################
 
 
 class ExarataWarning(UserWarning):
     """The base warning class which all of the other OpihiExarata warnings
     are derived from."""
 
+class AccuracyWarning(ExarataWarning):
+    """This warning is to be used when something is not as accurate as it 
+    should be."""
+class InputWarning(ExarataWarning):
+    """This warning is to be used when something was incorrectly input."""
+
+class FilterWarning(ExarataWarning):
+    """This warning is to be used when improper filters were used."""
+
+class SequentialOrderWarning(ExarataWarning):
+    """This warning is to be used when something is being done out of order or
+    the specific order is not being followed.."""
+
+class UnknownWarning(ExarataWarning):
+    """This warning is to be used when something was incorrectly input."""
+
 
 def warn(
     warn_class: type[ExarataWarning] = ExarataWarning,
     message: str = "",
     stacklevel: int = 2,
 ):
     """The common method to use to warn for any OpihiExarata based warnings.
```

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/fits.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/fits.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/hint.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/hint.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/http.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/http.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/image.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/image.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/json.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/json.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/mpcrecord.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/mpcrecord.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/path.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/path.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/phototable.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/phototable.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/tcs.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/tcs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/library/temporary.py` & `OpihiExarata-2023.5.26/src/opihiexarata/library/temporary.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/opihi/database.py` & `OpihiExarata-2023.5.26/src/opihiexarata/opihi/database.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/opihi/preprocess.py` & `OpihiExarata-2023.5.26/src/opihiexarata/opihi/preprocess.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/opihi/solution.py` & `OpihiExarata-2023.5.26/src/opihiexarata/opihi/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/orbit/custom.py` & `OpihiExarata-2023.5.26/src/opihiexarata/orbit/custom.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/orbit/orbfit.py` & `OpihiExarata-2023.5.26/src/opihiexarata/orbit/orbfit.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/orbit/solution.py` & `OpihiExarata-2023.5.26/src/opihiexarata/orbit/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/photometry/panstarrs.py` & `OpihiExarata-2023.5.26/src/opihiexarata/photometry/panstarrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,30 +328,29 @@
             raise error.InputError(
                 "The data release version provided is not supported."
             )
 
         # The MAST API service is a url request. Constructing the URL based on
         # the provided information.
         mast_api_url = (
-            "https://catalogs.mast.stsci.edu/api/v0.1/panstarrs/dr{v}/mean?"
+            "https://catalogs.mast.stsci.edu/api/v0.1/panstarrs/dr{v}/mean.csv?"
             "ra={a}&dec={d}&radius={r}&nDetections.gte={n}&columns={c}&pagesize={l}&"
-            "ng.gte={p}&nr.gte={p}&ni.gte={p}&nz.gte={p}&"
-            "format=csv"
+            "ng.gte={p}&nr.gte={p}&ni.gte={p}&nz.gte={p}"
         ).format(
             v=data_release,
             a=ra,
             d=dec,
             r=radius,
             n=detections,
             c=colstring,
             l=max_rows,
             p=color_detections,
         )
         # Pull the data into a table.
-        query = requests.post(mast_api_url, verify=self.verify_ssl)
+        query = requests.get(mast_api_url, verify=self.verify_ssl)
         catalog_results = ap_ascii.read(query.text, format="csv")
         return catalog_results
 
     def masked_cone_search(self, *args, **kwargs) -> hint.Table:
         """The same as cone_search, but it also masks the data based on the
         masking idiosyncrasies of PanSTARRS.
```

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/photometry/solution.py` & `OpihiExarata-2023.5.26/src/opihiexarata/photometry/solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,16 +510,17 @@
         sqrt5_100 = 2.51188643151
         inst_magnitude = -sqrt5_100 * np.log10(counts / exposure_time)
 
         # We filter the stars so that we avoid using stars and targets
         # which otherwise would skew our results.
         # Stars which are too bright saturate our detector. We limit based on
         # the magnitude as specified. A dimmer object has a higher magnitude.
-        LIM_MAG = library.config.PHOTOMETRY_ZERO_POINT_BRIGHTEST_MAGNITUDE
-        invalid_filter_magnitude = np.where(magnitude <= LIM_MAG, True, False)
+        DIM_MAG = library.config.PHOTOMETRY_ZERO_POINT_DIMMEST_MAGNITUDE
+        BRIGHT_MAG = library.config.PHOTOMETRY_ZERO_POINT_BRIGHTEST_MAGNITUDE
+        invalid_filter_magnitude = np.where(np.logical_and(BRIGHT_MAG <= magnitude, magnitude <= DIM_MAG), False, True)
         # We only can use count data which is actually valid, using invalid
         # count data corrupts our instrument magnitudes and everything else
         # down the line.
         invalid_instrument_magnitude = ~np.logical_and(np.isfinite(counts), counts > 0)
 
         # The valid points that we can use are those not caught with the
         # filter.
@@ -527,15 +528,17 @@
         # Using only the remaining/valid targets for the photometric
         # calculation.
         valid_magnitude = magnitude[valid_points]
         valid_inst_magnitude = inst_magnitude[valid_points]
 
         # Zero points via the definition equation
         zero_points = valid_magnitude - valid_inst_magnitude
-        zero_point = np.nanmedian(zero_points)
+        # Zero points are technically a magnitude so we can only find its 
+        # average by converting to linear space.
+        zero_point = -sqrt5_100 * np.log10(np.nanmedian(10**(-zero_points*0.4)))
         # We use the error on the mean, but instead we use medians and its
         # standard deviation equivalent to be robust to bad data points.
         n_stars = np.sum(np.isfinite(zero_points))
         zero_point_deviation = sp_stats.median_abs_deviation(
             zero_points, nan_policy="omit"
         )
         zero_point_error = zero_point_deviation / np.sqrt(n_stars)
```

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/propagate/polynomial.py` & `OpihiExarata-2023.5.26/src/opihiexarata/propagate/polynomial.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.5.19/src/opihiexarata/propagate/solution.py` & `OpihiExarata-2023.5.26/src/opihiexarata/propagate/solution.py`

 * *Files identical despite different names*


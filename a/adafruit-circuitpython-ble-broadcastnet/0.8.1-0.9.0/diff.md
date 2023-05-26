# Comparing `tmp/adafruit-circuitpython-ble-broadcastnet-0.8.1.tar.gz` & `tmp/adafruit-circuitpython-ble-broadcastnet-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adafruit-circuitpython-ble-broadcastnet-0.8.1.tar", last modified: Thu Mar 12 18:18:39 2020, max compression
+gzip compressed data, was "dist/adafruit-circuitpython-ble-broadcastnet-0.9.0.tar", last modified: Mon Mar 23 20:59:40 2020, max compression
```

## Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1.tar` & `adafruit-circuitpython-ble-broadcastnet-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-12 18:18:39.438458 adafruit-circuitpython-ble-broadcastnet-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-12 18:18:39.434458 adafruit-circuitpython-ble-broadcastnet-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-12 18:18:39.434458 adafruit-circuitpython-ble-broadcastnet-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (115)     1862 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (115)      102 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (115)    16127 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (115)       59 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (115)     5831 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (115)     1110 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)     3766 2020-03-12 18:18:39.438458 adafruit-circuitpython-ble-broadcastnet-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2382 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (115)     7448 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_ble_broadcastnet.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-12 18:18:39.434458 adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     3766 2020-03-12 18:18:37.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      880 2020-03-12 18:18:39.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-12 18:18:37.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       43 2020-03-12 18:18:37.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       26 2020-03-12 18:18:37.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-12 18:18:39.434458 adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-12 18:18:39.434458 adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (115)      275 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (115)     5428 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (115)      206 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (115)     1287 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-12 18:18:39.438458 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (115)      757 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_battery_level.py
--rw-r--r--   0 runner    (1001) docker     (115)     1027 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_battery_level_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (115)     5681 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_blinka_bridge.py
--rw-r--r--   0 runner    (1001) docker     (115)      600 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_cpb.py
--rw-r--r--   0 runner    (1001) docker     (115)     1625 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_expo_backoff.py
--rw-r--r--   0 runner    (1001) docker     (115)     1282 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_multisensor.py
--rw-r--r--   0 runner    (1001) docker     (115)      549 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)       43 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-03-12 18:18:39.438458 adafruit-circuitpython-ble-broadcastnet-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1920 2020-03-12 18:18:30.000000 adafruit-circuitpython-ble-broadcastnet-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-23 20:59:40.971141 adafruit-circuitpython-ble-broadcastnet-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-23 20:59:40.967141 adafruit-circuitpython-ble-broadcastnet-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-23 20:59:40.967141 adafruit-circuitpython-ble-broadcastnet-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (115)     1855 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (115)      102 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (115)    16127 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (115)       59 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     5991 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (115)     1110 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)     3766 2020-03-23 20:59:40.971141 adafruit-circuitpython-ble-broadcastnet-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2382 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     7448 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_ble_broadcastnet.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-23 20:59:40.967141 adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     3766 2020-03-23 20:59:40.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)      880 2020-03-23 20:59:40.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-23 20:59:40.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       43 2020-03-23 20:59:40.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       26 2020-03-23 20:59:40.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-23 20:59:40.971141 adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-23 20:59:40.971141 adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (115)      275 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     5428 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (115)      206 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     1287 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-23 20:59:40.971141 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (115)      757 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_battery_level.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1027 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_battery_level_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5681 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_blinka_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (115)      600 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_cpb.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1625 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_expo_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1282 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_multisensor.py
+-rw-r--r--   0 runner    (1001) docker     (115)      549 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)       43 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-03-23 20:59:40.971141 adafruit-circuitpython-ble-broadcastnet-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1920 2020-03-23 20:59:32.000000 adafruit-circuitpython-ble-broadcastnet-0.9.0/setup.py
```

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/.github/workflows/build.yml` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/.github/workflows/build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         path: actions-ci
     - name: Install dependencies
       # (e.g. - apt-get: gettext, etc; pip: circuitpython-build-tools, requirements.txt; etc.)
       run: |
         source actions-ci/install.sh
     - name: Pip install pylint, black, & Sphinx
       run: |
-        pip install --force-reinstall pylint==1.9.2 black==19.10b0 Sphinx sphinx-rtd-theme
+        pip install --force-reinstall pylint black==19.10b0 Sphinx sphinx-rtd-theme
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Check formatting
       run: |
         black --check --target-version=py35 .
     - name: PyLint
       run: |
```

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/.github/workflows/release.yml` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/.pylintrc` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/CODE_OF_CONDUCT.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,24 @@
 * The use of sexualized language or imagery and sexual attention or advances
 * The use of inappropriate images, including in a community member's avatar
 * The use of inappropriate language, including in a community member's nickname
 * Any spamming, flaming, baiting or other attention-stealing behavior
 * Excessive or unwelcome helping; answering outside the scope of the question
   asked
 * Trolling, insulting/derogatory comments, and personal or political attacks
+* Promoting or spreading disinformation, lies, or conspiracy theories against
+  a person, group, organisation, project, or community
 * Public or private harassment
 * Publishing others' private information, such as a physical or electronic
   address, without explicit permission
 * Other conduct which could reasonably be considered inappropriate
 
 The goal of the standards and moderation guidelines outlined here is to build
 and maintain a respectful community. We ask that you don’t just aim to be
-"technically unimpeachable", but rather try to be your best self.
+"technically unimpeachable", but rather try to be your best self. 
 
 We value many things beyond technical expertise, including collaboration and
 supporting others within our community. Providing a positive experience for
 other community members can have a much more significant impact than simply
 providing the correct answer.
 
 ## Our Responsibilities
@@ -68,18 +70,18 @@
 involving other community members.
 
 You may report in the following ways:
 
 In any situation, you may send an email to <support@adafruit.com>.
 
 On the Adafruit Discord, you may send an open message from any channel
-to all Community Helpers by tagging @community moderators. You may also send an
-open message from any channel, or a direct message to @kattni#1507,
-@tannewt#4653, @Dan Halbert#1614, @cater#2442, @sommersoft#0222, or
-@Andon#8175.
+to all Community Moderators by tagging @community moderators. You may 
+also send an open message from any channel, or a direct message to 
+@kattni#1507, @tannewt#4653, @Dan Halbert#1614, @cater#2442, 
+@sommersoft#0222, @Mr. Certainly#0472 or @Andon#8175.
 
 Email and direct message reports will be kept confidential.
 
 In situations on Discord where the issue is particularly egregious, possibly
 illegal, requires immediate action, or violates the Discord terms of service,
 you should also report the message directly to Discord.
```

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/LICENSE` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/PKG-INFO` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-broadcastnet
-Version: 0.8.1
+Version: 0.9.0
 Summary: Basic IOT over BLE advertisements.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BroadcastNet
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/README.rst` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_ble_broadcastnet.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_ble_broadcastnet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-broadcastnet
-Version: 0.8.1
+Version: 0.9.0
 Summary: Basic IOT over BLE advertisements.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BroadcastNet
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/adafruit_circuitpython_ble_broadcastnet.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/adafruit_circuitpython_ble_broadcastnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/conf.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/docs/index.rst` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_battery_level.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_battery_level.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_battery_level_neopixel.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_battery_level_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_blinka_bridge.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_blinka_bridge.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_cpb.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_cpb.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_expo_backoff.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_expo_backoff.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_multisensor.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_multisensor.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/examples/ble_broadcastnet_simpletest.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/examples/ble_broadcastnet_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-broadcastnet-0.8.1/setup.py` & `adafruit-circuitpython-ble-broadcastnet-0.9.0/setup.py`

 * *Files identical despite different names*


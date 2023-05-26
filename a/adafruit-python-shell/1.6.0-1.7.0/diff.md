# Comparing `tmp/adafruit-python-shell-1.6.0.tar.gz` & `tmp/adafruit-python-shell-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-python-shell-1.6.0.tar", last modified: Thu Nov 17 21:24:00 2022, max compression
+gzip compressed data, was "adafruit-python-shell-1.7.0.tar", last modified: Fri May 26 16:24:15 2023, max compression
```

## Comparing `adafruit-python-shell-1.6.0.tar` & `adafruit-python-shell-1.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:24:00.694352 adafruit-python-shell-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:24:00.690352 adafruit-python-shell-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:24:00.690352 adafruit-python-shell-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:24:00.694352 adafruit-python-shell-1.6.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-11-17 21:24:00.694352 adafruit-python-shell-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:24:00.694352 adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-11-17 21:24:00.000000 adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-17 21:24:00.000000 adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 21:24:00.000000 adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-17 21:24:00.000000 adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-17 21:24:00.000000 adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19754 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/adafruit_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:24:00.694352 adafruit-python-shell-1.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 21:24:00.694352 adafruit-python-shell-1.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 21:24:00.694352 adafruit-python-shell-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-11-17 21:23:48.000000 adafruit-python-shell-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:15.445926 adafruit-python-shell-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:15.429926 adafruit-python-shell-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:15.437926 adafruit-python-shell-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:15.437926 adafruit-python-shell-1.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-26 16:24:15.445926 adafruit-python-shell-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:15.441926 adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-26 16:24:15.000000 adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-26 16:24:15.000000 adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:24:15.000000 adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 16:24:15.000000 adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 16:24:15.000000 adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/adafruit_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:15.441926 adafruit-python-shell-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:15.445926 adafruit-python-shell-1.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:24:15.445926 adafruit-python-shell-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-26 16:23:58.000000 adafruit-python-shell-1.7.0/setup.py
```

### Comparing `adafruit-python-shell-1.6.0/.github/workflows/build.yml` & `adafruit-python-shell-1.7.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/.github/workflows/release.yml` & `adafruit-python-shell-1.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/.pylintrc` & `adafruit-python-shell-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/CODE_OF_CONDUCT.md` & `adafruit-python-shell-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/LICENSE` & `adafruit-python-shell-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/LICENSES/CC-BY-4.0.txt` & `adafruit-python-shell-1.7.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/LICENSES/MIT.txt` & `adafruit-python-shell-1.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/LICENSES/Unlicense.txt` & `adafruit-python-shell-1.7.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/PKG-INFO` & `adafruit-python-shell-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-python-shell
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python helper for running Shell scripts in Python
 Home-page: https://github.com/adafruit/Adafruit_Python_Shell
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython python shell installation raspberry pi console terminal installer
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `adafruit-python-shell-1.6.0/README.rst` & `adafruit-python-shell-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/PKG-INFO` & `adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-python-shell
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python helper for running Shell scripts in Python
 Home-page: https://github.com/adafruit/Adafruit_Python_Shell
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython python shell installation raspberry pi console terminal installer
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `adafruit-python-shell-1.6.0/adafruit_python_shell.egg-info/SOURCES.txt` & `adafruit-python-shell-1.7.0/adafruit_python_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/adafruit_shell.py` & `adafruit-python-shell-1.7.0/adafruit_shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from datetime import datetime
 from clint.textui import colored, prompt
 import adafruit_platformdetect
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Python_Shell.git"
 
+
 # pylint: disable=too-many-public-methods
 class Shell:
     """
     Class to help with converting Shell scripts over to Python. Having all
     the functions in one place makes updates easier and code shorter.
     """
 
@@ -559,14 +560,30 @@
         if not self.exists(f"/lib/modules/{self.release()}"):
             self.error(
                 "OS has not been rebooted since last kernel update. "
                 "Please reboot and re-run the script."
             )
             self.prompt_reboot()
 
+    def check_kernel_userspace_mismatch(self):
+        """
+        Check if the userspace is 64-bit and kernel is 32-bit
+        """
+        if self.is_arm64() and platform.architecture()[0] == "32bit":
+            print(
+                "Unable to compile driver because kernel space is 64-bit, but user space is 32-bit."
+            )
+            if self.is_raspberry_pi_os() and self.prompt(
+                "Add parameter to /boot/config.txt to use 32-bit kernel?"
+            ):
+                self.reconfig("/boot/config.txt", "^.*arm_64bit.*$", "arm_64bit=0")
+                self.prompt_reboot()
+            else:
+                self.bail("Unable to continue while mismatch is present.")
+
     # pylint: enable=invalid-name
 
     def is_raspberry_pi_os(self):
         """
         Check if we are running Raspberry Pi OS or Raspbian
         """
         return self.get_os() == "Raspbian"
```

### Comparing `adafruit-python-shell-1.6.0/docs/_static/favicon.ico` & `adafruit-python-shell-1.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/docs/conf.py` & `adafruit-python-shell-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/docs/index.rst` & `adafruit-python-shell-1.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.6.0/setup.py` & `adafruit-python-shell-1.7.0/setup.py`

 * *Files identical despite different names*


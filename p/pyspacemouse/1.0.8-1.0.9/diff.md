# Comparing `tmp/pyspacemouse-1.0.8.tar.gz` & `tmp/pyspacemouse-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspacemouse-1.0.8.tar", last modified: Tue Jan 24 23:44:05 2023, max compression
+gzip compressed data, was "pyspacemouse-1.0.9.tar", last modified: Fri May 26 12:54:23 2023, max compression
```

## Comparing `pyspacemouse-1.0.8.tar` & `pyspacemouse-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-01-24 23:44:05.864054 pyspacemouse-1.0.8/
--rw-r--r--   0 kuba       (501) staff       (20)     1108 2022-09-26 12:42:07.000000 pyspacemouse-1.0.8/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     8267 2023-01-24 23:44:05.863796 pyspacemouse-1.0.8/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     7556 2023-01-24 23:34:01.000000 pyspacemouse-1.0.8/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-01-24 23:44:05.862017 pyspacemouse-1.0.8/pyspacemouse/
--rw-r--r--   0 kuba       (501) staff       (20)       27 2022-09-26 12:42:07.000000 pyspacemouse-1.0.8/pyspacemouse/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)    36482 2023-01-24 23:09:55.000000 pyspacemouse-1.0.8/pyspacemouse/pyspacemouse.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-01-24 23:44:05.863614 pyspacemouse-1.0.8/pyspacemouse.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     8267 2023-01-24 23:44:05.000000 pyspacemouse-1.0.8/pyspacemouse.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)      294 2023-01-24 23:44:05.000000 pyspacemouse-1.0.8/pyspacemouse.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2023-01-24 23:44:05.000000 pyspacemouse-1.0.8/pyspacemouse.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2022-10-15 23:04:25.000000 pyspacemouse-1.0.8/pyspacemouse.egg-info/not-zip-safe
--rw-r--r--   0 kuba       (501) staff       (20)        8 2023-01-24 23:44:05.000000 pyspacemouse-1.0.8/pyspacemouse.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)       13 2023-01-24 23:44:05.000000 pyspacemouse-1.0.8/pyspacemouse.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-01-24 23:44:05.864089 pyspacemouse-1.0.8/setup.cfg
--rw-r--r--   0 kuba       (501) staff       (20)     1121 2023-01-24 23:41:42.000000 pyspacemouse-1.0.8/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-05-26 12:54:23.865767 pyspacemouse-1.0.9/
+-rw-r--r--   0 kuba       (501) staff       (20)     1108 2022-09-26 12:42:07.000000 pyspacemouse-1.0.9/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     8986 2023-05-26 12:54:23.865519 pyspacemouse-1.0.9/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     8184 2023-05-26 12:32:06.000000 pyspacemouse-1.0.9/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-05-26 12:54:23.863591 pyspacemouse-1.0.9/pyspacemouse/
+-rw-rw-r--   0 kuba       (501) staff       (20)       27 2023-05-26 11:00:52.000000 pyspacemouse-1.0.9/pyspacemouse/__init__.py
+-rw-rw-r--   0 kuba       (501) staff       (20)    37803 2023-05-26 11:26:13.000000 pyspacemouse-1.0.9/pyspacemouse/pyspacemouse.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-05-26 12:54:23.865280 pyspacemouse-1.0.9/pyspacemouse.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     8986 2023-05-26 12:54:23.000000 pyspacemouse-1.0.9/pyspacemouse.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)      294 2023-05-26 12:54:23.000000 pyspacemouse-1.0.9/pyspacemouse.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2023-05-26 12:54:23.000000 pyspacemouse-1.0.9/pyspacemouse.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2022-10-15 23:04:25.000000 pyspacemouse-1.0.9/pyspacemouse.egg-info/not-zip-safe
+-rw-r--r--   0 kuba       (501) staff       (20)      141 2023-05-26 12:54:23.000000 pyspacemouse-1.0.9/pyspacemouse.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       13 2023-05-26 12:54:23.000000 pyspacemouse-1.0.9/pyspacemouse.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-05-26 12:54:23.865809 pyspacemouse-1.0.9/setup.cfg
+-rw-r--r--   0 kuba       (501) staff       (20)     1457 2023-05-26 12:51:48.000000 pyspacemouse-1.0.9/setup.py
```

### Comparing `pyspacemouse-1.0.8/LICENSE` & `pyspacemouse-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspacemouse-1.0.8/PKG-INFO` & `pyspacemouse-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 Metadata-Version: 2.1
 Name: pyspacemouse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator
 Home-page: https://github.com/JakubAndrysek/pyspacemouse
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
-Keywords: pyspacemouse,3d,6 DoF,HID
+Keywords: pyspacemouse,3d,6 DoF,HID,python,open-source,spacemouse,spacenavigator,3dconnection,3d-mouse
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: develop
 License-File: LICENSE
 
-# PySpaceMouse 
+# PySpaceMouse
 
 A Python library for 3Dconnexion SpaceMouse devices
 
 3Dconnexion Space Mouse in Python using raw HID.
 Note: you **don't** need to install or use any of the drivers or 3Dconnexion software to use this package.
 It interfaces with the controller directly with `hidapi` and python wrapper library `easyhid`.
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fpyspacemouse&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <img src="https://img.shields.io/github/license/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/stars/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/forks/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/issues/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://static.pepy.tech/personalized-badge/pyspacemouse?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads">
 </p>
 
 [PySpaceMouse](https://github.com/JakubAndrysek/pyspacemouse) is forked from: [johnhw/pyspacenavigator](https://github.com/johnhw/pyspacenavigator)
 
 Connected project [PySpaceApp](https://github.com/JakubAndrysek/pyspaceapp) is a simple example of how controll your PC with SpaceMouse.
 
-Implements a simple interface to the 6 DoF 3Dconnexion [Space Mouse](https://3dconnexion.com/uk/spacemouse) device as
+Implements a simple interface to the 6 DoF 3Dconnexion [Space Mouse](https://3dconnexion.com/uk/spacemouse/) device as
 well as similar devices.
 
 ![](https://github.com/JakubAndrysek/pyspacemouse/raw/master/media/spacemouse-robot.jpg)
 Control a [robot](https://roboruka.robotickytabor.cz/) with a Space Mouse
 
 ## Supported 3Dconnexion devices
 
@@ -50,14 +55,22 @@
 * SpaceMouse Compact
 * SpacePilot
 * SpacePilot Pro
 * [Add more devices](https://github.com/johnhw/pyspacenavigator/issues/1)
 
 ## Installation
 
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [pyspacemouse](https://pypi.org/project/pyspacemouse/).
+
+```bash
+pip install pyspacemouse
+```
+
+## Dependencies
+
 - [hidapi](https://github.com/libusb/hidapi) is `C` library for direct communication with HID devices
     - ### Linux
         - [libhidapi-dev]() to access HID data
         - `sudo apt-get install libhidapi-dev` (Debian/Ubuntu)
         - Compile and install [hidapi](https://github.com/libusb/hidapi/#build-from-source).  (other Linux
           distributions)
```

### Comparing `pyspacemouse-1.0.8/README.md` & `pyspacemouse-1.0.9/pyspacemouse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,49 @@
-# PySpaceMouse 
+Metadata-Version: 2.1
+Name: pyspacemouse
+Version: 1.0.9
+Summary: Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator
+Home-page: https://github.com/JakubAndrysek/pyspacemouse
+Author: Jakub Andrýsek
+Author-email: email@kubaandrysek.cz
+License: MIT
+Keywords: pyspacemouse,3d,6 DoF,HID,python,open-source,spacemouse,spacenavigator,3dconnection,3d-mouse
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
+# PySpaceMouse
 
 A Python library for 3Dconnexion SpaceMouse devices
 
 3Dconnexion Space Mouse in Python using raw HID.
 Note: you **don't** need to install or use any of the drivers or 3Dconnexion software to use this package.
 It interfaces with the controller directly with `hidapi` and python wrapper library `easyhid`.
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fpyspacemouse&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <img src="https://img.shields.io/github/license/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/stars/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/forks/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/issues/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://static.pepy.tech/personalized-badge/pyspacemouse?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads">
 </p>
 
 [PySpaceMouse](https://github.com/JakubAndrysek/pyspacemouse) is forked from: [johnhw/pyspacenavigator](https://github.com/johnhw/pyspacenavigator)
 
 Connected project [PySpaceApp](https://github.com/JakubAndrysek/pyspaceapp) is a simple example of how controll your PC with SpaceMouse.
 
-Implements a simple interface to the 6 DoF 3Dconnexion [Space Mouse](https://3dconnexion.com/uk/spacemouse) device as
+Implements a simple interface to the 6 DoF 3Dconnexion [Space Mouse](https://3dconnexion.com/uk/spacemouse/) device as
 well as similar devices.
 
 ![](https://github.com/JakubAndrysek/pyspacemouse/raw/master/media/spacemouse-robot.jpg)
 Control a [robot](https://roboruka.robotickytabor.cz/) with a Space Mouse
 
 ## Supported 3Dconnexion devices
 
@@ -31,14 +55,22 @@
 * SpaceMouse Compact
 * SpacePilot
 * SpacePilot Pro
 * [Add more devices](https://github.com/johnhw/pyspacenavigator/issues/1)
 
 ## Installation
 
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [pyspacemouse](https://pypi.org/project/pyspacemouse/).
+
+```bash
+pip install pyspacemouse
+```
+
+## Dependencies
+
 - [hidapi](https://github.com/libusb/hidapi) is `C` library for direct communication with HID devices
     - ### Linux
         - [libhidapi-dev]() to access HID data
         - `sudo apt-get install libhidapi-dev` (Debian/Ubuntu)
         - Compile and install [hidapi](https://github.com/libusb/hidapi/#build-from-source).  (other Linux
           distributions)
 
@@ -186,8 +218,8 @@
 ### ModuleNotFoundError: No module named 'easyhid'
 
 - Install `easyhid` by `pip install easyhid`.
 
 ### AttributeError: function/symbol 'hid_enumerate' not found in library '<None>': python3: undefined symbol: hid_enumerate
 
 - HID library for your computer is not installed.
-- Follow the instructions in [requirements](#requirements).
+- Follow the instructions in [requirements](#requirements).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyspacemouse-1.0.8/pyspacemouse/pyspacemouse.py` & `pyspacemouse-1.0.9/pyspacemouse/pyspacemouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from easyhid import Enumeration
+from easyhid import Enumeration, HIDException
 from collections import namedtuple
 import timeit
 import copy
 from typing import Callable, Union, List
 
 # current version number
 __version__ = "1.0.3"
@@ -133,15 +133,15 @@
         self.device = None
         self.callback = None
         self.dof_callback = None
         self.dof_callback_arr = None
         self.button_callback = None
         self.button_callback_arr = None
         self.set_nonblocking_loop = True
-        
+
     def __get_num_bytes_to_read(self):
         byte_indices = []
         for value in self.__mappings.values():
             byte_indices.extend([value.byte1, value.byte2])
 
         return max(byte_indices) + 1
 
@@ -152,15 +152,15 @@
             return f"{self.name} [disconnected]"
         else:
             return f"{self.name} connected to {self.vendor_name} {self.product_name} version: {self.version_number} [serial: {self.serial_number}]"
 
     @property
     def mappings(self):
         return self.__mappings
-    
+
     @mappings.setter
     def mappings(self, val):
         self.__mappings = val
         self.__bytes_to_read = self.__get_num_bytes_to_read()
 
     @property
     def connected(self):
@@ -175,15 +175,19 @@
                 None if the device is not open.
         """
         return self.read()
 
     def open(self):
         """Open a connection to the device, if possible"""
         if self.device:
-            self.device.open()
+            try:
+                self.device.open()
+            except HIDException as e:
+                raise Exception("Failed to open device") from e
+
         # copy in product details
         self.product_name = self.device.product_string
         self.vendor_name = self.device.manufacturer_string
         self.version_number = self.device.release_number
         # doesn't seem to work on 3dconnexion devices...
         # serial number will be a byte string, we convert to a hex id
         self.serial_number = "".join(
@@ -288,15 +292,15 @@
                     if block_dof_callback.callback_minus:
                         # is axis value greater than filter
                         if axis_val > block_dof_callback.filter:
                             block_dof_callback.callback(self.tuple_state, axis_val)
                         elif axis_val < -block_dof_callback.filter:
                             block_dof_callback.callback_minus(self.tuple_state, axis_val)
                     elif axis_val > block_dof_callback.filter or axis_val < -block_dof_callback.filter:
-                        block_dof_callback.callback(self.tuple_state, axis_val)
+                        block_dof_callback.cafllback(self.tuple_state, axis_val)
                     self.dict_state_last[axis_name] = now
 
         # only call the button callback if the button state actually changed
         if self.button_callback and button_changed:
             self.button_callback(self.tuple_state, self.tuple_state.buttons)
 
         # only call the button callback_arr if the specific button state actually changed
@@ -369,14 +373,33 @@
         },
         button_mapping=[
             ButtonSpec(channel=3, byte=1, bit=0),  # LEFT
             ButtonSpec(channel=3, byte=1, bit=1),  # RIGHT
         ],
         axis_scale=350.0,
     ),
+    "SpaceMouse USB": DeviceSpec(
+        name="SpaceMouseUSB",
+        # vendor ID and product ID
+        hid_id=[0x256f, 0xc641],
+        # LED HID usage code pair
+        led_id=None,
+        mappings={
+            "x": AxisSpec(channel=1, byte1=1, byte2=2, scale=1),
+            "y": AxisSpec(channel=1, byte1=3, byte2=4, scale=-1),
+            "z": AxisSpec(channel=1, byte1=5, byte2=6, scale=-1),
+            "pitch": AxisSpec(channel=2, byte1=1, byte2=2, scale=-1),
+            "roll": AxisSpec(channel=2, byte1=3, byte2=4, scale=-1),
+            "yaw": AxisSpec(channel=2, byte1=5, byte2=6, scale=1),
+        },
+        button_mapping=[
+            ButtonSpec(channel=None, byte=None, bit=None),  # No buttons
+            ],
+        axis_scale=350.0,
+    ),
     "SpaceMouse Compact": DeviceSpec(
         name="SpaceMouse Compact",
         # vendor ID and product ID
         hid_id=[0x256F, 0xC635],
         # LED HID usage code pair
         led_id=[0x8, 0x4B],
         mappings={
@@ -636,15 +659,19 @@
 def list_devices():
     """Return a list of the supported devices connected
 
     Returns:
         A list of string names of the devices supported which were found. Empty if no supported devices found
     """
     devices = []
-    hid = Enumeration()
+    try:
+        hid = Enumeration()
+    except AttributeError:
+        raise Exception("HID API is probably not installed. See README.md for details.")
+
     all_hids = hid.find()
 
     if all_hids:
         for device in all_hids:
             devices.extend(
                 device_name
                 for device_name, spec in device_specs.items()
@@ -673,27 +700,29 @@
         callback: Callable[[object], None] = None,
         dof_callback: Callable[[object], None] = None,
         dof_callback_arr: List[DofCallback] = None,
         button_callback: Callable[[object, list], None] = None,
         button_callback_arr: List[ButtonCallback] = None,
         set_nonblocking_loop=True,
         device: str = None,
+        path: str = None,
         DeviceNumber=0) -> Union[None, DeviceSpec]:
     """
     Open a 3D space navigator device. Makes this device the current active device, which enables the module-level read() and close()
     calls. For multiple devices, use the read() and close() calls on the returned object instead, and don't use the module-level calls.
 
     Parameters:
         callback: If callback is provided, it is called only on DoF state changes with a copy of the current state tuple.
         dof_callback: If dof_callback is provided, it is called only on DOF state changes with the argument (state).
         dof_callback_arr: If dof_callback_arr is provided, it is called only on DOF state changes with the argument (state, axis).
         button_callback: If button_callback is provided, it is called only on button state changes with the argument (state, buttons).
         button_callback_arr: If button_callbacks_arr is provided, it is called only on specific button state true with the argument (state, buttons, pressed_buttons).
         set_nonblocking_loop: Disable waiting for input from SpaceMouse. It is required for using callbacks
         device: name of device to open. Must be one of the values in supported_devices. If None, chooses the first supported device found.
+        path: path of the device to open. If path is specified it will try to open at that path regardless of what is connected to it
         DeviceNumber: use the first (DeviceNumber=0) device you find. (for universal wireless receiver)
     Returns:
         Device object if the device was opened successfully
         None if the device could not be opened
     """
     # only used if the module-level functions are used
     global _active_device
@@ -707,14 +736,16 @@
             raise Exception("No device connected/supported!")
 
     found_devices = []
     hid = Enumeration()
     all_hids = hid.find()
     if all_hids:
         for dev in all_hids:
+            if path:
+                dev.path = path
             spec = device_specs[device]
             if dev.vendor_id == spec.hid_id[0] and dev.product_id == spec.hid_id[1]:
                 found_devices.append({"Spec": spec, "HIDDevice": dev})
                 print(f"{device} found")
 
     else:
         print("No HID devices detected")
@@ -876,14 +907,19 @@
                 [
                     "%4s %+.2f" % (k, getattr(state, k))
                     for k in ["x", "y", "z", "roll", "pitch", "yaw", "t"]
                 ]
             )
         )
 
+def silent_callback(state):
+    """Silent callback
+    Does nothing
+    """
+    pass
 
 def print_buttons(state, buttons):
     """Simple default button callback
     Print all buttons to output
     """
     # simple default button callback
     print(
```

### Comparing `pyspacemouse-1.0.8/pyspacemouse.egg-info/PKG-INFO` & `pyspacemouse-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,29 @@
-Metadata-Version: 2.1
-Name: pyspacemouse
-Version: 1.0.8
-Summary: Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator
-Home-page: https://github.com/JakubAndrysek/pyspacemouse
-Author: Jakub Andrýsek
-Author-email: email@kubaandrysek.cz
-License: MIT
-Keywords: pyspacemouse,3d,6 DoF,HID
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PySpaceMouse 
+# PySpaceMouse
 
 A Python library for 3Dconnexion SpaceMouse devices
 
 3Dconnexion Space Mouse in Python using raw HID.
 Note: you **don't** need to install or use any of the drivers or 3Dconnexion software to use this package.
 It interfaces with the controller directly with `hidapi` and python wrapper library `easyhid`.
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fpyspacemouse&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <img src="https://img.shields.io/github/license/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/stars/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/forks/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://img.shields.io/github/issues/JakubAndrysek/pyspacemouse?style=flat-square">
+<img src="https://static.pepy.tech/personalized-badge/pyspacemouse?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads">
 </p>
 
 [PySpaceMouse](https://github.com/JakubAndrysek/pyspacemouse) is forked from: [johnhw/pyspacenavigator](https://github.com/johnhw/pyspacenavigator)
 
 Connected project [PySpaceApp](https://github.com/JakubAndrysek/pyspaceapp) is a simple example of how controll your PC with SpaceMouse.
 
-Implements a simple interface to the 6 DoF 3Dconnexion [Space Mouse](https://3dconnexion.com/uk/spacemouse) device as
+Implements a simple interface to the 6 DoF 3Dconnexion [Space Mouse](https://3dconnexion.com/uk/spacemouse/) device as
 well as similar devices.
 
 ![](https://github.com/JakubAndrysek/pyspacemouse/raw/master/media/spacemouse-robot.jpg)
 Control a [robot](https://roboruka.robotickytabor.cz/) with a Space Mouse
 
 ## Supported 3Dconnexion devices
 
@@ -50,14 +35,22 @@
 * SpaceMouse Compact
 * SpacePilot
 * SpacePilot Pro
 * [Add more devices](https://github.com/johnhw/pyspacenavigator/issues/1)
 
 ## Installation
 
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [pyspacemouse](https://pypi.org/project/pyspacemouse/).
+
+```bash
+pip install pyspacemouse
+```
+
+## Dependencies
+
 - [hidapi](https://github.com/libusb/hidapi) is `C` library for direct communication with HID devices
     - ### Linux
         - [libhidapi-dev]() to access HID data
         - `sudo apt-get install libhidapi-dev` (Debian/Ubuntu)
         - Compile and install [hidapi](https://github.com/libusb/hidapi/#build-from-source).  (other Linux
           distributions)
 
@@ -205,8 +198,8 @@
 ### ModuleNotFoundError: No module named 'easyhid'
 
 - Install `easyhid` by `pip install easyhid`.
 
 ### AttributeError: function/symbol 'hid_enumerate' not found in library '<None>': python3: undefined symbol: hid_enumerate
 
 - HID library for your computer is not installed.
-- Follow the instructions in [requirements](#requirements).
+- Follow the instructions in [requirements](#requirements).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyspacemouse-1.0.8/setup.py` & `pyspacemouse-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,27 +7,37 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 long_description = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name='pyspacemouse',
-    version='1.0.8',
+    version='1.0.9',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
     description='Multiplatform Python interface to the 3DConnexion Space Mouse - forked from pyspacenavigator',
     url='https://github.com/JakubAndrysek/pyspacemouse',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    keywords='pyspacemouse, 3d, 6 DoF, HID',
+    keywords='pyspacemouse, 3d, 6 DoF, HID, python, open-source, spacemouse, spacenavigator, 3dconnection, 3d-mouse',
     license='MIT',
     packages=['pyspacemouse'],
     install_requires=[
         "easyhid",
     ],
+    extras_require={
+        'develop': [
+            'mkdocs',
+            'mkdocs-material',
+            'mkdocs-glightbox',
+            'mkdocs-redirects',
+            'mkdocs-open-in-new-tab',
+            'mkdocs-git-revision-date-localized-plugin'],
+    },
+
     zip_safe=False,
     include_package_data=True,
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```


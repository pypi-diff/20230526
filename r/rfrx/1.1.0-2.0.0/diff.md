# Comparing `tmp/rfrx-1.1.0.tar.gz` & `tmp/rfrx-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfrx-1.1.0.tar", max compression
+gzip compressed data, was "rfrx-2.0.0.tar", max compression
```

## Comparing `rfrx-1.1.0.tar` & `rfrx-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1303 2023-05-25 19:06:40.172778 rfrx-1.1.0/LICENSE
--rw-r--r--   0        0        0      873 2023-05-25 19:06:40.172778 rfrx-1.1.0/README.md
--rw-r--r--   0        0        0      853 2023-05-25 19:06:40.176778 rfrx-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-05-25 19:06:40.176778 rfrx-1.1.0/rfrx/__init__.py
--rw-r--r--   0        0        0     2410 2023-05-25 19:06:40.176778 rfrx-1.1.0/rfrx/protronik.py
--rw-r--r--   0        0        0     3942 2023-05-25 19:06:40.176778 rfrx-1.1.0/rfrx/sbus.py
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 rfrx-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-05-26 08:19:07.771155 rfrx-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1832 2023-05-26 08:19:07.771155 rfrx-2.0.0/README.md
+-rw-r--r--   0        0        0      852 2023-05-26 08:19:07.771155 rfrx-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-05-26 08:19:07.771155 rfrx-2.0.0/rfrx/__init__.py
+-rw-r--r--   0        0        0     2475 2023-05-26 08:19:07.771155 rfrx-2.0.0/rfrx/protronik.py
+-rw-r--r--   0        0        0     4542 2023-05-26 08:19:07.771155 rfrx-2.0.0/rfrx/sbus.py
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 rfrx-2.0.0/PKG-INFO
```

### Comparing `rfrx-1.1.0/LICENSE` & `rfrx-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfrx-1.1.0/rfrx/protronik.py` & `rfrx-2.0.0/rfrx/protronik.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 """Process protronik data."""
 
 from logging import getLogger
 from os import environ
 
 from .sbus import SbusDecoder, SbusReader
 
-LOGGER = getLogger("protronik.protronik")
+LOGGER = getLogger("rfrx.protronik")
 
-RH_MIN, RH_MID, RH_MAX = (
-    int(environ.get("RH_MIN", 192)),
-    int(environ.get("RH_MID", 992)),
-    int(environ.get("RH_MAX", 1796)),
+RX_MIN, RX_MID, RX_MAX = (
+    int(environ.get("RFRX_RX_MIN", 192)),
+    int(environ.get("RFRX_RX_MID", 992)),
+    int(environ.get("RFRX_RX_MAX", 1796)),
 )
-RV_MIN, RV_MID, RV_MAX = (
-    int(environ.get("RV_MIN", 302)),
-    int(environ.get("RV_MID", 1100)),
-    int(environ.get("RV_MAX", 1900)),
+RY_MIN, RY_MID, RY_MAX = (
+    int(environ.get("RFRX_RY_MIN", 302)),
+    int(environ.get("RFRX_RY_MID", 1100)),
+    int(environ.get("RFRX_RY_MAX", 1900)),
 )
-LV_MIN, LV_MID, LV_MAX = (
-    int(environ.get("LV_MIN", 180)),
-    int(environ.get("LV_MID", 980)),
-    int(environ.get("LV_MAX", 1779)),
+LY_MIN, LY_MID, LY_MAX = (
+    int(environ.get("RFRX_LY_MIN", 180)),
+    int(environ.get("RFRX_LY_MID", 980)),
+    int(environ.get("RFRX_LY_MAX", 1779)),
 )
-LH_MIN, LH_MID, LH_MAX = (
-    int(environ.get("LH_MIN", 192)),
-    int(environ.get("LH_MID", 992)),
-    int(environ.get("LH_MAX", 1790)),
+LX_MIN, LX_MID, LX_MAX = (
+    int(environ.get("RFRX_LX_MIN", 192)),
+    int(environ.get("RFRX_LX_MID", 992)),
+    int(environ.get("RFRX_LX_MAX", 1790)),
 )
 
 
 class ProTronikDecoder(SbusDecoder):
     """Decode S-BUS frames from Pro-Tronik PTR-6A v2."""
 
     def __init__(self, frame):
         """Decode SBUS, then parse it according to Pro-Tronik use."""
         super().__init__(frame, n_chans=6)
 
-        # calibration: position, mini, middle, maxi
-        rh = RH_MIN, RH_MID, RH_MAX, "right horizontal"
-        rv = RV_MIN, RV_MID, RV_MAX, "right vertical"
-        lv = LV_MIN, LV_MID, LV_MAX, "left vertical"
-        lh = LH_MIN, LH_MID, LH_MAX, "left horizontal"
+        # calibration: minimum, middle, maximum, name
+        rx = RX_MIN, RX_MID, RX_MAX, "right horizontal"
+        ry = RY_MIN, RY_MID, RY_MAX, "right vertical"
+        ly = LY_MIN, LY_MID, LY_MAX, "left vertical"
+        lx = LX_MIN, LX_MID, LX_MAX, "left horizontal"
 
-        def scale(val, mini, middle, maxi, pos):
+        def scale(val, mini, middle, maxi, name):
             """Convert read value to -1.0 -> 1.0."""
             if val < mini:
-                LOGGER.debug(f"{pos} value lower than min: {val} < {mini}")
+                LOGGER.debug(f"{name} value lower than min: {val} < {mini}")
                 return -1.0
             if val > maxi:
-                LOGGER.debug(f"{pos} value higher than max: {val} > {maxi}")
+                LOGGER.debug(f"{name} value higher than max: {val} > {maxi}")
                 return 1.0
             if val < middle:
                 return (val - mini) / (middle - mini) - 1.0
             return (val - middle) / (maxi - middle)
 
-        self.rh = +scale(self.chans[0], *rh)
-        self.rv = -scale(self.chans[1], *rv)
-        self.lv = -scale(self.chans[2], *lv)
-        self.lh = +scale(self.chans[3], *lh)
+        self.rx = +scale(self.chans[0], *rx)
+        self.ry = -scale(self.chans[1], *ry)
+        self.ly = -scale(self.chans[2], *ly)
+        self.lx = +scale(self.chans[3], *lx)
 
         self.ch5 = 2 if self.chans[4] < 500 else 1 if self.chans[4] < 1500 else 0
         self.ch6 = 0 if self.chans[5] < 1000 else 1
 
     def __str__(self):
         """Show decoded data."""
         return (
-            f"{self.rh:+.3f} {self.rv:+.3f} {self.lv:+.3f} {self.lh:+.3f} "
+            f"{self.rx:+.3f} {self.ry:+.3f} {self.ly:+.3f} {self.lx:+.3f} "
             f"{self.ch5} {self.ch6}"
         )
 
 
 class ProTronikReader(SbusReader):
-    """Bind to a serial port, read SBUS frames and process them."""
+    """Bind to a serial port, read SBUS pro-tronik frames and process them."""
 
-    decoder_class = ProTronikDecoder
+    decoder = ProTronikDecoder
```

### Comparing `rfrx-1.1.0/rfrx/sbus.py` & `rfrx-2.0.0/rfrx/sbus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 """Process SBUS data."""
-from logging import getLogger
+from logging import basicConfig, getLogger, root
+from os import environ
 from time import sleep
 
 import serial
 
-LOGGER = getLogger("protronik.sbus")
+LOGGER = getLogger("rfrx.sbus")
+
+_FALSY = ("0", "NO", "OFF", "FALSE")
+PORT = environ.get("RFRX_PORT", "/dev/ttyS0")
+RUNNING = environ.get("RFRX_RUNNING", "ON") not in _FALSY
+RETRY = environ.get("RFRX_RETRY", "ON") not in _FALSY
+TIMEOUT = int(environ.get("RFRX_TIMEOUT", 1))
+N_CHANS = int(environ.get("RFRX_N_CHANS", 16))
+LOG_LEVEL = environ.get("RFRX_LOG_LEVEL", "WARNING").upper()
 
 
 class SbusError(Exception):
     """Exception class for SbusDecoder."""
 
     pass
 
 
 class SbusDecoder:
     """Decode SBUS frames."""
 
-    def __init__(self, frame, n_chans=16):
+    def __init__(self, frame, n_chans=N_CHANS):
         """Parse a frame with `n_chans` used channels."""
         LOGGER.info("parsing frame")
         self.frame = frame
         self.val = int.from_bytes(frame, byteorder="little")
         if not (0 <= n_chans <= 16):
-            err = "Wrong number of channels. "
-            err += f"Expected 0 <= n_chans <= 16, got {n_chans}."
+            err = (
+                "Wrong number of channels. "
+                f"Expected 0 <= n_chans <= 16, got {n_chans}."
+            )
             raise ValueError(err)
         self.n_chans = n_chans
         self.chans = [None] * n_chans
         self.failsafe = None
         self.frame_lost = None
         self.ch17 = None
         self.ch18 = None
@@ -63,26 +74,27 @@
         self.failsafe = self.frame[23] & 0x10
         self.frame_lost = self.frame[23] & 0x20
         self.ch18 = self.frame[23] & 0x40
         self.ch17 = self.frame[23] & 0x80
 
     def __str__(self):
         """Show decoded data."""
-        ret = " ".join(f"{c:4}" for c in self.chans)
-        ret += f"{self.failsafe} {self.frame_lost} {self.ch18} {self.ch17}"
-        return ret
+        data = [*self.chans, self.failsafe, self.frame_lost, self.ch18, self.ch17]
+        return " ".join(f"{c:4}" for c in data)
 
 
 class SbusReader:
     """Bind to a serial port, read SBUS frames and process them."""
 
-    decoder_class = SbusDecoder
+    decoder = SbusDecoder
 
-    def __init__(self, port="/dev/ttyS0", running=True, retry=True, timeout=1):
+    def __init__(self, port=PORT, running=RUNNING, retry=RETRY, timeout=TIMEOUT):
         """Configure the serial port parameters."""
+        if len(root.handlers) == 0:
+            basicConfig(level=LOG_LEVEL)
         self.port = port
         self.running = running
         self.retry = retry
         self.timeout = timeout
 
         self.run()
 
@@ -90,27 +102,30 @@
         """Run main loop."""
         while self.running and self.retry:
             with serial.Serial(
                 port=self.port,
                 baudrate=100_000,
                 bytesize=serial.EIGHTBITS,
                 # TODO: broken on raspbian buster & pyserial 3.5
+                # works well on same setup but with pyserial 3.4…
                 # parity=serial.PARITY_EVEN,
                 stopbits=serial.STOPBITS_TWO,
                 timeout=self.timeout,
             ) as ser:
                 while self.running:
                     try:
                         data = ser.read(25)
                         if len(data) == 0:
-                            err = f"no data on {self.port} "
-                            err += f"in the last {self.timeout} seconds."
+                            err = (
+                                f"no data on {self.port} "
+                                f"in the last {self.timeout} seconds."
+                            )
                             LOGGER.warning(err)
                         else:
-                            frame = self.decoder_class(data)
+                            frame = self.decoder(data)
                             self.process(frame)
                     except SbusError as e:
                         LOGGER.error(f"SBUS error: {e}")
                         break
             LOGGER.warning("sleeping a bit.")
             sleep(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


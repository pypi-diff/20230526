# Comparing `tmp/aiopioneer-0.4.2.tar.gz` & `tmp/aiopioneer-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopioneer-0.4.2.tar", last modified: Mon Apr 17 19:55:52 2023, max compression
+gzip compressed data, was "aiopioneer-0.4.3.tar", last modified: Fri May 26 08:00:09 2023, max compression
```

## Comparing `aiopioneer-0.4.2.tar` & `aiopioneer-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.917482 aiopioneer-0.4.2/
--rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.4.2/LICENSE
--rw-rw----   0 root         (0) adm          (4)    13768 2023-04-17 19:55:52.924227 aiopioneer-0.4.2/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)    13119 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/README.md
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.637485 aiopioneer-0.4.2/aiopioneer/
--rw-rw----   0 root         (0) adm          (4)       68 2022-11-17 13:13:41.000000 aiopioneer-0.4.2/aiopioneer/__init__.py
--rw-rw----   0 root         (0) adm          (4)    10142 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/cli.py
--rw-rw----   0 root         (0) adm          (4)    12269 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/commands.py
--rw-rw----   0 root         (0) adm          (4)    14927 2023-04-17 19:55:12.000000 aiopioneer-0.4.2/aiopioneer/const.py
--rw-rw----   0 root         (0) adm          (4)    43845 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/param.py
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.887482 aiopioneer-0.4.2/aiopioneer/parsers/
--rw-rw----   0 root         (0) adm          (4)       35 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/__init__.py
--rw-rw----   0 root         (0) adm          (4)     3205 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/audio.py
--rw-rw----   0 root         (0) adm          (4)       41 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/const.py
--rw-rw----   0 root         (0) adm          (4)    20107 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/dsp.py
--rw-rw----   0 root         (0) adm          (4)    26292 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/information.py
--rw-rw----   0 root         (0) adm          (4)     8010 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/parsers/parse.py
--rw-rw----   0 root         (0) adm          (4)      630 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/response.py
--rw-rw----   0 root         (0) adm          (4)    23791 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/settings.py
--rw-rw----   0 root         (0) adm          (4)    16160 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/parsers/system.py
--rw-rw----   0 root         (0) adm          (4)     3667 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/tuner.py
--rw-rw----   0 root         (0) adm          (4)     8753 2023-04-07 14:25:01.000000 aiopioneer-0.4.2/aiopioneer/parsers/video.py
--rw-rw----   0 root         (0) adm          (4)    78131 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/pioneer_avr.py
--rw-rw----   0 root         (0) adm          (4)     5297 2023-04-16 20:13:15.000000 aiopioneer-0.4.2/aiopioneer/util.py
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-17 19:55:52.717484 aiopioneer-0.4.2/aiopioneer.egg-info/
--rw-rw----   0 root         (0) adm          (4)    13768 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)      670 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) adm          (4)        1 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) adm          (4)       51 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/entry_points.txt
--rw-rw----   0 root         (0) adm          (4)       11 2023-04-17 19:55:52.000000 aiopioneer-0.4.2/aiopioneer.egg-info/top_level.txt
--rw-rw----   0 root         (0) adm          (4)       38 2023-04-17 19:55:52.934653 aiopioneer-0.4.2/setup.cfg
--rw-rw----   0 root         (0) adm          (4)     1100 2023-03-10 20:49:55.000000 aiopioneer-0.4.2/setup.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-05-26 08:00:09.380765 aiopioneer-0.4.3/
+-rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.4.3/LICENSE
+-rw-rw----   0 root         (0) adm          (4)    13862 2023-05-26 08:00:09.385435 aiopioneer-0.4.3/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)    13213 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/README.md
+drwxrwx---   0 root         (0) adm          (4)        0 2023-05-26 08:00:09.020770 aiopioneer-0.4.3/aiopioneer/
+-rw-rw----   0 root         (0) adm          (4)       68 2022-11-17 13:13:41.000000 aiopioneer-0.4.3/aiopioneer/__init__.py
+-rw-rw----   0 root         (0) adm          (4)    10630 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/cli.py
+-rw-rw----   0 root         (0) adm          (4)    12269 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/commands.py
+-rw-rw----   0 root         (0) adm          (4)    14927 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/const.py
+-rw-rw----   0 root         (0) adm          (4)    43845 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/param.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-05-26 08:00:09.360765 aiopioneer-0.4.3/aiopioneer/parsers/
+-rw-rw----   0 root         (0) adm          (4)       35 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     3205 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/audio.py
+-rw-rw----   0 root         (0) adm          (4)       41 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/const.py
+-rw-rw----   0 root         (0) adm          (4)    20107 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/dsp.py
+-rw-rw----   0 root         (0) adm          (4)    26292 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/information.py
+-rw-rw----   0 root         (0) adm          (4)     8010 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/parsers/parse.py
+-rw-rw----   0 root         (0) adm          (4)      630 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/response.py
+-rw-rw----   0 root         (0) adm          (4)    23791 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/settings.py
+-rw-rw----   0 root         (0) adm          (4)    16160 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/parsers/system.py
+-rw-rw----   0 root         (0) adm          (4)     3706 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/parsers/tuner.py
+-rw-rw----   0 root         (0) adm          (4)     8753 2023-04-07 14:25:01.000000 aiopioneer-0.4.3/aiopioneer/parsers/video.py
+-rw-rw----   0 root         (0) adm          (4)    80438 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/pioneer_avr.py
+-rw-rw----   0 root         (0) adm          (4)     5283 2023-05-26 07:59:58.000000 aiopioneer-0.4.3/aiopioneer/util.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-05-26 08:00:09.130769 aiopioneer-0.4.3/aiopioneer.egg-info/
+-rw-rw----   0 root         (0) adm          (4)    13862 2023-05-26 08:00:08.000000 aiopioneer-0.4.3/aiopioneer.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)      670 2023-05-26 08:00:08.000000 aiopioneer-0.4.3/aiopioneer.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) adm          (4)        1 2023-05-26 08:00:08.000000 aiopioneer-0.4.3/aiopioneer.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) adm          (4)       51 2023-05-26 08:00:08.000000 aiopioneer-0.4.3/aiopioneer.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) adm          (4)       11 2023-05-26 08:00:08.000000 aiopioneer-0.4.3/aiopioneer.egg-info/top_level.txt
+-rw-rw----   0 root         (0) adm          (4)       38 2023-05-26 08:00:09.394116 aiopioneer-0.4.3/setup.cfg
+-rw-rw----   0 root         (0) adm          (4)     1100 2023-03-10 20:49:55.000000 aiopioneer-0.4.3/setup.py
```

### Comparing `aiopioneer-0.4.2/LICENSE` & `aiopioneer-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/PKG-INFO` & `aiopioneer-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.4.2
+Version: 0.4.3
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -125,14 +125,15 @@
 | `debug_responder` | _state_ (bool) | Enable/disable the `debug_responder` parameter.
 | `debug_updater` | _state_ (bool) | Enable/disable the `debug_updater` parameter.
 | `debug_command` | _state_ (bool) | Enable/disable the `debug_command` parameter.
 | `set_scan_interval` | _scan_interval_ (float) | Set the scan interval to _scan_interval_.
 | `get_scan_interval` | | Return the current scan interval.
 | `set_volume_level` | _volume_level_ (int) | Set the volume level for the current zone.
 | `select_source` | _source_name_ | Set the input source for the current zone.
+| `set_tuner_frequency` | _band_ _frequency_ | Set the tuner band and (optionally) frequency.
 | `send_raw_command` | _raw_command_ | Send the raw command _raw_command_ to the AVR.
 
 **NOTE:** The CLI interface may change in the future, and should not be used in scripts. Use the Python API instead.
 
 ## Source list
 
 | ID | Default Name
```

### Comparing `aiopioneer-0.4.2/README.md` & `aiopioneer-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 | `debug_responder` | _state_ (bool) | Enable/disable the `debug_responder` parameter.
 | `debug_updater` | _state_ (bool) | Enable/disable the `debug_updater` parameter.
 | `debug_command` | _state_ (bool) | Enable/disable the `debug_command` parameter.
 | `set_scan_interval` | _scan_interval_ (float) | Set the scan interval to _scan_interval_.
 | `get_scan_interval` | | Return the current scan interval.
 | `set_volume_level` | _volume_level_ (int) | Set the volume level for the current zone.
 | `select_source` | _source_name_ | Set the input source for the current zone.
+| `set_tuner_frequency` | _band_ _frequency_ | Set the tuner band and (optionally) frequency.
 | `send_raw_command` | _raw_command_ | Send the raw command _raw_command_ to the AVR.
 
 **NOTE:** The CLI interface may change in the future, and should not be used in scripts. Use the Python API instead.
 
 ## Source list
 
 | ID | Default Name
```

### Comparing `aiopioneer-0.4.2/aiopioneer/cli.py` & `aiopioneer-0.4.3/aiopioneer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,25 @@
                 volume_level = int(arg)
                 await pioneer.set_volume_level(volume_level, zone=zone)
             except Exception as exc:  # pylint: disable=broad-except
                 print(f'ERROR: Invalid volume level "{arg}": {exc}')
         elif cmd == "select_source":
             source = arg if arg else ""
             await pioneer.select_source(source, zone=zone)
-        elif cmd == "send_raw_command" or cmd == ">":
+        elif cmd == "set_tuner_frequency":
+            subargs = arg.split(" ", maxsplit=1)
+            try:
+                band = subargs[0]
+                frequency = float(subargs[1]) if len(subargs) > 1 else None
+                await pioneer.set_tuner_frequency(band, frequency, zone=zone)
+            except Exception as exc:  # pylint: disable=broad-except
+                print(
+                    f'ERROR: Invalid parameters for set_tuner_frequency "{arg}": {exc}'
+                )
+        elif cmd in ["send_raw_command", ">"]:
             if arg:
                 print(f"Sending raw command {arg}")
                 await pioneer.send_raw_command(arg)
             else:
                 print("ERROR: No raw command specified")
         elif cmd in PIONEER_COMMANDS:
             print(f"Executing command {cmd}")
```

### Comparing `aiopioneer-0.4.2/aiopioneer/commands.py` & `aiopioneer-0.4.3/aiopioneer/commands.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/const.py` & `aiopioneer-0.4.3/aiopioneer/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Constants for aiopioneer."""
 
 from enum import Enum
 
 DEFAULT_PORT = 8102
-VERSION = "0.4.2"
+VERSION = "0.4.3"
 
 
 class Zones(Enum):
     """Valid aiopioneer zones"""
 
     ALL = "ALL"
     Z1 = "1"
```

### Comparing `aiopioneer-0.4.2/aiopioneer/param.py` & `aiopioneer-0.4.3/aiopioneer/param.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/audio.py` & `aiopioneer-0.4.3/aiopioneer/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/dsp.py` & `aiopioneer-0.4.3/aiopioneer/parsers/dsp.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/information.py` & `aiopioneer-0.4.3/aiopioneer/parsers/information.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/parse.py` & `aiopioneer-0.4.3/aiopioneer/parsers/parse.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/response.py` & `aiopioneer-0.4.3/aiopioneer/parsers/response.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/settings.py` & `aiopioneer-0.4.3/aiopioneer/parsers/settings.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/system.py` & `aiopioneer-0.4.3/aiopioneer/parsers/system.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/tuner.py` & `aiopioneer-0.4.3/aiopioneer/parsers/tuner.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,24 +31,25 @@
         return parsed
 
     @staticmethod
     def frequency_am(raw: str, _param: dict, zone = Zones.Z1, command = "FR") -> list:
         """Defines a AM Tuner Frequency response parser."""
         freq = float(raw)
         parsed = []
+        queue_commands = None
+        if _param.get(PARAM_TUNER_AM_FREQ_STEP) is None:
+            queue_commands = ["_calculate_am_frequency_step"]
+
         parsed.append(Response(raw=raw,
                             response_command=command,
                             base_property="tuner",
                             property_name="band",
                             zone=zone,
                             value="AM",
-                            queue_commands=None))
-
-        if _param.get(PARAM_TUNER_AM_FREQ_STEP) is None:
-            parsed[0].queue_commands=["_calculate_am_frequency_step"]
+                            queue_commands=queue_commands))
 
         parsed.append(Response(raw=raw,
                             response_command=command,
                             base_property="tuner",
                             property_name="frequency",
                             zone=zone,
                             value=freq,
@@ -85,14 +86,14 @@
     def am_frequency_step(raw: str, _param: dict, zone = None, command = "SUQ") -> list:
         """Response parser for frequency step.
         NOTE: This is supported on very few AVRs"""
 
         parsed = []
         parsed.append(Response(raw=raw,
                             response_command=command,
-                            base_property="_params",
+                            base_property="_system_params",
                             property_name=PARAM_TUNER_AM_FREQ_STEP,
                             zone=zone,
                             value=9 if raw == "0" else 10,
                             queue_commands=None))
 
         return parsed
```

### Comparing `aiopioneer-0.4.2/aiopioneer/parsers/video.py` & `aiopioneer-0.4.3/aiopioneer/parsers/video.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/aiopioneer/pioneer_avr.py` & `aiopioneer-0.4.3/aiopioneer/pioneer_avr.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,17 @@
 
         # Internal state
         self._connect_lock = asyncio.Lock()
         self._disconnect_lock = asyncio.Lock()
         self._update_lock = asyncio.Lock()
         self._request_lock = asyncio.Lock()
         self._update_event = asyncio.Event()
+        self._response_event = asyncio.Event()
+        self._response_queue = []
+        self._queue_responses = False
         self._reconnect = True
         self._full_update = True
         self._last_updated = None
         self._last_command = None
         self._reader = None
         self._writer = None
         self._listener_task = None
@@ -416,14 +419,20 @@
                     _LOGGER.debug("received AVR response: %s", response)
 
                 # Parse response, update cached properties
                 action = " parsing response " + response
                 parse_result = self._parse_response(response)
                 updated_zones = parse_result.get("updated_zones")
 
+                ## Queue raw response and signal response handler
+                if self._queue_responses:
+                    self._response_queue.append(response)
+                    self._response_event.set()
+                    ## Do not yield, process all responses first
+
                 # Detect Main Zone power on for volume workaround
                 action = ""
                 power_on_volume_bounce = self._params[PARAM_POWER_ON_VOLUME_BOUNCE]
                 if power_on_volume_bounce and self._power_zone_1 is not None:
                     if not self._power_zone_1 and self.power.get("1"):
                         # Main zone powered on, schedule bounce task
                         _LOGGER.info("scheduling main zone volume workaround")
@@ -434,21 +443,16 @@
                             "volume_down", skip_if_queued=False, insert_at=1
                         )
                 self._power_zone_1 = self.power.get("1")  # cache value
 
                 # Implement a command queue so that we can queue commands if we
                 # need to update attributes that only get updated when we
                 # request them to change.
-                if len(self._command_queue) > 0 and (
-                    self._command_queue_task is None or self._command_queue_task.done()
-                ):  # pylint: disable=W0212
-                    _LOGGER.info(
-                        "Scheduling command queue. (%s)", str(self._command_queue)
-                    )
-                    await self._command_queue_schedule()
+                if len(self._command_queue) > 0:
+                    self._command_queue_schedule()
 
                 # NOTE: to avoid deadlocks, do not run any operations that
                 # depend on further responses (returned by the listener) within
                 # the listener loop.
 
                 if updated_zones:
                     action = f" while calling zone callbacks for {updated_zones}"
@@ -460,15 +464,14 @@
             except asyncio.CancelledError:
                 if debug_listener:
                     _LOGGER.debug(">> PioneerAVR._connection_listener() cancelled")
                 running = False
                 break
             except Exception as exc:  # pylint: disable=broad-except
                 _LOGGER.error("listener exception%s: %s", action, str(exc))
-                print(exc)
                 # continue listening on exception
 
         if running and self.available:
             # Trigger disconnection if not already disconnected
             await self.disconnect()
 
         _LOGGER.debug(">> PioneerAVR._connection_listener() completed")
@@ -585,52 +588,77 @@
                     _LOGGER.debug("delaying command for %.3f s", delay)
                 await asyncio.sleep(command_delay - since_command)
         _LOGGER.debug("sending command: %s", command)
         self._writer.write(command.encode("ASCII") + b"\r")
         await self._writer.drain()
         self._last_command = time.time()
 
+    async def _wait_for_response(
+        self, command: str, response_prefix: str, ignore_error: bool
+    ) -> str | bool:
+        """Wait for a response to a request."""
+        debug_command = self._params[PARAM_DEBUG_COMMAND]
+
+        while True:
+            await self._response_event.wait()
+            self._response_event.clear()
+            for response in self._response_queue:
+                if response.startswith(response_prefix):
+                    if debug_command:
+                        _LOGGER.debug(
+                            "AVR command %s returned response: %s", command, response
+                        )
+                    return response
+                if response.startswith("E"):
+                    err = f"AVR command {command} returned error: {response}"
+                    if ignore_error is None:
+                        raise RuntimeError(err)
+                    if ignore_error:
+                        _LOGGER.debug(err)
+                    else:
+                        _LOGGER.error(err)
+                    return False
+            self._response_queue = []
+
     async def send_raw_request(
-        self, command, response_prefix, ignore_error=None, rate_limit=True
-    ):
+        self,
+        command: str,
+        response_prefix: str,
+        ignore_error: bool | None = None,
+        rate_limit: bool = True,
+    ) -> str | bool | None:
         """Send a raw command to the AVR and return the response."""
         debug_command = self._params[PARAM_DEBUG_COMMAND]
         if debug_command:
             _LOGGER.debug(
                 '>> PioneerAVR.send_raw_request("%s", %s, ignore_error=%s, rate_limit=%s)',
                 command,
                 response_prefix,
                 ignore_error,
                 rate_limit,
             )
-        async with self._request_lock:
+        async with self._request_lock:  ## Only send one request at a time
+            self._response_queue = []
+            self._queue_responses = (
+                True  ## Start queueing responses before sending command
+            )
+            self._response_event.clear()
             await self.send_raw_command(command, rate_limit=rate_limit)
-            while True:
-                response = await self._read_response(timeout=self._timeout)
-
-                # Check response
-                if response is None:
-                    _LOGGER.debug("AVR command %s timed out", command)
-                    return None
-                elif response.startswith(response_prefix):
-                    if debug_command:
-                        _LOGGER.debug(
-                            "AVR command %s returned response: %s", command, response
-                        )
-                    return response
-                elif response.startswith("E"):
-                    err = f"AVR command {command} returned error: {response}"
-                    if ignore_error is None:
-                        raise RuntimeError(err)
-                    elif not ignore_error:
-                        _LOGGER.error(err)
-                        return False
-                    elif ignore_error:
-                        _LOGGER.debug(err)
-                        return False
+            try:
+                response = await safe_wait_for(
+                    self._wait_for_response(command, response_prefix, ignore_error),
+                    timeout=self._timeout,
+                )
+            except asyncio.TimeoutError:  # response timer expired
+                _LOGGER.debug("AVR command %s timed out", command)
+                response = None
+
+            self._queue_responses = False
+            self._response_queue = []
+            return response
 
     async def send_command(
         self,
         command,
         zone="1",
         prefix="",
         ignore_error=None,
@@ -756,14 +784,15 @@
 
     async def build_source_dict(self):
         """Generate source id<->name translation tables."""
         timeouts = 0
         self._set_query_sources(True)
         self._source_name_to_id = {}
         self._source_id_to_name = {}
+        await self._command_queue_wait()  ## wait for command queue to complete
         _LOGGER.info("querying AVR source names")
         async with self._update_lock:
             for src_id in range(self._params[PARAM_MAX_SOURCE_ID] + 1):
                 response = await self.send_raw_request(
                     "?RGB" + str(src_id).zfill(2),
                     "RGB",
                     ignore_error=True,
@@ -944,32 +973,35 @@
         if parsed_response is not None:
             for response in parsed_response:
                 if isfunction(response.base_property):
                     ## Call PioneerAVR class function
                     response.base_property(self)
                 elif response.base_property is not None:
                     current_value = getattr(self, response.base_property)
-                    if response.property_name is None and response.zone not in [Zones.ALL, None]:
+                    if response.property_name is None and response.zone not in [
+                        Zones.ALL,
+                        None,
+                    ]:
                         if current_value.get(response.zone.value) is not response.value:
                             current_value[response.zone.value] = response.value
                             setattr(self, response.base_property, current_value)
                             _LOGGER.info(
                                 "Zone %s: %s: %s (%s)",
                                 response.zone.value,
                                 response.base_property,
                                 getattr(self, response.base_property)[
                                     response.zone.value
                                 ],
                                 response.raw,
                             )
 
-                    elif (
-                        response.property_name is not None and
-                        response.zone not in [Zones.ALL, None]
-                    ):
+                    elif response.property_name is not None and response.zone not in [
+                        Zones.ALL,
+                        None,
+                    ]:
                         # Set default value first otherwise we hit an exception
                         current_value.setdefault(response.zone.value, {})
                         if (
                             current_value.get(response.zone.value).get(
                                 response.property_name
                             )
                             is not response.value
@@ -986,15 +1018,18 @@
                                 response.property_name,
                                 getattr(self, response.base_property)[
                                     response.zone.value
                                 ][response.property_name],
                                 response.raw,
                             )
 
-                    elif response.property_name is None and response.zone in [Zones.ALL, None]:
+                    elif response.property_name is None and response.zone in [
+                        Zones.ALL,
+                        None,
+                    ]:
                         if current_value is not response.value:
                             current_value = response.value
                             setattr(self, response.base_property, current_value)
                             _LOGGER.info(
                                 "Global: %s: %s (%s)",
                                 response.base_property,
                                 getattr(self, response.base_property),
@@ -1176,15 +1211,15 @@
             now = time.time()
             full_update = self._full_update
             scan_interval = self.scan_interval
             since_updated = scan_interval + 1
             since_updated_str = "never"
             if self._last_updated:
                 since_updated = now - self._last_updated
-                since_updated_str = "%.3f s ago" % since_updated
+                since_updated_str = f"{since_updated:.3f} s ago"
 
             if full_update or not scan_interval or since_updated > scan_interval:
                 _LOGGER.info(
                     "updating AVR status (full=%s, last updated %s)",
                     full_update,
                     since_updated_str,
                 )
@@ -1307,28 +1342,42 @@
                 await self.send_command(command, ignore_error=True)
             self._command_queue.pop(0)
 
         if debug_command:
             _LOGGER.debug("command queue finished")
         return True
 
+    async def _command_queue_wait(self):
+        """Wait for command queue to be flushed."""
+        if self._params[PARAM_DEBUG_COMMAND]:
+            _LOGGER.debug(">> PioneerAVR._command_queue_wait()")
+        if self._command_queue_task:
+            if self._command_queue_task.done():
+                self._command_queue_task = None
+            else:
+                await asyncio.wait([self._command_queue_task])
+
     async def _command_queue_cancel(self):
         """Cancel any pending commands and the task itself."""
         debug_command = self._params[PARAM_DEBUG_COMMAND]
         await cancel_task(
             self._command_queue_task, "command_queue", debug=debug_command
         )
         self._command_queue_task = None
+        self._command_queue = []
 
-    async def _command_queue_schedule(self):
+    def _command_queue_schedule(self):
         """Schedule commands to queue."""
         if self._params[PARAM_DEBUG_COMMAND]:
             _LOGGER.debug(">> PioneerAVR._command_queue_schedule()")
-        await self._command_queue_cancel()
-        self._command_queue_task = asyncio.create_task(self._execute_command_queue())
+        ## NOTE: does not create new task if one already exists
+        if self._command_queue_task is None or self._command_queue_task.done():
+            self._command_queue_task = asyncio.create_task(
+                self._execute_command_queue()
+            )
 
     def queue_command(self, command, skip_if_queued=True, insert_at=-1):
         """Add a new command to the queue to run."""
         if self._params[PARAM_DEBUG_COMMAND]:
             _LOGGER.debug(">> PioneerAVR.queue_command(%s)", command)
         if not skip_if_queued or command not in self._command_queue:
             if insert_at >= 0:
@@ -1340,43 +1389,40 @@
                 _LOGGER.debug("command %s already queued, skipping", command)
 
     async def _calculate_am_frequency_step(self):
         """
         Automatically calculate the AM frequency step by stepping the frequency
         up and then down.
         """
-        _LOGGER.debug(">> PioneerAVR._calculate_am_frequency_step() ")
+        debug_command = self._params[PARAM_DEBUG_COMMAND]
+        if debug_command:
+            _LOGGER.debug(">> PioneerAVR._calculate_am_frequency_step() ")
         # Try sending the query_tuner_am_step command first.
         await self.send_command(command="query_tuner_am_step", ignore_error=True)
+
         # Check if freq step is None, band is set to AM and current source is
         # set to tuner for at least one zone. This function otherwise does not work.
         if (
             self._params.get(PARAM_TUNER_AM_FREQ_STEP) is None
-            and self.tuner.get("band") == "A"
-            and ("02" in list([v for k, v in self.source.items()]))
+            and self.tuner.get("band") == "AM"
+            and "02" in self.source.values()
         ):
-            current_f = self.tuner.get("frequency")
-            await self.send_command("increase_tuner_frequency", ignore_error=False)
-            # Sleep for 1s to allow for other updates and the responses to be parsed
-            await asyncio.sleep(1)
-            new_f = self.tuner.get("frequency")
-
-            while new_f == current_f:
-                _LOGGER.warning(
-                    "Frequency increment has not changed value, %s old %s",
-                    new_f,
-                    current_f,
-                )
-                # Wait until new_f != current_f
+            current_freq = self.tuner.get("frequency")
+            new_freq = current_freq
+            count = 5
+            while new_freq == current_freq and count > 0:
                 await self.send_command("increase_tuner_frequency", ignore_error=False)
-                # Sleep for 1s to allow for other updates and the responses to be parsed
-                await asyncio.sleep(1)
-                new_f = self.tuner.get("frequency")
-
-            self._params[PARAM_TUNER_AM_FREQ_STEP] = new_f - current_f
+                new_freq = self.tuner.get("frequency")
+                count -= 1
+            if new_freq == current_freq and count == 0:
+                _LOGGER.warning("unable to calculate tuner AM frequency step")
+
+            self._system_params[PARAM_TUNER_AM_FREQ_STEP] = new_freq - current_freq
+            self._update_params()
+            await asyncio.sleep(1)  ## wait for tuner command to complete
             await self.send_command("decrease_tuner_frequency", ignore_error=True)
 
         return True
 
     async def set_volume_level(self, target_volume: int, zone="1"):
         """Set volume level (0..185 for Zone 1, 0..81 for other Zones)."""
         self._check_zone(zone)
@@ -1584,85 +1630,95 @@
             await self.send_command(
                 "set_amp_status",
                 zone,
                 self._get_parameter_key_from_value(amp, AMP_MODES),
                 ignore_error=False,
             )
 
-    async def set_tuner_frequency(self, band: str, frequency: float, zone: str = "1"):
-        """Set the tuner frequency and band."""
+    async def _set_tuner_band(self, band: str = "FM", zone: str = "1"):
+        """Set the tuner band."""
 
+        band = band.upper()
         if (self.tuner.get("band") is None) or (self.power.get(zone) is False):
-            raise SystemError(
-                "Tuner functions are currently not available. "
-                "Ensure Zone is on and source is set to tuner."
-            )
+            raise SystemError("tuner is unavailable")
+        if band not in ["AM", "FM"]:
+            raise ValueError(f"tuner band {band} is invalid")
 
-        if band.upper() == "AM" and self._params.get(PARAM_TUNER_AM_FREQ_STEP) is None:
-            raise ValueError(
-                "AM Tuner functions are currently not available. "
-                "Ensure 'am_frequency_step' is set."
+        # Set the tuner band
+        if band != self.tuner.get("band"):
+            await self.send_command(
+                {"AM": "set_tuner_band_am", "FM": "set_tuner_band_fm"}[band],
+                zone,
+                ignore_error=False,
             )
 
-        if band.upper() != "AM" and band.upper() != "FM":
-            raise ValueError("The provided band is invalid")
+    async def _step_tuner_frequency(self, band: str, frequency: float):
+        """Step the tuner frequency until requested frequency is reached."""
+        current_freq = self.tuner.get("frequency")
+        if band == "AM":
+            if (freq_step := self._params.get(PARAM_TUNER_AM_FREQ_STEP)) is None:
+                raise ValueError(
+                    "AM Tuner functions are currently not available. "
+                    "Ensure 'am_frequency_step' is set."
+                )
 
-        if band.upper() == "AM" and self.tuner.get("band") == "F":
-            band = "A"
-            # Set the tuner band
-            await self.send_command("set_tuner_band_am", zone, ignore_error=False)
-        elif band.upper() == "FM" and self.tuner.get("band") == "A":
-            band = "F"
-            # Set the tuner band
-            await self.send_command("set_tuner_band_fm", zone, ignore_error=False)
-
-        # Round the frequency to nearest 0.05 if band is FM, otherwise divide
-        # frequency by 9 using modf so that the remainder is split out, then
-        # select the whole number response and times by 9
-        if band.upper() == "FM":
-            frequency = round(0.05 * round(frequency / 0.05), 2)
-        elif band.upper() == "AM":
-            frequency = (
-                math.modf(frequency / self._params.get(PARAM_TUNER_AM_FREQ_STEP))[1]
-            ) * self._params.get(PARAM_TUNER_AM_FREQ_STEP)
+            # Divide frequency by freq_step using modf so that the remainder is
+            # split out, then select the whole number response and times by
+            # freq_step
+            # pylint: disable=unsubscriptable-object
+            target_freq = (math.modf(frequency / freq_step)[1]) * freq_step
+        else:
+            # Round the frequency to nearest 0.05
+            target_freq = 0.05 * round(frequency / 0.05)
 
-        resp = True
-        increasing = False
         # Continue adjusting until frequency is set
-        while True:
-            to_freq = str(frequency)
-            current_freq = str(self.tuner.get("frequency"))
-
-            if increasing:
-                if current_freq >= to_freq:
-                    break
-            else:
-                if current_freq <= to_freq:
-                    break
-
-            # Decrease frequency
-            if self.tuner.get("frequency") > frequency:
+        resp = True
+        count = 100  ## Stop stepping after maximum steps
+        if target_freq > current_freq:
+            while current_freq < target_freq and count > 0 and resp:
                 resp = await self.send_command(
-                    "decrease_tuner_frequency", ignore_error=False
+                    "increase_tuner_frequency", ignore_error=False
                 )
-                increasing = False
-            else:
+                if resp is None:  ## ignore timeouts
+                    resp = True
+                current_freq = self.tuner.get("frequency")
+                count -= 1
+        elif target_freq < current_freq:
+            while current_freq > target_freq and count > 0 and resp:
                 resp = await self.send_command(
-                    "increase_tuner_frequency", ignore_error=False
+                    "decrease_tuner_frequency", ignore_error=False
                 )
-                increasing = True
+                if resp is None:  ## ignore timeouts
+                    resp = True
+                current_freq = self.tuner.get("frequency")
+                count -= 1
+
+        if count == 0:
+            _LOGGER.warning("maximum frequency step count exceeded")
+            resp = False
+        return resp
 
-            if not resp:
-                # On error, exit loop
-                break
+    async def set_tuner_frequency(
+        self, band: str, frequency: float = None, zone: str = "1"
+    ):
+        """Set the tuner frequency and band."""
+        band = band.upper()
+        await self._set_tuner_band(band, zone)
+        await self._command_queue_wait()  ## wait for AM step to be calculated
 
-        if resp:
+        if frequency is None:
             return True
-        else:
-            return False
+        elif not isinstance(frequency, float):
+            raise ValueError(f"invalid frequency {frequency}")
+        elif (band == "AM" and not 530 < frequency < 1700) or (
+            band == "FM" and not 87.5 < frequency < 108.0
+        ):
+            raise ValueError(f"frequency {frequency} out of range for band {band}")
+
+        return await self._step_tuner_frequency(band, frequency)
 
     async def set_tuner_preset(self, tuner_class: str, preset: int, zone="1"):
         """Set the tuner preset."""
         self._check_zone(zone)
         return await self.send_command(
             "set_tuner_preset",
             zone,
```

### Comparing `aiopioneer-0.4.2/aiopioneer/util.py` & `aiopioneer-0.4.3/aiopioneer/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Pioneer AVR utils. """
 import asyncio
+import contextlib
 import socket
 import random
 import logging
 
 RECONNECT_DELAY_MAX = 64
 
 _LOGGER = logging.getLogger(__name__)
@@ -80,22 +81,22 @@
     Work around issue: https://bugs.python.org/issue42130
     """
     task = asyncio.create_task(awt)
     try:
         await asyncio.wait({task}, timeout=timeout)
         if task.done():
             return task.result()
-        else:  # timeout
-            try:
-                task.cancel()
-                await task
-            except asyncio.CancelledError:
-                ## TODO: what if wait_for is cancelled when waiting for task to be cancelled?
-                pass
-            raise asyncio.TimeoutError()
+        ## timed out
+        try:
+            task.cancel()
+            await task
+        except asyncio.CancelledError:
+            ## TODO: what if wait_for is cancelled when waiting for task to be cancelled?
+            pass
+        raise asyncio.TimeoutError()
     except asyncio.CancelledError as exc:
         raise exc
 
 
 async def cancel_task(task, task_name=None, debug=False):
     """Cancels a task and waits for it to finish."""
     if task:
```

### Comparing `aiopioneer-0.4.2/aiopioneer.egg-info/PKG-INFO` & `aiopioneer-0.4.3/aiopioneer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.4.2
+Version: 0.4.3
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -125,14 +125,15 @@
 | `debug_responder` | _state_ (bool) | Enable/disable the `debug_responder` parameter.
 | `debug_updater` | _state_ (bool) | Enable/disable the `debug_updater` parameter.
 | `debug_command` | _state_ (bool) | Enable/disable the `debug_command` parameter.
 | `set_scan_interval` | _scan_interval_ (float) | Set the scan interval to _scan_interval_.
 | `get_scan_interval` | | Return the current scan interval.
 | `set_volume_level` | _volume_level_ (int) | Set the volume level for the current zone.
 | `select_source` | _source_name_ | Set the input source for the current zone.
+| `set_tuner_frequency` | _band_ _frequency_ | Set the tuner band and (optionally) frequency.
 | `send_raw_command` | _raw_command_ | Send the raw command _raw_command_ to the AVR.
 
 **NOTE:** The CLI interface may change in the future, and should not be used in scripts. Use the Python API instead.
 
 ## Source list
 
 | ID | Default Name
```

### Comparing `aiopioneer-0.4.2/aiopioneer.egg-info/SOURCES.txt` & `aiopioneer-0.4.3/aiopioneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.2/setup.py` & `aiopioneer-0.4.3/setup.py`

 * *Files identical despite different names*


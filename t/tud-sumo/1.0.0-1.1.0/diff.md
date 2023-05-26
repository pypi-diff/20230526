# Comparing `tmp/tud_sumo-1.0.0.tar.gz` & `tmp/tud_sumo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tud_sumo-1.0.0.tar", last modified: Tue Apr 18 16:17:38 2023, max compression
+gzip compressed data, was "tud_sumo-1.1.0.tar", last modified: Fri May 26 14:31:09 2023, max compression
```

## Comparing `tud_sumo-1.0.0.tar` & `tud_sumo-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.571575 tud_sumo-1.0.0/
--rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.0.0/.gitattributes
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.569332 tud_sumo-1.0.0/.github/
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.570456 tud_sumo-1.0.0/.github/workflows/
--rw-r--r--   0 callumevans (50765939) 1653728465     1084 2023-04-18 15:38:19.000000 tud_sumo-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 callumevans (50765939) 1653728465        8 2023-04-18 15:02:55.000000 tud_sumo-1.0.0/.gitignore
--rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.0.0/LICENSE
--rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-04-18 16:17:38.571428 tud_sumo-1.0.0/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      760 2023-04-18 15:15:39.000000 tud_sumo-1.0.0/README.md
--rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-04-18 16:17:33.000000 tud_sumo-1.0.0/pyproject.toml
--rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-04-18 16:17:38.571619 tud_sumo-1.0.0/setup.cfg
--rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.0.0/setup.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.570585 tud_sumo-1.0.0/tud_sumo/
--rw-r--r--   0 callumevans (50765939) 1653728465    22888 2023-04-18 15:04:51.000000 tud_sumo-1.0.0/tud_sumo/tud_sumo.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-04-18 16:17:38.571231 tud_sumo-1.0.0/tud_sumo.egg-info/
--rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      284 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/requires.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-04-18 16:17:38.000000 tud_sumo-1.0.0/tud_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:31:09.690202 tud_sumo-1.1.0/
+-rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.1.0/.gitattributes
+-rw-r--r--   0 callumevans (50765939) 1653728465       35 2023-04-18 16:21:02.000000 tud_sumo-1.1.0/.gitignore
+-rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.1.0/LICENSE
+-rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-05-26 14:31:09.690087 tud_sumo-1.1.0/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      760 2023-04-18 15:15:39.000000 tud_sumo-1.1.0/README.md
+-rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-05-26 14:28:13.000000 tud_sumo-1.1.0/pyproject.toml
+-rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-05-26 14:31:09.690244 tud_sumo-1.1.0/setup.cfg
+-rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.1.0/setup.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:31:09.688927 tud_sumo-1.1.0/tud_sumo/
+-rw-r--r--   0 callumevans (50765939) 1653728465    24250 2023-05-26 14:26:41.000000 tud_sumo-1.1.0/tud_sumo/tud_sumo.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:31:09.689926 tud_sumo-1.1.0/tud_sumo.egg-info/
+-rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/requires.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/top_level.txt
```

### Comparing `tud_sumo-1.0.0/LICENSE` & `tud_sumo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tud_sumo-1.0.0/PKG-INFO` & `tud_sumo-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud_sumo
-Version: 1.0.0
+Version: 1.1.0
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tud_sumo-1.0.0/README.md` & `tud_sumo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tud_sumo-1.0.0/pyproject.toml` & `tud_sumo-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tud_sumo"
-version = "1.0.0"
+version = "1.1.0"
 description = "TU Delft SUMO wrapper"
 readme = "README.md"
 authors = [{ name = "Callum Evans", email = "c.evans@tudelft.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `tud_sumo-1.0.0/tud_sumo/tud_sumo.py` & `tud_sumo-1.1.0/tud_sumo/tud_sumo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 
-import os, sys, traci
+import os, sys, traci, json
 from functools import reduce
 from tqdm import tqdm
 from random import randint
 import matplotlib.pyplot as plt
 import math
 
 class Simulation:
-    def __init__(self, main_junction: str = None, verbose: bool = False) -> None:
+    def __init__(self, main_junction = None, verbose = False) -> None:
         path_tools = os.path.join(os.environ.get("SUMO_HOME"), 'tools')
 
         if path_tools in sys.path: pass
         else: sys.path.append(path_tools)
 
         self.gui = False
         self.verbose = verbose or '-v' in sys.argv
 
+        self.junc_phases = None
         self.def_junc = main_junction
 
-        self.detector_list = []
+        self.available_detectors = {}
         self.step_length = 0.5
 
         self.known_vehicles = {}
         self.light_changes = 0
 
-    def start(self, config_file: str | None = None, net_file: str | None = None, route_file: str | None = None, add_file: str | None = None, cmd_options: list | None = None, warnings: bool = False, gui: bool = False) -> None:
+    def start(self, config_file = None, net_file = None, route_file = None, add_file = None, cmd_options = None, step_len = None, warnings = False, gui = False) -> None:
         """
         Intialises SUMO simulation.
         :param config_file: Location of '.sumocfg' file (can be given instead of net_file)
         :param net_file:    Location of '.net.xml' file (can be given instead of config_file)
         :param route_file:  Location of '.rou.xml' route file
         :param add_file:    Location of '.add.xml' additional file
         :param cmd_options: List of any other command line options
+        :param step_len:    Simulation step length
         :param warnings:    Print warnings
         :param gui:         Bool denoting whether to run GUI
         """
 
         self.gui = gui
         sumoCMD = ["sumo-gui"] if gui else ["sumo"]
 
@@ -46,45 +48,51 @@
             else: raise ValueError("Invalid config file extension.")
         else:
             sumoCMD += ["-n", net_file]
             if route_file != None: sumoCMD += ["-r", route_file]
             if add_file != None: sumoCMD += ["-a", add_file]
             if cmd_options != None: sumoCMD += cmd_options
         
+        if step_len != None: self.step_length = step_len
         sumoCMD += ["--step-length", str(self.step_length)]
         if not warnings or not self.verbose: sumoCMD.append("--no-warnings")
 
         traci.start(sumoCMD)
         
-        self.update_lights()
+        if self.junc_phases != None: self.update_lights()
         self.curr_step = 0
         self.time_val = traci.simulation.getTime()
-        self.detector_list = list(traci.multientryexit.getIDList())
+
+        self.available_detectors = {detector_id: 'multientryexit' for detector_id in list(traci.multientryexit.getIDList())}
+        self.available_detectors.update({detector_id: 'inductionloop' for detector_id in list(traci.inductionloop.getIDList())})
     
     def end(self):
         traci.close()
 
-    def step_to(self, end_step: int | None = None, n_steps: int | None = None, n_light_changes: int | None = None, detector_list: list | None = None, prev_data: dict | None = None, vTypes: list | str | None = None, cumulative_data: bool = False) -> dict:
+    def step_to(self, end_step = None, n_steps = None, sim_dur = None, n_light_changes = None, detector_list = None, prev_data = None, vTypes = None, get_individual_vehicles = True, cumulative_data = False) -> dict:
         """
         Step through simulation from the current time until end_step, aggregating
         data during this period.
         :param end_step:        End point for stepping through simulation
         :param n_steps:         Perform n steps of the simulation (given instead of end_steps)
+        :param sim_dur:         Simulation duration
         :param n_light_changes: Run for n light changes (across all junctions)
         :param detector_list:   List of detector IDs to collect data from (defaults to all)
         :param prev_data:       If given, new data is appended to this dictionary
         :param vTypes:          Vehicle type(s) to collect data of (list of types or string, defaults to all)
+        :param get_individual_vehicles: Collect all individual vehicle data
         :param cumulative_data: Denotes whether to get cumulative veh count and TTS values
         :return dict:           All data collected through the time period, separated by detector
         """
 
-        if detector_list == None: detector_list = self.detector_list
+        if detector_list == None: detector_list = list(self.available_detectors.keys())
         start_time = self.curr_step
 
         if end_step == None and n_steps != None: end_step = self.curr_step + n_steps
+        elif end_step == None and sim_dur != None: end_step = self.curr_step + (sim_dur / self.step_length)
         elif end_step == None and n_light_changes != None: end_step, init_changes = math.inf, self.light_changes
         elif end_step == None: raise ValueError("No time value given for step_to() function.")
 
         if prev_data == None:
             prev_steps, all_data = 0, {"data": {"detector": {}, "vehicle": {}, "all_vehicles": []}, "step_len": self.step_length, "start": start_time}
         else: 
             prev_steps = set([len(data_arr) for data_arr in prev_data["data"]["vehicle"].values()] +
@@ -95,20 +103,20 @@
             else:
                 prev_steps = prev_steps.pop()
                 all_data = prev_data
 
         if self.verbose: pbar = tqdm(desc="Running simulation", total=end_step - self.curr_step)
         while self.curr_step < end_step:
 
-            last_step_data, all_v_data = self.step(detector_list, vTypes)
-            all_data["data"]["all_vehicles"].append(all_v_data)
+            last_step_data, all_v_data = self.step(detector_list, vTypes, get_individual_vehicles)
+            if get_individual_vehicles: all_data["data"]["all_vehicles"].append(all_v_data)
 
             if len(all_data["data"]["detector"]) == 0:
                 for detector_id in detector_list:
-                    all_data["data"]["detector"][detector_id] = {"speeds": [], "veh_counts": []}
+                    all_data["data"]["detector"][detector_id] = {"type": self.available_detectors[detector_id], "speeds": [], "veh_counts": [], "occupancies": []}
                 all_data["data"]["vehicle"] = {"no_vehicles": [], "tts": [], "delay": []}
 
             for detector_id in last_step_data["detector"].keys():
                 if detector_id not in all_data["data"]["detector"].keys(): raise KeyError("Unrecognised detector ID found: "+detector_id)
                 for data_key, data_val in last_step_data["detector"][detector_id].items():
                     all_data["data"]["detector"][detector_id][data_key].append(data_val)
 
@@ -131,57 +139,63 @@
             all_data["data"]["vehicle"]["no_vehicles"] = get_cumulative_arr(all_data["data"]["vehicle"]["no_vehicles"], prev_steps)
             all_data["data"]["vehicle"]["tts"] = get_cumulative_arr(all_data["data"]["vehicle"]["tts"], prev_steps)
 
         all_data["end"] = self.curr_step
 
         return all_data
 
-    def step(self, detector_list: list | None = None, vTypes: list | str | None = None) -> dict:
+    def step(self, detector_list = None, vTypes = None, get_individual_vehicles = True) -> dict:
         """
         Increment simulation by one time step, updating light state.
         :param detector_list: List of detector IDs to collect data from
         :param vTypes:        Vehicle type(s) to collect data of (list of types or string, defaults to all)
         :return dict:         Simulation data
         """
 
         data = {"detector": {}, "vehicle": {}}
         
         traci.simulationStep()
         time_diff = traci.simulation.getTime() - self.time_val
         self.time_val = traci.simulation.getTime()
 
-        update_junc_lights = []
-        for junction_id, phases in self.junc_phases.items():
-            phases["curr_time"] += time_diff
-            if phases["curr_time"] >= phases["cycle_len"]:
-                phases["curr_time"] = 0
-                phases["curr_phase"] = 0
-                update_junc_lights.append(junction_id)
-            elif phases["curr_time"] >= sum(phases["times"][:phases["curr_phase"] + 1]): # Can't handle a phase time < the time step
-                phases["curr_phase"] += 1                                                # Need to support this?
-                update_junc_lights.append(junction_id)
+        if self.junc_phases != None:
+            update_junc_lights = []
+            for junction_id, phases in self.junc_phases.items():
+                phases["curr_time"] += time_diff
+                if phases["curr_time"] >= phases["cycle_len"]:
+                    phases["curr_time"] = 0
+                    phases["curr_phase"] = 0
+                    update_junc_lights.append(junction_id)
+                elif phases["curr_time"] >= sum(phases["times"][:phases["curr_phase"] + 1]): # Can't handle a phase time < the time step
+                    phases["curr_phase"] += 1                                                # Need to support this?
+                    update_junc_lights.append(junction_id)
 
-        self.update_lights(update_junc_lights)
+            self.update_lights(update_junc_lights)
 
-        if detector_list == None: detector_list = self.detector_list
+        if detector_list == None: detector_list = list(self.available_detectors.keys())
         for detector_id in detector_list:
-            speed = traci.multientryexit.getLastStepMeanSpeed(detector_id)
-            veh_count = traci.multientryexit.getLastStepVehicleNumber(detector_id)
-            data["detector"][detector_id] = {"speeds": speed, "veh_counts": veh_count}
+            data["detector"][detector_id] = {}
+            if self.available_detectors[detector_id] == "multientryexit":
+                data["detector"][detector_id]["speeds"] = traci.multientryexit.getLastStepMeanSpeed(detector_id)
+                data["detector"][detector_id]["veh_counts"] = traci.multientryexit.getLastStepVehicleNumber(detector_id)
+            elif self.available_detectors[detector_id] == "inductionloop":
+                data["detector"][detector_id]["speeds"] = traci.inductionloop.getLastStepMeanSpeed(detector_id)
+                data["detector"][detector_id]["veh_counts"] = traci.inductionloop.getLastStepVehicleNumber(detector_id)
+                data["detector"][detector_id]["occupancies"] = traci.inductionloop.getLastStepOccupancy(detector_id)
 
-        total_v_data, all_v_data = self.get_vehicle_data(types=vTypes)
+        total_v_data, all_v_data = self.get_vehicle_data(types=vTypes, get_individual_data=get_individual_vehicles)
         data["vehicle"]["no_vehicles"] = total_v_data["no_vehicles"]
         data["vehicle"]["tts"] = total_v_data["no_vehicles"] * self.step_length
         data["vehicle"]["delay"] = total_v_data["no_waiting"] * self.step_length
 
         self.curr_step += 1
 
         return data, all_v_data
     
-    def set_phases(self, junc_phases: dict, start_phase: int = 0) -> None:
+    def set_phases(self, junc_phases, start_phase = 0) -> None:
         """
         Sets the phases for the simulation.
         :param junc_phases: Can either be for a single junction (no junction ID given),
                             or for multiple junctions, with keys as junction ID.
         :param start_phase: Phase number to start at, defaults to 0
         """
 
@@ -197,57 +211,57 @@
         for junc_phase in self.junc_phases.values():
             if "curr_phase" not in junc_phase.keys(): junc_phase["curr_phase"] = start_phase
             if junc_phase["curr_phase"] > len(junc_phase["phases"]): junc_phase["curr_phase"] -= len(junc_phase["phases"])
 
             junc_phase["curr_time"] = sum(junc_phase["times"][:junc_phase["curr_phase"]])
             junc_phase["cycle_len"] = sum(junc_phase["times"])
 
-    def set_phase(self, junction: str, phase_no: int) -> None:
+    def set_phase(self, junction, phase_no) -> None:
         """
         Change to a different phase at the specified junction
         :param junction_id: Junction ID
         :param phase_no: Phase number
         """
         
         if 0 < phase_no < len(self.junc_phases[junction]["phases"]):
             self.junc_phases[junction]["curr_phase"] = phase_no
             self.junc_phases[junction]["curr_time"] = sum(self.junc_phase["times"][:phase_no])
 
             self.update_lights(junction)
 
         else: raise ValueError("Invalid phase number '{0}', must be: [0-{1}]".format(phase_no, len(self.junc_phases[junction]["phases"])))
 
-    def set_lights(self, junction_id: str, light_str: str) -> None:
+    def set_lights(self, junction_id, light_str) -> None:
         """
         Set lights to a specific setting. Will be overwritten at next
         light update.
         :param junction_id: Junction ID
         :param light_str: SUMO light string
         """
         traci.trafficlight.setRedYellowGreenState(junction_id, light_str)
 
-    def update_lights(self, junction_ids: list | str | None = None) -> None:
+    def update_lights(self, junction_ids = None) -> None:
         """
         Update light settings for given junctions
         :param junction_ids: Junction ID, or list of IDs (defaults to all)
         """
 
         if junction_ids is None: junction_ids = self.junc_phases.keys()
         elif isinstance(junction_ids, str): junction_ids = [junction_ids]
 
         for junction_id in junction_ids:
             curr_setting = traci.trafficlight.getRedYellowGreenState(junction_id)
             self.light_changes += 1
-            new_phase = self.junc_phases[junction_id]["phases"][self.junc_phases[junction_id]["curr_phase"]]
+            new_phase = self.junc_phases[junction_id]["phases"][self.junc_phases[junction_id]["curr_phase"]].lower()
             if '-' in new_phase:
                 new_phase = new_phase.split()
                 new_phase = "".join([new_phase[i] if new_phase[i] != '-' else curr_setting[i] for i in range(len(new_phase))])
             traci.trafficlight.setRedYellowGreenState(junction_id, new_phase)
 
-    def get_vehicle_data(self, ids: list | None = None, types: list | str | None = None, get_individual_data: bool = True) -> dict:
+    def get_vehicle_data(self, ids = None, types = None, get_individual_data = True) -> dict:
         """
         Collects vehicle data from SUMO, by id and/or type (defaults to all vehicles)
         :param ids: IDs of vehicles to fetch
         :param types: Type(s) of vehicles to fetch
         :param get_individual_data: Denotes whether to get individual speed, location & heading data
         :return dict: Vehicle data by id
         """
@@ -288,46 +302,48 @@
                                             }
                     
                 total_vehicle_data["no_vehicles"] += 1
                 if speed < 0.1: total_vehicle_data["no_waiting"] += 1
 
         return total_vehicle_data, all_vehicle_data
     
-def get_cumulative_arr(arr: list, start: int) -> list:
+def get_cumulative_arr(arr, start) -> list:
     for i in range(start, len(arr)):
         arr[i] += arr[i - 1]
     return arr
 
-def plot_vehicle_data(all_data: dict, dataset: str | list, save_fig: None | str = None) -> None:
+def plot_vehicle_data(all_data, dataset, save_fig = None) -> None:
     """
     Plots all collected vehicle or detector data.
     :param all_data: Data collected from the Simulation.step_to() function
     :param dataset: Dataset key (either "vehicle" or ["detector", detector_id])
     """
 
     default_labels = {"no_vehicles": "No. of Vehicles", "tts": "TTS (s)", "delay": "Delay (s)",
-                      "speeds": "Avg. Speed (km/h)", "veh_counts": "No. of Vehicles"}
+                      "speeds": "Avg. Speed (km/h)", "veh_counts": "No. of Vehicles", "occupancies": "Occupancy (%)"}
 
-    if isinstance(dataset, str):
+    if isinstance(dataset, str): # Sim data
         if dataset in all_data["data"].keys(): data = all_data["data"][dataset]
         else: raise KeyError("Dataset not found: '{0}'".format(dataset))
         title = dataset.title()
-    elif isinstance(dataset, list):
+    elif isinstance(dataset, list): # Detector data
         data = all_data["data"]
         for key in dataset:
             if key in data.keys(): data = data[key]
             else: raise KeyError("Dataset not found: '{0}'".format(dataset[-1]))
         title = ': '.join(dataset)
 
     else: raise ValueError("Invalid dataset key type, must be [int|str], not '{0}'".format(type(dataset).__name__))
 
-    fig, axes = plt.subplots(len(data))
+    plot_data = {key: data[key] for key in data if key in default_labels and len(data[key]) != 0}
+    fig, axes = plt.subplots(len(plot_data))
     start, end, step = all_data["start"], all_data["end"], all_data["step_len"]
 
-    for idx, (ax, (data_key, data_vals)) in enumerate(zip(axes, data.items())):
+    for idx, (ax, (data_key, data_vals)) in enumerate(zip(axes, plot_data.items())):
+        if not isinstance(data_vals, list): continue
         ax.plot([x * step for x in range(start, end)], data_vals, zorder=3)
         ax.set_title(data_key)
         if data_key in default_labels.keys(): ax.set_ylabel(default_labels[data_key])
         if idx < len(axes) - 1: ax.tick_params('x', labelbottom=False)
         else: ax.set_xlabel('Time (s)')
         ax.set_xlim([start * step, (end - 1) * step])
         ax.set_ylim([0, max(data_vals) * 1.05])
@@ -335,15 +351,15 @@
 
     fig.suptitle(title)
     fig.tight_layout()
 
     if save_fig is None: plt.show(block=True)
     else: plt.savefig(save_fig)
 
-def get_phases(Qcolor: dict, Qtime: dict, M_map: dict, blocks_lim: int | None = None, simulation_time: int | None = None) -> dict:
+def get_phases(Qcolor, Qtime, M_map, blocks_lim = None, simulation_time = None) -> dict:
     """
     Converts Qcolor, Qtime dictionaries into light settings and times
     for SUMO.
     :param Qcolor: Qcolor movement dictionary
     :param Qtime:  Qtime movement timings dictionary
     :param M_map:  Movement mapping dictionary
     :param blocks_lim: Limit on the number of blocks to convert (defaults to all)
@@ -404,15 +420,15 @@
         phases_dict["phases"].append(light_string)
         curr_time += time
 
     phases_dict["times"] = times[:blocks_lim]
 
     return phases_dict
 
-def generate_rnd_mapping(n_movements: int, map_length: int) -> dict:
+def generate_rnd_mapping(n_movements, map_length) -> dict:
     mapping = {m: ["0"]*map_length for m in range(n_movements)}
     for i in range(map_length): mapping[randint(0, n_movements-1)][i] = "1"
     mapping = {m: "".join(arr) for m, arr in mapping.items()}
     return mapping
 
 if __name__ == "__main__":
     default_junction = "J2"
```

### Comparing `tud_sumo-1.0.0/tud_sumo.egg-info/PKG-INFO` & `tud_sumo-1.1.0/tud_sumo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud-sumo
-Version: 1.0.0
+Version: 1.1.0
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


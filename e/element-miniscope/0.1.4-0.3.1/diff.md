# Comparing `tmp/element-miniscope-0.1.4.tar.gz` & `tmp/element-miniscope-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-miniscope-0.1.4.tar", last modified: Tue Nov  1 21:54:01 2022, max compression
+gzip compressed data, was "element-miniscope-0.3.1.tar", last modified: Fri May 26 19:36:57 2023, max compression
```

## Comparing `element-miniscope-0.1.4.tar` & `element-miniscope-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:54:01.945869 element-miniscope-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-01 21:53:59.000000 element-miniscope-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-11-01 21:54:01.945869 element-miniscope-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-11-01 21:53:59.000000 element-miniscope-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:54:01.945869 element-miniscope-0.1.4/element_miniscope/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:53:59.000000 element-miniscope-0.1.4/element_miniscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    45210 2022-11-01 21:53:59.000000 element-miniscope-0.1.4/element_miniscope/miniscope.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-01 21:53:59.000000 element-miniscope-0.1.4/element_miniscope/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:54:01.945869 element-miniscope-0.1.4/element_miniscope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-11-01 21:54:01.000000 element-miniscope-0.1.4/element_miniscope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-01 21:54:01.000000 element-miniscope-0.1.4/element_miniscope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:54:01.000000 element-miniscope-0.1.4/element_miniscope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-01 21:54:01.000000 element-miniscope-0.1.4/element_miniscope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-01 21:54:01.000000 element-miniscope-0.1.4/element_miniscope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:54:01.945869 element-miniscope-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-11-01 21:53:59.000000 element-miniscope-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:57.171882 element-miniscope-0.3.1/element_miniscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46341 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/miniscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/miniscope_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/element_miniscope/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/element_miniscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 19:36:57.000000 element-miniscope-0.3.1/element_miniscope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:36:57.175881 element-miniscope-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-26 19:36:54.000000 element-miniscope-0.3.1/setup.py
```

### Comparing `element-miniscope-0.1.4/LICENSE` & `element-miniscope-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `element-miniscope-0.1.4/element_miniscope/miniscope.py` & `element-miniscope-0.3.1/element_miniscope/miniscope.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-import datajoint as dj
-import numpy as np
-import pathlib
-from datetime import datetime
+import csv
 import importlib
 import inspect
-import cv2
 import json
-import csv
+import logging
+import pathlib
+from datetime import datetime
+
+import cv2
+import datajoint as dj
+import numpy as np
 from element_interface.utils import dict_to_uuid, find_full_path, find_root_directory
 
+from . import miniscope_report
+
 schema = dj.Schema()
 
 _linking_module = None
+logger = logging.getLogger("datajoint")
 
 
 def activate(
     miniscope_schema_name: str,
     *,
     create_schema: bool = True,
     create_tables: bool = True,
     linking_module: str = None,
 ):
     """Activate this schema.
 
     Args:
-        model_schema_name (str): schema name on the database server
-        create_schema (bool): when True (default), create schema in the database if it does not yet exist.
-        create_tables (str): when True (default), create schema tabkes in the database if they do not yet exist.
+        miniscope_schema_name (str): schema name on the database server
+        create_schema (bool): when True (default), create schema in the database if it
+            does not yet exist.
+        create_tables (str): when True (default), create schema takes in the database
+            if they do not yet exist.
         linking_module (str): a module (or name) containing the required dependencies.
 
     Dependencies:
 
     Upstream tables:
-        Session: parent table to Recording,
-        identifying a recording session.
-        Equipment: Reference table for Recording,
-        specifying the acquisition equipment.
+        Session: parent table to Recording, identifying a recording session.
+        Device: Reference table for Recording, specifying the acquisition device.
+        AnatomicalLocation: Reference table for anatomical region for recording acquisition.
 
     Functions:
-        get_miniscope_root_data_dir(): Returns absolute path for root data director(y/ies) with all subject/sessions data, as (list of) string(s).
-        get_session_directory(session_key: dict) Returns the session directory with all data for the session in session_key, as a string.
-        get_processed_root_data_dir(): Returns absolute path for all processed data as a string. 
+        get_miniscope_root_data_dir(): Returns absolute path for root data director(y/ies)
+            with all subject/sessions data, as (list of) string(s).
+        get_session_directory(session_key: dict) Returns the session directory with all
+            data for the session in session_key, as a string.
+        get_processed_root_data_dir(): Returns absolute path for all processed data as
+            a string.
     """
 
     if isinstance(linking_module, str):
         linking_module = importlib.import_module(linking_module)
     assert inspect.ismodule(
         linking_module
     ), "The argument 'dependency' must be a module's name or a module"
@@ -54,24 +63,25 @@
 
     schema.activate(
         miniscope_schema_name,
         create_schema=create_schema,
         create_tables=create_tables,
         add_objects=_linking_module.__dict__,
     )
+    miniscope_report.activate(f"{miniscope_schema_name}_report", miniscope_schema_name)
 
 
 # Functions required by the element-miniscope  -----------------------------------------
 
 
 def get_miniscope_root_data_dir() -> list:
     """Fetches absolute data path to miniscope data directory.
-    
+
     The absolute path here is used as a reference for all downstream relative paths used in DataJoint.
-    
+
     Returns:
         A list of the absolute path to miniscope data directory.
     """
 
     root_directories = _linking_module.get_miniscope_root_data_dir()
     if isinstance(root_directories, (str, pathlib.Path)):
         root_directories = [root_directories]
@@ -83,43 +93,33 @@
 
 
 def get_session_directory(session_key: dict) -> str:
     """Pulls session directory information from database.
 
     Args:
         session_key (dict): a dictionary containing session information.
-    
+
     Returns:
         Session directory as a string.
     """
     return _linking_module.get_session_directory(session_key)
 
 
-def get_processed_root_data_dir() -> str:
-    """Retrieves the root directory for all processed data
-    """
-
-    if hasattr(_linking_module, "get_processed_root_data_dir"):
-        return _linking_module.get_processed_root_data_dir()
-    else:
-        return get_miniscope_root_data_dir()[0]
-
-
 # Experiment and analysis meta information -------------------------------------
 
 
 @schema
 class AcquisitionSoftware(dj.Lookup):
     """Software used for miniscope acquisition.
 
     Attributes:
-        acquisition_software (varchar(24) ): Name of the miniscope acquisition software."""
+        acq_software (varchar(24) ): Name of the miniscope acquisition software."""
 
     definition = """
-    acquisition_software: varchar(24)
+    acq_software: varchar(24)
     """
     contents = zip(["Miniscope-DAQ-V3", "Miniscope-DAQ-V4"])
 
 
 @schema
 class Channel(dj.Lookup):
     """Number of channels in the miniscope recording.
@@ -136,38 +136,36 @@
 @schema
 class Recording(dj.Manual):
     """Table for discrete recording sessions with the miniscope.
 
     Attributes:
         Session (foreign key): Session primary key.
         recording_id (foreign key, int): Unique recording ID.
-        Equipment: Lookup table for miniscope equipment information.
+        Device: Lookup table for miniscope device information.
         AcquisitionSoftware: Lookup table for miniscope acquisition software.
-        recording_directory (varchar(255) ): relative path to recording files.
         recording_notes (varchar(4095) ): notes about the recording session.
     """
 
     definition = """
     -> Session
     recording_id: int
     ---
-    -> Equipment
+    -> Device
     -> AcquisitionSoftware
-    recording_directory: varchar(255)  # relative to root data directory
     recording_notes='' : varchar(4095) # free-notes
     """
 
 
 @schema
 class RecordingLocation(dj.Manual):
     """Brain location where the miniscope recording is acquired.
 
     Attributes:
         Recording (foreign key): Recording primary key.
-        Anatomical Location: Select the anatomical region where miniscope recording was acquired. 
+        Anatomical Location: Select the anatomical region where recording was acquired.
     """
 
     definition = """
     # Brain location where this miniscope recording is acquired
     -> Recording
     ---
     -> AnatomicalLocation
@@ -180,23 +178,23 @@
 
     Attributes:
         Recording (foreign key): Recording primary key.
         nchannels (tinyint): Number of recording channels.
         nframes (int): Number of recorded frames.
         px_height (smallint): Height in pixels.
         px_width (smallint): Width in pixels.
-        um_height (float): Height in microns. 
+        um_height (float): Height in microns.
         um_width (float): Width in microns.
         fps (float): Frames per second, (Hz).
         gain (float): Recording gain.
         spatial_downsample (tinyint): Amount of downsampling applied.
         led_power (float): LED power used for the recording.
         time_stamps (longblob): Time stamps for each frame.
         recording_datetime (datetime): Datetime of the recording.
-        recording_duration (float): Total recording duration (seconds). 
+        recording_duration (float): Total recording duration (seconds).
     """
 
     definition = """
     # Store metadata about recording
     -> Recording
     ---
     nchannels            : tinyint   # number of channels
@@ -230,30 +228,29 @@
         file_path: varchar(255)      # relative to root data directory
         """
 
     def make(self, key):
         """Populate table with recording file metadata."""
 
         # Search recording directory for miniscope raw files
-        acquisition_software, recording_directory = (Recording & key).fetch1(
-            "acquisition_software", "recording_directory"
-        )
+        acq_software = (Recording & key).fetch1("acq_software")
+        recording_directory = get_session_directory(key)
 
         recording_path = find_full_path(
             get_miniscope_root_data_dir(), recording_directory
         )
 
         recording_filepaths = [
             file_path.as_posix() for file_path in recording_path.glob("*.avi")
         ]
 
         if not recording_filepaths:
             raise FileNotFoundError(f"No .avi files found in " f"{recording_directory}")
 
-        if acquisition_software == "Miniscope-DAQ-V3":
+        if acq_software == "Miniscope-DAQ-V3":
             recording_timestamps = recording_path / "timestamp.dat"
             if not recording_timestamps.exists():
                 raise FileNotFoundError(
                     f"No timestamp file found in " f"{recording_directory}"
                 )
 
             nchannels = 1  # Assumes a single channel
@@ -268,15 +265,15 @@
             _, frame = video.read()
             frame_size = np.shape(frame)
             px_height = frame_size[0]
             px_width = frame_size[1]
 
             fps = video.get(cv2.CAP_PROP_FPS)
 
-        elif acquisition_software == "Miniscope-DAQ-V4":
+        elif acq_software == "Miniscope-DAQ-V4":
             recording_metadata = list(recording_path.glob("metaData.json"))[0]
             recording_timestamps = list(recording_path.glob("timeStamps.csv"))[0]
 
             if not recording_metadata.exists():
                 raise FileNotFoundError(
                     f"No .json file found in " f"{recording_directory}"
                 )
@@ -300,15 +297,15 @@
             spatial_downsample = 1  # Assumes no spatial downsampling
             led_power = metadata["led0"]
             time_stamps = np.array(
                 [list(map(int, time_stamps[i])) for i in range(1, len(time_stamps))]
             )
         else:
             raise NotImplementedError(
-                f"Loading routine not implemented for {acquisition_software}"
+                f"Loading routine not implemented for {acq_software}"
                 " acquisition software"
             )
 
         # Insert in RecordingInfo
         self.insert1(
             dict(
                 key,
@@ -346,19 +343,19 @@
 
 @schema
 class ProcessingMethod(dj.Lookup):
     """Method or analysis software to process miniscope acquisition.
 
     Attributes:
         processing_method (foreign key, varchar16): Recording processing method (e.g. CaImAn).
-        processing_method_desc (varchar(1000) ): Additional information about the processing method. 
+        processing_method_desc (varchar(1000) ): Additional information about the processing method.
     """
 
     definition = """
-    # Method, package, analysis software used for processing of miniscope data 
+    # Method, package, analysis software used for processing of miniscope data
     # (e.g. CaImAn, etc.)
     processing_method: varchar(16)
     ---
     processing_method_desc='': varchar(1000)
     """
 
     contents = [("caiman", "caiman analysis suite")]
@@ -430,22 +427,37 @@
                     "The specified param-set already exists - name: {}".format(pname)
                 )
         else:
             cls.insert1(param_dict)
 
 
 @schema
+class MaskType(dj.Lookup):
+    """Possible classifications of a segmented mask.
+
+    Attributes:
+        mask_type (foreign key, varchar(16) ): Type of segmented mask.
+    """
+
+    definition = """ # Possible classifications for a segmented mask
+    mask_type        : varchar(16)
+    """
+
+    contents = zip(["soma", "axon", "dendrite", "neuropil", "artefact", "unknown"])
+
+
+@schema
 class ProcessingTask(dj.Manual):
     """Table marking manual or automatic processing task.
 
     Attributes:
         RecordingInfo (foreign key): Recording info primary key.
         ProcessingParamSet (foreign key): Processing param set primary key.
         processing_output_dir (varchar(255) ): relative output data directory for processed files.
-        task_mode (enum): `Load` existing results or `trigger` new processing task.   
+        task_mode (enum): `Load` existing results or `trigger` new processing task.
     """
 
     definition = """
     # Manual table marking a processing task to be triggered or manually processed
     -> RecordingInfo
     -> ProcessingParamSet
     ---
@@ -458,15 +470,15 @@
 @schema
 class Processing(dj.Computed):
     """Automatic table that beings the miniscope processing pipeline.
 
     Attributes:
         ProcessingTask (foreign key): Processing task primary key.
         processing_time (datetime): Generates time of the processed results.
-        package_version (varchar(16) ): Package version information. 
+        package_version (varchar(16) ): Package version information.
     """
 
     definition = """
     -> ProcessingTask
     ---
     processing_time     : datetime  # generation time of processed, segmented results
     package_version=''  : varchar(16)
@@ -482,15 +494,15 @@
         if task_mode == "load":
             method, loaded_result = get_loader_result(key, ProcessingTask)
             if method == "caiman":
                 loaded_caiman = loaded_result
                 key = {**key, "processing_time": loaded_caiman.creation_time}
             else:
                 raise NotImplementedError(
-                    f"Loading of {method} data is not yet" f"supported"
+                    f"Loading of {method} data is not yet supported"
                 )
         elif task_mode == "trigger":
             method = (
                 ProcessingTask * ProcessingParamSet * ProcessingMethod * Recording & key
             ).fetch1("processing_method")
 
             if method == "caiman":
@@ -561,29 +573,29 @@
         curation_time (datetime): Time of generation of curated results.
         curation_output_dir (varchar(255) ): Output directory for curated results.
         manual_curation (bool): If True, manual curation has been performed.
         curation_note (varchar(2000) ): Optional description of the curation procedure.
     """
 
     definition = """
-    # Different rounds of curation performed on the processing results of the data 
+    # Different rounds of curation performed on the processing results of the data
     # (no-curation can also be included here)
     -> Processing
     curation_id: int
     ---
-    curation_time: datetime             # time of generation of these curated results 
-    curation_output_dir: varchar(255)   # output directory of the curated results, 
+    curation_time: datetime             # time of generation of these curated results
+    curation_output_dir: varchar(255)   # output directory of the curated results,
                                         # relative to root data directory
     manual_curation: bool               # has manual curation been performed?
-    curation_note='': varchar(2000)  
+    curation_note='': varchar(2000)
     """
 
+    @classmethod
     def create1_from_processing_task(self, key, is_curated=False, curation_note=""):
-        """Given a "ProcessingTask", create a new corresponding "Curation"
-        """
+        """Given a "ProcessingTask", create a new corresponding "Curation" """
         if key not in Processing():
             raise ValueError(
                 f"No corresponding entry in Processing available for: "
                 f"{key}; run `Processing.populate(key)`"
             )
 
         output_dir = (ProcessingTask & key).fetch1("processing_output_dir")
@@ -622,117 +634,113 @@
         Curation (foreign key): Curation primary key.
         Channel.proj(motion_correct_channel='channel'): Channel used for motion correction.
     """
 
     definition = """
     -> Curation
     ---
-    -> Channel.proj(motion_correct_channel='channel') # channel used for 
+    -> Channel.proj(motion_correct_channel='channel') # channel used for
                                                       # motion correction
     """
 
     class RigidMotionCorrection(dj.Part):
-        """Automated table with ridge motion correction data. 
+        """Automated table with ridge motion correction data.
 
         Attributes:
             MotionCorrection (foreign key): MotionCorrection primary key.
             outlier_frames (longblob): Mask with true for frames with outlier shifts.
             y_shifts (longblob): y motion correction shifts, pixels.
             x_shifts (longblob): x motion correction shifts, pixels.
             y_std (float): Standard deviation of y shifts across all frames, pixels.
             x_std (float): Standard deviation of x shifts across all frames, pixels.
         """
 
         definition = """
         -> master
         ---
-        outlier_frames=null : longblob  # mask with true for frames with outlier shifts 
+        outlier_frames=null : longblob  # mask with true for frames with outlier shifts
                                         # (already corrected)
         y_shifts            : longblob  # (pixels) y motion correction shifts
         x_shifts            : longblob  # (pixels) x motion correction shifts
-        y_std               : float     # (pixels) standard deviation of 
+        y_std               : float     # (pixels) standard deviation of
                                         # y shifts across all frames
-        x_std               : float     # (pixels) standard deviation of 
+        x_std               : float     # (pixels) standard deviation of
                                         # x shifts across all frames
         """
 
     class NonRigidMotionCorrection(dj.Part):
         """Automated table with piece-wise rigid motion correction data.
 
         Attributes:
             MotionCorrection (foreign key): MotionCorrection primary key.
             outlier_frames (longblob): Mask with true for frames with outlier shifts (already corrected).
             block_height (int): Height in pixels.
             block_width (int): Width in pixels.
             block_count_y (int): Number of blocks tiled in the y direction.
-            block_count_x (int): Number of blocks tiled in the x direction. 
+            block_count_x (int): Number of blocks tiled in the x direction.
         """
 
         definition = """
         -> master
         ---
-        outlier_frames=null             : longblob  # mask with true for frames with 
+        outlier_frames=null             : longblob  # mask with true for frames with
                                                     # outlier shifts (already corrected)
         block_height                    : int       # (pixels)
         block_width                     : int       # (pixels)
-        block_count_y                   : int       # number of blocks tiled in the 
+        block_count_y                   : int       # number of blocks tiled in the
                                                     # y direction
-        block_count_x                   : int       # number of blocks tiled in the 
+        block_count_x                   : int       # number of blocks tiled in the
                                                     # x direction
         """
 
     class Block(dj.Part):
         """Automated table with data for blocks used in non-rigid motion correction.
 
         Attributes:
             master.NonRigidMotionCorrection (foreign key): NonRigidMotionCorrection primary key.
             block_id (foreign key, int): Unique ID for each block.
             block_y (longblob): y_start and y_end of this block in pixels.
             block_x (longblob): x_start and x_end of this block in pixels.
             y_shifts (longblob): y motion correction shifts for every frame in pixels.
-            x_shifts (longblob): x motion correction shifta for every frame in pixels. 
+            x_shifts (longblob): x motion correction shifts for every frame in pixels.
             y_std (float): standard deviation of y shifts across all frames in pixels.
-            x_std (float): standard deviation of x shifts across all frames in pixels.  
+            x_std (float): standard deviation of x shifts across all frames in pixels.
         """
 
         definition = """  # FOV-tiled blocks used for non-rigid motion correction
         -> master.NonRigidMotionCorrection
-        block_id        : int
+        block_id : int
         ---
-        block_y         : longblob  # (y_start, y_end) in pixel of this block
-        block_x         : longblob  # (x_start, x_end) in pixel of this block
-        y_shifts        : longblob  # (pixels) y motion correction shifts for 
-                                    # every frame
-        x_shifts        : longblob  # (pixels) x motion correction shifts for 
-                                    # every frame
-        y_std           : float     # (pixels) standard deviation of y shifts 
-                                    # across all frames
-        x_std           : float     # (pixels) standard deviation of x shifts 
-                                    # across all frames
+        block_y  : longblob  # (y_start, y_end) in pixel of this block
+        block_x  : longblob  # (x_start, x_end) in pixel of this block
+        y_shifts : longblob  # (pixels) y motion correction shifts for every frame
+        x_shifts : longblob  # (pixels) x motion correction shifts for every frame
+        y_std    : float     # (pixels) standard deviation of y shifts across all frames
+        x_std    : float     # (pixels) standard deviation of x shifts across all frames
         """
 
     class Summary(dj.Part):
         """A summary image for each field and channel after motion correction.
 
         Attributes:
             MotionCorrection (foreign key): MotionCorrection primary key.
             ref_image (longblob): Image used as the alignment template.
             average_image (longblob): Mean of registered frames.
-            correlation_image (longblob): Correlation map computed during cell detection. 
+            correlation_image (longblob): Correlation map computed during cell detection.
             max_proj_image (longblob): Maximum of registered frames.
         """
 
         definition = """ # summary images for each field and channel after corrections
         -> master
         ---
-        ref_image=null          : longblob  # image used as alignment template
-        average_image           : longblob  # mean of registered frames
-        correlation_image=null  : longblob  # correlation map 
-                                            # (computed during cell detection)
-        max_proj_image=null     : longblob  # max of registered frames
+        ref_image=null         : longblob  # image used as alignment template
+        average_image          : longblob  # mean of registered frames
+        correlation_image=null : longblob  # correlation map
+                                           # (computed during cell detection)
+        max_proj_image=null    : longblob  # max of registered frames
         """
 
     def make(self, key):
         """Populate tables with motion correction data."""
         method, loaded_result = get_loader_result(key, ProcessingTask)
 
         if method == "caiman":
@@ -843,90 +851,95 @@
 
 
 @schema
 class Segmentation(dj.Computed):
     """Automated table computes different mask segmentations.
 
     Attributes:
-        Curations (foreign key): Curation primary key.
+        Curation (foreign key): Curation primary key.
     """
 
     definition = """ # Different mask segmentations.
     -> Curation
     """
 
     class Mask(dj.Part):
         """Image masks produced during segmentation.
 
         Attributes:
             Segmentation (foreign key): Segmentation primary key.
-            mask_id (foreign key, smallint): Unique ID for each mask.
+            mask (smallint): Unique ID for each mask.
             channel.proj(segmentation_channel='channel') (query): Channel to be used for segmentation.
             mask_npix (int): Number of pixels in the mask.
             mask_center_x (int): Center x coordinate in pixels.
             mask_center_y (int): Center y coordinate in pixels.
             mask_xpix (longblob): x coordinates of the mask in pixels.
             mask_ypix (longblob): y coordinates of the mask in pixels.
-            mask_weights (longblob): weights of the mask at the indicies above.
+            mask_weights (longblob): weights of the mask at the indices above.
         """
 
         definition = """ # A mask produced by segmentation.
         -> master
-        mask_id              : smallint
+        mask                 : smallint
         ---
         -> Channel.proj(segmentation_channel='channel')  # channel used for segmentation
         mask_npix            : int       # number of pixels in this mask
         mask_center_x=null   : int       # (pixels) center x coordinate
         mask_center_y=null   : int       # (pixels) center y coordinate
         mask_xpix=null       : longblob  # (pixels) x coordinates
         mask_ypix=null       : longblob  # (pixels) y coordinates
         mask_weights         : longblob  # weights of the mask at the indices above
         """
 
     def make(self, key):
-        """Populates table with segementation data."""
+        """Populates table with segmentation data."""
         method, loaded_result = get_loader_result(key, Curation)
 
         if method == "caiman":
             loaded_caiman = loaded_result
 
             # infer `segmentation_channel` from `params` if available,
             # else from caiman loader
             params = (ProcessingParamSet * ProcessingTask & key).fetch1("params")
             segmentation_channel = params.get(
                 "segmentation_channel", loaded_caiman.segmentation_channel
             )
 
             masks, cells = [], []
             for mask in loaded_caiman.masks:
+                # Sample data had _id key, not mask. Permitting both
+                mask_id = mask.get("mask", mask["mask_id"])
                 masks.append(
                     {
                         **key,
                         "segmentation_channel": segmentation_channel,
-                        "mask_id": mask["mask_id"],
+                        "mask": mask_id,
                         "mask_npix": mask["mask_npix"],
                         "mask_center_x": mask["mask_center_x"],
                         "mask_center_y": mask["mask_center_y"],
                         "mask_xpix": mask["mask_xpix"],
                         "mask_ypix": mask["mask_ypix"],
                         "mask_weights": mask["mask_weights"],
                     }
                 )
 
                 if loaded_caiman.cnmf.estimates.idx_components is not None:
-                    if mask["mask_id"] in loaded_caiman.cnmf.estimates.idx_components:
+                    if mask_id in loaded_caiman.cnmf.estimates.idx_components:
                         cells.append(
                             {
                                 **key,
                                 "mask_classification_method": "caiman_default_classifier",
-                                "mask_id": mask["mask_id"],
+                                "mask": mask_id,
                                 "mask_type": "soma",
                             }
                         )
 
+            if not all([all(m.values()) for m in masks]):
+                logger.warning("Could not load all pixel values for at least one mask")
+
             self.insert1(key)
             self.Mask.insert(masks, ignore_extra_fields=True)
 
             if cells:
                 MaskClassification.insert1(
                     {**key, "mask_classification_method": "caiman_default_classifier"},
                     allow_direct_insert=True,
@@ -936,47 +949,33 @@
                 )
 
         else:
             raise NotImplementedError(f"Unknown/unimplemented method: {method}")
 
 
 @schema
-class MaskType(dj.Lookup):
-    """Possible classifications of a segmented mask. 
-
-    Attributes:
-        mask_type (foreign key, varchar(16) ): Type of segmented mask.
-    """
-
-    definition = """ # Possible classifications for a segmented mask
-    mask_type        : varchar(16)
-    """
-
-    contents = zip(["soma", "axon", "dendrite", "neuropil", "artefact", "unknown"])
-
-
-@schema
 class MaskClassificationMethod(dj.Lookup):
     """Method to classify segmented masks.
 
     Attributes:
-        mask_classification_method (foreign key, varchar(48) ): Method by which masks are classified into mask types.
+        mask_classification_method (foreign key, varchar(48) ): Method by which masks
+            are classified into mask types.
     """
 
     definition = """
     mask_classification_method: varchar(48)
     """
 
     contents = zip(["caiman_default_classifier"])
 
 
 @schema
 class MaskClassification(dj.Computed):
     """Automated table with mask classification data.
-    
+
     Attributes:
         Segmentation (foreign key): Segmentation primary key.
         MaskClassificationMethod (foreign key): MaskClassificationMethod primary key.
     """
 
     definition = """
     -> Segmentation
@@ -998,23 +997,25 @@
         -> Segmentation.Mask
         ---
         -> MaskType
         confidence=null: float
         """
 
     def make(self, key):
-        pass
+        raise NotImplementedError(
+            "To add to this table, use `insert` with allow_direct_insert=True"
+        )
 
 
 # Fluorescence & Activity Traces -------------------------------------------------------
 
 
 @schema
 class Fluorescence(dj.Computed):
-    """Extracts fluoresence trace information.
+    """Extracts fluorescence trace information.
 
     Attributes:
         Segmentation (foreign key): Segmentation primary key.
     """
 
     definition = """  # fluorescence traces before spike extraction or filtering
     -> Segmentation
@@ -1022,25 +1023,26 @@
 
     class Trace(dj.Part):
         """Automated table with Fluorescence traces
 
         Attributes:
             Fluorescence (foreign key): Fluorescence primary key.
             Segmentation.Mask (foreign key): Segmentation.Mask primary key.
-            Channel.proj(fluorescence_channel='channel') (foreign key, query): Channel used for this trace.
+            Channel.proj(fluorescence_channel='channel') (foreign key, query): Channel
+                used for this trace.
             fluorescence (longblob): A fluorescence trace associated with a given mask.
-            neurpil_fluorescence (longblob): A neuropil fluorescence trace.
+            neuropil_fluorescence (longblob): A neuropil fluorescence trace.
         """
 
         definition = """
         -> master
         -> Segmentation.Mask
         -> Channel.proj(fluorescence_channel='channel')  # channel used for this trace
         ---
-        fluorescence                : longblob  # fluorescence trace associated 
+        fluorescence                : longblob  # fluorescence trace associated
                                                 # with this mask
         neuropil_fluorescence=null  : longblob  # Neuropil fluorescence trace
         """
 
     def make(self, key):
         """Populates table with fluorescence trace data."""
         method, loaded_result = get_loader_result(key, Curation)
@@ -1056,15 +1058,15 @@
             )
 
             self.insert1(key)
             self.Trace.insert(
                 [
                     {
                         **key,
-                        "mask_id": mask["mask_id"],
+                        "mask": mask.get("mask", mask["mask_id"]),
                         "fluorescence_channel": segmentation_channel,
                         "fluorescence": mask["inferred_trace"],
                     }
                     for mask in loaded_caiman.masks
                 ]
             )
 
@@ -1073,27 +1075,27 @@
 
 
 @schema
 class ActivityExtractionMethod(dj.Lookup):
     """Lookup table for activity extraction methods.
 
     Attributes:
-        extraction_method (foreign key, varchar(200) ): Extraction method from CaImAn.
+        extraction_method (foreign key, varchar(32) ): Extraction method from CaImAn.
     """
 
     definition = """
-    extraction_method: varchar(200)
+    extraction_method: varchar(32)
     """
 
     contents = zip(["caiman_deconvolution", "caiman_dff"])
 
 
 @schema
 class Activity(dj.Computed):
-    """Inferred neural activty from the fluorescence trace. 
+    """Inferred neural activity from the fluorescence trace.
 
     Attributes:
         Fluorescence (foreign key): Fluorescence primary key.
         ActivityExtractionMethod (foreign key): ActivityExtractionMethod primary key.
     """
 
     definition = """
@@ -1103,15 +1105,15 @@
     """
 
     class Trace(dj.Part):
         """Automated table with activity traces.
 
         Attributes:
             Activity (foreign key): Activity primary key.
-            Fluorescence.Trace (foreign key): Fluoresence.Trace primary key.
+            Fluorescence.Trace (foreign key): fluorescence.Trace primary key.
             activity_trace (longblob): Inferred activity trace.
         """
 
         definition = """
         -> master
         -> Fluorescence.Trace
         ---
@@ -1149,47 +1151,105 @@
                 )
 
                 self.insert1(key)
                 self.Trace.insert(
                     [
                         {
                             **key,
-                            "mask_id": mask["mask_id"],
+                            "mask": mask.get("mask", mask["mask_id"]),
                             "fluorescence_channel": segmentation_channel,
                             "activity_trace": mask[
                                 attr_mapper[key["extraction_method"]]
                             ],
                         }
                         for mask in loaded_caiman.masks
                     ]
                 )
 
         else:
             raise NotImplementedError("Unknown/unimplemented method: {}".format(method))
 
 
+@schema
+class ProcessingQualityMetrics(dj.Computed):
+    """Quality metrics used to evaluate the results of the calcium imaging analysis pipeline.
+
+    Attributes:
+        Fluorescence (foreign key): Primary key from Fluorescence.
+    """
+
+    definition = """
+    -> Fluorescence
+    """
+
+    class Trace(dj.Part):
+        """Quality metrics used to evaluate the fluorescence traces.
+
+        Attributes:
+            Fluorescence (foreign key): Primary key from Fluorescence.
+            Fluorescence.Trace (foreign key): Primary key from Fluorescence.Trace.
+            skewness (float): Skewness of the fluorescence trace.
+            variance (float): Variance of the fluorescence trace.
+        """
+
+        definition = """
+        -> master
+        -> Fluorescence.Trace
+        ---
+        skewness: float   # Skewness of the fluorescence trace.
+        variance: float   # Variance of the fluorescence trace.
+        """
+
+    def make(self, key):
+        """Populate the ProcessingQualityMetrics table and its part tables."""
+        from scipy.stats import skew
+
+        (fluorescence, fluorescence_channels, mask_ids,) = (
+            Segmentation.Mask * RecordingInfo * Fluorescence.Trace & key
+        ).fetch("fluorescence", "fluorescence_channel", "mask")
+
+        fluorescence = np.stack(fluorescence)
+
+        self.insert1(key)
+
+        self.Trace.insert(
+            dict(
+                key,
+                fluorescence_channel=fluorescence_channel,
+                mask=mask_id,
+                skewness=skewness,
+                variance=variance,
+            )
+            for fluorescence_channel, mask_id, skewness, variance in zip(
+                fluorescence_channels,
+                mask_ids,
+                skew(fluorescence, axis=1),
+                fluorescence.std(axis=1),
+            )
+        )
+
+
 # Helper Functions ---------------------------------------------------------------------
 
 _table_attribute_mapper = {
     "ProcessingTask": "processing_output_dir",
     "Curation": "curation_output_dir",
 }
 
 
-def get_loader_result(key, table):
+def get_loader_result(key, table) -> tuple:
     """Retrieve the loaded processed imaging results from the loader (e.g. caiman, etc.)
-    
+
     Args:
         key (dict): the `key` to one entry of ProcessingTask or Curation.
         table (str): the class defining the table to retrieve
-         the loaded results from (e.g. ProcessingTask, Curation).
-    
+            the loaded results from (e.g. ProcessingTask, Curation).
+
     Returns:
-        a loader object of the loaded results
-         (e.g. caiman.CaImAn, etc.)
+        method, loaded_output (tuple): method string and loader object with results (e.g. caiman.CaImAn, etc.)
     """
 
     method, output_dir = (ProcessingParamSet * table & key).fetch1(
         "processing_method", _table_attribute_mapper[table.__name__]
     )
 
     output_dir = find_full_path(get_miniscope_root_data_dir(), output_dir)
@@ -1198,31 +1258,7 @@
         from element_interface import caiman_loader
 
         loaded_output = caiman_loader.CaImAn(output_dir)
     else:
         raise NotImplementedError("Unknown/unimplemented method: {}".format(method))
 
     return method, loaded_output
-
-
-def populate_all(display_progress=True, reserve_jobs=False, suppress_errors=False):
-    """Populates all Computed/Imported tables in this schema, in order."""
-
-    populate_settings = {
-        "display_progress": display_progress,
-        "reserve_jobs": reserve_jobs,
-        "suppress_errors": suppress_errors,
-    }
-
-    RecordingInfo.populate(**populate_settings)
-
-    Processing.populate(**populate_settings)
-
-    MotionCorrection.populate(**populate_settings)
-
-    Segmentation.populate(**populate_settings)
-
-    MaskClassification.populate(**populate_settings)
-
-    Fluorescence.populate(**populate_settings)
-
-    Activity.populate(**populate_settings)
```

### Comparing `element-miniscope-0.1.4/setup.py` & `element-miniscope-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
-from setuptools import setup, find_packages
 from os import path
 
+from setuptools import find_packages, setup
+
 pkg_name = next(p for p in find_packages() if "." not in p)
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), "r") as f:
     long_description = f.read()
 
 with open(path.join(here, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 with open(path.join(here, pkg_name, "version.py")) as f:
     exec(f.read())
 
 setup(
     name=pkg_name.replace("_", "-"),
-    version=__version__,
+    version=__version__,  # noqa F821
     description="Miniscope DataJoint Element",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DataJoint",
     author_email="info@datajoint.com",
     license="MIT",
     url=f'https://github.com/datajoint/{pkg_name.replace("_", "-")}',
```


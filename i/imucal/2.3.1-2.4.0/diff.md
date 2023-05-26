# Comparing `tmp/imucal-2.3.1.tar.gz` & `tmp/imucal-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imucal-2.3.1.tar", max compression
+gzip compressed data, was "imucal-2.4.0.tar", max compression
```

## Comparing `imucal-2.3.1.tar` & `imucal-2.4.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1073 2022-10-17 08:42:03.253944 imucal-2.3.1/LICENSE
--rw-r--r--   0        0        0     8389 2022-10-17 08:42:03.253944 imucal-2.3.1/README.md
--rw-r--r--   0        0        0      739 2022-10-17 08:42:03.265944 imucal-2.3.1/imucal/__init__.py
--rw-r--r--   0        0        0     8447 2022-10-17 08:42:03.265944 imucal-2.3.1/imucal/calibration_gui.py
--rw-r--r--   0        0        0    11687 2022-10-17 08:42:03.265944 imucal-2.3.1/imucal/calibration_info.py
--rw-r--r--   0        0        0    20528 2022-10-17 08:42:03.265944 imucal-2.3.1/imucal/ferraris_calibration.py
--rw-r--r--   0        0        0     5485 2022-10-17 08:42:03.265944 imucal-2.3.1/imucal/ferraris_calibration_info.py
--rw-r--r--   0        0        0     1791 2022-10-17 08:42:03.265944 imucal-2.3.1/imucal/legacy.py
--rw-r--r--   0        0        0    11276 2022-10-17 08:42:03.265944 imucal-2.3.1/imucal/management.py
--rw-r--r--   0        0        0     1697 2022-10-17 08:42:03.269945 imucal-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     9396 1970-01-01 00:00:00.000000 imucal-2.3.1/setup.py
--rw-r--r--   0        0        0     9593 1970-01-01 00:00:00.000000 imucal-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-26 07:50:02.886675 imucal-2.4.0/LICENSE
+-rw-r--r--   0        0        0     8342 2023-05-26 07:50:02.886675 imucal-2.4.0/README.md
+-rw-r--r--   0        0        0      752 2023-05-26 07:50:02.902675 imucal-2.4.0/imucal/__init__.py
+-rw-r--r--   0        0        0     8418 2023-05-26 07:50:02.902675 imucal-2.4.0/imucal/calibration_gui.py
+-rw-r--r--   0        0        0    11568 2023-05-26 07:50:02.902675 imucal-2.4.0/imucal/calibration_info.py
+-rw-r--r--   0        0        0    20483 2023-05-26 07:50:02.902675 imucal-2.4.0/imucal/ferraris_calibration.py
+-rw-r--r--   0        0        0     5410 2023-05-26 07:50:02.902675 imucal-2.4.0/imucal/ferraris_calibration_info.py
+-rw-r--r--   0        0        0     1819 2023-05-26 07:50:02.902675 imucal-2.4.0/imucal/legacy.py
+-rw-r--r--   0        0        0    11198 2023-05-26 07:50:02.902675 imucal-2.4.0/imucal/management.py
+-rw-r--r--   0        0        0     2406 2023-05-26 07:50:02.906675 imucal-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9548 1970-01-01 00:00:00.000000 imucal-2.4.0/PKG-INFO
```

### Comparing `imucal-2.3.1/LICENSE` & `imucal-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imucal-2.3.1/README.md` & `imucal-2.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,14 @@
 pip install imucal[calplot]
 ```
 
 ### Supported Python versions and Platforms
 
 `imucal` is officially tested on Python 3.7, 3.8, 3.9 and 3.10.
 It should further work with all major operating systems.
-However, you might run into some issues on ARM based MacBooks, as `hd5py` does not seem to be properly supported yet.
-However, as `hd5py` is only an optional dependency, you can still use `imucal` without it, if you do not need support
-for HDF5 import or export of calibration files.
 
 ## Quickstart
 This package implements the IMU-infield calibration based on [Ferraris1995](https://www.researchgate.net/publication/245080041_Calibration_of_three-axial_rate_gyros_without_angular_velocity_standards).
 This calibration method requires the IMU data from 6 static positions (3 axes parallel and antiparallel to the gravitation
 vector) for calibrating the accelerometer and 3 rotations around the 3 main axes for calibrating the gyroscope.
 In this implementation, these parts are referred to as `{acc,gyr}_{x,y,z}_{p,a}` for the static regions and
 `{acc,gyr}_{x,y,z}_rot` for the rotations.
@@ -129,36 +126,48 @@
 ## Dev Setup
 
 We use [poetry](https://python-poetry.org) to manage our dependencies.
 Therefore, you need to first install Poetry locally on you machine.
 
 Then you can run the following command to install a local development version of this library in a dedicated venv.
 
-```
-poetry install -E calplot -E h5py
+```bash
+git clone https://github.com/mad-lab-fau/imucal
+cd imucal
+poetry install --all-extras
 ```
 
-To run tests/the linter/... we use [doit](https://pydoit.org/tasks.html).
+To run tests/the linter/... we use [poethepoet](https://github.com/nat-n/poethepoet).
 You can see all available commands by running:
 
 ```
-poetry run doit list
+poetry run poe list
+```
+
+This should show you all configured commands:
+
+```
+CONFIGURED TASKS
+  format         
+  lint           Lint all files with ruff.
+  ci_check       Check all potential format and linting issues.
+  test           Run Pytest with coverage.
+  docs           Build the html docs using Sphinx.
+  bump_version  
 ```
 
-and execute any command by running
+You execute any command by running
 
 ```
 poetry run doit <command-name>
 ```
 
 ### Updating dependencies
 
 If you update or add dependencies using (`poetry add` or `poetry update`) you will see that the `pyproject.toml` and the `poetry.lock` files are both updated.
-This might take a while (>10 min) depending on the dependency you updated.
-Unfortunately, we can not do anything about that at the moment.
 Make sure you commit the changes to **both** files.
 Otherwise, wrong versions of dependencies will be used in the CI and by other developers.
 
 In case you update dependencies by directly editing the `pyproject.toml` file, you need to be very careful and make sure, you run `poetry lock [--no-update]` afterwards.
 Otherwise, the lock file will be out of date.
 
 In general, it is a good idea to just run `poetry update` from time to time.
```

### Comparing `imucal-2.3.1/imucal/__init__.py` & `imucal-2.4.0/imucal/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from imucal.calibration_info import CalibrationInfo  # noqa: F401
+"""A library to calibrate 6 DOF IMUs."""
+from imucal.calibration_info import CalibrationInfo
 from imucal.ferraris_calibration import (
     FerrarisCalibration,
+    FerrarisSignalRegions,
     TurntableCalibration,
     ferraris_regions_from_df,
     ferraris_regions_from_interactive_plot,
     ferraris_regions_from_section_list,
-    FerrarisSignalRegions,
 )
-from imucal.ferraris_calibration_info import FerrarisCalibrationInfo, TurntableCalibrationInfo  # noqa: F401
+from imucal.ferraris_calibration_info import FerrarisCalibrationInfo, TurntableCalibrationInfo
 
-__version__ = "2.3.1"
+__version__ = "2.4.0"
 
 __all__ = [
     "CalibrationInfo",
     "FerrarisCalibration",
     "TurntableCalibration",
     "FerrarisSignalRegions",
     "FerrarisCalibrationInfo",
```

### Comparing `imucal-2.3.1/imucal/calibration_gui.py` & `imucal-2.4.0/imucal/calibration_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Helper providing a small GUI to label timeseries data."""
 import tkinter as tk  # noqa: import-error
 from collections import OrderedDict
 from itertools import chain
-from tkinter.messagebox import showinfo  # noqa: import-error
+from tkinter.messagebox import showinfo  # : import-error
 from typing import Sequence, Optional
 
 import numpy as np
 
 
 class CalibrationGui:
     """A Gui that can be used to label the different required sections of a calibration.
@@ -65,34 +65,34 @@
             List of all label names that should be labeled
         title :
             Title displayed in the titlebar of the GUI
         master :
             Parent window if GUI should be embedded in larger application
 
         """
-        import matplotlib  # noqa: import-outside-toplevel
-        from matplotlib.backends.backend_tkagg import (  # noqa: import-outside-toplevel
+        import matplotlib  # : import-outside-toplevel
+        from matplotlib.backends.backend_tkagg import (  # : import-outside-toplevel
             FigureCanvasTkAgg,
             NavigationToolbar2Tk,
         )
 
         self.expected_labels = expected_labels
         cmap = matplotlib.cm.get_cmap("Set3")
         self.colors = {k: matplotlib.colors.to_hex(cmap(i / 12)) for i, k in enumerate(expected_labels)}
 
-        self.text_label = "Labels set: {{}}/{}".format(len(expected_labels))
+        self.text_label = f"Labels set: {{}}/{len(expected_labels)}"
 
         if not master:
             master = tk.Tk()
 
         master.title(title or "Calibration Gui")
-        master.bind("<Return>", lambda x: self._select_next(self.labels.curselection()[0]))
+        master.bind("<Return>", lambda _: self._select_next(self.labels.curselection()[0]))
 
         # reset variables
-        self.section_list = OrderedDict(((k, [None, None]) for k in expected_labels))
+        self.section_list = OrderedDict((k, [None, None]) for k in expected_labels)
         self.acc_list_markers = {k: [] for k in expected_labels}
         self.gyro_list_markers = {k: [] for k in expected_labels}
 
         self.main_area = tk.Frame(master=master, relief=tk.RAISED)
         self.main_area.pack(fill=tk.BOTH, expand=1)
 
         self.side_bar = tk.Frame(master=self.main_area)
@@ -173,15 +173,14 @@
 
         self.label_text.delete("1.0", tk.END)
         self.label_text.insert(tk.END, self.text_label.format(str(self._n_labels())))
 
         self._update_list_box()
 
     def _update_marker(self, key):
-
         for line in chain(self.acc_list_markers[key], self.gyro_list_markers[key]):
             line.remove()
             self.acc_list_markers[key] = []
             self.gyro_list_markers[key] = []
 
         for val in self.section_list[key]:
             if val:
@@ -200,19 +199,19 @@
             self.acc_list_markers[key].append(a_acc)
             self.gyro_list_markers[key].append(a_gyr)
 
         self.fig.canvas.draw()
         self.fig.canvas.flush_events()
 
     def _n_labels(self):
-        return sum((all(v) for v in self.section_list.values()))
+        return sum(all(v) for v in self.section_list.values())
 
 
 def _create_figure(acc, gyro):
-    from matplotlib.figure import Figure  # noqa: import-outside-toplevel
+    from matplotlib.figure import Figure  # : import-outside-toplevel
 
     fig = Figure(figsize=(20, 10))
     ax1 = fig.add_subplot(211)
     lines = ax1.plot(acc)
     ax1.grid(True)
     ax1.set_title("Use this plot to find the static regions for acc calibration")
     ax1.set_xlabel("time [s]")
```

### Comparing `imucal-2.3.1/imucal/calibration_info.py` & `imucal-2.4.0/imucal/calibration_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Base Class for all CalibrationInfo objects."""
 import json
-from dataclasses import dataclass, fields, asdict
+from dataclasses import asdict, dataclass, fields
 from pathlib import Path
-from typing import Tuple, Union, TypeVar, ClassVar, Optional, Type, Iterable
+from typing import ClassVar, Iterable, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from packaging.version import Version
 
 CalInfo = TypeVar("CalInfo", bound="CalibrationInfo")
 
@@ -25,16 +25,16 @@
 
         >>> json_string = "{cal_type: 'Ferraris', ...}"
         >>> CalibrationInfo.from_json(json_string)
         <FerrarisCalibrationInfo ...>
 
     """
 
-    CAL_FORMAT_VERSION: ClassVar[Version] = _CAL_FORMAT_VERSION  # noqa: invalid-name
-    CAL_TYPE: ClassVar[str] = None  # noqa: invalid-name
+    CAL_FORMAT_VERSION: ClassVar[Version] = _CAL_FORMAT_VERSION  # : invalid-name
+    CAL_TYPE: ClassVar[str] = None  # : invalid-name
     acc_unit: Optional[str] = None
     gyr_unit: Optional[str] = None
     from_acc_unit: Optional[str] = None
     from_gyr_unit: Optional[str] = None
     comment: Optional[str] = None
 
     _cal_paras: ClassVar[Tuple[str, ...]]
@@ -128,32 +128,29 @@
     def __eq__(self, other):
         """Check if two calibrations are identical.
 
         Note, we use a custom function for that, as we need to compare the numpy arrays.
         """
         # Check type:
         if not isinstance(other, self.__class__):
-            raise ValueError("Comparison is only defined between two {} object!".format(self.__class__.__name__))
+            raise TypeError(f"Comparison is only defined between two {self.__class__.__name__} object!")
 
         # Test keys equal:
         if fields(self) != fields(other):
             return False
 
         # Test method equal
         if not self.CAL_TYPE == other.CAL_TYPE:
             return False
 
         # Test all values
         for f in fields(self):
             a1 = getattr(self, f.name)
             a2 = getattr(other, f.name)
-            if isinstance(a1, np.ndarray):
-                equal = np.array_equal(a1, a2)
-            else:
-                equal = a1 == a2
+            equal = np.array_equal(a1, a2) if isinstance(a1, np.ndarray) else a1 == a2
             if not equal:
                 return False
         return True
 
     def _to_list_dict(self):
         d = asdict(self)
         d["cal_type"] = self.CAL_TYPE
@@ -171,18 +168,18 @@
         for subclass in cls.__subclasses__():
             yield from subclass._get_subclasses()
             yield subclass
 
     @classmethod
     def find_subclass_from_cal_type(cls, cal_type):
         """Get a SensorCalibration subclass that handles the specified calibration type."""
-        if cls.CAL_TYPE == cal_type:
+        if cal_type == cls.CAL_TYPE:
             return cls
         try:
-            out_cls = next(x for x in cls._get_subclasses() if x.CAL_TYPE == cal_type)
+            out_cls = next(x for x in cls._get_subclasses() if cal_type == x.CAL_TYPE)
         except StopIteration as e:
             raise ValueError(
                 "No suitable calibration info class could be found for caltype `{}`. "
                 "The following classes were checked: {}. "
                 "If your CalibrationInfo class is missing, make sure it is imported before loading a "
                 "file.".format(cal_type, (cls.__name__, *(x.__name__ for x in cls._get_subclasses())))
             ) from e
@@ -220,15 +217,15 @@
         Parameters
         ----------
         path :
             path to the json file
 
         """
         data_dict = self._to_list_dict()
-        return json.dump(data_dict, open(path, "w", encoding="utf8"), cls=NumpyEncoder, indent=4)
+        return json.dump(data_dict, Path(path).open("w", encoding="utf8"), cls=NumpyEncoder, indent=4)
 
     @classmethod
     def from_json_file(cls: Type[CalInfo], path: Union[str, Path]) -> CalInfo:
         """Create a calibration object from a valid json file (created by `CalibrationInfo.to_json_file`).
 
         Parameters
         ----------
@@ -238,30 +235,30 @@
         Returns
         -------
         cal_info
             A CalibrationInfo object.
             The exact child class is determined by the `cal_type` key in the json string.
 
         """
-        with open(path, "r", encoding="utf8") as f:
+        with Path(path).open(encoding="utf8") as f:
             raw_json = json.load(f)
         check_cal_format_version(raw_json.pop("_format_version", None), cls.CAL_FORMAT_VERSION)
         subclass = cls.find_subclass_from_cal_type(raw_json.pop("cal_type"))
         return subclass._from_list_dict(raw_json)
 
     def to_hdf5(self, path: Union[str, Path]):
         """Save calibration matrices to hdf5 file format.
 
         Parameters
         ----------
         path :
             Path to the hdf5 file
 
         """
-        import h5py  # noqa: import-outside-toplevel
+        import h5py  # : import-outside-toplevel
 
         with h5py.File(path, "w") as hdf:
             for k, v in self._to_list_dict().items():
                 if k in self._cal_paras:
                     hdf.create_dataset(k, data=v.tolist())
                 elif v:
                     hdf[k] = v
@@ -278,20 +275,20 @@
         Returns
         -------
         cal_info
             A CalibrationInfo object.
             The exact child class is determined by the `cal_type` key in the json string.
 
         """
-        import h5py  # noqa: import-outside-toplevel
+        import h5py
 
         with h5py.File(path, "r") as hdf:
             format_version = hdf.get("_format_version")
             if format_version:
-                format_version = format_version.asstr()[()]  # type: ignore
+                format_version = format_version.asstr()[()]
             check_cal_format_version(format_version, cls.CAL_FORMAT_VERSION)
             subcls = cls.find_subclass_from_cal_type(hdf["cal_type"][()].decode("utf-8"))
             data = {}
             for k in fields(subcls):
                 dp = hdf.get(k.name)
                 if h5py.check_string_dtype(dp.dtype):
                     # String data
```

### Comparing `imucal-2.3.1/imucal/ferraris_calibration.py` & `imucal-2.4.0/imucal/ferraris_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Calculate a Ferraris calibration from sensor data."""
-from typing import Optional, TypeVar, Type, NamedTuple, Iterable, Tuple
+from typing import ClassVar, Iterable, NamedTuple, Optional, Tuple, Type, TypeVar
 
 import numpy as np
 import pandas as pd
 from numpy.linalg import inv
-from typing_extensions import ClassVar
 
 from imucal.calibration_info import CalibrationInfo
 from imucal.ferraris_calibration_info import FerrarisCalibrationInfo, TurntableCalibrationInfo
 
 T = TypeVar("T", bound="FerrarisCalibration")
 
 
@@ -233,20 +232,20 @@
         # Eq. 21
         U_a_d = U_a_p - U_a_n  # noqa: invalid_name
 
         # Calculate Scaling matrix
         # Eq. 23
         k_a_sq = 1 / (4 * self.grav**2) * np.diag(U_a_d @ U_a_d.T)
         K_a = np.diag(np.sqrt(k_a_sq))  # noqa: invalid_name
-        cal_mat.K_a = K_a  # noqa: invalid_name
+        cal_mat.K_a = K_a  # : invalid_name
 
         # Calculate Rotation matrix
         # Eq. 22
         R_a = inv(K_a) @ U_a_d / (2 * self.grav)  # noqa: invalid_name
-        cal_mat.R_a = R_a  # noqa: invalid_name
+        cal_mat.R_a = R_a  # : invalid_name
 
         ###############################################################################################################
         # Calculate Gyroscope Matrix
 
         # Gyro Bias from the static phases of the acc calibration
         # One static phase would be sufficient, but why not use all of them if you have them.
         # Note that this calibration ignores any influences due to the earth rotation.
@@ -283,15 +282,15 @@
                 np.mean(signal_regions.gyr_y_a, axis=0),
                 np.mean(signal_regions.gyr_z_a, axis=0),
             )
         ).T
 
         # Eq. 9
         K_ga = (U_g_p - U_g_a) / (2 * self.grav)  # noqa: invalid_name
-        cal_mat.K_ga = K_ga  # noqa: invalid_name
+        cal_mat.K_ga = K_ga  # : invalid_name
 
         # Gyroscope Scaling and Rotation
 
         # First apply partial calibration to remove offset and acc influence
         acc_x_rot_cor = cal_mat._calibrate_acc(signal_regions.acc_x_rot)
         acc_y_rot_cor = cal_mat._calibrate_acc(signal_regions.acc_y_rot)
         acc_z_rot_cor = cal_mat._calibrate_acc(signal_regions.acc_z_rot)
@@ -309,18 +308,18 @@
         # Eq.15
         expected_angles = self.expected_angle * np.identity(3)
         multiplied = W_s @ inv(expected_angles)
 
         # Eq. 12
         k_g_sq = np.diag(multiplied @ multiplied.T)
         K_g = np.diag(np.sqrt(k_g_sq))  # noqa: invalid_name
-        cal_mat.K_g = K_g  # noqa: invalid_name
+        cal_mat.K_g = K_g  # : invalid_name
 
         R_g = inv(K_g) @ multiplied  # noqa: invalid_name
-        cal_mat.R_g = R_g  # noqa: invalid_name
+        cal_mat.R_g = R_g  # : invalid_name
 
         return cal_mat
 
 
 class TurntableCalibration(FerrarisCalibration):
     """Calculate a Ferraris calibration matrices based on a turntable measurement.
 
@@ -392,16 +391,16 @@
     --------
     ferraris_regions_from_interactive_plot
     ferraris_regions_from_section_list
 
     """
     acc_df = df[list(acc_cols)]
     gyro_df = df[list(gyr_cols)]
-    acc_dict = acc_df.groupby(level=0).apply(lambda x: x.values).to_dict()
-    gyro_dict = gyro_df.groupby(level=0).apply(lambda x: x.values).to_dict()
+    acc_dict = acc_df.groupby(level=0).apply(lambda x: x.to_numpy()).to_dict()
+    gyro_dict = gyro_df.groupby(level=0).apply(lambda x: x.to_numpy()).to_dict()
     acc_dict = {"acc_" + k: v for k, v in acc_dict.items()}
     gyro_dict = {"gyr_" + k: v for k, v in gyro_dict.items()}
 
     return FerrarisSignalRegions(**acc_dict, **gyro_dict)
 
 
 def ferraris_regions_from_section_list(
@@ -522,15 +521,15 @@
         Acceleration data
     gyro : (n, 3) array
         Gyroscope data
     title :
         Optional title for the Calibration GUI
 
     """
-    from imucal.calibration_gui import CalibrationGui  # noqa: import-outside-toplevel
+    from imucal.calibration_gui import CalibrationGui  # : import-outside-toplevel
 
     plot = CalibrationGui(acc, gyro, FerrarisCalibration.FERRARIS_SECTIONS, title=title)
 
     section_list = plot.section_list
 
     check_all = (all(v) for v in section_list.values())
     if not all(check_all):
```

### Comparing `imucal-2.3.1/imucal/ferraris_calibration_info.py` & `imucal-2.4.0/imucal/ferraris_calibration_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Wrapper object to hold calibration matrices for a Ferraris Calibration."""
 from dataclasses import dataclass
-from typing import Tuple, ClassVar, Optional
+from typing import ClassVar, Optional, Tuple
 
 import numpy as np
 
 from imucal.calibration_info import CalibrationInfo
 
 
 @dataclass(eq=False)
@@ -26,24 +26,24 @@
     K_ga :
         Influence of acceleration on gyroscope
     b_g :
         Gyroscope bias
 
     """
 
-    CAL_TYPE: ClassVar[str] = "Ferraris"  # noqa: invalid-name
+    CAL_TYPE: ClassVar[str] = "Ferraris"  # : invalid-name
 
     acc_unit: str = "m/s^2"
     gyr_unit: str = "deg/s"
-    K_a: Optional[np.ndarray] = None  # noqa: invalid-name
-    R_a: Optional[np.ndarray] = None  # noqa: invalid-name
+    K_a: Optional[np.ndarray] = None  # : invalid-name
+    R_a: Optional[np.ndarray] = None  # : invalid-name
     b_a: Optional[np.ndarray] = None
-    K_g: Optional[np.ndarray] = None  # noqa: invalid-name
-    R_g: Optional[np.ndarray] = None  # noqa: invalid-name
-    K_ga: Optional[np.ndarray] = None  # noqa: invalid-name
+    K_g: Optional[np.ndarray] = None  # : invalid-name
+    R_g: Optional[np.ndarray] = None  # : invalid-name
+    K_ga: Optional[np.ndarray] = None  # : invalid-name
     b_g: Optional[np.ndarray] = None
 
     _cal_paras: ClassVar[Tuple[str, ...]] = ("K_a", "R_a", "b_a", "K_g", "R_g", "K_ga", "b_g")
 
     def calibrate(
         self, acc: np.ndarray, gyr: np.ndarray, acc_unit: Optional[str], gyr_unit: Optional[str]
     ) -> Tuple[np.ndarray, np.ndarray]:
@@ -99,15 +99,15 @@
 
         """
         # Check if all required paras are initialized to throw appropriate error messages:
         paras = ("K_a", "R_a", "b_a")
         for v in paras:
             if getattr(self, v, None) is None:
                 raise ValueError(
-                    "{} need to initialised before an acc calibration can be performed. {} is missing".format(paras, v)
+                    f"{paras} need to initialised before an acc calibration can be performed. {v} is missing"
                 )
 
         # Combine Scaling and rotation matrix to one matrix
         acc_mat = np.linalg.inv(self.R_a) @ np.linalg.inv(self.K_a)
         acc_out = acc_mat @ (acc - self.b_a).T
 
         return acc_out.T
@@ -128,18 +128,15 @@
         gyro_mat = np.matmul(np.linalg.inv(self.R_g), np.linalg.inv(self.K_g))
         tmp = self._calibrate_gyr_offsets(gyr, calibrated_acc)
 
         gyro_out = gyro_mat @ tmp.T
         return gyro_out.T
 
     def _calibrate_gyr_offsets(self, gyr, calibrated_acc=None):
-        if calibrated_acc is None:
-            d_ga = np.array(0)
-        else:
-            d_ga = self.K_ga @ calibrated_acc.T
+        d_ga = np.array(0) if calibrated_acc is None else self.K_ga @ calibrated_acc.T
         offsets = d_ga.T + self.b_g
         return gyr - offsets
 
 
 class TurntableCalibrationInfo(FerrarisCalibrationInfo):
     """Calibration object that represents all the required information to apply a Turntable calibration to a dataset.
```

### Comparing `imucal-2.3.1/imucal/legacy.py` & `imucal-2.4.0/imucal/legacy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Helper functions to import calibration info export from older imucal versions."""
 
 import json
 import warnings
 from pathlib import Path
-from typing import Union, Type
+from typing import Type, Union
 
 from packaging.version import Version
 
 from imucal import CalibrationInfo
 
 
 def load_v1_json_files(
     path: Union[Path, str],
     base_class: Type[CalibrationInfo] = CalibrationInfo,
 ):
     """Load a exported json file that was created using imucal <= 2.0."""
-    with open(path, encoding="utf8") as f:
+    with Path(path).open(encoding="utf8") as f:
         json_str = f.read()
     return load_v1_json(json_str, base_class=base_class)
 
 
 def load_v1_json(
     json_str: str,
     base_class: Type[CalibrationInfo] = CalibrationInfo,
@@ -28,15 +28,16 @@
     warnings.warn(
         "Importing a legacy calibration file, will use default values for all parameters that were newly"
         "introduced. "
         "These default values might not be correct for your calibration. "
         "Double check the resulting calibration info object and adapt the parameters manually. "
         "\n"
         "If you made any changes, make sure to save the modified calibration and load it with the normal "
-        "loading function in the future."
+        "loading function in the future.",
+        stacklevel=2,
     )
     json_dict = json.loads(json_str)
 
     # Check that the provided json is indeed a v1 calibration
     if "_format_version" in json_dict:
         raise ValueError(
             "The provided json does not seem to be a v1 json export, but has the format version {}.".format(
```

### Comparing `imucal-2.3.1/imucal/management.py` & `imucal-2.4.0/imucal/management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """A set of highly opinionated helper functions to store and load calibration files for a medium number of sensors."""
 import datetime
 import re
 import warnings
 from pathlib import Path
-from typing import Optional, List, Callable, TypeVar, Union, Type
+from typing import Callable, List, Literal, Optional, Type, TypeVar, Union
 
 import numpy as np
-from typing_extensions import Literal
 
 from imucal import CalibrationInfo
 
-path_t = TypeVar("path_t", str, Path)  # noqa: invalid-name
+path_t = TypeVar("path_t", str, Path)  # : invalid-name
 
 
 class CalibrationWarning(Warning):
     """Indicate potential issues with a calibration."""
 
 
 def save_calibration_info(
@@ -115,38 +114,38 @@
     """
     method = "glob"
     if recursive is True:
         method = "rglob"
 
     r = sensor_id.lower() + r"_\d{4}-\d{2}-\d{2}_\d{2}-\d{2}"
 
-    matches = [f for f in getattr(Path(folder), method)("{}_*.json".format(sensor_id)) if re.fullmatch(r, f.stem)]
+    matches = [f for f in getattr(Path(folder), method)(f"{sensor_id}_*.json") if re.fullmatch(r, f.stem)]
 
     final_matches = []
     for m in matches:
         cal = load_calibration_info(m, file_type="json")
         if (filter_cal_type is None or cal.CAL_TYPE.lower() == filter_cal_type.lower()) and (
             custom_validator is None or custom_validator(cal)
         ):
             final_matches.append(m)
 
     if not final_matches and ignore_file_not_found is not True:
-        raise ValueError("No Calibration for the sensor_type with the id {} could be found".format(sensor_id))
+        raise ValueError(f"No Calibration for the sensor_type with the id {sensor_id} could be found")
     return final_matches
 
 
 def find_closest_calibration_info_to_date(
     sensor_id: str,
     cal_time: datetime.datetime,
     folder: Optional[path_t] = None,
     recursive: bool = True,
     filter_cal_type: Optional[str] = None,
     custom_validator: Optional[Callable[[CalibrationInfo], bool]] = None,
     before_after: Optional[str] = None,
-    warn_thres: datetime.timedelta = datetime.timedelta(days=30),  # noqa E252
+    warn_thres: datetime.timedelta = datetime.timedelta(days=30),  # E252
     ignore_file_not_found: Optional[bool] = False,
 ) -> Optional[Path]:
     """Find the calibration file for a sensor_type, that is closes to a given date.
 
     As this only checks the filenames, this might return a false positive depending on your folder structure and naming.
 
     Parameters
@@ -201,15 +200,15 @@
         filter_cal_type=filter_cal_type,
         custom_validator=custom_validator,
         ignore_file_not_found=ignore_file_not_found,
     )
     if not potential_list:
         if ignore_file_not_found is True:
             return None
-        raise ValueError("No Calibration for the sensor with the id {} could be found".format(sensor_id))
+        raise ValueError(f"No Calibration for the sensor with the id {sensor_id} could be found")
 
     dates = [datetime.datetime.strptime("_".join(d.stem.split("_")[1:]), "%Y-%m-%d_%H-%M") for d in potential_list]
 
     dates = np.array(dates, dtype="datetime64[s]")
     potential_list, _ = zip(*sorted(zip(potential_list, dates), key=lambda x: x[1]))
     dates.sort()
 
@@ -217,26 +216,25 @@
 
     if before_after == "after":
         diffs[diffs < 0] = np.nan
     elif before_after == "before":
         diffs[diffs > 0] = np.nan
 
     if np.all(diffs) == np.nan:
-        raise ValueError(
-            "No calibrations between {} and {} were found for sensor {}.".format(before_after, cal_time, sensor_id)
-        )
+        raise ValueError(f"No calibrations between {before_after} and {cal_time} were found for sensor {sensor_id}.")
 
     min_dist = float(np.nanmin(np.abs(diffs)))
     if warn_thres < datetime.timedelta(seconds=min_dist):
         warnings.warn(
             "For the sensor {} no calibration could be located that was in {} of the {}."
             "The closest calibration is {} away.".format(
                 sensor_id, warn_thres, cal_time, datetime.timedelta(seconds=min_dist)
             ),
             CalibrationWarning,
+            stacklevel=2,
         )
 
     return potential_list[int(np.nanargmin(np.abs(diffs)))]
 
 
 def load_calibration_info(
     path: Union[Path, str],
@@ -275,10 +273,10 @@
         elif suffix[1:] in ["hdf", "h5"]:
             file_type = "hdf"
         else:
             raise ValueError(
                 "The loader format could not be determined from the file suffix. Please specify `format` explicitly."
             )
     if file_type not in format_options:
-        raise ValueError("`format` must be one of {}".format(list(format_options.keys())))
+        raise ValueError(f"`format` must be one of {list(format_options.keys())}")
 
     return getattr(base_class, format_options[file_type])(path)
```

### Comparing `imucal-2.3.1/pyproject.toml` & `imucal-2.4.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imucal"
-version = "2.3.1"
+version = "2.4.0"
 description = "A Python library to calibrate 6 DOF IMUs"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
     "Nils Roth <nils.roth@fau.de>",
     "Robert Richer <robert.richer@fau.de"
 ]
 license = "MIT"
@@ -28,29 +28,30 @@
 matplotlib = {version = ">=3.3.2", optional = true}
 h5py = {version = ">=3", optional = true}
 
 [tool.poetry.extras]
 calplot = ["matplotlib"]
 h5py = ["h5py"]
 
-[tool.poetry.dev-dependencies]
-doit = "^0.33.1"
+[tool.poetry.group.dev.dependencies]
 pytest = "^6.1.1"
 pytest-cov = "^2.10.1"
 coverage = "^5.3"
-prospector = "^1.7.6"
-black = "^22.3.0"
-sphinx-gallery = "^0.10.1"
-Sphinx = "^4.4.0"
+prospector = "^1.10.2"
+sphinx-gallery = "^0.13.0"
+Sphinx = "^7.0.1"
 numpydoc = "^1.2.0"
-pydata-sphinx-theme = "^0.8.0"
 recommonmark = "^0.7.1"
 memory-profiler = "^0.58.0"
 Pillow = "^8.0.1"
 toml = "^0.10.2"
+pydata-sphinx-theme = "^0.13.3"
+black = "^23.3.0"
+poethepoet = "^0.20.0"
+ruff = "^0.0.270"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 exclude = '''
 (
   /(
@@ -65,10 +66,22 @@
     | build
     | dist
     | \.virtual_documents
   )/
 )
 '''
 
+[tool.poe.tasks]
+_format_black = "black ."
+_format_ruff = "ruff . --fix-only --exit-zero"
+format = ["_format_black", "_format_ruff", "_format_black"]
+lint = { cmd = "ruff imucal --fix", help = "Lint all files with ruff." }
+_lint_ci = "ruff imucal --format=github"
+_check_black = "black . --check"
+ci_check = { sequence = ["_check_black", "_lint_ci"], help = "Check all potential format and linting issues." }
+test = { cmd = "pytest --cov imucal --cov-report=term-missing --cov-report=xml", help = "Run Pytest with coverage." }
+docs = { "script" = "_tasks:task_docs()",  help = "Build the html docs using Sphinx." }
+bump_version = { "script" = "_tasks:task_update_version()" }
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `imucal-2.3.1/setup.py` & `imucal-2.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,207 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: imucal
+Version: 2.4.0
+Summary: A Python library to calibrate 6 DOF IMUs
+Home-page: https://github.com/mad-lab-fau/imucal
+License: MIT
+Keywords: sensors,scientific,IMU,accelerometer
+Author: Arne Küderle
+Author-email: arne.kuederle@fau.de
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Provides-Extra: calplot
+Provides-Extra: h5py
+Requires-Dist: h5py (>=3) ; extra == "h5py"
+Requires-Dist: matplotlib (>=3.3.2) ; extra == "calplot"
+Requires-Dist: numpy (>=1.19.2)
+Requires-Dist: packaging (>=21.3)
+Requires-Dist: pandas (>=1.1.3)
+Requires-Dist: typing-extensions (>=3.7.4)
+Project-URL: Documentation, https://imcucal.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/mad-lab-fau/imucal
+Description-Content-Type: text/markdown
+
+# imucal - A Python library to calibrate 6 DOF IMUs
+![Test and Lint](https://github.com/mad-lab-fau/imucal/workflows/Test%20and%20Lint/badge.svg)
+[![codecov](https://codecov.io/gh/mad-lab-fau/imucal/branch/master/graph/badge.svg?token=0OPHTQDYIB)](https://codecov.io/gh/mad-lab-fau/imucal)
+[![Documentation Status](https://readthedocs.org/projects/imucal/badge/?version=latest)](https://imucal.readthedocs.io/en/latest/?badge=latest)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI](https://img.shields.io/pypi/v/imucal)](https://pypi.org/project/imucal/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/imucal)
+[![status](https://joss.theoj.org/papers/3dd1a7dd5ba06ce024326eee2e9be148/status.svg)](https://joss.theoj.org/papers/3dd1a7dd5ba06ce024326eee2e9be148)
+
+This package provides methods to calculate and apply calibrations for 6 DOF IMUs based on multiple different methods.
+
+So far supported are:
+
+- Ferraris Calibration ([Ferraris1994](https://www.sciencedirect.com/science/article/pii/0924424794800316) / [Ferraris1995](https://www.researchgate.net/publication/245080041_Calibration_of_three-axial_rate_gyros_without_angular_velocity_standards))
+- Ferraris Calibration using a Turntable
+
+For more information check the quickstart guide below and the [documentation](https://imucal.readthedocs.io/en/latest/).
+
+## Installation
+
+```
+pip install imucal
+```
+
+To use the included calibration GUI you also need [matplotlib](https://pypi.org/project/matplotlib/) (version >2.2).
+You can install it using:
+
+```
+pip install imucal[calplot]
+```
+
+### Supported Python versions and Platforms
+
+`imucal` is officially tested on Python 3.7, 3.8, 3.9 and 3.10.
+It should further work with all major operating systems.
+
+## Quickstart
+This package implements the IMU-infield calibration based on [Ferraris1995](https://www.researchgate.net/publication/245080041_Calibration_of_three-axial_rate_gyros_without_angular_velocity_standards).
+This calibration method requires the IMU data from 6 static positions (3 axes parallel and antiparallel to the gravitation
+vector) for calibrating the accelerometer and 3 rotations around the 3 main axes for calibrating the gyroscope.
+In this implementation, these parts are referred to as `{acc,gyr}_{x,y,z}_{p,a}` for the static regions and
+`{acc,gyr}_{x,y,z}_rot` for the rotations.
+As example, `acc_y_a` would be the 3D-acceleration data measured during a static phase, where the **y-axis** was 
+oriented **antiparallel** to the gravitation vector.
+For more information on how to perform the calibration check [our guide](https://imucal.readthedocs.io/en/latest/guides/ferraris_guide.html).
+
+For the calibration, you need to separate your data into these individual sections.
+If you already recorded them separately or know where each section starts and ends in a continuous recording, you can 
+use [`ferraris_regions_from_df`](https://imucal.readthedocs.io/en/latest/modules/generated/imucal.ferraris_regions_from_df.html)
+and [`ferraris_regions_from_section_list`](https://imucal.readthedocs.io/en/latest/modules/generated/imucal.ferraris_regions_from_section_list.html),
+respectively to convert the data into the correct format for the calibration (`section_data` in the snippet below).
+
+If you don't have that information yet, we recommend to use the included GUI to annotate the data.
+To annotate a Ferraris calibration session that was recorded in a single go, you can use the following code snippet.  
+**Note**: This will open an interactive Tkinter plot. Therefore, this will only work on your local PC and not on a server or remote hosted Jupyter instance.
+
+```python
+from imucal import ferraris_regions_from_interactive_plot
+
+# Your data as a 6 column dataframe
+data = ...
+
+section_data, section_list = ferraris_regions_from_interactive_plot(
+    data, acc_cols=["acc_x", "acc_y", "acc_z"], gyr_cols=["gyr_x", "gyr_y", "gyr_z"]
+)
+# Save the section list as reference for the future
+section_list.to_csv('./calibration_sections.csv')  # This is optional, but recommended
+```
+
+Independent of how you obtained the `section_data` in the correct format, you can now calculate the calibration
+parameters:
+
+```python
+from imucal import FerrarisCalibration
+
+sampling_rate = 100 #Hz 
+cal = FerrarisCalibration()
+cal_mat = cal.compute(section_data, sampling_rate, from_acc_unit="m/s^2", from_gyr_unit="deg/s")
+# `cal_mat` is your final calibration matrix object you can use to calibrate data
+cal_mat.to_json_file('./calibration.json')
+```
+
+Applying a calibration:
+
+```python
+from imucal.management import load_calibration_info
+
+cal_mat = load_calibration_info('./calibration.json')
+new_data = pd.DataFrame(...)
+calibrated_data = cal_mat.calibrate_df(new_data, acc_unit="m/s^2", gyr_unit="deg/s")
+```
+
+For further information on how to perform a calibration check the 
+[User Guides](https://imucal.readthedocs.io/en/latest/guides/index.html) or the
+[Examples](https://imucal.readthedocs.io/en/latest/auto_examples/index.html).
+
+## Further Calibration Methods
+
+At the moment, this package only implements calibration methods based on Ferraris1994/95, because this is what we use to
+calibrate our IMUs.
+We are aware that various other methods exist and would love to add them to this package as well.
+Unfortunately, at the moment we can not justify the time investment.
+
+Still, we think that this package provides a suitable framework to implement other calibration methods with relative
+ease.
+If you would like to contribute such a method, let us know via [GitHub Issue](https://github.com/mad-lab-fau/imucal/issues), and we will try to help you as good
+as possible.
+
+## Citation
+
+If you are using `imucal` in your scientific work, we would appreciate if you would cite our [JOSS paper](https://joss.theoj.org/papers/3dd1a7dd5ba06ce024326eee2e9be148) or link the project.
+
+```
+Küderle, Arne, Nils Roth, Robert Richer, and Bjoern M. Eskofier. 
+“Imucal - A Python Library to Calibrate 6 DOF IMUs.”
+Journal of Open Source Software 7, no. 73 (May 26, 2022): 4338. https://doi.org/10.21105/joss.04338.
+```
+
+## Contributing
+
+All project management and development happens through [this GitHub project](https://github.com/mad-lab-fau/imucal).
+If you have any issues, ideas, or any comments at all, just open a new issue.
+We are always happy when people are interested to use our work and would like to support you in this process.
+In particular, we want to welcome contributions of new calibration algorithms, to make this package even more useful for a wider audience.
+
+## Dev Setup
+
+We use [poetry](https://python-poetry.org) to manage our dependencies.
+Therefore, you need to first install Poetry locally on you machine.
+
+Then you can run the following command to install a local development version of this library in a dedicated venv.
+
+```bash
+git clone https://github.com/mad-lab-fau/imucal
+cd imucal
+poetry install --all-extras
+```
+
+To run tests/the linter/... we use [poethepoet](https://github.com/nat-n/poethepoet).
+You can see all available commands by running:
+
+```
+poetry run poe list
+```
+
+This should show you all configured commands:
+
+```
+CONFIGURED TASKS
+  format         
+  lint           Lint all files with ruff.
+  ci_check       Check all potential format and linting issues.
+  test           Run Pytest with coverage.
+  docs           Build the html docs using Sphinx.
+  bump_version  
+```
+
+You execute any command by running
+
+```
+poetry run doit <command-name>
+```
+
+### Updating dependencies
+
+If you update or add dependencies using (`poetry add` or `poetry update`) you will see that the `pyproject.toml` and the `poetry.lock` files are both updated.
+Make sure you commit the changes to **both** files.
+Otherwise, wrong versions of dependencies will be used in the CI and by other developers.
+
+In case you update dependencies by directly editing the `pyproject.toml` file, you need to be very careful and make sure, you run `poetry lock [--no-update]` afterwards.
+Otherwise, the lock file will be out of date.
+
+In general, it is a good idea to just run `poetry update` from time to time.
+This will install the latest version of all dependencies that are still allowed by the version constrains in the `pyproject.toml`.
+This allows to check, if everything still works well with the newest versions of all libraries.
 
-packages = \
-['imucal']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.19.2',
- 'packaging>=21.3',
- 'pandas>=1.1.3',
- 'typing-extensions>=3.7.4']
-
-extras_require = \
-{'calplot': ['matplotlib>=3.3.2'], 'h5py': ['h5py>=3']}
-
-setup_kwargs = {
-    'name': 'imucal',
-    'version': '2.3.1',
-    'description': 'A Python library to calibrate 6 DOF IMUs',
-    'long_description': '# imucal - A Python library to calibrate 6 DOF IMUs\n![Test and Lint](https://github.com/mad-lab-fau/imucal/workflows/Test%20and%20Lint/badge.svg)\n[![codecov](https://codecov.io/gh/mad-lab-fau/imucal/branch/master/graph/badge.svg?token=0OPHTQDYIB)](https://codecov.io/gh/mad-lab-fau/imucal)\n[![Documentation Status](https://readthedocs.org/projects/imucal/badge/?version=latest)](https://imucal.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI](https://img.shields.io/pypi/v/imucal)](https://pypi.org/project/imucal/)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/imucal)\n[![status](https://joss.theoj.org/papers/3dd1a7dd5ba06ce024326eee2e9be148/status.svg)](https://joss.theoj.org/papers/3dd1a7dd5ba06ce024326eee2e9be148)\n\nThis package provides methods to calculate and apply calibrations for 6 DOF IMUs based on multiple different methods.\n\nSo far supported are:\n\n- Ferraris Calibration ([Ferraris1994](https://www.sciencedirect.com/science/article/pii/0924424794800316) / [Ferraris1995](https://www.researchgate.net/publication/245080041_Calibration_of_three-axial_rate_gyros_without_angular_velocity_standards))\n- Ferraris Calibration using a Turntable\n\nFor more information check the quickstart guide below and the [documentation](https://imucal.readthedocs.io/en/latest/).\n\n## Installation\n\n```\npip install imucal\n```\n\nTo use the included calibration GUI you also need [matplotlib](https://pypi.org/project/matplotlib/) (version >2.2).\nYou can install it using:\n\n```\npip install imucal[calplot]\n```\n\n### Supported Python versions and Platforms\n\n`imucal` is officially tested on Python 3.7, 3.8, 3.9 and 3.10.\nIt should further work with all major operating systems.\nHowever, you might run into some issues on ARM based MacBooks, as `hd5py` does not seem to be properly supported yet.\nHowever, as `hd5py` is only an optional dependency, you can still use `imucal` without it, if you do not need support\nfor HDF5 import or export of calibration files.\n\n## Quickstart\nThis package implements the IMU-infield calibration based on [Ferraris1995](https://www.researchgate.net/publication/245080041_Calibration_of_three-axial_rate_gyros_without_angular_velocity_standards).\nThis calibration method requires the IMU data from 6 static positions (3 axes parallel and antiparallel to the gravitation\nvector) for calibrating the accelerometer and 3 rotations around the 3 main axes for calibrating the gyroscope.\nIn this implementation, these parts are referred to as `{acc,gyr}_{x,y,z}_{p,a}` for the static regions and\n`{acc,gyr}_{x,y,z}_rot` for the rotations.\nAs example, `acc_y_a` would be the 3D-acceleration data measured during a static phase, where the **y-axis** was \noriented **antiparallel** to the gravitation vector.\nFor more information on how to perform the calibration check [our guide](https://imucal.readthedocs.io/en/latest/guides/ferraris_guide.html).\n\nFor the calibration, you need to separate your data into these individual sections.\nIf you already recorded them separately or know where each section starts and ends in a continuous recording, you can \nuse [`ferraris_regions_from_df`](https://imucal.readthedocs.io/en/latest/modules/generated/imucal.ferraris_regions_from_df.html)\nand [`ferraris_regions_from_section_list`](https://imucal.readthedocs.io/en/latest/modules/generated/imucal.ferraris_regions_from_section_list.html),\nrespectively to convert the data into the correct format for the calibration (`section_data` in the snippet below).\n\nIf you don\'t have that information yet, we recommend to use the included GUI to annotate the data.\nTo annotate a Ferraris calibration session that was recorded in a single go, you can use the following code snippet.  \n**Note**: This will open an interactive Tkinter plot. Therefore, this will only work on your local PC and not on a server or remote hosted Jupyter instance.\n\n```python\nfrom imucal import ferraris_regions_from_interactive_plot\n\n# Your data as a 6 column dataframe\ndata = ...\n\nsection_data, section_list = ferraris_regions_from_interactive_plot(\n    data, acc_cols=["acc_x", "acc_y", "acc_z"], gyr_cols=["gyr_x", "gyr_y", "gyr_z"]\n)\n# Save the section list as reference for the future\nsection_list.to_csv(\'./calibration_sections.csv\')  # This is optional, but recommended\n```\n\nIndependent of how you obtained the `section_data` in the correct format, you can now calculate the calibration\nparameters:\n\n```python\nfrom imucal import FerrarisCalibration\n\nsampling_rate = 100 #Hz \ncal = FerrarisCalibration()\ncal_mat = cal.compute(section_data, sampling_rate, from_acc_unit="m/s^2", from_gyr_unit="deg/s")\n# `cal_mat` is your final calibration matrix object you can use to calibrate data\ncal_mat.to_json_file(\'./calibration.json\')\n```\n\nApplying a calibration:\n\n```python\nfrom imucal.management import load_calibration_info\n\ncal_mat = load_calibration_info(\'./calibration.json\')\nnew_data = pd.DataFrame(...)\ncalibrated_data = cal_mat.calibrate_df(new_data, acc_unit="m/s^2", gyr_unit="deg/s")\n```\n\nFor further information on how to perform a calibration check the \n[User Guides](https://imucal.readthedocs.io/en/latest/guides/index.html) or the\n[Examples](https://imucal.readthedocs.io/en/latest/auto_examples/index.html).\n\n## Further Calibration Methods\n\nAt the moment, this package only implements calibration methods based on Ferraris1994/95, because this is what we use to\ncalibrate our IMUs.\nWe are aware that various other methods exist and would love to add them to this package as well.\nUnfortunately, at the moment we can not justify the time investment.\n\nStill, we think that this package provides a suitable framework to implement other calibration methods with relative\nease.\nIf you would like to contribute such a method, let us know via [GitHub Issue](https://github.com/mad-lab-fau/imucal/issues), and we will try to help you as good\nas possible.\n\n## Citation\n\nIf you are using `imucal` in your scientific work, we would appreciate if you would cite our [JOSS paper](https://joss.theoj.org/papers/3dd1a7dd5ba06ce024326eee2e9be148) or link the project.\n\n```\nKüderle, Arne, Nils Roth, Robert Richer, and Bjoern M. Eskofier. \n“Imucal - A Python Library to Calibrate 6 DOF IMUs.”\nJournal of Open Source Software 7, no. 73 (May 26, 2022): 4338. https://doi.org/10.21105/joss.04338.\n```\n\n## Contributing\n\nAll project management and development happens through [this GitHub project](https://github.com/mad-lab-fau/imucal).\nIf you have any issues, ideas, or any comments at all, just open a new issue.\nWe are always happy when people are interested to use our work and would like to support you in this process.\nIn particular, we want to welcome contributions of new calibration algorithms, to make this package even more useful for a wider audience.\n\n## Dev Setup\n\nWe use [poetry](https://python-poetry.org) to manage our dependencies.\nTherefore, you need to first install Poetry locally on you machine.\n\nThen you can run the following command to install a local development version of this library in a dedicated venv.\n\n```\npoetry install -E calplot -E h5py\n```\n\nTo run tests/the linter/... we use [doit](https://pydoit.org/tasks.html).\nYou can see all available commands by running:\n\n```\npoetry run doit list\n```\n\nand execute any command by running\n\n```\npoetry run doit <command-name>\n```\n\n### Updating dependencies\n\nIf you update or add dependencies using (`poetry add` or `poetry update`) you will see that the `pyproject.toml` and the `poetry.lock` files are both updated.\nThis might take a while (>10 min) depending on the dependency you updated.\nUnfortunately, we can not do anything about that at the moment.\nMake sure you commit the changes to **both** files.\nOtherwise, wrong versions of dependencies will be used in the CI and by other developers.\n\nIn case you update dependencies by directly editing the `pyproject.toml` file, you need to be very careful and make sure, you run `poetry lock [--no-update]` afterwards.\nOtherwise, the lock file will be out of date.\n\nIn general, it is a good idea to just run `poetry update` from time to time.\nThis will install the latest version of all dependencies that are still allowed by the version constrains in the `pyproject.toml`.\nThis allows to check, if everything still works well with the newest versions of all libraries.\n',
-    'author': 'Arne Küderle',
-    'author_email': 'arne.kuederle@fau.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mad-lab-fau/imucal',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```


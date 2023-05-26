# Comparing `tmp/spl_widgets-1.0.0.tar.gz` & `tmp/spl_widgets-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.0.0.tar", last modified: Fri Dec 23 22:31:21 2022, max compression
+gzip compressed data, was "spl_widgets-1.5.0.tar", last modified: Fri May 26 16:38:24 2023, max compression
```

## Comparing `spl_widgets-1.0.0.tar` & `spl_widgets-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2022-12-23 22:31:21.638280 spl_widgets-1.0.0/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.0.0/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      481 2022-12-23 22:31:21.638024 spl_widgets-1.0.0/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.0.0/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.0.0/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2022-12-23 22:31:21.638359 spl_widgets-1.0.0/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1187 2022-12-23 22:31:14.000000 spl_widgets-1.0.0/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2022-12-23 22:31:21.625387 spl_widgets-1.0.0/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2022-12-23 22:31:21.635993 spl_widgets-1.0.0/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.0.0/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.0.0/src/spl_widgets/__main__.py
--rw-r--r--   0 colin      (501) staff       (20)     3695 2022-11-11 23:24:19.000000 spl_widgets-1.0.0/src/spl_widgets/batch_tune.py
--rw-r--r--   0 colin      (501) staff       (20)      323 2022-06-26 16:24:05.000000 spl_widgets-1.0.0/src/spl_widgets/clear_aliases.py
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.0.0/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.0.0/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2022-12-23 19:57:45.000000 spl_widgets-1.0.0/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2022-12-23 19:42:07.000000 spl_widgets-1.0.0/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2022-12-23 22:30:42.000000 spl_widgets-1.0.0/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17140 2022-12-23 22:29:14.000000 spl_widgets-1.0.0/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2022-12-23 22:31:21.637719 spl_widgets-1.0.0/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      481 2022-12-23 22:31:21.000000 spl_widgets-1.0.0/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      567 2022-12-23 22:31:21.000000 spl_widgets-1.0.0/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2022-12-23 22:31:21.000000 spl_widgets-1.0.0/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      253 2022-12-23 22:31:21.000000 spl_widgets-1.0.0/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)        7 2022-12-23 22:31:21.000000 spl_widgets-1.0.0/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2022-12-23 22:31:21.000000 spl_widgets-1.0.0/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.517957 spl_widgets-1.5.0/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.5.0/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:38:24.517649 spl_widgets-1.5.0/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.5.0/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.5.0/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-05-26 16:38:24.518037 spl_widgets-1.5.0/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1178 2023-05-26 16:38:11.000000 spl_widgets-1.5.0/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.475472 spl_widgets-1.5.0/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.489323 spl_widgets-1.5.0/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.5.0/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.5.0/src/spl_widgets/__main__.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.5.0/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.494042 spl_widgets-1.5.0/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.5.0/src/spl_widgets/data/cmudict.sqlite
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.5.0/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.5.0/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.5.0/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.5.0/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.5.0/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.5.0/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-05-26 16:38:24.493461 spl_widgets-1.5.0/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      570 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)        7 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-05-26 16:38:24.000000 spl_widgets-1.5.0/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.0.0/LICENSE` & `spl_widgets-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.0.0/README.md` & `spl_widgets-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.0.0/setup.py` & `spl_widgets-1.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.0.0",
+    version="1.5.0",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
-    url="https://github.com/ctsf1/spl_widgets",
-    project_urls={
-        "Changelog":"https://github.com/ctsf1/spl_widgets#changelog"
-    },
+    url="https://github.com/clntsf/spl_widgets",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     install_requires=['pandas'],
     python_requires=">=3.8",
     entry_points='''
         [console_scripts]
-        rm_aliases=spl_widgets.clear_aliases:main
         gorilla_clean=spl_widgets.gorilla_clean:main
         tuner=spl_widgets.tuner:main
         stk_swx=spl_widgets.stk_swx:main
         batch_tune=spl_widgets.batch_tune:main
         jukemake=spl_widgets.jukemake:main
-    '''
+        autoscorer=spl_widgets.autoscorer.autoscorer_gui:main
+    ''',
+    include_package_data=True,
+    package_data={'': ['data/*.sqlite']}
 )
```

### Comparing `spl_widgets-1.0.0/src/spl_widgets/batch_tune.py` & `spl_widgets-1.5.0/src/spl_widgets/batch_tune.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from argparse import ArgumentParser, RawTextHelpFormatter
 from textwrap import dedent
 from pathlib import Path
 from sys import exit
 from tkinter import filedialog
 from subprocess import run
 import re
-from spl_widgets.misc_util import get_scale
+from spl_widgets.misc_util import get_tuning_info
 from spl_widgets.tune_freq import tune_cols
 
 KEY_REGEX = r"^([01][0-9]{2}-[0-9A-Fa-f]{3})$"
 
 def get_file(*args, **kwargs):
     params_file = filedialog.askopenfilename(*args, **kwargs)
-    if params_file is None:                                     # user bailed in filedialog
+    if params_file == "":                                       # user bailed in filedialog
         print("User bailed in filedialog")
         exit(1)
 
     return params_file
 
 def make_parser():
     parser_desc = "A companion script to tuner, tunes a passed .swx file with each tuning key in a passed params file."
@@ -70,15 +70,15 @@
         raise ValueError(f"Invalid path to parameter file: {params_fp}")
 
     keys = re.findall(KEY_REGEX, text, re.MULTILINE)        # get keys from params file text
 
     successful=False    # whether the program has successfully done any tunings
     for k in keys:      # tune with each key
         try:                                                # get tuning params from key
-            tune_freqs, interval, scale_list = get_scale(k)
+            tune_freqs, interval, scale_list, _fmts_to_tune = get_tuning_info(k)
             tune_freqs = bool(tune_freqs)
             successful = True
         except Exception:                                   # bad key, skip tune
             print(f"[Warning]: Invalid tuning key: {k}")
             continue
         
         print(f"[DEBUG]: Tuning with key '{k}':")
```

### Comparing `spl_widgets-1.0.0/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.5.0/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.0.0/src/spl_widgets/jukemake.py` & `spl_widgets-1.5.0/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.0.0/src/spl_widgets/misc_util.py` & `spl_widgets-1.5.0/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.0.0/src/spl_widgets/stk_swx.py` & `spl_widgets-1.5.0/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.0.0/src/spl_widgets/tune_freq.py` & `spl_widgets-1.5.0/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.0.0/src/spl_widgets/tuner.py` & `spl_widgets-1.5.0/src/spl_widgets/tuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,53 @@
-from tkinter import *
+import tkinter as tk
 from tkinter import filedialog, ttk
 from spl_widgets.misc_util import *
 from spl_widgets.tune_freq import tune_cols
 from subprocess import run
 from pathlib import Path
 
-class RadioFrame(Frame):
+class RadioFrame(tk.Frame):
 
     def __init__(
         self,
-        master: Frame,
+        master: tk.Frame,
         options: "list[str]",
         label: str,
         onchange: "function",
         orientation="v",
         **kwargs
-        ) -> Frame:
-        Frame.__init__(self, master, **kwargs)
+        ) -> tk.Frame:
+        tk.Frame.__init__(self, master, **kwargs)
 
         self.master = master
-        self.variable = IntVar()
+        self.variable = tk.IntVar()
         self.onchange = lambda: onchange(self.variable) if onchange else None
 
         packside = "top" if orientation == "v" else "left"
-        anchorside = W if orientation == "v" else N
+        anchorside = "w" if orientation == "v" else "n"
 
-        self.label = Label(self,text=label)
-        self.label.pack(side="top", anchor=W)
+        self.label = tk.Label(self,text=label)
+        self.label.pack(side="top", anchor="w")
 
-        self.radios = [Radiobutton(self,text=o, variable=self.variable, value=i, command=self.onchange) for i,o in enumerate(options)]
-        for b in self.radios: b.pack(side=packside, anchor=anchorside)
+        self.radios = [
+            tk.Radiobutton(self,text=o, variable=self.variable, value=i, command=self.onchange)
+            for i,o in enumerate(options)
+        ]
+        for b in self.radios:
+            b.pack(side=packside, anchor=anchorside)
 
     def disable(self):
         for b in self.radios:
             b.configure(state="disabled")
 
     def enable(self):
         for b in self.radios:
             b.configure(state="normal")
 
-class TunerApp(Tk):
+class TunerApp(tk.Tk):
 
     cb_values = [f"{n} Major Scale" for n in notes]
     cb_values_ext = [f"{notes[i]} {n}" for n in default_scales.keys() for i in range(len(notes))]
 
     fmts_to_tune: list[int] = None
 
     # KEY FORMAT:
@@ -56,19 +60,19 @@
         new_key = key
 
         def is_hexadecimal(char: str):
             return (char.isdigit()) or (char.lower() in 'abcdef')
 
         invalid_key = any([
             len(key) > 10,
-            (9<=len(key)<=10) and not ( is_hexadecimal(key[-1]) ),
+            (8<len(key)<11) and not ( is_hexadecimal(key[-1]) ),
             (len(key)==8)     and ( key[-1] != "-" ),
-            (5<=len(key)<=7)  and not ( is_hexadecimal(key[-1]) ),
+            (4<len(key)<8)  and not ( is_hexadecimal(key[-1]) ),
             (len(key) == 4)   and ( key[-1] != "-" ),
-            (2<=len(key)<=3)  and not ( key[-1].isdigit() ),
+            (1<len(key)<4)  and not ( key[-1].isdigit() ),
             (len(key)==1)     and not ( key[0] in '01' )
         ])
 
         if invalid_key:
             new_key = key[:-1]
         self.key_var.set(new_key.upper())
 
@@ -107,15 +111,15 @@
         self.scale_combobox.configure(state="readonly")
         self.adv_scale_checkbox.configure(state="normal")
 
     def enable_note_tuning(self):
         for note_checkbox in self.note_buttons:
             note_checkbox.configure(state="normal")
 
-    def showsel(self, v: IntVar):
+    def showsel(self, v: tk.IntVar):
 
         if v.get():
             self.disable_scale_tuning()
             self.enable_note_tuning()
         else:
             self.disable_note_tuning()
             self.enable_scale_tuning()
@@ -133,15 +137,15 @@
                 filetypes=[("SWX Files","*.swx")]
                 )
             if file != "":
                 self.file_name.configure(text=f'File: {file[file.rfind("/")+1:]}')
 
         self.file_var.set(file)
 
-    def change_file_type(self, v: IntVar):
+    def change_file_type(self, v: tk.IntVar):
         if v.get():
             self.file_label.configure(text="Set Path to Tune: ")
             self.file_var.set("")
             self.file_name.configure(text="")
         else:
             self.file_label.configure(text="Set File to Tune: ")
             self.file_var.set("")
@@ -228,303 +232,311 @@
         self.title("CTSF's SWX Tuner")
         self.geometry("460x330+50+50")
         self.resizable(False, False)
         self.config(padx=4, pady=5, background="darkgray")
 
         # CONFIG: Tracked variables setup
 
-        self.interval_var = StringVar()
+        self.interval_var = tk.StringVar()
         self.interval_var.trace('w',self.limit_interval_len)
 
-        self.file_var = StringVar()
-        self.scale_var = StringVar(value="C Major Scale")
-        self.key_var = StringVar()
-
-        self.tune_type_var = IntVar()
-        self.show_scales_var = IntVar()
-        self.note_vars = [IntVar() for _ in range(len(notes))]
-        self.tune_freqs_var = IntVar(value=1)
+        self.file_var = tk.StringVar()
+        self.scale_var = tk.StringVar(value="C Major Scale")
+        self.key_var = tk.StringVar()
+
+        self.tune_type_var = tk.IntVar()
+        self.show_scales_var = tk.IntVar()
+        self.note_vars = [tk.IntVar() for _ in range(len(notes))]
+        self.tune_freqs_var = tk.IntVar(value=1)
 
 
         # Top-level Frames for left and right sides
 
         # Frame for main options
-        options_frame = Frame(self,
+        options_frame = tk.Frame(self,
             highlightbackground="black",
             highlightthickness="1",
         )
         
         # Frame for tuning method options (scales/notes)
-        tuning_frame = Frame(self,
+        tuning_frame = tk.Frame(self,
             highlightbackground="black",
             highlightthickness=1
         )
 
         # Packing frames in this order so the options frame expands correctly
         tuning_frame.pack(
-            side='right', anchor=N, fill=BOTH,
+            side='right', anchor="n", fill="both",
             padx=1
         )
         options_frame.pack(
-            side='left', anchor=N, fill=BOTH,
-            padx=1, expand=TRUE
+            side='left', anchor="n", fill="both",
+            padx=1, expand=True
         )
 
         # File input
 
         # Frame for file input widgets
-        file_input_frame = Frame(
+        file_input_frame = tk.Frame(
             options_frame,
             highlightbackground="black",
             highlightthickness=1,
             
         )
         file_input_frame.pack(
-            side='top', anchor=W, fill=X,
+            side='top', anchor="w", fill="x",
             padx=2, pady=2
         )
 
         # RadioFrame for whether to tune a file or a directory
         file_radio_frame = RadioFrame(
             file_input_frame,
             options=['Single file', 'Directory'],
             label="Object to Tune:",
             orientation="h",
             onchange=self.change_file_type,
             pady=3
         )
-        file_radio_frame.pack(side='top', anchor=W)
+        file_radio_frame.pack(side='top', anchor="w")
         self.file_type_var = file_radio_frame.variable  # get var from RadioFrame object and store locally
 
         # Frame for file input button
-        file_button_frame = Frame(file_input_frame)
-        file_button_frame.pack(side='top', fill=X, expand=TRUE)
+        file_button_frame = tk.Frame(file_input_frame)
+        file_button_frame.pack(side='top', fill="x", expand=True)
 
         # Label for file input
-        self.file_label = Label(file_button_frame, text="Set File to Tune:")
-        self.file_label.pack(side='left', anchor=W)
+        self.file_label = tk.Label(file_button_frame, text="Set File to Tune:")
+        self.file_label.pack(side='left', anchor="w")
 
         # File input widget
-        file_input_button = Button(
+        file_input_button = tk.Button(
             file_button_frame, text="Browse...", 
             command=self.get_file
         )
-        file_input_button.pack(side='right', anchor=W)
+        file_input_button.pack(side='right', anchor="w")
 
         # Label for filename (updated when a new file/dir is selected)
-        self.file_name = Label(file_input_frame)
-        self.file_name.pack(side='top', anchor=W, pady=3)
+        self.file_name = tk.Label(file_input_frame)
+        self.file_name.pack(side='top', anchor="w", pady=3)
 
 
         # Interval input widget
 
         # Frame for interval input
-        interval_frame = Frame(
+        interval_frame = tk.Frame(
             options_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         interval_frame.pack(
-            side='top', anchor=W, fill=X,
+            side='top', anchor="w", fill="x",
             padx=2, pady=0
         )
 
         # Label for interval input
-        interval_input_label = Label(interval_frame, text="Tuning interval (x10ms): ")
-        interval_input_label.pack(side='left',anchor=N, pady=2)
+        interval_input_label = tk.Label(interval_frame, text="Tuning interval (x10ms): ")
+        interval_input_label.pack(side='left',anchor="n", pady=2)
 
         # Interval input textbox
-        interval_input = Entry(interval_frame, width=2, textvariable=self.interval_var)
-        interval_input.pack(side='left',anchor=N)
+        interval_input = tk.Entry(interval_frame, width=2, textvariable=self.interval_var)
+        interval_input.pack(side='left',anchor="n")
 
 
         # Tunetype settings input
 
         # Frame for selector
-        selector_frame = Frame(
+        selector_frame = tk.Frame(
             options_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         selector_frame.pack(
-            side='top', anchor=W, fill=X,
+            side='top', anchor="w", fill="x",
             padx=2, pady=2
         )
 
         # checkbutton for whether to tune the file at all
-        tune_freqs_checkbox = Checkbutton(
+        tune_freqs_checkbox = tk.Checkbutton(
             selector_frame,
             text="Tune Frequencies",
             pady=10,
             command=self.change_tune_freqs,
             onvalue=1, offvalue=0,
             variable=self.tune_freqs_var
         )
-        tune_freqs_checkbox.pack(anchor=W, side='top')
+        tune_freqs_checkbox.pack(anchor="w", side='top')
 
         # RadioFrame for whether to tune by scale or by notes
         self.selector_radios_frame = RadioFrame(
             selector_frame,
             options=["Scale", "Notes"],
             label="Tune File By:",
             onchange=self.showsel,
             pady=5
         )
         self.tune_type_var = self.selector_radios_frame.variable    # get var from RadioFrame object and store locally
-        self.selector_radios_frame.pack(side="top", anchor=W)
+        self.selector_radios_frame.pack(side="top", anchor="w")
 
 
         # Submit Button
-
-        submit_button = Button(
+        submit_frame = tk.Frame(
             options_frame,
-            text="Tune File",
-            command=self.tune_with_data,
+            highlightbackground="black",
+            highlightthickness=1
+        )
+        submit_frame.pack(
+            side="left", anchor="center", fill="both", expand=True,
+            padx=2, pady=2
         )
-        submit_button.pack(
-            side='left', anchor=CENTER, fill=BOTH,
-            expand=TRUE
+        submit_button = tk.Button(
+            submit_frame,
+            text="Tune File",
+            relief="flat",
+            borderwidth=0,
+            highlightthickness=0,
+            command=self.tune_with_data
         )
+        submit_button.pack( fill="both",expand=True )
 
         ##### RIGHT SIDE FRAME #####
 
         # Scale selection combobox widget
 
         # frame for scale selector
-        scale_radio_frame = Frame(
+        scale_radio_frame = tk.Frame(
             tuning_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         scale_radio_frame.pack(
-            side="top", anchor=N, fill=X, 
+            side="top", anchor="n", fill="x", 
             padx=2, pady=2
         )
 
         # Label for the scale selection combobox
-        scaleRadioLabel = Label(
+        scaleRadioLabel = tk.Label(
             scale_radio_frame,
             text="Select scale to tune to: "
         )
-        scaleRadioLabel.pack(anchor=W, padx=2)
+        scaleRadioLabel.pack(anchor="w", padx=2)
 
         # Combobox scale selector
         self.scale_combobox = ttk.Combobox(
             scale_radio_frame,
             textvariable = self.scale_var,
             values=self.cb_values,
             state = "readonly"
         )
-        self.scale_combobox.pack(anchor=W, padx=2)
+        self.scale_combobox.pack(anchor="w", padx=2)
 
         # Checkbutton for displaying/hiding additional scales
-        self.adv_scale_checkbox = Checkbutton(
+        self.adv_scale_checkbox = tk.Checkbutton(
             scale_radio_frame,
             command=self.change_scales_shown,
             text="Show additional scales",
             onvalue=1,offvalue=0,
             variable=self.show_scales_var
         )
-        self.adv_scale_checkbox.pack(anchor=W, pady=2)
+        self.adv_scale_checkbox.pack(anchor="w", pady=2)
 
 
         # Note selection checkbuttons widget
 
         # Frame for note selection label and checkbuttons
-        note_buttons_frame = Frame(
+        note_buttons_frame = tk.Frame(
             tuning_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         note_buttons_frame.pack(
-            anchor=SW, fill=X, expand=TRUE,
+            anchor="sw", fill="x", expand=True,
             padx=2, pady=0, ipadx=10
         )
 
         # label for note checkbuttons
-        note_buttons_label = Label(
+        note_buttons_label = tk.Label(
             note_buttons_frame,
             text="Select note(s) to tune to: "
         )
-        note_buttons_label.pack(anchor=N)
+        note_buttons_label.pack(anchor="n")
 
         # Frame for note checkbuttons (Goes below label)
-        bottom_notes_frame=Frame(note_buttons_frame)
+        bottom_notes_frame=tk.Frame(note_buttons_frame)
         bottom_notes_frame.pack(side='bottom')
 
         # left column frame for note checkbuttons
-        notes_leftcol_frame = Frame(
+        notes_leftcol_frame = tk.Frame(
             bottom_notes_frame,
             borderwidth=3, padx=10
         )        
-        notes_leftcol_frame.pack(side='left', anchor=W)
+        notes_leftcol_frame.pack(side='left', anchor="w")
 
         # right column frame for note checkbuttons
-        notes_rightcol_frame = Frame(
+        notes_rightcol_frame = tk.Frame(
             bottom_notes_frame,
             borderwidth=3, padx=10
         )
-        notes_rightcol_frame.pack(side='right', anchor=W)
+        notes_rightcol_frame.pack(side='right', anchor="w")
 
         # ugly list comprehension to generate note checkbuttons
         # (but it works and it'll never need to be changed)
         self.note_buttons = [
-            Checkbutton(
+            tk.Checkbutton(
                 master=(notes_leftcol_frame if i<6 else notes_rightcol_frame),  # half in the left column, half in the right (the ugliness)
                 text=n,
                 variable=self.note_vars[i],
                 onvalue=1, offvalue=0,
                 state="disabled"
             )
             for i,n in enumerate(notes)
         ]
         for n in self.note_buttons:         # packing the note buttons
-            n.pack(anchor=W)
+            n.pack(anchor="w")
 
 
         # Tuning key Frame
-        key_frame = Frame(
+        key_frame = tk.Frame(
             tuning_frame,
             highlightbackground="black",
             highlightthickness=1
         )
         key_frame.pack(
-            side='top', anchor=W, fill=X, expand=TRUE,
+            side='top', anchor="w", fill="x", expand=True,
             ipady=3, pady=2, padx=2
         )
 
         # Frame for tuning key input widget
-        key_input_frame = Frame(key_frame)
+        key_input_frame = tk.Frame(key_frame)
         key_input_frame.pack(side="top")
 
         # key input label
-        key_input_label = Label(key_input_frame, text="Tune with key:")
+        key_input_label = tk.Label(key_input_frame, text="Tune with key:")
         key_input_label.pack(side='left')
 
         # key input textbox
-        key_input = Entry(key_input_frame, width=9, textvariable=self.key_var)
+        key_input = tk.Entry(key_input_frame, width=9, textvariable=self.key_var)
         key_input.pack(side='left')
 
         # validate tuning key on edit of textbox content with event listener
         self.key_var.trace('w', self.validate_key)
 
 
         # frame for set/get key buttons
-        key_buttons_frame = Frame(key_frame)
-        key_buttons_frame.pack(side="top", anchor=CENTER)
+        key_buttons_frame = tk.Frame(key_frame)
+        key_buttons_frame.pack(side="top", anchor="center")
 
         # button to generate parameters from current tuning key
-        set_key_button = Button(
+        set_key_button = tk.Button(
             key_buttons_frame, text="Set Key",
             command=self.process_tuning_key
         )
         set_key_button.pack(side='left')
 
         # button to generate key from current params
-        get_key_button = Button(
+        get_key_button = tk.Button(
             key_buttons_frame, text="Get Key",
             command=self.generate_tuning_key
         )
         get_key_button.pack(side="right")
 
 
 def main():
```

### Comparing `spl_widgets-1.0.0/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.5.0/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/spl_widgets/__init__.py
 src/spl_widgets/__main__.py
 src/spl_widgets/batch_tune.py
-src/spl_widgets/clear_aliases.py
 src/spl_widgets/gorilla_clean.py
 src/spl_widgets/jukemake.py
 src/spl_widgets/misc_util.py
 src/spl_widgets/stk_swx.py
 src/spl_widgets/tune_freq.py
 src/spl_widgets/tuner.py
 src/spl_widgets.egg-info/PKG-INFO
 src/spl_widgets.egg-info/SOURCES.txt
 src/spl_widgets.egg-info/dependency_links.txt
 src/spl_widgets.egg-info/entry_points.txt
 src/spl_widgets.egg-info/requires.txt
-src/spl_widgets.egg-info/top_level.txt
+src/spl_widgets.egg-info/top_level.txt
+src/spl_widgets/data/cmudict.sqlite
```


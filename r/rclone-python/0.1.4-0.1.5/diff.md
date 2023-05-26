# Comparing `tmp/rclone-python-0.1.4.tar.gz` & `tmp/rclone-python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclone-python-0.1.4.tar", last modified: Tue May  2 16:51:38 2023, max compression
+gzip compressed data, was "rclone-python-0.1.5.tar", last modified: Fri May 26 21:20:29 2023, max compression
```

## Comparing `rclone-python-0.1.4.tar` & `rclone-python-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:51:38.092476 rclone-python-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 16:51:26.000000 rclone-python-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-02 16:51:38.092476 rclone-python-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-02 16:51:26.000000 rclone-python-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:51:38.088476 rclone-python-0.1.4/rclone_python/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/rclone.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/remote_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:51:38.092476 rclone-python-0.1.4/rclone_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:51:38.092476 rclone-python-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 16:51:26.000000 rclone-python-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:20:29.191297 rclone-python-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 21:20:16.000000 rclone-python-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 21:20:29.187297 rclone-python-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-26 21:20:16.000000 rclone-python-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:20:29.187297 rclone-python-0.1.5/rclone_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/remote_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:20:29.187297 rclone-python-0.1.5/rclone_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:20:29.191297 rclone-python-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-26 21:20:16.000000 rclone-python-0.1.5/setup.py
```

### Comparing `rclone-python-0.1.4/LICENSE` & `rclone-python-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.4/PKG-INFO` & `rclone-python-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.4/README.md` & `rclone-python-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.4/rclone_python/rclone.py` & `rclone-python-0.1.5/rclone_python/rclone.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import re
 import subprocess
 from functools import wraps
 from pathlib import Path
 from shutil import which
 from typing import Union, List, Dict, Tuple, Callable, Any
 
-from tqdm import tqdm
-
 from rclone_python import utils
 from rclone_python.remote_types import RemoteTypes
 
 
 def __check_installed(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
@@ -223,21 +221,15 @@
     if move_files:
         command = f'rclone move'
         prog_title = f'Moving'
     else:
         command = f'rclone copyto'
         prog_title = f'Copying'
 
-    # generate progress title from in path. When copying the root directory use the remote name instead
-    if ':' in in_path:
-        in_path_no_prefix = in_path[in_path.index(':') + 1:] if in_path.index(':') + 1 < len(in_path) \
-            else in_path[0:in_path.index(':')]
-    else:
-        in_path_no_prefix = in_path
-    prog_title += f" {Path(in_path_no_prefix).name}"
+    prog_title += f" [bold magenta]{utils.shorten_filepath(in_path, 20)}[/bold magenta] to [bold magenta]{utils.shorten_filepath(out_path, 20)}"
 
     # add global rclone flags
     if ignore_existing:
         command += ' --ignore-existing'
     command += ' --progress'
 
     # in path
@@ -261,65 +253,72 @@
 
 def _rclone_progress(command: str, pbar_title: str, stderr=subprocess.PIPE, show_progress=True,
                      listener: Callable[[Dict], None] = None) -> subprocess.Popen:
     process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=stderr, shell=True)
 
     buffer = ""
     pbar = None
+    total_progress_id = None
+    subprocesses = {}
 
     if show_progress:
-        pbar = tqdm(bar_format='{l_bar}{bar}| {n:.1f}/{total_fmt} {unit}{postfix}')
-        pbar.set_description(f'☁ {pbar_title}')
+        pbar, total_progress_id = utils.create_progress_bar(pbar_title)
+
 
     for c in iter(lambda: process.stdout.read(1), b''):
-        var = c.decode('utf-8')
+        var = c.decode('utf-8', 'ignore')
         if '\n' not in var:
             buffer += var
         else:
             valid, update_dict = _extract_rclone_progress(buffer)
 
             if valid:
                 if show_progress:
-                    pbar.set_postfix_str(f'{update_dict["transfer_speed"]:.1f} {update_dict["transfer_speed_unit"]}, '
-                                         f'ETA: {update_dict["eta"]}')
-                    pbar.total = update_dict['total_bits']
-                    pbar.unit = update_dict['unit_total']
-                    pbar.update(update_dict['sent_bits'] - pbar.n, )
+                    utils.update_tasks(pbar, total_progress_id, update_dict, subprocesses)
 
                 # call the listener
                 if listener:
                     listener(update_dict)
 
                 # reset the buffer
                 buffer = ""
 
     if show_progress:
-        if not pbar.total:
-            # if no data is downloaded/ upload because the data is already present: manually set progress to 100%
-            pbar.total = 1
-            pbar.update()
-        pbar.close()
+        utils.complete_task(total_progress_id, pbar)
+        pbar.stop()
 
     return process
 
-
 def _extract_rclone_progress(buffer: str) -> Tuple[bool, Union[Dict[str, Any], None]]:
     # matcher that checks if the progress update block is completely buffered yet (defines start and stop)
     # it gets the sent bits, total bits, progress, transfer-speed and eta
     reg_transferred = re.findall(
         r'Transferred:\s+(\d+.\d+ \w+) \/ (\d+.\d+ \w+), (\d{1,3})%, (\d+.\d+ \w+\/\w+), ETA (\S+)',
         buffer)
 
     if reg_transferred:  # transferred block is completely buffered
         # get the progress of the individual files
         # matcher gets the currently transferring files and their individual progress
-        # returns list of tuples: (name, progress)
-        out = {'prog_transferring': re.findall(r'\* +(\S+):[ ]+(\d{1,2})%', buffer)}
+        # returns list of tuples: (name, progress, file_size, unit)
+        prog_transfering = []
+        prog_regex = re.findall(r'\* +(\S+):[ ]+(\d{1,2})% \/(\d+.\d+)([a-zA-Z]+),', buffer)
+        for item in prog_regex:
+            prog_transfering.append(
+                (
+                    item[0],
+                    int(item[1]),
+                    float(item[2]),
+                    # the suffix B of the unit is missing for subprocesses
+                    item[3] + "B",  
+                )
+            )
 
+        out = {'prog_transferring': prog_transfering}
         sent_bits, total_bits, progress, transfer_speed_str, eta = reg_transferred[0]
+        out['progress'] = float(progress.strip())
         out['total_bits'] = float(re.findall(r'\d+.\d+', total_bits)[0])
         out['sent_bits'] = float(re.findall(r'\d+.\d+', sent_bits)[0])
         out['unit_sent'] = re.findall(r'[a-zA-Z]+', sent_bits)[0]
         out['unit_total'] = re.findall(r'[a-zA-Z]+', total_bits)[0]
         out['transfer_speed'] = float(re.findall(r'\d+.\d+', transfer_speed_str)[0])
         out['transfer_speed_unit'] = re.findall(r'[a-zA-Z]+/[a-zA-Z]+', transfer_speed_str)[0]
         out['eta'] = eta
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rclone-python-0.1.4/rclone_python.egg-info/PKG-INFO` & `rclone-python-0.1.5/rclone_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.4/setup.py` & `rclone-python-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     name='rclone-python',
     version=VERSION,
     description='A python wrapper for rclone.',
     author='Johannes Gundlach',
     url='https://github.com/Johannes11833/rclone_python',
-    install_requires=['tqdm'],
+    install_requires=['rich'],
     packages=['rclone_python'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['rclone', 'wrapper', 'cloud sync'],
     python_requires='>=3.6',
     classifiers=[
         "Programming Language :: Python :: 3",
```


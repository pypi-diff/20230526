# Comparing `tmp/dankware-3.3.8.tar.gz` & `tmp/dankware-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.3.8.tar", last modified: Tue May 16 10:17:15 2023, max compression
+gzip compressed data, was "dankware-3.3.9.tar", last modified: Fri May 26 12:37:54 2023, max compression
```

## Comparing `dankware-3.3.8.tar` & `dankware-3.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:17:15.805780 dankware-3.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:16:59.000000 dankware-3.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-16 10:17:15.805780 dankware-3.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-16 10:16:59.000000 dankware-3.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:17:15.801780 dankware-3.3.8/dankware/
--rw-r--r--   0 runner    (1001) docker     (123)    46421 2023-05-16 10:16:59.000000 dankware-3.3.8/dankware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:17:15.805780 dankware-3.3.8/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:17:15.805780 dankware-3.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-16 10:16:59.000000 dankware-3.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:37:54.516018 dankware-3.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 12:37:43.000000 dankware-3.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-26 12:37:54.516018 dankware-3.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-26 12:37:43.000000 dankware-3.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:37:54.512018 dankware-3.3.9/dankware/
+-rw-r--r--   0 runner    (1001) docker     (123)    46356 2023-05-26 12:37:43.000000 dankware-3.3.9/dankware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:37:54.516018 dankware-3.3.9/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:37:54.516018 dankware-3.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-26 12:37:43.000000 dankware-3.3.9/setup.py
```

### Comparing `dankware-3.3.8/LICENSE` & `dankware-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.3.8/PKG-INFO` & `dankware-3.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.8
+Version: 3.3.9
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.3.8/README.md` & `dankware-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dankware-3.3.8/dankware/__init__.py` & `dankware-3.3.9/dankware/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""
+> Please read the documentation on https://github.com/SirDank/dankware before using this module!
+"""
+
 ###################################################################################
 
 #                            https://github.com/SirDank                            
 
 ###################################################################################
 
-# > Please read the documentation on github before using this module!
-
 import os
 import sys
 import time
 import random
 from datetime import datetime
 from colorama import Fore, Style
 
@@ -26,19 +28,17 @@
 yellow = Fore.YELLOW + Style.BRIGHT
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def multithread(function: callable, threads: int = 1, *args, progress_bar: bool = True) -> None:
     
     """
-    > Please read the documentation on github before using this function!
-    
-    ________________________________________________________________________________
-
     Run the given function in multiple threads with the specified inputs.
+    
+    ________________________________________________________________________
 
     - function: The function to run in multiple threads.
     - threads: The number of threads to use.
     - *args: Input(s) for the function. Can be a list, a single value.
     - progress_bar: Whether to display a progress bar.
     """
     
@@ -116,27 +116,22 @@
     ```python
     from dankware import github_downloads
     for _ in github_downloads("SirDank/dank.tool"): print(_)
     ```
     """
     
     import requests
-    
-    urls = []
 
     #if "https://api.github.com/repos/" not in url or "/releases/latest" not in url:
     #    raise ValueError(clr('  > Invalid url! Must follow: "https://api.github.com/repos/NAME/NAME/releases/latest"',2)) 
     while True:
         try: response = requests.get(f"https://api.github.com/repos/{user_repo}/releases/latest").json(); break
         except: input(clr("  > Make sure you are connected to the Internet! Press [ENTER] to try again... ",2))
     
-    for data in response["assets"]:
-        urls.append(data["browser_download_url"])
-
-    return urls
+    return [data["browser_download_url"] for data in response["assets"]]
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def github_file_selector(user_repo: str, filter_mode: str, name_list: list) -> list:
     
     """
     
@@ -233,18 +228,16 @@
         elif first_octet == 192:
             if fourth_octet == 170 or fourth_octet == 171 or third_octet == 2: continue
         elif first_octet == 203 and third_octet == 113: continue
         elif first_octet == 216 and second_octet == 83 and third_octet >= 33 and third_octet <= 63: continue
         elif second_octet == 255 and third_octet == 255 and third_octet == 255: continue
 
         break
-    
-    ip = f"{first_octet}.{second_octet}.{third_octet}.{fourth_octet}"
         
-    return ip
+    return f"{first_octet}.{second_octet}.{third_octet}.{fourth_octet}"
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def is_admin() -> bool:
     
     import ctypes
     
@@ -264,15 +257,15 @@
     
     ctypes.windll.shell32.ShellExecuteW(None, "runas", sys.executable, __file__, None, 1)
     #sys.exit(clr("\n  > Exiting original un-elevated script...",2))
 '''
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def export_registry_keys(registry_root: str, registry_path: str, recursive: bool = True, export_path: str = "export.reg") -> None:
+def export_registry_keys(registry_root: str, registry_path: str, recursive: bool = True, export_path: str = "export.reg", verbose: bool = True) -> None:
 
     """
     Function to export registry keys with or without its subkeys and saves them to export_path
     - Examples for registry_root: 'HKEY_CLASSES_ROOT', 'HKEY_CURRENT_USER', 'HKEY_LOCAL_MACHINE', 'HKEY_USERS', 'HKEY_CURRENT_CONFIG'
     - Example for registry_path: r'Software\Google\Chrome\PreferenceMACs'
     - recursive: True (subkeys saved)
     - recursive: False (subkeys not saved)
@@ -327,15 +320,17 @@
                 if recursive: exporter(key, registry_root, subkey_full_path, key_data, recursive)
 
             winreg.CloseKey(subkey)
 
         key = key_map[registry_root]
         exporter(key, registry_root, registry_path, key_data, recursive)
         open(export_path, 'w', encoding='utf-16').write('Windows Registry Editor Version 5.00\n\n' + '\n'.join(key_data))
-        print(clr(f"\n  > Successfully exported registry keys to \"{os.path.join(os.getcwd(), 'export.reg') if export_path == 'export.reg' else export_path}\""))
+        
+        if verbose:
+            print(clr(f"\n  > Successfully exported registry keys to \"{os.path.join(os.getcwd(), 'export.reg') if export_path == 'export.reg' else export_path}\""))
     
     except: sys.exit(clr(err(sys.exc_info()),2))
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def clr(text: str, mode: int = 1, colour_one: str = white, colour_two: str = magenta) -> str:
     
@@ -433,15 +428,15 @@
 
         else: raise ValueError(f"\n  {white}> {red}Invalid Mode {white}[{red}{mode}{white}] | Valid Modes{white}: {red}1{white},{red}2{white},{red}3{white},{red}4" + reset)
 
         if mode not in [3, 4]:
             for _ in range(len(colours_to_replace)):
                 text = text.replace(colours_alt[_], colours_to_replace[_])
 
-        if mode == 1: return white + text + reset
+        if mode == 1: return colour_one + text + reset
         elif mode == 2: return red + text + reset
         elif mode == 3 or mode == 4: return text + reset
     
     except: sys.exit(clr(err(sys.exc_info()),2))
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
@@ -601,14 +596,15 @@
                     faded += f"\033[38;2;{R};{G};{B}m{char}\033[0m"
                 if multi_line: faded += "\n"
         
         else: raise ValueError(clr(f"\n  > FADE ERROR! - [{colour}] is not supported yet!",2))
         
         if multi_line: faded = faded[:-1]
         return faded
+
     except: sys.exit(clr(err(sys.exc_info()),2))
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def get_duration(then: datetime, now: datetime = None, interval = "default"):
 
     """
@@ -858,23 +854,23 @@
 def get_path(name: str) -> str:
     
     """
     Returns path from registry
     - Supports: Desktop / Documents / Favorites / Pictures / Videos / Music
     """
     
+    import os
+    import winreg
+    
     if name in ["Desktop", "Documents", "Favorites", "Pictures", "My Pictures", "Videos", "My Video", "Music", "My Music"]:
         
         if name == "Documents": name = "Personal"
         elif name == "Pictures": name = "My Pictures"
         elif name == "Videos": name = "My Video"
         elif name == "Music": name = "My Music"
-        
-        import winreg
-        import os
 
         key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders", access=winreg.KEY_READ)
         path = os.path.expandvars(winreg.QueryValueEx(key, name)[0])
         return path
     
     else: raise ValueError("Invalid name")
```

### Comparing `dankware-3.3.8/dankware.egg-info/PKG-INFO` & `dankware-3.3.9/dankware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.8
+Version: 3.3.9
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.3.8/setup.py` & `dankware-3.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.3.8",
+    version = "3.3.9",
     author = "SirDank",
     
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
```


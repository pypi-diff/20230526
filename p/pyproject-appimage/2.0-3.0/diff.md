# Comparing `tmp/pyproject-appimage-2.0.tar.gz` & `tmp/pyproject-appimage-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-appimage-2.0.tar", last modified: Thu Jan 19 15:48:46 2023, max compression
+gzip compressed data, was "pyproject-appimage-3.0.tar", last modified: Fri May 26 08:15:11 2023, max compression
```

## Comparing `pyproject-appimage-2.0.tar` & `pyproject-appimage-3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 15:48:46.348241 pyproject-appimage-2.0/
--rw-r--r--   0 root         (0) root         (0)     1313 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4260 2023-01-19 15:48:46.348241 pyproject-appimage-2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3078 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1654 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 15:48:46.348241 pyproject-appimage-2.0/pyproject_appimage/
--rw-r--r--   0 root         (0) root         (0)    13007 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/pyproject_appimage/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/pyproject_appimage/__main__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/pyproject_appimage/default.desktop
--rw-r--r--   0 root         (0) root         (0)    28792 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/pyproject_appimage/default.png
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-19 15:48:10.000000 pyproject-appimage-2.0/pyproject_appimage/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 15:48:46.348241 pyproject-appimage-2.0/pyproject_appimage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4260 2023-01-19 15:48:46.000000 pyproject-appimage-2.0/pyproject_appimage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      445 2023-01-19 15:48:46.000000 pyproject-appimage-2.0/pyproject_appimage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-19 15:48:46.000000 pyproject-appimage-2.0/pyproject_appimage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-01-19 15:48:46.000000 pyproject-appimage-2.0/pyproject_appimage.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-01-19 15:48:46.000000 pyproject-appimage-2.0/pyproject_appimage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-01-19 15:48:46.000000 pyproject-appimage-2.0/pyproject_appimage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-19 15:48:46.348241 pyproject-appimage-2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 08:15:11.199147 pyproject-appimage-3.0/
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4260 2023-05-26 08:15:11.199147 pyproject-appimage-3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 08:15:11.199147 pyproject-appimage-3.0/pyproject_appimage/
+-rw-r--r--   0 root         (0) root         (0)    15126 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/pyproject_appimage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/pyproject_appimage/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/pyproject_appimage/default.desktop
+-rw-r--r--   0 root         (0) root         (0)    28792 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/pyproject_appimage/default.png
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-26 08:14:31.000000 pyproject-appimage-3.0/pyproject_appimage/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 08:15:11.199147 pyproject-appimage-3.0/pyproject_appimage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4260 2023-05-26 08:15:11.000000 pyproject-appimage-3.0/pyproject_appimage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 08:15:11.000000 pyproject-appimage-3.0/pyproject_appimage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 08:15:11.000000 pyproject-appimage-3.0/pyproject_appimage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-26 08:15:11.000000 pyproject-appimage-3.0/pyproject_appimage.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-26 08:15:11.000000 pyproject-appimage-3.0/pyproject_appimage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-26 08:15:11.000000 pyproject-appimage-3.0/pyproject_appimage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 08:15:11.199147 pyproject-appimage-3.0/setup.cfg
```

### Comparing `pyproject-appimage-2.0/LICENSE` & `pyproject-appimage-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-appimage-2.0/PKG-INFO` & `pyproject-appimage-3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-appimage
-Version: 2.0
+Version: 3.0
 Summary: Generate AppImages from your Python projects
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Downloads, https://codeberg.org/JakobDev/pyproject-appimage/releases
 Project-URL: Issues, https://codeberg.org/JakobDev/pyproject-appimage/issues
 Project-URL: Source, https://codeberg.org/JakobDev/pyproject-appimage
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `pyproject-appimage-2.0/README.md` & `pyproject-appimage-3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-appimage-2.0/pyproject.toml` & `pyproject-appimage-3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject-appimage-2.0/pyproject_appimage/__init__.py` & `pyproject-appimage-3.0/pyproject_appimage/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,59 +20,74 @@
 
 PyprojectDict = TypedDict("PyprojectDict", {
     "script": str,
     "icon": str,
     "rename-icon": str,
     "desktop-entry": str,
     "rename-desktop-entry": str,
+    "gettext-desktop-entry": bool,
     "appstream": str,
     "rename-appstream": str,
+    "gettext-appstream": bool,
+    "gettext-directory": str,
     "python-version": str,
     "output": str
 }, total=False)
 
 
 def check_key(project_dir: str, pyproject: PyprojectDict, key: str, error_list: list[str], checks: list[str]) -> None:
     if key not in pyproject:
         if "required" in checks:
             error_list.append(f"\"{key}\" is required but not present")
         return
 
     if "string" in checks:
         if not isinstance(pyproject[key], str):
-            error_list.append("\"{key}\" must be a string")
+            error_list.append(f"\"{key}\" must be a string")
         elif pyproject[key].strip() == "":
             error_list.append(f"\"{key}\" must not be empty")
-        elif "path" in checks and not os.path.isfile(os.path.join(project_dir, pyproject[key])):
+        elif "path" in checks and not os.path.exists(os.path.join(project_dir, pyproject[key])):
             error_list.append("The path " + os.path.join(project_dir, pyproject[key]) + f" for \"{key}\" is not valid")
+    if "bool" in checks:
+        if not isinstance(pyproject[key], bool):
+            error_list.append(f"\"{key}\" must be a bool")
 
 
 def check_pyproject(project_dir: str, pyproject: PyprojectDict) -> None:
     error_list: list[str] = []
 
     check_key(project_dir, pyproject, "script", error_list, ["required", "string"])
     check_key(project_dir, pyproject, "icon", error_list, ["string", "path"])
     check_key(project_dir, pyproject, "rename-icon", error_list, ["string"])
     check_key(project_dir, pyproject, "desktop-entry", error_list, ["string", "path"])
     check_key(project_dir, pyproject, "rename-desktop-entry", error_list, ["string"])
+    check_key(project_dir, pyproject, "gettext-desktop-entry", error_list, ["bool"])
     check_key(project_dir, pyproject, "appstream", error_list, ["string", "path"])
     check_key(project_dir, pyproject, "rename-appstream", error_list, ["string"])
+    check_key(project_dir, pyproject, "gettext-appstream", error_list, ["bool"])
+    check_key(project_dir, pyproject, "gettext-directory", error_list, ["string", "path"])
     check_key(project_dir, pyproject, "python-version", error_list, ["string"])
     check_key(project_dir, pyproject, "output", error_list, ["string"])
     check_key(project_dir, pyproject, "updateinformation", error_list, ["string"])
     check_key(project_dir, pyproject, "compression", error_list, ["string"])
 
+    if ("gettext-desktop-entry" in pyproject or "gettext-appstream" in pyproject) and not "gettext-directory" in pyproject:
+        error_list.append("\"gettext-directory\" must be set when using gettext")
+
+    if "gettext-directory" in pyproject and shutil.which("msgfmt") is None:
+        error_list.append("msgfmt must be installed when using gettext")
+
     if len(error_list) > 0:
         print(f"There are errors in the {PYPROJECT_SECTION} section of your pyproject.toml:", file=sys.stderr)
         print("\n".join(error_list), file=sys.stderr)
         sys.exit(1)
 
 
 def download_file(url: str, path: str) -> None:
-    print(f"Donwload {url} as {path}")
+    print(f"Download {url} as {path}")
     r = requests.get(url, stream=True)
     if r.status_code != 200:
         print(f"{url} returns {r.status_code}", file=sys.stderr)
         sys.exit(1)
     with open(path, "wb") as f:
         shutil.copyfileobj(r.raw, f)
 
@@ -158,15 +173,15 @@
 
         if "rename-icon" in pyproject:
             os.rename(os.path.join(app_root, os.path.basename(pyproject["icon"])), os.path.join(app_root, pyproject["rename-icon"]))
             icon_name = pyproject["rename-icon"]
         else:
             icon_name = os.path.basename(pyproject["icon"])
 
-        os.symlink(icon_name, os.path.join(app_root, ".DirIcon"))
+        shutil.copyfile(os.path.join(app_root, icon_name), os.path.join(app_root, ".DirIcon"))
 
         if icon_name.endswith(".svg"):
             icon_dir = os.path.join(app_root, "usr", "share", "icons", "hicolor", "scalable", "apps")
         else:
             icon_size = get_icon_size(work_dir, os.path.join(app_root, icon_name))
             icon_dir = os.path.join(app_root, "usr", "share", "icons", "hicolor", f"{icon_size[0]}x{icon_size[1]}", "apps")
 
@@ -174,26 +189,49 @@
             os.makedirs(icon_dir)
 
         shutil.copyfile(os.path.join(app_root, icon_name), os.path.join(icon_dir, icon_name))
     else:
         shutil.copyfile(os.path.join(os.path.dirname(__file__), "default.png"), os.path.join(app_root, ".DirIcon"))
 
     if "desktop-entry" in pyproject:
-        shutil.copyfile(os.path.join(project_dir, pyproject["desktop-entry"]), os.path.join(app_root, pyproject.get("rename-desktop-entry", os.path.basename(pyproject["desktop-entry"]))))
+        desktop_source_path = os.path.join(project_dir, pyproject["desktop-entry"])
+        desktop_dest_path = os.path.join(app_root, pyproject.get("rename-desktop-entry", os.path.basename(pyproject["desktop-entry"])))
+
+        if pyproject.get("gettext-desktop-entry", False):
+            subprocess.run(["msgfmt", "--desktop", "--template", desktop_source_path, "-d", os.path.join(project_dir, pyproject["gettext-directory"]), "-o", desktop_dest_path], check=True)
+        else:
+            shutil.copyfile(desktop_source_path, desktop_dest_path)
+
+        desktop_share_dir = os.path.join(app_root, "usr", "share", "applications")
+
+        if not os.path.isdir(desktop_share_dir):
+            os.makedirs(desktop_share_dir)
+
+        shutil.copyfile(desktop_dest_path, os.path.join(desktop_share_dir, os.path.basename(desktop_dest_path)))
     else:
         shutil.copyfile(os.path.join(os.path.dirname(__file__), "default.desktop"), os.path.join(app_root, "App.desktop"))
         os.symlink(".DirIcon", os.path.join(app_root, "Icon.png"))
 
     if "appstream" in pyproject:
         appstream_path = os.path.join(app_root, "usr", "share", "metainfo")
 
+        appstream_source_path = os.path.join(project_dir, pyproject["appstream"])
+        appstream_dest_path = os.path.join(appstream_path, pyproject.get("rename-appstream", os.path.basename(pyproject["appstream"])))
+
+        # .metainfo.xml is currently not supported by AppImage
+        if appstream_dest_path.endswith(".metainfo.xml"):
+            appstream_dest_path = appstream_dest_path.removesuffix(".metainfo.xml") + ".appdata.xml"
+
         if not os.path.isdir(appstream_path):
             os.makedirs(appstream_path)
 
-        shutil.copyfile(os.path.join(project_dir, pyproject["appstream"]), os.path.join(appstream_path, pyproject.get("rename-appstream", os.path.basename(pyproject["appstream"]))))
+        if pyproject.get("gettext-desktop-entry", False):
+            subprocess.run(["msgfmt", "--xml", "--template", appstream_source_path, "-d", os.path.join(project_dir, pyproject["gettext-directory"]), "-o", appstream_dest_path], check=True)
+        else:
+            shutil.copyfile(appstream_source_path, appstream_dest_path)
 
     if args.output is not None:
         output = args.output
     elif "output" in pyproject:
         output = pyproject["output"]
     else:
         output = "MyApp.AppImage"
```

### Comparing `pyproject-appimage-2.0/pyproject_appimage/default.png` & `pyproject-appimage-3.0/pyproject_appimage/default.png`

 * *Files identical despite different names*

### Comparing `pyproject-appimage-2.0/pyproject_appimage.egg-info/PKG-INFO` & `pyproject-appimage-3.0/pyproject_appimage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-appimage
-Version: 2.0
+Version: 3.0
 Summary: Generate AppImages from your Python projects
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Downloads, https://codeberg.org/JakobDev/pyproject-appimage/releases
 Project-URL: Issues, https://codeberg.org/JakobDev/pyproject-appimage/issues
 Project-URL: Source, https://codeberg.org/JakobDev/pyproject-appimage
 Project-URL: Donation, https://ko-fi.com/jakobdev
```


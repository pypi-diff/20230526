# Comparing `tmp/install_release-0.3.3.tar.gz` & `tmp/install_release-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install_release-0.3.3.tar", max compression
+gzip compressed data, was "install_release-0.3.4.tar", max compression
```

## Comparing `install_release-0.3.3.tar` & `install_release-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      295 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/Makefile
--rw-r--r--   0        0        0       22 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/__init__.py
--rw-r--r--   0        0        0     5070 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/cli.py
--rw-r--r--   0        0        0     8560 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/cli_interact.py
--rw-r--r--   0        0        0     1288 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/constants.py
--rw-r--r--   0        0        0     7226 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/core.py
--rw-r--r--   0        0        0     2221 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/data.py
--rw-r--r--   0        0        0     2285 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/state.py
--rw-r--r--   0        0        0     7351 2023-04-15 11:36:21.006124 install_release-0.3.3/InstallRelease/utils.py
--rw-r--r--   0        0        0    35149 2023-04-15 11:36:21.006124 install_release-0.3.3/LICENSE
--rw-r--r--   0        0        0     8430 2023-04-15 11:36:21.006124 install_release-0.3.3/README.md
--rw-r--r--   0        0        0      927 2023-04-15 11:36:21.006124 install_release-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 install_release-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      295 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/Makefile
+-rw-r--r--   0        0        0       22 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/__init__.py
+-rw-r--r--   0        0        0     5070 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/cli.py
+-rw-r--r--   0        0        0     9143 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/cli_interact.py
+-rw-r--r--   0        0        0     1288 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/constants.py
+-rw-r--r--   0        0        0     7473 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/core.py
+-rw-r--r--   0        0        0     2221 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/data.py
+-rw-r--r--   0        0        0     2285 2023-05-26 06:56:39.230911 install_release-0.3.4/InstallRelease/state.py
+-rw-r--r--   0        0        0     7351 2023-05-26 06:56:39.234911 install_release-0.3.4/InstallRelease/utils.py
+-rw-r--r--   0        0        0    35149 2023-05-26 06:56:39.234911 install_release-0.3.4/LICENSE
+-rw-r--r--   0        0        0     8430 2023-05-26 06:56:39.234911 install_release-0.3.4/README.md
+-rw-r--r--   0        0        0      927 2023-05-26 06:56:39.234911 install_release-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 install_release-0.3.4/PKG-INFO
```

### Comparing `install_release-0.3.3/InstallRelease/cli.py` & `install_release-0.3.4/InstallRelease/cli.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.3/InstallRelease/cli_interact.py` & `install_release-0.3.4/InstallRelease/cli_interact.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from typing import Dict
 from tempfile import TemporaryDirectory
+import platform
 
 # pipi
 import requests
 from rich.progress import track
 from rich.console import Console
 
 # locals
@@ -38,14 +39,17 @@
 cache_config = State(
     file_path=platform_path(paths=config_path, alt=__spath["config_path"]),
     obj=ToolConfig,
 )
 
 
 def load_config():
+    """
+    Load config from cache_config
+    """
     config: ToolConfig = cache_config.state.get("config")
 
     if config != None:
         return config
     else:
         cache_config.set("config", ToolConfig())
         cache_config.save()
@@ -68,16 +72,27 @@
 def get(
     repo: GithubInfo,
     tag_name: str = "",
     local: bool = True,
     prompt: bool = False,
     name: str = None,
 ):
+    """
+    | Get a release from a github repository
+    """
     state_info()
 
+    logger.debug(f"Python version: {platform.python_version()}")
+    logger.debug(f"Platform: {platform.platform()}")
+    try:
+        logger.debug(f"Platform version: {platform.version()}")
+        logger.debug(f"Platform release: {platform.release()}")
+    except:
+        ...
+
     releases = repo.release(tag_name=tag_name, pre_release=config.pre_release)
 
     if not len(releases) > 0:
         logger.error(f"No releases found: {repo.repo_url}")
         return
 
     if isNone(name):
@@ -134,14 +149,17 @@
     #     releases[0].hold_update = True
 
     cache.set(f"{repo.repo_url}#{toolname}", value=releases[0])
     cache.save()
 
 
 def upgrade(force: bool = False):
+    """
+    | Upgrade all tools
+    """
     state_info()
 
     state: TypeState = cache.state
 
     upgrades: Dict[str, GithubInfo] = {}
 
     def task(k: str):
@@ -185,23 +203,29 @@
             f"Updating: {name}, {state[k].tag_name} => {releases[0].tag_name}"
             "[/]"
         )
         get(repo, prompt=False, name=name)
 
 
 def show_state():
+    """
+    | Show state of all tools
+    """
     state_info()
     if os.path.exists(cache.state_file) and os.path.isfile(cache.state_file):
         with open(cache.state_file) as f:
             print(f.read())
 
 
 def list_install(
     state: TypeState = None, title: str = "Installed tools", hold_update=False
 ):
+    """
+    | List all installed tools
+    """
     if state == None:
         state_info()
         state = cache.state
 
     _table = []
     _hold_table = []
     for key in state:
@@ -228,14 +252,17 @@
     if hold_update:
         show_table(_hold_table, title=f"{title} kept on hold")
     else:
         show_table(_table, title=title)
 
 
 def remove(name: str):
+    """
+    | Remove any cli tool.
+    """
     state_info()
     state: TypeState = cache.state
     popKey = ""
 
     for key in state:
         i = irKey(key)
         if i.name == name:
```

### Comparing `install_release-0.3.3/InstallRelease/constants.py` & `install_release-0.3.4/InstallRelease/constants.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.3/InstallRelease/core.py` & `install_release-0.3.4/InstallRelease/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,14 +104,18 @@
                 for r in req
             ]
 
         return self.response
 
 
 class installRelease:
+    """
+    Install a release from github
+    """
+
     USER: str
     SUDO_USER: str
 
     bin_path = {
         "linux": {"local": f"{HOME}/.local/bin", "global": "/usr/local/bin"},
         "darwin": {"local": f"{HOME}/.local/bin", "global": "/usr/local/bin"},
     }
@@ -156,14 +160,17 @@
         self._install_linux(local, at)
 
     def _install_windows(self, local: bool, at: str = None):
         ...
 
 
 def get_release(releases: List[GithubRelease], repo_url: str, extra_words: list = []):
+    """
+    Get the release with the highest priority
+    """
     selected = 0.0
     name = ""
 
     # temp fix: install not configured for distro based on platform
     platform_words = _platform_words + ["(.tar|.zip)"]
 
     logger.debug(msg=("platform_words: ", platform_words))
@@ -213,14 +220,17 @@
             f"Final Selected item has low probability"
             f"Object: {item.name}, content_type: {item.content_type}, chances: {selected}"
         )
     return item
 
 
 def extract_release(item: GithubReleaseAssets, at):
+    """
+    Download and extract release
+    """
     logger.debug(f"Download path: {at}")
 
     path = download(item.browser_download_url, at)
     logger.debug(f"path: {path}")
 
     logger.debug(f"Extracting: {path}")
     if not re.match(
@@ -229,14 +239,17 @@
         extract(path=path, at=at)
         logger.debug("Extracting done.")
 
     return True
 
 
 def install_bin(src: str, dest: str, local: bool, name: str = None):
+    """
+    Install single binary executable file from source to destination
+    """
     bin_files = []
 
     for file in glob.iglob(f"{src}/**", recursive=True):
         f = detect_from_filename(file)
         if f.name == "directory":
             continue
         elif not re.match(pattern=__exec_pattern, string=f.mime_type):
```

### Comparing `install_release-0.3.3/InstallRelease/data.py` & `install_release-0.3.4/InstallRelease/data.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.3/InstallRelease/state.py` & `install_release-0.3.4/InstallRelease/state.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.3/InstallRelease/utils.py` & `install_release-0.3.4/InstallRelease/utils.py`

 * *Files identical despite different names*

### Comparing `install_release-0.3.3/LICENSE` & `install_release-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `install_release-0.3.3/README.md` & `install_release-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `install_release-0.3.3/pyproject.toml` & `install_release-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [virtualenvs]
 in-project = true
 
 [tool.poetry]
 name = "install-release"
-version = "0.3.3"
+version = "0.3.4"
 readme = "README.md"
 description = "A cli tool to install tools based on your device info directly from github releases and keep them updated."
 authors = ["Rishang <rishangbhavsarcs@gmail.com>"]
 packages = [
   { include = "InstallRelease" }
 ]
 homepage = "https://github.com/Rishang/install-releases"
```

### Comparing `install_release-0.3.3/PKG-INFO` & `install_release-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-release
-Version: 0.3.3
+Version: 0.3.4
 Summary: A cli tool to install tools based on your device info directly from github releases and keep them updated.
 Home-page: https://github.com/Rishang/install-releases
 Author: Rishang
 Author-email: rishangbhavsarcs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


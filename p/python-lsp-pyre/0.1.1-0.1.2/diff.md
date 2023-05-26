# Comparing `tmp/python_lsp_pyre-0.1.1.tar.gz` & `tmp/python_lsp_pyre-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_lsp_pyre-0.1.1.tar", max compression
+gzip compressed data, was "python_lsp_pyre-0.1.2.tar", max compression
```

## Comparing `python_lsp_pyre-0.1.1.tar` & `python_lsp_pyre-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2235 2023-05-24 17:38:00.656313 python_lsp_pyre-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-24 17:38:00.656313 python_lsp_pyre-0.1.1/pylsp_pyre/__init__.py
--rw-r--r--   0        0        0     5134 2023-05-24 17:38:00.656313 python_lsp_pyre-0.1.1/pylsp_pyre/plugin.py
--rw-r--r--   0        0        0      730 2023-05-24 17:38:00.656313 python_lsp_pyre-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 python_lsp_pyre-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2800 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/pylsp_pyre/__init__.py
+-rw-r--r--   0        0        0     5701 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/pylsp_pyre/plugin.py
+-rw-r--r--   0        0        0      730 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3390 1970-01-01 00:00:00.000000 python_lsp_pyre-0.1.2/PKG-INFO
```

### Comparing `python_lsp_pyre-0.1.1/README.md` & `python_lsp_pyre-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # python-lsp-pyre
 
-Implements support for calling Meta's [Pyre type checker](https://github.com/facebook/pyre-check) via a subprocess.
-
 This is a plugin for the [Python LSP Server](https://github.com/python-lsp/python-lsp-server).
 
-It was written to scratch an itch, so may not be quite what you're looking for.
+It implements support for calling Meta's [Pyre type checker](https://github.com/facebook/pyre-check) via a subprocess.
 
 ## Installation
 
 To use this plugin, you need to install this plugin in the same virtualenv as `python-lsp-server` itself.
 
 ```bash
 pip install python-lsp-pyre
@@ -16,24 +14,25 @@
 
 or to make it a development requirement in Poetry
 
 ```bash
 poetry add -G dev python-lsp-pyre
 ```
 
-Then run `python-lsp-server` as usual, the plugin will be auto-discovered by
-`python-lsp-server` if you've installed it to the right environment. Refer to
-`python-lsp-server` and your IDE/text editor documentation on how to setup
-`python-lsp-server`. An example is provided for KDE's [Kate editor](/docs/kate.md).
+Then run `python-lsp-server` as usual, the plugin will be auto-discovered by `python-lsp-server` if you've installed it to the right environment. Refer to `python-lsp-server` and your IDE/text editor documentation on how to setup `python-lsp-server`. The plugin's default `enabled` status is `True`.
+
+## Editor integration
+
+* An example is provided for KDE's [Kate editor](/docs/kate.md)
 
 ## Configuration
 
 Meta's Pyre uses `.pyre_configuration` files in your project to set up lint controls. It does not read `pyproject.toml`.
 
-On first run of this plugin, it will detect a missing `.pyre_configuration`, and write out one for you. It relies on the workspace root passed to the language server for this write. This file is not immutable, and the [reference documentation](https://pyre-check.org/docs/configuration/) may be useful.
+On first run of this plugin, it will detect a missing `.pyre_configuration` and write out one for you if the `create-pyre-config` [configuration](docs/Configuration.md) option is enabled. It relies on the workspace root passed to the language server for this write. This file is not immutable, and the [reference documentation](https://pyre-check.org/docs/configuration/) may be useful.
 
 You can also use `pyre init` instead to set up the configuration.
 
 The configuration written by this plugin is:
 
 ```json
 {
@@ -46,29 +45,40 @@
         ".*/build/.*"
     ]
 }
 ```
 
 The noteable difference from `pyre init` is the change to the search strategy (pep561 to all).
 
+If the file is not present, the LSP error log, LSP output, and your editor's LSP messages will display an ABEND message containing the error from Pyre as it fails to run.
+
 ## Features
 
-This plugin adds the following features to `pylsp`:
+This plugin adds the following features to `python-lsp-server`:
 
 - Type linting via Meta's Pyre (pyre-check)
 
 ## Developing
 
 Install development dependencies with (you might want to create a virtualenv first):
 
 ```bash
 git clone https://github.com/cricalix/python-lsp-pyre python-lsp-pyre
 cd python-lsp-pyre
 pip install -e '.[dev]'
 ```
 
 Alterately, if you use Poetry,
-```
+
+```bash
+git clone https://github.com/cricalix/python-lsp-pyre python-lsp-pyre
+cd python-lsp-pyre
 poetry install
 ```
 
 will set up a virtualenv if necessary, install all dependencies, and then install this project in editable/development mode.
+
+## Contributing
+
+This plugin was written to scratch an itch. If you find it useful, great!
+
+If something about it annoys you, or you think there's a better way to do something, you're welcome to send a PR.
```

### Comparing `python_lsp_pyre-0.1.1/pylsp_pyre/plugin.py` & `python_lsp_pyre-0.1.2/pylsp_pyre/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,76 +2,52 @@
 import logging
 import subprocess
 from pathlib import Path
 from typing import Any, Dict, List
 
 import lsprotocol.converters as lsp_con
 import lsprotocol.types as lsp_types
+import pylsp.config.config as pylsp_conf
 import pylsp.lsp as pylsp_lsp
 import pylsp.workspace as pylsp_ws
 import pyre_check.client.language_server.protocol as pyre_proto
 from pylsp import hookimpl
-from pylsp.config.config import Config
 
 logger: logging.Logger = logging.getLogger(__name__)
+# A logging prefix.
+PLUGIN: str = "[python-lsp-pyre]"
 
 
 @hookimpl
-def pylsp_settings() -> Dict[str, Dict[str, Dict[str, bool]]]:
+def pylsp_settings(config: pylsp_conf.Config) -> Dict[str, Dict[str, Dict[str, bool]]]:
+    """
+    Default configuration for the plugin. Ensures all keys are set.
+    """
     return {
         "plugins": {
             "pyre": {
                 "enabled": True,
-                "auto-config": True,
+                "create-pyre-config": False,
             }
         }
     }
 
 
 @hookimpl
-def pylsp_initialize(config: Config, workspace: pylsp_ws.Workspace) -> None:
-    """
-    Checks for a Pyre configuration existence.
-
-    Runs on plugin init, relies on the workspace document root to know where to look for
-    the config file.
-    """
-    default_config = json.loads(
-        """
-        {
-      "site_package_search_strategy": "all",
-      "source_directories": [
-        "."
-      ],
-      "exclude": [
-        "\/setup.py",
-        ".*\/build\/.*"
-      ]
-    }
-    """
-    )
-    settings = config.plugin_settings("pyre")
-    if settings["auto-config"]:
-        docroot = workspace.root_path
-        path = Path(docroot).joinpath(".pyre_configuration")
-        if not path.exists():
-            logger.info(f"Initializing {path}")
-            with path.open(mode="w") as f:
-                f.write(json.dumps(default_config, indent=4))
-                f.write("\n")
-
-
-@hookimpl
 def pylsp_lint(
-    config: Config, workspace: pylsp_ws.Workspace, document: pylsp_ws.Document, is_saved: bool
+    config: pylsp_conf.Config,
+    workspace: pylsp_ws.Workspace,
+    document: pylsp_ws.Document,
+    is_saved: bool,
 ) -> List[Dict[str, Any]]:
     """
     Lints files (saved, not in-progress) and returns found problems.
     """
     logger.debug(f"Working with {document.path}, {is_saved=}")
+    maybe_create_pyre_config(config=config, workspace=workspace)
     if is_saved:
         with workspace.report_progress("lint: pyre check", "running"):
             settings = config.plugin_settings("pyre")
             diagnostics = run_pyre(workspace=workspace, document=document, settings=settings)
         workspace.show_message(message=f"Pyre reported {len(diagnostics)} issue(s).")
         # Deal with location stuff by using unstructure() for now.
         return lsp_con.get_converter().unstructure(diagnostics)
@@ -82,16 +58,18 @@
 def abend(message: str, workspace: pylsp_ws.Workspace) -> Dict[str, Any]:
     """
     Deals with exceptions that Pyre might throw via subprocess.
 
     Basically, make it visible in as many ways as possible - logging, workspace messaging, and
     actual lint results.
     """
-    logger.exception(message)
-    workspace.show_message(message=message, msg_type=pylsp_lsp.MessageType.Error)
+    logger.exception(f"{PLUGIN} {message}")
+    workspace.show_message(
+        message=f"{PLUGIN} {message}", msg_type=pylsp_lsp.MessageType.Error
+    )
     return {
         "source": "pyre",
         "severity": lsp_types.DiagnosticSeverity.Error,
         "code": "E999",
         "message": message,
         "range": pyre_proto.LspRange(
             start=pyre_proto.LspPosition(line=0, character=0),
@@ -152,7 +130,46 @@
     except subprocess.CalledProcessError as e:
         # If there are no typing errors, pyre exits with returncode 0
         # If there are typing errors, pyre exits with returncode 1
         # If there are configuration errors, pyre exits with returncode 6
         if e.returncode in (0, 1):
             return e.output
         raise
+
+
+def maybe_create_pyre_config(
+    config: pylsp_conf.Config, workspace: pylsp_ws.Workspace
+) -> None:
+    """
+    Initializes a .pyre_configuration file if `create-pyre-config` setting is enabled.
+
+    Only initializes if the file is missing.
+    """
+    default_config = json.loads(
+        """
+        {
+      "site_package_search_strategy": "all",
+      "source_directories": [
+        "."
+      ],
+      "exclude": [
+        "\/setup.py",
+        ".*\/build\/.*"
+      ]
+    }
+    """
+    )
+    settings = config.plugin_settings("pyre")
+    try:
+        if settings["create-pyre-config"]:
+            docroot = workspace.root_path
+            path = Path(docroot).joinpath(".pyre_configuration")
+            if not path.exists():
+                logger.info(f"Initializing {path}")
+                with path.open(mode="w") as f:
+                    f.write(json.dumps(default_config, indent=4))
+                    f.write("\n")
+
+    except KeyError:
+        message = f"{PLUGIN} create-pyre-config setting not found in dictionary"
+        logger.exception(message)
+        workspace.show_message(message=message, msg_type=pylsp_lsp.MessageType.Warning)
```

### Comparing `python_lsp_pyre-0.1.1/pyproject.toml` & `python_lsp_pyre-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-lsp-pyre"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pyre linting plugin for pylsp"
 authors = ["Duncan Hill <python.projects@cricalix.net>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pylsp_pyre"}]
 
 [tool.poetry.dependencies]
```

### Comparing `python_lsp_pyre-0.1.1/PKG-INFO` & `python_lsp_pyre-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-pyre
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pyre linting plugin for pylsp
 License: MIT
 Author: Duncan Hill
 Author-email: python.projects@cricalix.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,19 +13,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyre-check (>=0.9.18,<0.10.0)
 Requires-Dist: python-lsp-server (>=1.7.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # python-lsp-pyre
 
-Implements support for calling Meta's [Pyre type checker](https://github.com/facebook/pyre-check) via a subprocess.
-
 This is a plugin for the [Python LSP Server](https://github.com/python-lsp/python-lsp-server).
 
-It was written to scratch an itch, so may not be quite what you're looking for.
+It implements support for calling Meta's [Pyre type checker](https://github.com/facebook/pyre-check) via a subprocess.
 
 ## Installation
 
 To use this plugin, you need to install this plugin in the same virtualenv as `python-lsp-server` itself.
 
 ```bash
 pip install python-lsp-pyre
@@ -33,24 +31,25 @@
 
 or to make it a development requirement in Poetry
 
 ```bash
 poetry add -G dev python-lsp-pyre
 ```
 
-Then run `python-lsp-server` as usual, the plugin will be auto-discovered by
-`python-lsp-server` if you've installed it to the right environment. Refer to
-`python-lsp-server` and your IDE/text editor documentation on how to setup
-`python-lsp-server`. An example is provided for KDE's [Kate editor](/docs/kate.md).
+Then run `python-lsp-server` as usual, the plugin will be auto-discovered by `python-lsp-server` if you've installed it to the right environment. Refer to `python-lsp-server` and your IDE/text editor documentation on how to setup `python-lsp-server`. The plugin's default `enabled` status is `True`.
+
+## Editor integration
+
+* An example is provided for KDE's [Kate editor](/docs/kate.md)
 
 ## Configuration
 
 Meta's Pyre uses `.pyre_configuration` files in your project to set up lint controls. It does not read `pyproject.toml`.
 
-On first run of this plugin, it will detect a missing `.pyre_configuration`, and write out one for you. It relies on the workspace root passed to the language server for this write. This file is not immutable, and the [reference documentation](https://pyre-check.org/docs/configuration/) may be useful.
+On first run of this plugin, it will detect a missing `.pyre_configuration` and write out one for you if the `create-pyre-config` [configuration](docs/Configuration.md) option is enabled. It relies on the workspace root passed to the language server for this write. This file is not immutable, and the [reference documentation](https://pyre-check.org/docs/configuration/) may be useful.
 
 You can also use `pyre init` instead to set up the configuration.
 
 The configuration written by this plugin is:
 
 ```json
 {
@@ -63,30 +62,41 @@
         ".*/build/.*"
     ]
 }
 ```
 
 The noteable difference from `pyre init` is the change to the search strategy (pep561 to all).
 
+If the file is not present, the LSP error log, LSP output, and your editor's LSP messages will display an ABEND message containing the error from Pyre as it fails to run.
+
 ## Features
 
-This plugin adds the following features to `pylsp`:
+This plugin adds the following features to `python-lsp-server`:
 
 - Type linting via Meta's Pyre (pyre-check)
 
 ## Developing
 
 Install development dependencies with (you might want to create a virtualenv first):
 
 ```bash
 git clone https://github.com/cricalix/python-lsp-pyre python-lsp-pyre
 cd python-lsp-pyre
 pip install -e '.[dev]'
 ```
 
 Alterately, if you use Poetry,
-```
+
+```bash
+git clone https://github.com/cricalix/python-lsp-pyre python-lsp-pyre
+cd python-lsp-pyre
 poetry install
 ```
 
 will set up a virtualenv if necessary, install all dependencies, and then install this project in editable/development mode.
 
+## Contributing
+
+This plugin was written to scratch an itch. If you find it useful, great!
+
+If something about it annoys you, or you think there's a better way to do something, you're welcome to send a PR.
+
```


# Comparing `tmp/archimedes_config-0.3.2.tar.gz` & `tmp/archimedes_config-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archimedes_config-0.3.2.tar", max compression
+gzip compressed data, was "archimedes_config-0.3.3.tar", max compression
```

## Comparing `archimedes_config-0.3.2.tar` & `archimedes_config-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      238 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/__init__.py
--rw-r--r--   0        0        0     8543 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/arckeyl.py
--rw-r--r--   0        0        0    13575 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/config_manager.py
--rw-r--r--   0        0        0     2527 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/keyvault_client.py
--rw-r--r--   0        0        0     1242 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/keyvault_config_manager.py
--rw-r--r--   0        0        0     1613 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/utils/path_utils.py
--rw-r--r--   0        0        0     3898 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/utils/util.py
--rw-r--r--   0        0        0      673 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/add_secrets.py
--rw-r--r--   0        0        0      965 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/lock_secrets.py
--rw-r--r--   0        0        0     2127 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/secret_creation.py
--rw-r--r--   0        0        0      944 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/unlock_secrets.py
--rw-r--r--   0        0        0     4126 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/archimedes_config/workflows/workflow_base.py
--rw-r--r--   0        0        0      753 2023-05-24 11:51:36.132879 archimedes_config-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      238 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/__init__.py
+-rw-r--r--   0        0        0     9478 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/arckeyl.py
+-rw-r--r--   0        0        0    13575 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/config_manager.py
+-rw-r--r--   0        0        0     2527 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/keyvault_client.py
+-rw-r--r--   0        0        0     1242 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/keyvault_config_manager.py
+-rw-r--r--   0        0        0     1613 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/utils/path_utils.py
+-rw-r--r--   0        0        0     3898 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/utils/util.py
+-rw-r--r--   0        0        0      673 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/workflows/add_secrets.py
+-rw-r--r--   0        0        0      737 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/workflows/extract_secret.py
+-rw-r--r--   0        0        0      965 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/workflows/lock_secrets.py
+-rw-r--r--   0        0        0     2127 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/workflows/secret_creation.py
+-rw-r--r--   0        0        0      944 2023-05-26 12:22:04.728901 archimedes_config-0.3.3/archimedes_config/workflows/unlock_secrets.py
+-rw-r--r--   0        0        0     4126 2023-05-26 12:22:04.732901 archimedes_config-0.3.3/archimedes_config/workflows/workflow_base.py
+-rw-r--r--   0        0        0      753 2023-05-26 12:22:04.732901 archimedes_config-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 archimedes_config-0.3.3/PKG-INFO
```

### Comparing `archimedes_config-0.3.2/archimedes_config/arckeyl.py` & `archimedes_config-0.3.3/archimedes_config/arckeyl.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     get_registered_configs,
     get_secret,
     register_config,
     register_secret,
     unregister_config,
 )
 from archimedes_config.workflows.add_secrets import AddSecret
+from archimedes_config.workflows.extract_secret import ExtractSecret
 from archimedes_config.workflows.lock_secrets import LockConfig
 from archimedes_config.workflows.secret_creation import ConfigCreator
 from archimedes_config.workflows.unlock_secrets import UnlockConfig
 
 ROOT_PATH = find_repo_root()
 
 PRE_COMMIT_CHECK_FILE_NAME = f".{COMMAND_NAME}_config"
@@ -40,14 +41,16 @@
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 def cli():
     """
     Welcome to The Archimedes Config Manager.
 
     \b
     Commands:
+        {COMMAND_NAME} list        Lists all registered config.
+        {COMMAND_NAME} extract-secret        Extracts a single secret from config.
         {COMMAND_NAME} new        Create a new config.
         {COMMAND_NAME} add        Add new keys to an existing config.
         {COMMAND_NAME} lock       Locks an existing config.
         {COMMAND_NAME} unlock     Unlocks an existing config.
         {COMMAND_NAME} check      Ensures all registered configs are encrypted.
         {COMMAND_NAME} register      Register config to pre-commit hook.
         {COMMAND_NAME} unregister   Unregister config from pre-commit hook
@@ -142,14 +145,38 @@
         )
     except:  # pylint:disable=bare-except
         print(
             f"Please make sure that the pre commit file located in `{pre_commit_path}` is executable."
         )
 
 
+@cli.command("list")
+def list_configs():
+    """Lists all registered config."""
+    with open(PRE_COMMIT_CHECK_FILE_NAME, encoding="utf8") as file:
+        configs = tomlkit.load(file)["registered_configs"]
+    print("\n".join([f"{idx+1}. {i}" for idx, i in enumerate(configs)]))
+
+
+@cli.command("extract-secret")
+@click.argument("file_name")
+@click.argument("group")
+@click.argument("key_name")
+@clean_filename
+def extract_secret(file_name, group, key_name):
+    """Extracts a single secret from the config file"""
+    extracted_secret = ExtractSecret().get_secret(
+        file_name,
+        group,
+        key_name,
+        get_secret(file_name, SECRET_PATH, default_return=None),
+    )
+    print(extracted_secret)
+
+
 @cli.command("add")
 @click.argument("file_name")
 @clean_filename
 def add(file_name):
     """Add a secret to the config"""
     secret = get_secret(file_name, SECRET_PATH, default_return=None)
     AddSecret().interactive(file_name, secret)
```

### Comparing `archimedes_config-0.3.2/archimedes_config/config_manager.py` & `archimedes_config-0.3.3/archimedes_config/config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/keyvault_client.py` & `archimedes_config-0.3.3/archimedes_config/keyvault_client.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/keyvault_config_manager.py` & `archimedes_config-0.3.3/archimedes_config/keyvault_config_manager.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/utils/path_utils.py` & `archimedes_config-0.3.3/archimedes_config/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/utils/util.py` & `archimedes_config-0.3.3/archimedes_config/utils/util.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/workflows/add_secrets.py` & `archimedes_config-0.3.3/archimedes_config/workflows/add_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/workflows/lock_secrets.py` & `archimedes_config-0.3.3/archimedes_config/workflows/lock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/workflows/secret_creation.py` & `archimedes_config-0.3.3/archimedes_config/workflows/secret_creation.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/workflows/unlock_secrets.py` & `archimedes_config-0.3.3/archimedes_config/workflows/unlock_secrets.py`

 * *Files identical despite different names*

### Comparing `archimedes_config-0.3.2/archimedes_config/workflows/workflow_base.py` & `archimedes_config-0.3.3/archimedes_config/workflows/workflow_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         try:
             self.conf = KeyvaultConfigManager()
         except ImportError:
             self.conf = ConfigManager()
 
     def config_has_remote_conn_parameters(self):
         """
-        Checks if config can accesss reote key vault
+        Checks if config can access remote key vault
         """
         try:
             self.conf.get("AZURE_KEYVAULT", "VAULT_NAME")
             self.conf.get("AZURE_KEYVAULT", "VAULT_KEY")
         except KeyError:
             return False
         if hasattr(self.conf, "set_default_key_from_key_vault"):
```

### Comparing `archimedes_config-0.3.2/pyproject.toml` & `archimedes_config-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archimedes-config"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["BigyaPradhan <bigya.pradhan@optimeering.com>"]
 packages = [{include = "archimedes_config"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 cryptography = "^39.0.1"
```

### Comparing `archimedes_config-0.3.2/PKG-INFO` & `archimedes_config-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archimedes-config
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Author: BigyaPradhan
 Author-email: bigya.pradhan@optimeering.com
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


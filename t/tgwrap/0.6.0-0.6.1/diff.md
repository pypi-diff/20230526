# Comparing `tmp/tgwrap-0.6.0.tar.gz` & `tmp/tgwrap-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.6.0.tar", max compression
+gzip compressed data, was "tgwrap-0.6.1.tar", max compression
```

## Comparing `tgwrap-0.6.0.tar` & `tgwrap-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.6.0/LICENSE
--rw-r--r--   0        0        0     6530 2023-05-02 09:53:07.369821 tgwrap-0.6.0/README.md
--rw-r--r--   0        0        0      902 2023-05-26 12:32:33.841195 tgwrap-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.6.0/tgwrap/__init__.py
--rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.6.0/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    25931 2023-05-26 12:32:25.246216 tgwrap-0.6.0/tgwrap/cli.py
--rwxr-xr-x   0        0        0    55993 2023-05-26 12:32:25.246843 tgwrap-0.6.0/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.6.0/tgwrap/printer.py
--rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 tgwrap-0.6.0/setup.py
--rw-r--r--   0        0        0     7613 1970-01-01 00:00:00.000000 tgwrap-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.6.1/LICENSE
+-rw-r--r--   0        0        0     7169 2023-05-26 12:45:31.451829 tgwrap-0.6.1/README.md
+-rw-r--r--   0        0        0      902 2023-05-26 13:27:35.357719 tgwrap-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.6.1/tgwrap/__init__.py
+-rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.6.1/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    25922 2023-05-26 13:18:56.546086 tgwrap-0.6.1/tgwrap/cli.py
+-rwxr-xr-x   0        0        0    56420 2023-05-26 13:25:59.444024 tgwrap-0.6.1/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.6.1/tgwrap/printer.py
+-rw-r--r--   0        0        0     8321 1970-01-01 00:00:00.000000 tgwrap-0.6.1/setup.py
+-rw-r--r--   0        0        0     8252 1970-01-01 00:00:00.000000 tgwrap-0.6.1/PKG-INFO
```

### Comparing `tgwrap-0.6.0/LICENSE` & `tgwrap-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.0/README.md` & `tgwrap-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,37 +34,57 @@
 
 So we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.
 
 And this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we're at it, replacing the aliases with this was then pretty straightforward next step as well.
 
 ## 4. Analyzing plan files
 
-When using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.
+When using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.
 
-It would provide output as follows:
+It needs a config file as follows:
 
-```console
-$ tgwrap analyze -x
-
-...
-
-Analyse project: inputs
-Run terrasafe: inputs
-Config loaded from /my/project/dir/terrasafe-config.json
-0 unauthorized deletion detected
-
-Analyse project: runners
-Changes:
-module.vmss.azurerm_key_vault_secret.pwd: delete,create
-module.vmss.azurerm_key_vault_secret.user: delete,create
-module.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update
-
-Run terrasafe: runners
-Config loaded from /my/project/dir/terrasafe-config.json
-0 unauthorized deletion detected
+```yaml
+---
+#
+# Critically of resources as interpreted by 'tgwrap analyze'.
+# It uses it for a 'terrasafe' like validation if resources can safely be deleted.
+# On top of that it tries to analyze and quantify the drift impact of the changes,
+# so that this can be monitored.
+#
+low:
+  # defaults:
+  #   terrasafe_level: ignore_deletions
+  #   drift_impact:
+  #     default: minor
+  #     delete: medium
+  azuread_application.: {} # if we you want to use the defaults
+  azuread_app_role_assignment: # or if you want to override these
+    drift_impact:
+      delete: minor
+  # and so on, and so forth
+medium:
+  # defaults:
+  #   terrasafe_level: ignore_deletion_if_recreation
+  #   drift_impact:
+  #     default: medium
+  #     delete: major
+  azurerm_data_factory_linked_service_key_vault.: {}
+  # and so on, and so forth
+high:
+  # defaults:
+  #   terrasafe_level: unauthorized_deletion
+  #   drift_impact:
+  #     default: major
+  #     update: medium
+  azuread_group.:
+    drift_impact:
+      create: minor
+      update: minor
+  azurerm_application_insights.: {}
+  # and so on, and so forth
 ```
 
 ## Usage
 
 ```console
 # general help
 tgwrap --help
```

### Comparing `tgwrap-0.6.0/pyproject.toml` & `tgwrap-0.6.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.6.0"
+version = "0.6.1"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.6.0/tgwrap/analyze.py` & `tgwrap-0.6.1/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.0/tgwrap/cli.py` & `tgwrap-0.6.1/tgwrap/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,15 +627,15 @@
         include_global_config_files=include_global_config_files,
         auto_approve=auto_approve,
         dry_run=dry_run,
         working_dir=working_dir,
     )
 
 @main.command(
-    name="check-deployed-versions",
+    name="check-deployments",
     context_settings=dict(
         ignore_unknown_options=True,
     ),
 )
 @click.option('--manifest-file', '-m',
     help='Manifest file describing the deployment options',
     required=True, default="manifest.yaml", show_default=True,
@@ -648,21 +648,21 @@
     help='Working directory, when omitted the current directory is used',
     )
 @click.option('--out', '-o', is_flag=True, default=False,
     help='Show output as json',
     show_default=True
     )
 @click.version_option(version=__version__)
-def check_deployed_versions(manifest_file, verbose, working_dir, out):
-    """ Check the freshness of deployed versions against the configured platform file """
+def check_deployments(manifest_file, verbose, working_dir, out):
+    """ Check the freshness of deployed configuration versions against the platform repository """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
-    tgwrap.check_deployed_versions(
+    tgwrap.check_deployments(
         manifest_file=manifest_file,
         working_dir=working_dir,
         out=out,
     )
 
 @main.command(
     name="show-graph",
```

### Comparing `tgwrap-0.6.0/tgwrap/main.py` & `tgwrap-0.6.1/tgwrap/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1098,15 +1098,17 @@
             sys.exit(1)
         finally:
             try:
                 shutil.rmtree(temp_dir)
             except Exception:
                 pass
 
-    def check_deployed_versions(self, manifest_file, working_dir, out):
+    def check_deployments(self, manifest_file, working_dir, out):
+        """ Check the freshness of deployed configuration versions against the platform repository """
+
         def locate_version_files(current_directory, found_files=[], root_directory=None, level=1):
             " This tries to find a version file in the current directory, or a given number of directories beneath it"
 
             if not root_directory:
                 root_directory = current_directory
 
             for entry in os.listdir(current_directory):
@@ -1218,14 +1220,22 @@
                 elif days_since_release > 30:
                     self.printer.error(message)
                 elif days_since_release < 7:
                     self.printer.success(message)
                 else:
                     self.printer.normal(message)
 
+            self.printer.warning("""
+Note:
+    This result only says something about the freshness of the deployed configurations,
+    but not whether the actual resources are in sync with these.
+    Check the drift of these configurations with the actual deployments by
+    planning and analyzing the results.
+            """)
+
             if out:
                 print(json.dumps(versions, indent=4, cls=DateTimeEncoder))
     
         except KeyError as e:
             self.printer.error(f'Error interpreting the manifest file. Please ensure it uses the proper format. Could not find element: {e}')
             if self.printer.print_verbose:
                 raise(e)
```

### Comparing `tgwrap-0.6.0/tgwrap/printer.py` & `tgwrap-0.6.1/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.6.0/setup.py` & `tgwrap-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
  'terrasafe>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['tgwrap = tgwrap.cli:main']}
 
 setup_kwargs = {
     'name': 'tgwrap',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
-    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.\n\nIt would provide output as follows:\n\n```console\n$ tgwrap analyze -x\n\n...\n\nAnalyse project: inputs\nRun terrasafe: inputs\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n\nAnalyse project: runners\nChanges:\nmodule.vmss.azurerm_key_vault_secret.pwd: delete,create\nmodule.vmss.azurerm_key_vault_secret.user: delete,create\nmodule.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update\n\nRun terrasafe: runners\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
+    'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.\n\nIt needs a config file as follows:\n\n```yaml\n---\n#\n# Critically of resources as interpreted by \'tgwrap analyze\'.\n# It uses it for a \'terrasafe\' like validation if resources can safely be deleted.\n# On top of that it tries to analyze and quantify the drift impact of the changes,\n# so that this can be monitored.\n#\nlow:\n  # defaults:\n  #   terrasafe_level: ignore_deletions\n  #   drift_impact:\n  #     default: minor\n  #     delete: medium\n  azuread_application.: {} # if we you want to use the defaults\n  azuread_app_role_assignment: # or if you want to override these\n    drift_impact:\n      delete: minor\n  # and so on, and so forth\nmedium:\n  # defaults:\n  #   terrasafe_level: ignore_deletion_if_recreation\n  #   drift_impact:\n  #     default: medium\n  #     delete: major\n  azurerm_data_factory_linked_service_key_vault.: {}\n  # and so on, and so forth\nhigh:\n  # defaults:\n  #   terrasafe_level: unauthorized_deletion\n  #   drift_impact:\n  #     default: major\n  #     update: medium\n  azuread_group.:\n    drift_impact:\n      create: minor\n      update: minor\n  azurerm_application_insights.: {}\n  # and so on, and so forth\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/lunadata/tgwrap',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tgwrap-0.6.0/PKG-INFO` & `tgwrap-0.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.6.0
+Version: 0.6.1
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
@@ -62,37 +62,57 @@
 
 So we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.
 
 And this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we're at it, replacing the aliases with this was then pretty straightforward next step as well.
 
 ## 4. Analyzing plan files
 
-When using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.
+When using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.
 
-It would provide output as follows:
+It needs a config file as follows:
 
-```console
-$ tgwrap analyze -x
-
-...
-
-Analyse project: inputs
-Run terrasafe: inputs
-Config loaded from /my/project/dir/terrasafe-config.json
-0 unauthorized deletion detected
-
-Analyse project: runners
-Changes:
-module.vmss.azurerm_key_vault_secret.pwd: delete,create
-module.vmss.azurerm_key_vault_secret.user: delete,create
-module.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update
-
-Run terrasafe: runners
-Config loaded from /my/project/dir/terrasafe-config.json
-0 unauthorized deletion detected
+```yaml
+---
+#
+# Critically of resources as interpreted by 'tgwrap analyze'.
+# It uses it for a 'terrasafe' like validation if resources can safely be deleted.
+# On top of that it tries to analyze and quantify the drift impact of the changes,
+# so that this can be monitored.
+#
+low:
+  # defaults:
+  #   terrasafe_level: ignore_deletions
+  #   drift_impact:
+  #     default: minor
+  #     delete: medium
+  azuread_application.: {} # if we you want to use the defaults
+  azuread_app_role_assignment: # or if you want to override these
+    drift_impact:
+      delete: minor
+  # and so on, and so forth
+medium:
+  # defaults:
+  #   terrasafe_level: ignore_deletion_if_recreation
+  #   drift_impact:
+  #     default: medium
+  #     delete: major
+  azurerm_data_factory_linked_service_key_vault.: {}
+  # and so on, and so forth
+high:
+  # defaults:
+  #   terrasafe_level: unauthorized_deletion
+  #   drift_impact:
+  #     default: major
+  #     update: medium
+  azuread_group.:
+    drift_impact:
+      create: minor
+      update: minor
+  azurerm_application_insights.: {}
+  # and so on, and so forth
 ```
 
 ## Usage
 
 ```console
 # general help
 tgwrap --help
```


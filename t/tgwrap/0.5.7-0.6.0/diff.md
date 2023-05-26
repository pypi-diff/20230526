# Comparing `tmp/tgwrap-0.5.7.tar.gz` & `tmp/tgwrap-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.5.7.tar", max compression
+gzip compressed data, was "tgwrap-0.6.0.tar", max compression
```

## Comparing `tgwrap-0.5.7.tar` & `tgwrap-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.5.7/LICENSE
--rw-r--r--   0        0        0     6530 2023-05-02 09:53:07.369821 tgwrap-0.5.7/README.md
--rw-r--r--   0        0        0      879 2023-05-12 14:10:45.034048 tgwrap-0.5.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.5.7/tgwrap/__init__.py
--rwxr-xr-x   0        0        0    24647 2023-05-02 09:54:39.822466 tgwrap-0.5.7/tgwrap/cli.py
--rwxr-xr-x   0        0        0    47295 2023-05-12 14:09:50.605033 tgwrap-0.5.7/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.5.7/tgwrap/printer.py
--rw-r--r--   0        0        0     4435 2023-01-17 14:04:36.314955 tgwrap-0.5.7/tgwrap/terrasafe.py
--rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 tgwrap-0.5.7/setup.py
--rw-r--r--   0        0        0     7569 1970-01-01 00:00:00.000000 tgwrap-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6530 2023-05-02 09:53:07.369821 tgwrap-0.6.0/README.md
+-rw-r--r--   0        0        0      902 2023-05-26 12:32:33.841195 tgwrap-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.6.0/tgwrap/__init__.py
+-rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.6.0/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    25931 2023-05-26 12:32:25.246216 tgwrap-0.6.0/tgwrap/cli.py
+-rwxr-xr-x   0        0        0    55993 2023-05-26 12:32:25.246843 tgwrap-0.6.0/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.6.0/tgwrap/printer.py
+-rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 tgwrap-0.6.0/setup.py
+-rw-r--r--   0        0        0     7613 1970-01-01 00:00:00.000000 tgwrap-0.6.0/PKG-INFO
```

### Comparing `tgwrap-0.5.7/LICENSE` & `tgwrap-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.7/README.md` & `tgwrap-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.7/pyproject.toml` & `tgwrap-0.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.5.7"
+version = "0.6.0"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
@@ -16,14 +16,15 @@
 pydot = "^1.4.2"
 networkx = "^2.8.8"
 click = ">= 8.0"
 terrasafe = "^0.5.1"
 outdated = ">= 0.2.2"
 pyhcl = "^0.4.4"
 pyyaml = ">= 6.0"
+python-hcl2 = "^4.3.2"
 
 [tool.poetry.scripts]
 tgwrap = "tgwrap.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.9"
```

### Comparing `tgwrap-0.5.7/tgwrap/cli.py` & `tgwrap-0.6.0/tgwrap/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,34 +132,39 @@
     help='Use the generated planfile when applying the changes',
     show_default=True
     )
 @click.option('--auto-approve', '-a', is_flag=True, default=False,
     help='Do not ask for confirmation before applying planned changes (where applicable)',
     show_default=True
     )
+@click.option('--clean', '-c', is_flag=True, default=False,
+    help='Clean up .terragrunt-cache before executing the command',
+    show_default=True
+    )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def run(command, verbose, debug, dry_run, no_lock, update,
-    planfile, auto_approve, working_dir, terragrunt_args):
+    planfile, auto_approve, clean, working_dir, terragrunt_args):
     """ [default] Executes a terragrunt command on a single project """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.run(
         command=command,
         debug=debug,
         dry_run=dry_run,
         no_lock=no_lock,
         update=update,
         planfile=planfile,
         auto_approve=auto_approve,
+        clean=clean,
         working_dir=working_dir,
         terragrunt_args=terragrunt_args,
     )
 
 @main.command(
     name="run-all",
     context_settings=dict(
@@ -200,14 +205,18 @@
     help='Use the generated planfile when applying the changes',
     show_default=True
     )
 @click.option('--auto-approve', '-a', is_flag=True, default=False,
     help='Do not ask for confirmation before applying planned changes (where applicable)',
     show_default=True
     )
+@click.option('--clean', '-c', is_flag=True, default=False,
+    help='Clean up .terragrunt-cache before executing the command',
+    show_default=True
+    )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
     )
 @click.option('--start-at-step', '-S', type=float, default=1.0,
     help='When running in step-by-step mode, start processing at the given step number',
     )
 @click.option('--limit-parallelism', '-l', type=int, default=None,
@@ -222,15 +231,15 @@
     multiple=True, default=[],
     help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
     show_default=True,
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
 def run_all(command, verbose, debug, dry_run, no_lock, update, exclude_external_dependencies,
-    step_by_step, planfile, auto_approve, working_dir, start_at_step,
+    step_by_step, planfile, auto_approve, clean, working_dir, start_at_step,
     limit_parallelism, include_dir, exclude_dir, terragrunt_args):
     """ Executes a terragrunt command across multiple projects """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.run_all(
@@ -239,14 +248,15 @@
         dry_run=dry_run,
         no_lock=no_lock,
         update=update,
         exclude_external_dependencies=exclude_external_dependencies,
         step_by_step=step_by_step,
         planfile=planfile,
         auto_approve=auto_approve,
+        clean=clean,
         working_dir=working_dir,
         start_at_step=start_at_step,
         limit_parallelism=limit_parallelism,
         include_dir=include_dir,
         exclude_dir=exclude_dir,
         terragrunt_args=terragrunt_args,
     )
@@ -301,18 +311,14 @@
         ignore_unknown_options=True,
     ),
 )
 @click.option('--verbose', '-v', is_flag=True, default=False,
     help='Verbose printing',
     show_default=True
     )
-@click.option('--dry-run', '-D', is_flag=True, default=False,
-    help='dry-run mode, no real actions are executed (only in combination with step-by-step mode)',
-    show_default=True
-    )
 @click.option('--exclude-external-dependencies/--include-external-dependencies', '-x/-i',
     is_flag=True, default=True,
     help='Whether or not external dependencies must be ignored',
     show_default=True
     )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
@@ -320,17 +326,17 @@
 @click.option('--start-at-step', '-S', type=float, default=1.0,
     help='When running in step-by-step mode, start processing at the given step number',
     )
 @click.option('--out', '-o', is_flag=True, default=False,
     help='Show output as json',
     show_default=True
     )
-@click.option('--terrasafe-config', '-T', default=None,
-    help='Name of the terrasafe config file (or set the TERRASAFE_CONFIG environment variable)',
-    envvar='TERRASAFE_CONFIG', type=click.Path(),
+@click.option('--analyze-config', '-A', default=None,
+    help='Name of the analyze config file (or set the TGWRAP_ANALYZE_CONFIG environment variable)',
+    envvar='TGWRAP_ANALYZE_CONFIG', type=click.Path(),
     )
 @click.option('--parallel-execution', '-p', is_flag=True, default=False,
     help='Whether or not to use parallel execution',
     )
 @click.option('--include-dir', '-I',
     multiple=True, default=[],
     help='A glob of a directory that needs to be included, this option can be used multiple times. For example: -I "integrations/\*/\*"',
@@ -339,28 +345,28 @@
 @click.option('--exclude-dir', '-E',
     multiple=True, default=[],
     help='A glob of a directory that needs to be excluded, this option can be used multiple times. For example: -E "integrations/\*/\*"',
     show_default=True,
     )
 @click.argument('terragrunt-args', nargs=-1, type=click.UNPROCESSED)
 @click.version_option(version=__version__)
-def analyze(verbose, dry_run, exclude_external_dependencies, working_dir, start_at_step,
-    out, terrasafe_config, parallel_execution, include_dir, exclude_dir, terragrunt_args):
+def run_analyze(verbose, exclude_external_dependencies, working_dir, start_at_step,
+            out, analyze_config, parallel_execution,
+            include_dir, exclude_dir, terragrunt_args):
     """ Analyzes the plan files """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.analyze(
-        dry_run=dry_run,
         exclude_external_dependencies=exclude_external_dependencies,
         working_dir=working_dir,
         start_at_step=start_at_step,
         out=out,
-        terrasafe_config=terrasafe_config,
+        analyze_config=analyze_config,
         parallel_execution=parallel_execution,
         include_dir=include_dir,
         exclude_dir=exclude_dir,
         terragrunt_args=terragrunt_args,
     )
 
 @main.command(
@@ -462,15 +468,15 @@
 @click.option('--target-stage', '-t',
     type=click.Choice(STAGES, case_sensitive=True),
     help='Target of config files',
     )
 @click.option('--module', '-m', default="",
     help='Name of the module, if omitted all modules will be copied.',
     )
-@click.option('--clean-up', '-c', is_flag=True, default=False,
+@click.option('--clean', '-c', is_flag=True, default=False,
     help='Clean up files on target side that do not exist as source',
     show_default=True
     )
 @click.option('--include-lock-file', '-i', is_flag=True, default=False,
     help='Include the terraform lock file',
     show_default=True
     )
@@ -488,30 +494,30 @@
     )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
     )
 @click.version_option(version=__version__)
 def sync(
     source_domain, source_stage, target_domain, target_stage, module, auto_approve,
-    verbose, dry_run, clean_up, include_lock_file, working_dir
+    verbose, dry_run, clean, include_lock_file, working_dir
     ):
     """ Syncs the terragrunt config files from one stage to another (and possibly to a different domain) """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.sync(
         source_domain=source_domain,
         source_stage=source_stage,
         target_domain=target_domain,
         target_stage=target_stage,
         module=module,
         auto_approve=auto_approve,
         dry_run=dry_run,
-        clean_up=clean_up,
+        clean=clean,
         include_lock_file=include_lock_file,
         working_dir=working_dir,
     )
 
 @main.command(
     name="sync-dir",
     context_settings=dict(
@@ -520,15 +526,15 @@
 )
 @click.option('--source-directory', '-s', required=True,
     help='Directory where source config files reside.',
     )
 @click.option('--target-directory', '-t', required=True,
     help='Directory where config files will be synced to.',
     )
-@click.option('--clean-up', '-c', is_flag=True, default=False,
+@click.option('--clean', '-c', is_flag=True, default=False,
     help='Clean up files on target side that do not exist as source',
     show_default=True
     )
 @click.option('--include-lock-file', '-i', is_flag=True, default=False,
     help='Include the terraform lock file',
     show_default=True
     )
@@ -546,27 +552,27 @@
     )
 @click.option('--working-dir', '-w', default=None,
     help='Working directory, when omitted the current directory is used',
     )
 @click.version_option(version=__version__)
 def sync_dir(
     source_directory, target_directory, auto_approve,
-    verbose, dry_run, clean_up, include_lock_file, working_dir
+    verbose, dry_run, clean, include_lock_file, working_dir
     ):
     """ Syncs the terragrunt config files from one directory to anothery """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.sync_dir(
         source_directory=source_directory,
         target_directory=target_directory,
         auto_approve=auto_approve,
         dry_run=dry_run,
-        clean_up=clean_up,
+        clean=clean,
         include_lock_file=include_lock_file,
         working_dir=working_dir,
     )
 
 @main.command(
     name="deploy",
     context_settings=dict(
@@ -605,15 +611,15 @@
     help='Working directory, when omitted the current directory is used',
     )
 @click.version_option(version=__version__)
 def deploy(
     manifest_file, version_tag, target_stage, include_global_config_files,
     auto_approve, verbose, dry_run, working_dir
     ):
-    """ [experimental] Deploys the terragrunt config files from a git repository """
+    """ Deploys the terragrunt config files from a git repository """
 
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.deploy(
         manifest_file=manifest_file,
         version_tag=version_tag,
@@ -621,14 +627,48 @@
         include_global_config_files=include_global_config_files,
         auto_approve=auto_approve,
         dry_run=dry_run,
         working_dir=working_dir,
     )
 
 @main.command(
+    name="check-deployed-versions",
+    context_settings=dict(
+        ignore_unknown_options=True,
+    ),
+)
+@click.option('--manifest-file', '-m',
+    help='Manifest file describing the deployment options',
+    required=True, default="manifest.yaml", show_default=True,
+    )
+@click.option('--verbose', '-v',
+    help='Verbose printing',
+    is_flag=True, default=False, show_default=True,
+    )
+@click.option('--working-dir', '-w', default=None,
+    help='Working directory, when omitted the current directory is used',
+    )
+@click.option('--out', '-o', is_flag=True, default=False,
+    help='Show output as json',
+    show_default=True
+    )
+@click.version_option(version=__version__)
+def check_deployed_versions(manifest_file, verbose, working_dir, out):
+    """ Check the freshness of deployed versions against the configured platform file """
+
+    check_latest_version(verbose)
+
+    tgwrap = TgWrap(verbose=verbose)
+    tgwrap.check_deployed_versions(
+        manifest_file=manifest_file,
+        working_dir=working_dir,
+        out=out,
+    )
+
+@main.command(
     name="show-graph",
     context_settings=dict(
         ignore_unknown_options=True,
     ),
 )
 @click.option('--verbose', '-v', is_flag=True, default=False,
     help='Verbose printing',
@@ -694,7 +734,10 @@
     check_latest_version(verbose)
 
     tgwrap = TgWrap(verbose=verbose)
     tgwrap.clean(
         working_dir=working_dir,
     )
 
+# this is needed for the vscode debugger to work
+if __name__ == '__main__':
+    main()
```

### Comparing `tgwrap-0.5.7/tgwrap/main.py` & `tgwrap-0.6.0/tgwrap/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,24 +23,36 @@
 import json
 import yaml
 import threading
 import queue
 import multiprocessing
 import click
 import networkx as nx
+import hcl2
 
+from datetime import datetime, timezone
 from .printer import Printer
-from .terrasafe import run_terrasafe
+from .analyze import run_analyze
+
+class DateTimeEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, datetime):
+            return obj.isoformat()
+        return super().default(obj)
+
 
 class TgWrap():
     """
     A wrapper around terragrunt with the sole purpose to make it a bit
     (in an opiionated way) easier to use
     """
     SEPARATOR=':|:'
+    VERSION_FILE="version.hcl"
+    LATEST_VERSION='latest'
+    LOCATE_VERSION_FILE_MAX_LEVELS=3
 
     def __init__(self, verbose):
         self.printer = Printer(verbose)
 
         # Check if the "TERRAGRUNT_SOURCE" environment variable is set
         env_var = "TERRAGRUNT_SOURCE"
         if env_var in os.environ:
@@ -53,16 +65,20 @@
                 )
 
     def _is_installed(self, program):
         """ Checks if a program is installed on the system """
         return shutil.which(program) is not None
 
     def load_yaml_file(self, filepath):
-        with open(filepath, 'r') as file:
-            return yaml.safe_load(file)
+        try:
+            with open(filepath, 'r') as file:
+                return yaml.safe_load(file)
+        except yaml.parser.ParserError as e:
+            print(f'Cannot parse YAML file {filepath}, check syntax please!')
+            sys.exit(1)
 
     def _construct_command(self, command, debug, exclude_external_dependencies,
         non_interactive=True, no_auto_approve=True, no_lock=True, update=False,
         planfile=None, working_dir=None, limit_parallelism=None, 
         include_dir=[], exclude_dir=[], terragrunt_args=()):
         """ Constructs the command """
 
@@ -221,14 +237,39 @@
             self.printer.error(e)
             raise click.ClickException(e)
         finally:
             f.close()
 
         return graph
 
+    def _clone_repo(self, manifest, target_dir, version_tag=None):
+        """Clones the repo, possibly a specific version, into a temp directory"""
+
+        # clone the repo
+        cmd = f"git clone {manifest['git_repository']} {target_dir}"
+        rc = subprocess.run(
+            shlex.split(cmd),
+            check=True,
+            stdout=sys.stdout if self.printer.print_verbose else subprocess.DEVNULL,
+            stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
+            )
+        self.printer.verbose(rc)
+
+        # now check out the specific version if we don't want latest
+        if version_tag and version_tag.lower() != self.LATEST_VERSION:
+            cmd = f"git checkout -b source {version_tag}"
+            rc = subprocess.run(
+                shlex.split(cmd),
+                cwd=target_dir,
+                check=True,
+                stdout=sys.stdout if self.printer.print_verbose else subprocess.DEVNULL,
+                stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
+                )
+            self.printer.verbose(rc)
+
     def _analyze_results(self, rc, messages):
         """ Checks for errors """
 
         error = False
         skip = False
 
         messages = messages.lower()
@@ -468,16 +509,16 @@
                 self.printer.verbose(f'Wait for thread #{counter} (of {total_counter}) to finish')
                 t.join()
                 collect_output_file.write(q.get())
         
         self.printer.verbose(f'Executed {group_nbr} groups and {step_nbr} steps')
 
     def _run_sync(
-        self, source_path, target_path, auto_approve, include_lock_file, dry_run, clean_up,
-        excludes=[], source_stage=None, target_stage=None, source_domain=None,
+        self, source_path, target_path, auto_approve, include_lock_file, dry_run, clean,
+        chmod_to_readonly=False, excludes=[], source_stage=None, target_stage=None, source_domain=None,
         ):
         """ Run a sync copying files from a source to a target path """
 
         if not self._is_installed('rsync'):
             self.printer.error("'rsync' seems not installed. Cannot continue")
         elif not os.path.exists(source_path):
             self.printer.error(f"Cannot find {source_path}. Cannot continue.")
@@ -496,25 +537,30 @@
             try:
                 os.makedirs(target_path)
             except OSError:
                 # directory already exists
                 pass
 
             dry_run_stmt = '--dry-run' if dry_run else ''
-            clean_stmt   = '--delete' if clean_up else ''
+            clean_stmt   = '--delete' if clean else ''
             env_file_stmt   = "--exclude='env.hcl'" if source_stage != target_stage else "--include='env.hcl'"
             lock_file_stmt  = "--include='.terraform.lock.hcl'" if include_lock_file \
                 else "--exclude='.terraform.lock.hcl'"
             excludes_stmt = ' '.join([f"--exclude={x}" for x in excludes])
 
+            include_statements = ""
+            if os.path.isdir(target_path):
+                include_statements = \
+                    f"--include='terragrunt.hcl' {lock_file_stmt} {env_file_stmt} {excludes_stmt} " + \
+                    "--exclude='.terragrunt-cache/' --exclude='.terraform/' " + \
+                    "--exclude='terragrunt-debug.tfvars.json' --exclude=planfile " + \
+                    "--exclude='.DS_Store' "
+
             cmd = f"rsync -aim {dry_run_stmt} {clean_stmt} " + \
-                f"--include='terragrunt.hcl' {lock_file_stmt} {env_file_stmt} {excludes_stmt} " + \
-                "--exclude='.terragrunt-cache/' --exclude='.terraform/' " + \
-                "--exclude='terragrunt-debug.tfvars.json' --exclude=planfile " + \
-                "--exclude='.DS_Store' " + \
+                include_statements + \
                 f"{source_path} {target_path}"
 
             cmd = re.sub(' +', ' ', cmd)
 
             self.printer.header("Will be deploying:", print_line_before=True)
             self.printer.normal(f"from: {source_path}")
             self.printer.normal(f"to:   {target_path}")
@@ -524,16 +570,32 @@
                 response = input("\nDo you want to continue? (y/n) ")
                 if response.lower() != "y":
                     sys.exit(1)
 
             rc = subprocess.run(shlex.split(cmd))
             self.printer.verbose(rc)
 
+            # not working, results in an 'permission denied' at first run
+            # more info see: https://github.com/gruntwork-io/terragrunt/issues/2578
+            # if chmod_to_readonly and os.path.isdir(target_path):
+            #     cmd = f"find {target_path} -type f -name '.terraform.lock.hcl' -exec chmod a-w {{}} \;"
+            #     self.printer.normal('Change .terraform-lock files to read only')
+            #     self.printer.verbose(f"Using command:\n$ {cmd}")
+            #     rc = subprocess.run(
+            #         cmd,
+            #         shell=True,
+            #         check=True,
+            #         stdout=sys.stdout if self.printer.print_verbose else subprocess.DEVNULL,
+            #         stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
+            #         cwd=target_path,
+            #     )
+            #     self.printer.verbose(rc)
+
     def run(self, command, debug, dry_run, no_lock, update,
-        planfile, auto_approve, working_dir, terragrunt_args):
+        planfile, auto_approve, clean, working_dir, terragrunt_args):
         """ Executes a terragrunt command on a single module """
 
         self.printer.verbose(f"Attempting to execute 'run {command}'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
         check_for_file="terragrunt.hcl"
@@ -556,22 +618,25 @@
             working_dir=working_dir,
             terragrunt_args=terragrunt_args,
         )
 
         if dry_run:
             self.printer.warning(f'In dry run mode, no real actions are executed!!')
         else:
+            if clean:
+                self.clean(working_dir=working_dir)
+
             # the `posix=False` is to prevent the split command to remove quotes from strings,
             # e.g. when executing commands like this:
             # tgwrap state mv 'azuread_group.this["viewers"]' 'azuread_group.this["readers"]'
             rc = subprocess.run(shlex.split(cmd, posix=False))
             self.printer.verbose(rc)
 
     def run_all(self, command, debug, dry_run, no_lock, update,
-        exclude_external_dependencies, step_by_step, planfile, auto_approve, 
+        exclude_external_dependencies, step_by_step, planfile, auto_approve, clean,
         working_dir, start_at_step, limit_parallelism, include_dir, exclude_dir, terragrunt_args):
         """ Executes a terragrunt command across multiple modules """
 
         self.printer.verbose(f"Attempting to execute 'run-all {command}'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
@@ -591,14 +656,17 @@
             working_dir=None if step_by_step else working_dir,
             terragrunt_args=terragrunt_args,
             limit_parallelism=limit_parallelism,
             include_dir=[] if step_by_step else include_dir,
             exclude_dir=[] if step_by_step else exclude_dir,
         )
 
+        if clean and not dry_run:
+            self.clean(working_dir=working_dir)
+
         if step_by_step:
             self.printer.verbose(
                 f'This command will be executed for each individual module:\n$ {cmd}'
                 )
 
             self._run_di_graph(
                 command=cmd,
@@ -660,54 +728,54 @@
             # tgwrap import 'azuread_group.this["viewers"]' '123e4567-e89b-12d3-a456-426655440000'
             rc = subprocess.run(
                 shlex.split(cmd, posix=False),
                 env=env,
             )
             self.printer.verbose(rc)
 
-    def analyze(self, dry_run, exclude_external_dependencies, working_dir, start_at_step,
-        out, terrasafe_config, parallel_execution, include_dir, exclude_dir, terragrunt_args):
+    def analyze(self, exclude_external_dependencies, working_dir, start_at_step,
+        out, analyze_config, parallel_execution,
+        include_dir, exclude_dir, terragrunt_args):
         """ Analyzes the plan files """
 
         self.printer.verbose("Attempting to 'analyze'")
         if terragrunt_args:
             self.printer.verbose(f"- with additional parameters: {' '.join(terragrunt_args)}")
 
         # first run a 'show' and write output to file
         cmd = self._construct_command(
             command='show',
             exclude_external_dependencies=True,
             debug=False,
             terragrunt_args=terragrunt_args,
             )
 
-        ts_config = None
-        if not terrasafe_config:
+        config = None
+        if not analyze_config:
             self.printer.warning(
-                f"Terrasafe config file is not set, this is required for running the terrasafe command!"
+                f"Analyze  config file is not set, this is required for checking for unauthorized deletions and drift detection scores!"
                 )
         else:
             self.printer.verbose(
-                f"\nRun terrasafe using config {terrasafe_config}"
+                f"\nAnalyze using config {config}"
                 )
-
-            with open(terrasafe_config) as f:
-                ts_config = json.load(f)
+            config = self.load_yaml_file(analyze_config)
 
         ts_validation_successful = True
         changes = {}
+        drifts = {}
         try:
             # then run it and capture the output
             with tempfile.NamedTemporaryFile(mode='w+', prefix='tgwrap-', delete=False) as f:
                 self.printer.verbose(f"Opened temp file for output collection: {f.name}")
 
                 self._run_di_graph(
                     command=cmd,
+                    dry_run=False, # no need for dryruns when analyzing
                     exclude_external_dependencies=exclude_external_dependencies,
-                    dry_run=dry_run,
                     collect_output_file=f,
                     working_dir=working_dir,
                     start_at_step=start_at_step,
                     ask_for_confirmation=False,
                     include_dir=include_dir,
                     exclude_dir=exclude_dir,
                     parallel_execution=parallel_execution,
@@ -718,83 +786,88 @@
                     split_line = line.split(self.SEPARATOR)
                     module = split_line[0]
                     try:
                         plan_file = split_line[1]
                     except IndexError:
                         self.printer.warning(f'Could not determine planfile: {line[:100]}')
 
-                    changes[module] = {
-                        "deletions" : [],
-                        "other" : [],
-                        "unauthorized" : [],
-                    }
-
                     try:
                         # plan file could be empty (except for new line) if module is skipped
                         if len(plan_file) > 1:
                             data = json.loads(plan_file)
 
-                            # check for unauthorized deletions
-                            if ts_config:
-                                changes[module]["unauthorized"] = run_terrasafe(
-                                    config=ts_config,
-                                    data=data,
-                                    verbose=self.printer.print_verbose,
-                                    )
-                                if len(changes[module]["unauthorized"]) > 0:
-                                    ts_validation_successful = False
-
                             # do we have an exception logged?
                             if 'exception' in data:
                                 raise Exception(data['exception'])
-                            elif len(data.get('resource_changes', [])) > 0:
-                                for rc in data['resource_changes']:
-                                    # check if we do have actual changes
-                                    actions = rc['change']['actions']
-                                    action = f'{rc["address"]}: {", ".join(actions)}'
-                                    if len(actions) == 1 and (actions[0] == 'no-op' or actions[0] == 'read'):
-                                        pass # ignore, just an state change
-                                    elif 'delete' in actions:
-                                        # only include if it is not already included in the unauthorized section
-                                        if action.split(":")[0] not in changes[module]["unauthorized"]:
-                                            changes[module]["deletions"].append(action)
-                                    else:
-                                        changes[module]["other"].append(action)
+
+                            changes[module], ts_success = run_analyze(
+                                config=config,
+                                data=data,
+                                verbose=self.printer.print_verbose,
+                                )
+                            if not ts_success:
+                                ts_validation_successful = False
                         else:
                             self.printer.warning(f'Planfile for module {module} is empty')
                     except json.decoder.JSONDecodeError as e:
                         raise Exception(
                             f"Exception detected or planfile for {module} was not proper json, further analysis not possible:\n{plan_file[:200]}"
                             ) from e
         finally:
             os.remove(f.name)
 
         self.printer.header("Analysis results:", print_line_before=True)
         for key, value in changes.items():
             self.printer.header(f'Module: {key}')
-            if not (value["deletions"] or value["other"] or value["unauthorized"]):
-                self.printer.success('- No changes detected')
+            if not value["all"]:
+                self.printer.success('No changes detected')
             if value["unauthorized"]:
-                self.printer.error('- Unauthorized deletions:')
+                self.printer.error('Unauthorized deletions:')
                 for m in value["unauthorized"]:
-                    self.printer.error(f' -> {m}')
+                    self.printer.error(f'-> {m}')
             if value["deletions"]:
-                self.printer.warning('- Deletions:')
+                self.printer.warning('Deletions:')
                 for m in value["deletions"]:
+                    self.printer.warning(f'-> {m}')
+            if value["creations"]:
+                self.printer.normal('Creations:')
+                for m in value["creations"]:
+                    self.printer.normal(f'-> {m}')
+            if value["updates"]:
+                self.printer.normal('Updates:')
+                for m in value["updates"]:
+                    self.printer.normal(f'-> {m}')
+
+        # calulate the total drifts and scoe
+        total_drifts = {
+            "minor": 0,
+            "medium": 0,
+            "major": 0,
+            "unknown": 0,
+            "total": 0
+        }
+
+        for key, value in changes.items():
+            for type in ["minor", "medium", "major", "unknown", "total"]:
+                total_drifts[type] += value["drifts"][type]
+
+        total_drift_score = f"{total_drifts['major']}.{total_drifts['medium']}.{total_drifts['minor']}"
+        self.printer.header(f"Drift score: {total_drift_score}")
+        if total_drifts["unknown"] > 0:
+            self.printer.warning(f"For {total_drifts['unknown']} resources, drift score is not configured, please update configuration!")
+            self.printer.warning('- Unknowns:')
+            for key, value in changes.items():
+                for m in value["unknowns"]:
                     self.printer.warning(f' -> {m}')
-            if value["other"]:
-                self.printer.normal('- Other:')
-                for m in value["other"]:
-                    self.printer.normal(f' -> {m}')
 
         if out:
             print(json.dumps(changes, indent=4))
 
         if not ts_validation_successful:
-            self.printer.error("Terrasafe validation failed on one or more modules")
+            self.printer.error("Analysis detected unauthorised deletions, please check your configuration!!!")
             sys.exit(1)
 
     def set_lock(self, module, lock_status, auto_approve, dry_run, working_dir):
         """ Set the lock status of the stage you're in """
     
         # do we have a working dir?
         working_dir = working_dir if working_dir else os.getcwd()
@@ -812,15 +885,15 @@
             update=False,
             planfile=None,
             terragrunt_args=[],
             )
 
     def sync(
         self, source_stage, target_stage, source_domain, target_domain, module,
-        auto_approve, dry_run, clean_up, include_lock_file, working_dir, 
+        auto_approve, dry_run, clean, include_lock_file, working_dir, 
         ):
         """ Syncs the terragrunt config files from one stage to another (and possibly to a different domain) """
     
         if target_domain and not source_domain:
             raise Exception("Providing a target domain while omitting the source domain is not supported!")
         if source_domain and not target_domain:
             raise Exception("Providing a source domain while omitting the target domain is not supported!")
@@ -843,20 +916,21 @@
             target_path=target_path,
             source_domain=source_domain,
             source_stage=source_stage,
             target_stage=target_stage,
             include_lock_file=include_lock_file,
             auto_approve=auto_approve,
             dry_run=dry_run,
-            clean_up=clean_up,
+            clean=clean,
+            chmod_to_readonly=False,
         )
 
     def sync_dir(
         self, source_directory, target_directory,
-        auto_approve, dry_run, clean_up, include_lock_file, working_dir, 
+        auto_approve, dry_run, clean, include_lock_file, working_dir, 
         ):
         """ Syncs the terragrunt config files from one directory to anothery """
     
         # do we have a working dir?
         working_dir = working_dir if working_dir else os.getcwd()
         # the domains will be ignored when omitted as input
         source_path = os.path.join(working_dir, source_directory, '')
@@ -864,25 +938,23 @@
 
         self._run_sync(
             source_path=source_path,
             target_path=target_path,
             include_lock_file=include_lock_file,
             auto_approve=auto_approve,
             dry_run=dry_run,
-            clean_up=clean_up,
+            clean=clean,
+            chmod_to_readonly=False,
         )
 
     def deploy(
         self, manifest_file, version_tag, target_stage,
         include_global_config_files, auto_approve, dry_run, working_dir, 
         ):
         """ Deploys the terragrunt config files from a git repository """
-
-        DEFAULT_VERSION='latest'
-
         try:
             temp_dir = os.path.join(tempfile.mkdtemp(prefix='tgwrap-'), "tg-source")
 
             # do we have a working dir? 
             working_dir = working_dir if working_dir else os.getcwd()
 
             manifest = self.load_yaml_file(os.path.join(working_dir, manifest_file))
@@ -891,43 +963,25 @@
             target_dir = os.path.join(working_dir, target_stage)
 
             try:
                 os.mkdir(target_dir)
             except FileExistsError:
                 pass
 
-            # clone the repo
-            cmd = f"git clone {manifest['git_repository']} {temp_dir}"
-            rc = subprocess.run(
-                shlex.split(cmd),
-                check=True,
-                stdout=sys.stdout if self.printer.print_verbose else subprocess.DEVNULL,
-                stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
-                )
-            self.printer.verbose(rc)
-
-            # now check out the specific version if we don't want latest
-            if version_tag.lower() != DEFAULT_VERSION:
-                cmd = f"git checkout -b source {version_tag}"
-                rc = subprocess.run(
-                    shlex.split(cmd),
-                    cwd=temp_dir,
-                    check=True,
-                    stdout=sys.stdout if self.printer.print_verbose else subprocess.DEVNULL,
-                    stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
-                    )
-                self.printer.verbose(rc)
+            self._clone_repo(manifest=manifest, target_dir=temp_dir, version_tag=version_tag)
 
             # collect all the base paths of the substacks as you don't want
-            # to include them in regular syncs
-            substacks = []
+            # to include them in regular syncs, add some standard paths there by default
+            substacks = ['substacks', 'sub_stacks']
             for ss, substack in manifest.get('sub_stacks', {}).items():
                 # get the base directory of the sub stack so that we can ignore it when deploying the regular modules
                 substacks.append(substack['source'].split(os.path.sep)[0])
 
+            substacks = set(substacks)
+
             deploy_actions = {}
             for key, value in manifest['deploy'].items():
                 if target_stage not in value['applies_to_stages']:
                     self.printer.verbose(f'Target stage {target_stage} not applicable for action {key}.')
                 else:
                     source_stage = value['source_stage']
                     self.printer.verbose(f'Found deployment step {key} using source stage {source_stage}')
@@ -1014,29 +1068,176 @@
                 self._run_sync(
                     source_path=value['source'],
                     target_path=value['target'],
                     excludes=value.get('excludes', []),
                     include_lock_file=True,
                     auto_approve=True,
                     dry_run=dry_run,
-                    clean_up=False,
+                    clean=False,
+                    chmod_to_readonly=True,
                 )
 
             if not dry_run:
-                with open(os.path.join(target_dir, 'version.hcl'), 'w') as f:
+                        # write the version file
+                with open(os.path.join(target_dir, self.VERSION_FILE), 'w') as f:
                     f.write(f"""
 locals {{
     version_tag="{version_tag}"
 }}
 """)
+
+                # clean up the cache in the deployed directory to avoid strange issues when planning
+                self.clean(working_dir=target_dir)
+
+        except KeyError as e:
+            self.printer.error(f'Error interpreting the manifest file. Please ensure it uses the proper format. Could not find element: {e}')
+            sys.exit(1)
+        except Exception as e:
+            self.printer.error(f'Unexpected error: {e}')
+            if self.printer.print_verbose:
+                raise(e)
+            sys.exit(1)
+        finally:
+            try:
+                shutil.rmtree(temp_dir)
+            except Exception:
+                pass
+
+    def check_deployed_versions(self, manifest_file, working_dir, out):
+        def locate_version_files(current_directory, found_files=[], root_directory=None, level=1):
+            " This tries to find a version file in the current directory, or a given number of directories beneath it"
+
+            if not root_directory:
+                root_directory = current_directory
+
+            for entry in os.listdir(current_directory):
+                full_entry = os.path.join(current_directory, entry)
+                if os.path.isdir(full_entry) and level < self.LOCATE_VERSION_FILE_MAX_LEVELS:
+                    found_files = locate_version_files(
+                        current_directory=full_entry,
+                        found_files=found_files,
+                        root_directory=root_directory,
+                        level=level+1,
+                    )
+                elif entry == self.VERSION_FILE:
+                    found_files.append(os.path.relpath(current_directory, root_directory))
+                    
+            return found_files
+
+        def get_all_version(repo_dir, min_version=None):
+            "Get all the version tags from the repo including their data"
+
+            # Execute 'git tag' command to get a list of all tags
+            cmd = "git tag --sort='-refname:short' --format='%(refname:short) %(creatordate:iso8601)'"
+            output = subprocess.check_output(
+                shlex.split(cmd),
+                cwd=repo_dir,
+                universal_newlines=True,
+                )
+
+            # Split the output into lines
+            lines = output.strip().split('\n')
+
+            # Iterate over the lines to extract tag names and creation dates
+            timestamp_format = '%Y-%m-%d %H:%M:%S %z'
+            tags = {}
+            for line in lines:
+                tag_name, created_date = line.split(' ', maxsplit=1)
+                tags[tag_name] = {'created_date': datetime.strptime(created_date, timestamp_format)}
+
+                if tag_name == min_version:
+                    break
+
+            self.printer.verbose(f'Found {len(tags)} tags: {tags}')
+
+            return tags
+
+        try:
+            # do we have a working dir? 
+            working_dir = working_dir if working_dir else os.getcwd()
+            self.printer.header(f'Check released versions ({self.LOCATE_VERSION_FILE_MAX_LEVELS} levels) in directory: {working_dir}')
+
+            result = locate_version_files(working_dir)
+
+            versions = []
+            for location in result:
+                # Determine the deployed version as defined in the version file
+                with open(os.path.join(working_dir, location, self.VERSION_FILE), 'r') as file:
+                    content = hcl2.load(file)
+                    try:
+                        version_tag = content['locals'][0]['version_tag']
+                        versions.append(
+                            {
+                                'path': location,
+                                'tag': version_tag
+                            }
+                        )
+                    except KeyError as e:
+                        versions.append({location: 'unknown'})
+
+            self.printer.verbose(f'Detected versions: {versions}')
+
+            # remove the 'latest' tag from the detected versions, as it is specific one
+            filtered_versions = list(filter(lambda x: x['tag'] != self.LATEST_VERSION, versions))
+
+            if filtered_versions:
+                min_version = min(filtered_versions, key=lambda x: x['tag'])
+                max_version = max(filtered_versions, key=lambda x: x['tag'])
+            else:
+                min_version = None
+                max_version = None
+
+            self.printer.verbose(f'Detected minimum version {min_version} and maximum version {max_version}')
+
+            temp_dir = os.path.join(tempfile.mkdtemp(prefix='tgwrap-'), "tg-source")
+            manifest = self.load_yaml_file(os.path.join(working_dir, manifest_file))
+            self._clone_repo(manifest=manifest, target_dir=temp_dir)
+
+            # determine the version tag from the repo, including their date
+            all_versions = get_all_version(repo_dir=temp_dir, min_version=min_version['tag'])
+
+            # so now we can determine how old the deployed versions are
+            now = datetime.now(timezone.utc)
+            for version in versions:
+                tag = version['tag']
+                if tag == self.LATEST_VERSION:
+                    version['release_date'] = 'unknown'
+                else:
+                    release_date = all_versions[tag]['created_date']
+                    version['release_date'] = release_date
+                    version['days_since_release'] = (now - release_date).days
+
+            self.printer.header(
+                'Deployed versions:' if len(versions) > 0 else 'No deployed versions detected'
+                )
+            
+            for version in versions:
+                days_since_release = version.get("days_since_release", 0)
+                message = f'-> {version["path"]}: {version["tag"]} (released {days_since_release} days ago)'
+                if days_since_release > 60:
+                    self.printer.error(message)
+                elif days_since_release > 30:
+                    self.printer.error(message)
+                elif days_since_release < 7:
+                    self.printer.success(message)
+                else:
+                    self.printer.normal(message)
+
+            if out:
+                print(json.dumps(versions, indent=4, cls=DateTimeEncoder))
+    
         except KeyError as e:
             self.printer.error(f'Error interpreting the manifest file. Please ensure it uses the proper format. Could not find element: {e}')
+            if self.printer.print_verbose:
+                raise(e)
             sys.exit(1)
         except Exception as e:
             self.printer.error(f'Unexpected error: {e}')
+            if self.printer.print_verbose:
+                raise(e)
             sys.exit(1)
         finally:
             try:
                 shutil.rmtree(temp_dir)
             except Exception:
                 pass
 
@@ -1058,28 +1259,34 @@
             graph=graph,
             exclude_external_dependencies=exclude_external_dependencies,
             working_dir=working_dir,
             include_dir=include_dir,
             exclude_dir=exclude_dir,
             )
 
-        self.printer.header("The following groups will be processed:")
-        for idx, group in enumerate(groups):
-            self.printer.normal(f"\nGroup {idx+1}:")
-            for directory in group:
-                self.printer.normal(f"- {directory}")
+        if not groups:
+            self.printer.error('No groups in scope, this smells fishy!')
+        else:
+            self.printer.header("The following groups are in scope:")
+            for idx, group in enumerate(groups):
+                self.printer.normal(f"\nGroup {idx+1}:")
+                for directory in group:
+                    self.printer.normal(f"- {directory}")
 
     def clean(self, working_dir):
         """ Clean the temporary files of a terragrunt/terraform project """
 
         cmd = 'find . -name ".terragrunt-cache" -type d -exec rm -rf {} \; ; find . -name ".terraform" -type d -exec rm -rf {} \;'
-        rc = subprocess.run(
-            cmd,
-            shell=True,
-            check=True,
-            stdout=sys.stdout if self.printer.print_verbose else subprocess.DEVNULL,
-            stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
-            cwd=working_dir if working_dir else None,
-            )
+        # we see the behaviour that with cleaning up large directories, it returns errorcode=1 upon first try
+        # never to shy away from a questionable solution to make your life easier, we just run it again :-)
+        rc = 'clean up not started!'
+        for check in [False, True]:
+            rc = subprocess.run(
+                cmd,
+                shell=True,
+                check=check,
+                stdout=sys.stdout if self.printer.print_verbose else subprocess.DEVNULL,
+                stderr=sys.stderr if self.printer.print_verbose else subprocess.DEVNULL,
+                cwd=working_dir if working_dir else None,
+                )
         self.printer.verbose(rc)
         self.printer.normal("Cleaned the temporary files")
-
```

### Comparing `tgwrap-0.5.7/tgwrap/printer.py` & `tgwrap-0.6.0/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.5.7/setup.py` & `tgwrap-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
 install_requires = \
 ['click>=8.0',
  'networkx>=2.8.8,<3.0.0',
  'outdated>=0.2.2',
  'pydot>=1.4.2,<2.0.0',
  'pyhcl>=0.4.4,<0.5.0',
+ 'python-hcl2>=4.3.2,<5.0.0',
  'pyyaml>=6.0',
  'terrasafe>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['tgwrap = tgwrap.cli:main']}
 
 setup_kwargs = {
     'name': 'tgwrap',
-    'version': '0.5.7',
+    'version': '0.6.0',
     'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
     'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if availabe) runs a [terrasafe](https://pypi.org/project/terrasafe/) validation check.\n\nIt would provide output as follows:\n\n```console\n$ tgwrap analyze -x\n\n...\n\nAnalyse project: inputs\nRun terrasafe: inputs\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n\nAnalyse project: runners\nChanges:\nmodule.vmss.azurerm_key_vault_secret.pwd: delete,create\nmodule.vmss.azurerm_key_vault_secret.user: delete,create\nmodule.vmss.azurerm_linux_virtual_machine_scale_set.this[0]: update\n\nRun terrasafe: runners\nConfig loaded from /my/project/dir/terrasafe-config.json\n0 unauthorized deletion detected\n```\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/lunadata/tgwrap',
```

### Comparing `tgwrap-0.5.7/PKG-INFO` & `tgwrap-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.5.7
+Version: 0.6.0
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0)
 Requires-Dist: networkx (>=2.8.8,<3.0.0)
 Requires-Dist: outdated (>=0.2.2)
 Requires-Dist: pydot (>=1.4.2,<2.0.0)
 Requires-Dist: pyhcl (>=0.4.4,<0.5.0)
+Requires-Dist: python-hcl2 (>=4.3.2,<5.0.0)
 Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: terrasafe (>=0.5.1,<0.6.0)
 Project-URL: Documentation, https://gitlab.com/lunadata/tgwrap/
 Project-URL: Repository, https://gitlab.com/lunadata/tgwrap
 Description-Content-Type: text/markdown
 
 # tg-wrap
```


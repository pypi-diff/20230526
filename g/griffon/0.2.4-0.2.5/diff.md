# Comparing `tmp/griffon-0.2.4.tar.gz` & `tmp/griffon-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffon-0.2.4.tar", last modified: Thu May 25 07:47:51 2023, max compression
+gzip compressed data, was "griffon-0.2.5.tar", last modified: Fri May 26 14:39:19 2023, max compression
```

## Comparing `griffon-0.2.4.tar` & `griffon-0.2.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 07:47:35.000000 griffon-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-25 07:47:51.815697 griffon-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-25 07:47:35.000000 griffon-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon/commands/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/community_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/corgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/entities/osidb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugin_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/griffon/commands/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/cve_mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/cvelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/go_vuln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/osv.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/plugins/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    52663 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/griffon/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/core_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/core_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/services/core_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/griffon/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-25 07:47:35.000000 griffon-0.2.4/griffon/static/default_griffonrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.811696 griffon-0.2.4/griffon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 07:47:51.000000 griffon-0.2.4/griffon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 07:47:35.000000 griffon-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:47:51.815697 griffon-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-25 07:47:35.000000 griffon-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:47:51.815697 griffon-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-25 07:47:35.000000 griffon-0.2.4/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 14:39:02.000000 griffon-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-26 14:39:19.517255 griffon-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-26 14:39:02.000000 griffon-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon/commands/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/community_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/corgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/entities/osidb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugin_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/griffon/commands/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/cve_mitre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/cvelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/go_vuln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/osv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/plugins/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26911 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52663 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/griffon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/core_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35881 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/core_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/services/core_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/griffon/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-26 14:39:02.000000 griffon-0.2.5/griffon/static/default_griffonrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.513256 griffon-0.2.5/griffon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 14:39:19.000000 griffon-0.2.5/griffon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 14:39:02.000000 griffon-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:39:19.517255 griffon-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-26 14:39:02.000000 griffon-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:39:19.517255 griffon-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-26 14:39:02.000000 griffon-0.2.5/tests/test_unit.py
```

### Comparing `griffon-0.2.4/LICENSE` & `griffon-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/PKG-INFO` & `griffon-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.4
+Version: 0.2.5
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.4/README.md` & `griffon-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/__init__.py` & `griffon-0.2.5/griffon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import osidb_bindings
 from osidb_bindings.bindings.python_client.models import Affect, Flaw, Tracker
 from pkg_resources import resource_filename  # type: ignore
 from rich.logging import RichHandler
 
 from griffon.output import console
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 if "CORGI_API_URL" not in os.environ:
     print("Must set CORGI_API_URL environment variable.")
     exit(1)
 CORGI_API_URL = os.environ["CORGI_API_URL"]
 
 if "OSIDB_API_URL" not in os.environ:
@@ -28,14 +28,17 @@
 OSIDB_AUTH_METHOD = os.getenv("OSIDB_AUTH_METHOD", "kerberos")
 
 # required to enable --search-community
 COMMUNITY_COMPONENTS_API_URL = os.getenv(
     "COMMUNITY_COMPONENTS_API_URL", "https://component-registry.fedoraproject.org"
 )
 
+# TODO: temporary hack required to enable searching of middleware
+MIDDLEWARE_CLI = os.getenv("GRIFFON_MIDDLEWARE_CLI")
+
 GRIFFON_CONFIG_DIR = os.getenv("GRIFFON_API_URL", "~/.griffon")
 GRIFFON_RC_FILE = "~/.griffonrc"
 GRIFFON_DEFAULT_LOG_FILE = os.getenv("GRIFFON_DEFAULT_LOG_FILE", "~/.griffon/history.log")
 
 logger = logging.getLogger("griffon")
 
 RELATED_MODELS_MAPPING = {Flaw: {"affects": Affect}, Affect: {"trackers": Tracker}}
```

### Comparing `griffon-0.2.4/griffon/autocomplete/__init__.py` & `griffon-0.2.5/griffon/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/cli.py` & `griffon-0.2.5/griffon/cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/configure.py` & `griffon-0.2.5/griffon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/docs.py` & `griffon-0.2.5/griffon/commands/docs.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/entities/__init__.py` & `griffon-0.2.5/griffon/commands/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/entities/community_component_registry.py` & `griffon-0.2.5/griffon/commands/entities/community_component_registry.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/entities/corgi.py` & `griffon-0.2.5/griffon/commands/entities/corgi.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/entities/helpers.py` & `griffon-0.2.5/griffon/commands/entities/helpers.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/entities/osidb.py` & `griffon-0.2.5/griffon/commands/entities/osidb.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/plugin_commands.py` & `griffon-0.2.5/griffon/commands/plugin_commands.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/plugins/bugzilla.py` & `griffon-0.2.5/griffon/commands/plugins/bugzilla.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/plugins/cve_mitre.py` & `griffon-0.2.5/griffon/commands/plugins/cve_mitre.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/plugins/go_vuln.py` & `griffon-0.2.5/griffon/commands/plugins/go_vuln.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/plugins/osv.py` & `griffon-0.2.5/griffon/commands/plugins/osv.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/plugins/semgrep.py` & `griffon-0.2.5/griffon/commands/plugins/semgrep.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/process.py` & `griffon-0.2.5/griffon/commands/process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/commands/queries.py` & `griffon-0.2.5/griffon/commands/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 """
 
 """
 import copy
 import logging
+import subprocess
+from json import loads
 
 import click
 from component_registry_bindings.bindings.python_client.api.v1 import v1_components_list
 from component_registry_bindings.bindings.python_client.models import Component
 
-from griffon import CorgiService, OSIDBService, get_config_option, progress_bar
+from griffon import (
+    MIDDLEWARE_CLI,
+    CorgiService,
+    OSIDBService,
+    get_config_option,
+    progress_bar,
+)
 from griffon.autocomplete import (
     get_component_names,
     get_cve_ids,
     get_product_stream_names,
     get_product_stream_ofuris,
     get_product_version_names,
 )
@@ -242,14 +250,21 @@
     "--no-community",
     "no_community",
     is_flag=True,
     default=False,
     help="Do not search community.",
 )
 @click.option(
+    "--no-middleware",
+    "no_middleware",
+    is_flag=True,
+    default=False,
+    help="Do not search middleware.",
+)
+@click.option(
     "-v",
     "verbose",
     count=True,
     default=get_config_option("default", "verbosity", 0),
     help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
 )  # noqa
 @click.pass_context
@@ -269,14 +284,15 @@
     filter_rh_naming,
     search_all,
     search_all_roots,
     search_redhat,
     search_community,
     search_upstreams,
     no_community,
+    no_middleware,
     verbose,
 ):
     with console.status("griffoning", spinner="line") as operation_status:
         """List products of a latest component."""
         if verbose:
             ctx.obj["VERBOSE"] = verbose
         if not purl and not component_name:
@@ -304,15 +320,65 @@
         if component_name:
             q = query_service.invoke(core_queries.products_containing_component_query, params)
         if purl:
             q = query_service.invoke(
                 core_queries.products_containing_specific_component_query, params
             )
 
-        # TODO - in the short term affect handling will be mediated via sfm2 here in the operation itself # noqa
+        # TODO: interim hack for middleware
+        if component_name and MIDDLEWARE_CLI and not no_middleware:
+            mw_command = [MIDDLEWARE_CLI, component_name, "-e", "maven", "--json"]
+            if strict_name_search:
+                mw_command.append("-s")
+            proc = subprocess.run(
+                mw_command,
+                capture_output=True,
+                text=True,
+            )
+            mw_json = loads(proc.stdout)
+            mw_components = mw_json["deps"]
+            # TODO: need to determine if we use "build" or "deps"
+            # if search_all:
+            #     mw_components.extend(mw_json["deps"])
+            for build in mw_components:
+                if build["build_type"] == "maven":
+                    component = {
+                        "product_versions": [{"name": build["ps_module"]}],
+                        "product_streams": [
+                            {
+                                "name": build["ps_update_stream"],
+                                "product_versions": [{"name": build["ps_module"]}],
+                            }
+                        ],
+                        "product_active": True,
+                        "type": build["build_type"],
+                        "name": build["build_name"],
+                        "nvr": build["build_nvr"],
+                        "upstreams": [],
+                        "sources": [],
+                        "software_build": {
+                            "build_id": build["build_id"],
+                            "source": build["build_repo"],
+                        },
+                    }
+                    if "sources" in build:
+                        for deps in build["sources"]:
+                            for dep in deps["dependencies"]:
+                                components = []
+                                components.append(
+                                    {
+                                        "name": dep.get("name"),
+                                        "nvr": dep.get("nvr"),
+                                        "type": dep.get("type"),
+                                    }
+                                )
+                                component["sources"] = components
+                    q.append(component)
+
+        # TODO: in the short term affect handling will be mediated via sfm2 here in the operation itself # noqa
         if ctx.params["sfm2_flaw_id"]:
             console.no_color = True
             console.highlighter = None
             operation_status.stop()
 
             # generate affects
             output = raw_json_transform(q, True)
```

### Comparing `griffon-0.2.4/griffon/commands/reports.py` & `griffon-0.2.5/griffon/commands/reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/output.py` & `griffon-0.2.5/griffon/output.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/services/__init__.py` & `griffon-0.2.5/griffon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/services/core_process.py` & `griffon-0.2.5/griffon/services/core_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/services/core_queries.py` & `griffon-0.2.5/griffon/services/core_queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -175,70 +175,36 @@
         "arch",
         "namespace",
         "component_type",
         "strict_name_search",
         "affect_mode",
         "search_latest",
         "search_all",
+        "search_all_roots",
         "search_related_url",
         "search_community",
         "search_upstreams",
         "filter_rh_naming",
         "search_redhat",
+        "no_community",
+        "no_middleware",
     ]
 
     def __init__(self, params: dict) -> None:
         self.corgi_session = CorgiService.create_session()
         self.params = params
         self.purl = self.params.get("purl")
 
     def execute(self) -> dict:
         c = self.corgi_session.components.retrieve_list(
             purl=self.purl,
         )
         return c["product_streams"]
 
 
-def output_component(pv, ps, c):
-    is_root = False
-    if (c.arch == "src" and c.type == "RPM") or (c.arch == "noarch" and c.type == "OCI"):
-        is_root = True
-    sources = [source for source in c.sources]
-    component = {
-        "is_root": is_root,
-        "product_version": pv["name"],
-        "product_version_ofuri": pv["ofuri"],
-        "product_stream": ps["name"],
-        "product_stream_ofuri": ps["ofuri"],
-        "product_active": True,
-        "purl": c.purl,
-        "type": str(c.type),
-        "namespace": str(c.namespace),
-        "name": c.name,
-        "arch": c.arch,
-        "release": c.release,
-        "version": c.version,
-        "sources": sources,
-        "nvr": c.nvr,
-        # "build_id": None,
-        # "build_type": None,
-        # "build_source_url": None,
-        # "related_url": None,
-        # "upstream_purl": None,
-    }
-    if c.software_build:
-        component["build_id"] = str(c.software_build.build_id)
-        component["build_type"] = str(c.software_build.build_type)
-        component["build_name"] = str(c.software_build.name)
-        component["build_source_url"] = str(c.software_build.source)
-    if c.upstreams:
-        component["upstream_purl"] = str(c.upstreams[0]["purl"])
-    return component
-
-
 def async_retrieve_components(corgi_session, params, components_initial, component_cnt):
     components = list()
     if component_cnt < 120:
         components.extend(components_initial.results)
     elif component_cnt > 120:
         components.extend(components_initial.results)
         with concurrent.futures.ThreadPoolExecutor() as executor:
@@ -277,14 +243,15 @@
         "search_all_roots",
         "search_related_url",
         "search_redhat",
         "search_community",
         "search_upstreams",
         "filter_rh_naming",
         "no_community",
+        "no_middleware",
     ]
 
     def __init__(self, params: dict) -> None:
         self.corgi_session = CorgiService.create_session()
         self.params = params
         self.component_name = self.params.get("component_name", "")
         self.component_type = self.params.get("component_type", "")
```

### Comparing `griffon-0.2.4/griffon/services/core_reports.py` & `griffon-0.2.5/griffon/services/core_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon/static/default_griffonrc` & `griffon-0.2.5/griffon/static/default_griffonrc`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/griffon.egg-info/PKG-INFO` & `griffon-0.2.5/griffon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.4
+Version: 0.2.5
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.4/griffon.egg-info/SOURCES.txt` & `griffon-0.2.5/griffon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/pyproject.toml` & `griffon-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/setup.py` & `griffon-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_cli.py` & `griffon-0.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_entities.py` & `griffon-0.2.5/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_manage.py` & `griffon-0.2.5/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_plugins.py` & `griffon-0.2.5/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_process.py` & `griffon-0.2.5/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_queries.py` & `griffon-0.2.5/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_reports.py` & `griffon-0.2.5/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.4/tests/test_unit.py` & `griffon-0.2.5/tests/test_unit.py`

 * *Files identical despite different names*


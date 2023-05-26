# Comparing `tmp/nci_cidc_cli-0.10.3.tar.gz` & `tmp/nci_cidc_cli-0.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-7kznu0r3/nci_cidc_cli-0.10.3.tar", last modified: Thu May 25 14:36:02 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-90vh0odb/nci_cidc_cli-0.10.4.tar", last modified: Fri May 26 17:28:55 2023, max compression
```

## Comparing `nci_cidc_cli-0.10.3.tar` & `nci_cidc_cli-0.10.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/consent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/tests/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/consent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/tests/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/util.py
```

### Comparing `nci_cidc_cli-0.10.3/LICENSE` & `nci_cidc_cli-0.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/PKG-INFO` & `nci_cidc_cli-0.10.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_cli
-Version: 0.10.3
+Version: 0.10.4
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.3/README.md` & `nci_cidc_cli-0.10.4/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/api.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/auth.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/cache.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/cli.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,19 +86,20 @@
         click.echo(f"* {assay}")
 
 
 #### $ nci-cidc assays upload ####
 @click.command("upload")
 @click.option("--assay", required=True, help="Assay type.")
 @click.option("--xlsx", required=True, help="Path to the assay metadata spreadsheet.")
-def upload_assay(assay, xlsx):
+@click.option("--testing", is_flag=True, default=False, help="Flag for BDD testing.")
+def upload_assay(assay, xlsx, testing):
     """
     Upload data for an assay.
     """
-    upload.run_upload(assay, xlsx)
+    upload.run_upload(assay, xlsx, is_testing=testing)
 
 
 #### $ nci-cidc analyses ####
 @click.group()
 def analyses():
     """Manage analysis data."""
 
@@ -114,19 +115,20 @@
 
 #### $ nci-cidc analyses upload ####
 @click.command("upload")
 @click.option("--analysis", required=True, help="Analysis type.")
 @click.option(
     "--xlsx", required=True, help="Path to the analysis metadata spreadsheet."
 )
-def upload_analysis(analysis, xlsx):
+@click.option("--testing", is_flag=True, default=False, help="Flag for BDD testing.")
+def upload_analysis(analysis, xlsx, testing):
     """
     Upload data for an analysis.
     """
-    upload.run_upload(analysis, xlsx, is_analysis=True)
+    upload.run_upload(analysis, xlsx, is_analysis=True, is_testing=testing)
 
 
 # Wire up the interface
 cidc.add_command(version)
 cidc.add_command(login)
 cidc.add_command(assays)
 cidc.add_command(analyses)
```

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/config.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/config.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/consent.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/consent.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/cli.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/core.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/list.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/remove.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/gcloud.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/gcloud.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli/upload.py` & `nci_cidc_cli-0.10.4/nci_cidc_cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 
 import click
 
 from . import api
 from . import gcloud
 
 
-def run_upload(upload_type: str, xlsx_path: str, is_analysis: bool = False):
+def run_upload(
+    upload_type: str,
+    xlsx_path: str,
+    is_analysis: bool = False,
+    is_testing: bool = False,
+):
     """
     Upload data.
 
     Orchestrator execution flow:
     1. Log in to gcloud. The CLI user must be authenticated with
        gcloud to be able to upload to GCS.
     2. Make an initiate_upload request to the API. The API adds a
@@ -26,16 +31,18 @@
        carry out the gsutil upload (like a mapping from local file paths
        to GCS URIs).
     3. Carry out the gsutil upload using the returned upload info.
     4. If the gsutil upload fails, alert the api that the job failed.
        Else, if the upload succeeds, alert the api that the job was
        successful.
     """
-    # Log in to gcloud (required for gsutil to work)
-    gcloud.login()
+    if not is_testing:
+        # Log in to gcloud (required for gsutil to work)
+        click.secho("> authenticating with gcloud", dim=True)
+        gcloud.login()
 
     try:
         click.secho("> preparing upload job via the CIDC API", dim=True)
         # Read the .xlsx file and make the API call
         # that initiates the upload job and grants object-level GCS access.
         with open(xlsx_path, "rb") as xlsx_file:
             upload_info = api.initiate_upload(upload_type, xlsx_file, is_analysis)
```

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/PKG-INFO` & `nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-cli
-Version: 0.10.3
+Version: 0.10.4
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/SOURCES.txt` & `nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/setup.py` & `nci_cidc_cli-0.10.4/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/dbedit/constants.py` & `nci_cidc_cli-0.10.4/tests/dbedit/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/dbedit/test_core.py` & `nci_cidc_cli-0.10.4/tests/dbedit/test_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/dbedit/test_list.py` & `nci_cidc_cli-0.10.4/tests/dbedit/test_list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/dbedit/test_remove.py` & `nci_cidc_cli-0.10.4/tests/dbedit/test_remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/test_api.py` & `nci_cidc_cli-0.10.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/test_auth.py` & `nci_cidc_cli-0.10.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/test_cache.py` & `nci_cidc_cli-0.10.4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/test_cli.py` & `nci_cidc_cli-0.10.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/test_upload.py` & `nci_cidc_cli-0.10.4/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.3/tests/util.py` & `nci_cidc_cli-0.10.4/tests/util.py`

 * *Files identical despite different names*


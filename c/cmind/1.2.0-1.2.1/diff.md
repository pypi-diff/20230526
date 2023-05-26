# Comparing `tmp/cmind-1.2.0.tar.gz` & `tmp/cmind-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.2.0.tar", last modified: Thu May 25 13:53:12 2023, max compression
+gzip compressed data, was "cmind-1.2.1.tar", last modified: Fri May 26 16:31:24 2023, max compression
```

## Comparing `cmind-1.2.0.tar` & `cmind-1.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-25 13:53:12.221126 cmind-1.2.0/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5112 2023-05-25 12:12:27.000000 cmind-1.2.0/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-25 13:52:19.000000 cmind-1.2.0/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    46002 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    24428 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9241 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.211126 cmind-1.2.0/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1858 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-04-16 15:58:21.000000 cmind-1.2.0/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-04-05 20:14:04.000000 cmind-1.2.0/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1020 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-04-16 15:58:21.000000 cmind-1.2.0/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1032 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-04-16 15:58:21.000000 cmind-1.2.0/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8771 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    31178 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-03-26 14:33:39.000000 cmind-1.2.0/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:12:27.000000 cmind-1.2.0/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-25 13:53:12.221126 cmind-1.2.0/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-25 13:53:12.000000 cmind-1.2.0/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-25 13:53:12.221126 cmind-1.2.0/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-03-26 14:33:39.000000 cmind-1.2.0/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-26 16:31:24.816393 cmind-1.2.1/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5112 2023-05-25 12:13:31.000000 cmind-1.2.1/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-26 16:24:59.000000 cmind-1.2.1/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    46002 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    24428 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9326 2023-05-26 16:24:59.000000 cmind-1.2.1/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1858 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1020 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1032 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.816393 cmind-1.2.1/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8771 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    31178 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.2.1/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-26 16:31:24.806393 cmind-1.2.1/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 12:15:08.000000 cmind-1.2.1/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-26 16:31:24.000000 cmind-1.2.1/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-26 16:31:24.816393 cmind-1.2.1/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-05-25 12:13:31.000000 cmind-1.2.1/setup.py
```

### Comparing `cmind-1.2.0/PKG-INFO` & `cmind-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.2.0
+Version: 1.2.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: grigori@octoml.ai
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
```

### Comparing `cmind-1.2.0/README.md` & `cmind-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/artifact.py` & `cmind-1.2.1/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/automation.py` & `cmind-1.2.1/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/cli.py` & `cmind-1.2.1/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/config.py` & `cmind-1.2.1/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/core.py` & `cmind-1.2.1/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/index.py` & `cmind-1.2.1/cmind/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,16 @@
                 if artifact_obj[1] in index_meta_automation:
                     self._add_if_exists(index_meta_automation, artifact_obj[1], artifacts, keys_to_delete)
             else:
                if ('*' in artifact_obj[0] or '?' in artifact_obj[0]):
                    import fnmatch
                    for artifact in index_meta_automation:
                        if fnmatch.fnmatch(artifact, artifact_obj[0]):
-                           self._add_if_exists(index_meta_automation, artifact, artifacts, keys_to_delete)
+                           if index_meta_automation[artifact].get('uid','')!='':
+                               self._add_if_exists(index_meta_automation, artifact, artifacts, keys_to_delete)
                elif artifact_obj[0]=='':
                    for artifact in index_meta_automation:
                        # Add only 1 (UID) to avoid adding 2 duplicates
                        if index_meta_automation[artifact].get('uid','')!='':
                            self._add_if_exists(index_meta_automation, artifact, artifacts, keys_to_delete)
                elif artifact_obj[0] in index_meta_automation:
                    self._add_if_exists(index_meta_automation, artifact_obj[0], artifacts, keys_to_delete)
```

### Comparing `cmind-1.2.0/cmind/net.py` & `cmind-1.2.1/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/automation/README.md` & `cmind-1.2.1/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/automation/module.py` & `cmind-1.2.1/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.2.1/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/automation/module_misc.py` & `cmind-1.2.1/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/ck/README.md` & `cmind-1.2.1/cmind/repo/automation/ck/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/ck/module.py` & `cmind-1.2.1/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/core/README.md` & `cmind-1.2.1/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/core/module.py` & `cmind-1.2.1/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/repo/README.md` & `cmind-1.2.1/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo/automation/repo/module.py` & `cmind-1.2.1/cmind/repo/automation/repo/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repo.py` & `cmind-1.2.1/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/repos.py` & `cmind-1.2.1/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind/utils.py` & `cmind-1.2.1/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/cmind.egg-info/PKG-INFO` & `cmind-1.2.1/cmind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.2.0
+Version: 1.2.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: grigori@octoml.ai
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
```

### Comparing `cmind-1.2.0/cmind.egg-info/SOURCES.txt` & `cmind-1.2.1/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-1.2.0/setup.py` & `cmind-1.2.1/setup.py`

 * *Files identical despite different names*

